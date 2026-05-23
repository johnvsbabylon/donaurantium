# Donaurantium HTML Implementation Notes
## What Was Built and Why

*Compiled 2026-05-23*

---

## Scope

The `versions/` directory contains eight standalone HTML session players:

- `donaurantium-anxiety-headphones.html`
- `donaurantium-anxiety-stereo.html`
- `donaurantium-depression-headphones.html`
- `donaurantium-depression-stereo.html`
- `donaurantium-spinal-stenosis-headphones.html`
- `donaurantium-spinal-stenosis-stereo.html`
- `donaurantium-general-improvement-headphones.html`
- `donaurantium-general-improvement-stereo.html`

Each file is intentionally self-contained. There are no JavaScript modules,
external libraries, imported assets, or build steps. Opening the HTML file in a
modern browser is enough to run the session.

---

## Main Implementation

Each HTML now includes:

- Complete landing screen
- 30-minute and 60-minute duration selector
- Therapeutic intensity slider (0.5×–1.8× range)
- Audio-only mode
- Physical output profile selector
- Visual safety modal
- Full Web Audio graph
- Voss-McCartney pink noise generator
- Biological drift LFO on each physical layer
- Harmonic reinforcement (1.5× overtone at 18% amplitude)
- Logarithmic fade-in curve
- Smooth phase transitions
- Breath pacing cue in session HUD
- Pause / resume behavior
- End screen
- Local session logging
- CSV export
- Fullscreen WebGL Julia set visual layer
- CSS fallback when WebGL is unavailable

The original files already contained most protocol constants and research
rationale. The implementation work filled the runtime gaps around those
constants.

---

## Audio Runtime

The audio engine uses the Web Audio API.

### Headphones Variants

Headphone files use binaural beat layers where the left and right channels are
kept separate with a `ChannelMergerNode`.

Example:

```text
left oscillator  -> left gain  -> merger channel 0
right oscillator -> right gain -> merger channel 1
merger -> master gain -> output
```

This preserves the protocol requirement that binaural beat variants require
stereo channel isolation.

### Stereo Variants

Stereo files use isochronic tones instead of binaural beats. These are carrier
sine waves amplitude-modulated by smooth cosine gates.

The point is compatibility: isochronic tones still create rhythmic auditory
envelopes but do not require left/right channel isolation, so they work through
speakers.

### Physical Layers

Physical mechanotransduction tones are implemented as monaural sine oscillators
sent equally to both channels. These include condition-specific layers such as
20 Hz, 30 Hz, 40 Hz, 90 Hz, 400 Hz, and 800 Hz where specified by the docs.

**Base gain:** Sub-300 Hz physical layers use a base gain of `0.075`. Layers at
300 Hz and above use `0.032`. This 37% boost over the earlier 0.055 value
compensates for headphone low-frequency rolloff and improves mechanotransductive
pressure at the PIEZO1/TRPV4 target window.

The physical output selector has two modes:

- `Standard`: baseline gain for ordinary headphones or speakers
- `Woofer / tactile`: raises physical-layer gain by 35% for actual low-frequency
  hardware such as a woofer or tactile transducer

The `intensityMultiplier` (from the intensity slider) multiplies on top of both
modes. This does not change the frequencies.

### Biological Drift LFO

Each physical layer includes a slow sine LFO (0.011–0.018 Hz, randomized per
layer; period ~55–90 seconds) that modulates the layer's gain by ±3%. The per-
layer randomization ensures the layers drift independently.

Purpose: prevents neural habituation to a perfectly static amplitude. Biological
systems are designed to habituate to constant stimuli; slow unpredictable
variation maintains salience throughout the session.

### Harmonic Reinforcement

For all physical layers between 8 Hz and 300 Hz, a second oscillator is added
at 1.5× the fundamental frequency (e.g., 20 Hz → 30 Hz harmonic; 40 Hz → 60 Hz
harmonic). This harmonic oscillator runs at 18% the amplitude of the fundamental.

Purpose: adds spectral texture without introducing harmonic-rich waveforms that
smear cymatic tissue patterns. The 1.5× interval (a perfect fifth) avoids
dissonance while reinforcing the fundamental's perceived presence.

### Intensity Slider

The landing screen includes a slider from 0.5× to 1.8× (default 1.0×). At
session start, the selected multiplier is read into `state.intensityMultiplier`
and applied to all physical layer gains. Binaural and isochronic layers are
not affected — only the physical mechanotransduction dose scales.

### Timing

Session timing now follows `AudioContext.currentTime` once audio starts. This is
more appropriate than relying only on `performance.now()` because the protocol's
primary dose is audio. Visual rendering still uses the same elapsed session time,
keeping the fractal pulse synchronized to the audio phase.

All audible transitions use ramped `AudioParam` changes. Direct hard changes were
avoided because they create clicks and startle discontinuities.

### Logarithmic Fade-In

The master gain uses a logarithmic curve rather than a linear ramp during the
fade-in period. The curve formula is:

```text
fadeCurve[i] = 0.72 * (0.45 + log10(1 + p * 9) * 0.55)
```

where `p` runs 0→1 over the fade duration. This reaches therapeutic amplitude
(~0.72) faster than linear ramp, spending more time near full dose while still
protecting the onset from a sudden jump. For the anxiety protocol, the fade is
120 seconds (mandatory for FKBP5=183.0 startle-sensitive profile); other
protocols use 90 seconds.

---

## Pink Noise

Each session includes a Voss-McCartney pink noise generator.

Purpose:

- Provide the stochastic-resonance substrate described in the audio docs
- Keep noise lower than the carrier layers
- Avoid external files or audio samples

The implementation uses a browser-compatible `ScriptProcessorNode` because every
HTML file must remain standalone.

---

## Visual Runtime

The visual layer is a WebGL Julia set renderer.

It implements:

- Fullscreen canvas
- Phase color mapping
- Julia `c` parameter morphing
- Slow zoom-in / return zoom-out
- Luminance pulsing at the active protocol frequency
- 40 Hz pulse during GENUS/gamma phases (pulseDepth 0.20)
- 10 Hz pulse during alpha phases (pulseDepth 0.12)
- 6 Hz and below phases (pulseDepth 0.10)
- CSS fallback when WebGL is unavailable

The fragment shader computes escape-time Julia values on the GPU. This keeps the
fractal responsive without importing a graphics library.

**Visual modulation depth:** The `u_depth` uniform that controls luminance
modulation is set to `0.20` during 40 Hz GENUS phases (up from 0.15 in earlier
versions). This remains within the Tsai lab safe-range and strengthens the
visual arm of the GENUS protocol. Alpha and gamma phases below 40 Hz use
shallower modulation (0.12 and 0.10 respectively) to avoid visual fatigue during
longer calm phases.

The app estimates display refresh rate on load. If the screen is below roughly
100 Hz, the app reports that 40 Hz visual pulse fidelity may alias. A 120 Hz or
higher display is preferred for the visual 40 Hz arm.

### Breath Pacing Cue

The session HUD displays a breath pacing prompt that updates each phase:

- `↕ 5 / min` during theta and sub-theta phases (≤6 Hz) — coherent breathing
  at ~0.1 Hz to support autonomic balance
- `↕ 6 / min` during alpha and gamma phases (>6 Hz) — relaxed pacing compatible
  with lighter entrainment

The prompt appears once the session starts and fades in over 800 ms. It is
implemented as an ARIA live region so screen readers announce it on phase change.

---

## Protocol Alignment Choices

Some original HTML comments conflicted with newer condition-specific docs. Where
that happened, the newer targeted docs were treated as source of truth.

### Anxiety

The anxiety sessions now follow:

```text
Entry / Alpha -> Deep Suppression -> Brake Reinforcement -> Return
```

This matches `ANXIETY_GENOMIC_ACOUSTIC_TARGETS.md`:

- 10 Hz alpha for entry / GABRA2 stabilization
- 6 Hz theta for FKBP5 / SLC6A4 / HPA suppression
- beta/gamma reinforcement for GABRA2 / COMT support

### Depression

The depression sessions keep theta-gamma coupling as the core phase. The visual
pulse during this core is set to 40 Hz so the visual GENUS arm is actually active
during the phase where the docs describe gamma reward-circuit support.

### Spinal Stenosis

The spinal sessions were aligned to `SPINE_GENOMIC_ACOUSTIC_TARGETS.md`.

Important correction:

- `BDNF_20HZ` is excluded from spinal variants

Reason: the spine docs specifically caution that BDNF in the spinal dorsal horn
can be pro-nociceptive in neuropathic pain models. The 20 Hz BDNF layer remains
in anxiety/depression contexts, not spine sessions.

The spine sequence now follows:

```text
Entry / Pain Gate -> Anti-Inflammation -> Disc Preservation -> Collagen Drive
```

### General Wellness

The general wellness color mapping was corrected to use the visual protocol's
amber/gold phase color for metabolic entry/return.

---

## Local Logging

Each completed session is logged in browser `localStorage`.

Recorded fields:

- Start time
- End time
- Protocol
- Variant mode
- Completion status
- Target duration
- Completed seconds
- Audio-only status
- Physical output scale
- Estimated display refresh rate

The end screen includes `Export Log`, which downloads the local log as CSV.

This matters because the biological hypothesis depends on repeated dose across
30, 60, and 90 days. Without adherence data, there is no serious experiment.

---

## Why These Optimizations Matter

The implementation is optimized around the parts of the hypothesis most likely
to matter:

1. **Dose consistency**
   Daily sessions need repeatable timing, phase order, and fade behavior.

2. **Signal purity**
   Sine waves are used for carriers and physical tones. Sudden gain changes are
   avoided.

3. **Correct delivery mode**
   Binaural protocols preserve left/right isolation. Speaker-compatible protocols
   use isochronic modulation.

4. **Physical coupling**
   Low-frequency mechanotransduction layers are more plausible with actual
   low-frequency hardware, so the app provides an explicit woofer/tactile profile.
   Sub-300 Hz base gain raised to 0.075 (37% above prior value) to compensate
   for headphone rolloff.

5. **Habituation resistance**
   Biological drift LFO (per-layer, randomized 55–90s period) prevents neural
   adaptation to constant amplitude. Harmonic reinforcement adds spectral texture
   that stimulates without introducing cymatic interference.

6. **Onset safety**
   Logarithmic fade-in reaches therapeutic level faster than linear while still
   protecting the onset — mechanistically important for the high-FKBP5 anxiety
   profile where any amplitude discontinuity can activate the stress axis being
   suppressed.

7. **Adaptive dosing**
   The intensity slider lets users start conservative (0.5×) and increase toward
   the validated range (1.0×–1.5×) as tolerance builds.

8. **Coherent breathing entrainment**
   The breath pacing cue adds a physiological synchronization layer: 5/min during
   theta phases engages vagal tone; 6/min during alpha/return phases maintains
   the same without pushing the user into forced resonance breathing.

9. **Visual fidelity**
   40 Hz visual stimulation needs adequate refresh rate. The app checks and
   reports this. GENUS phase visual depth raised to 0.20 for stronger PV+
   interneuron activation.

10. **Measurement**
    Session logs make adherence and dose visible over time.

---

## Scientific Boundary

This code implements the protocol described by the project docs. It does not
prove the protocol works clinically.

The accurate claim is:

```text
This is a research implementation intended to deliver acoustic and visual
stimulation patterns that may influence neural state and downstream biological
signaling pathways.
```

The code should not claim guaranteed DNA rewriting, guaranteed RNA modulation,
or guaranteed treatment of any condition. If measurable biology changes occur,
the most plausible categories are:

- RNA expression changes
- inflammatory marker changes
- stress hormone changes
- methylation or chromatin-state changes
- neural oscillation / entrainment changes
- subjective symptom changes

Those outcomes require measurement.

---

## Verification Performed

After implementation, all eight HTML files were checked for:

- No `TODO` or placeholder markers
- No external modules or imports
- JavaScript syntax validity with `node --check`
- 30-minute and 60-minute phase schedule continuity
- Correct exclusion of `BDNF_20HZ` from spine variants
- Correct 40 Hz visual pulse in depression theta-gamma phase
- Headless Chrome landing screenshots
- Headless Chrome WebGL session render path

---

## Best-Use Notes

For the strongest experiment:

- Use 60-minute sessions
- Use the same target protocol daily for 90 days
- Use wired closed-back headphones for headphone variants
- Use a 120 Hz or higher display for visual 40 Hz phases
- Use a woofer or tactile transducer for the physical layer when possible
- Export the session log periodically
- Track symptoms and any lab markers separately

---

*End of implementation notes.*
