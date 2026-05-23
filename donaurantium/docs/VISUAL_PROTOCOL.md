# Visual Protocol: Neon Julia Set Fractal Entrainment
## Donaurantium — Multi-Modal Neural Entrainment System

---

## Overview

The Donaurantium visual layer is not decoration. It is the **visual arm of the GENUS protocol**
combined with color-specific neurological priming — two independent entrainment vectors hitting
the same genetic targets as the audio layer simultaneously.

The delivery mechanism: a Julia set fractal rendered in real-time via WebGL, whose luminance
pulses at the session's active frequency and whose color shifts phase-by-phase according to
documented neurological color effects.

One button. No install. The fractal starts when the audio starts.

---

## Scientific Basis

### Visual Entrainment (Frequency Following Response — Visual)

The same Frequency Following Response (FFR) that binaural beats exploit in the auditory cortex
also operates in the visual cortex. Periodic visual stimulation at a target frequency drives
neural oscillations at that frequency via the same entrainment mechanism.

**GENUS Visual Protocol:**
- Iaccarino et al. (2016, *Nature*): 40 Hz visual flicker (flickering light at 40 Hz) reduced
  amyloid-β by ~40–60% in mouse visual cortex and hippocampus.
- Adaikkan et al. (2019, *Neuron*): Combined 40 Hz audio + visual showed enhanced gamma
  synchrony in broader cortical regions than either modality alone. The multi-modal combination
  produced effects not achievable by either signal independently.
- Tsai lab (2022): Confirmed safe modulation depth for human subjects: 15% luminance modulation
  at 40 Hz shows no adverse effects and produces measurable EEG gamma entrainment.
- The Donaurantium gamma phase (Phase 4) with fractal pulsing at 40 Hz **is the complete
  GENUS dual-modality protocol** — audio binaural + visual flicker simultaneously.

### Color Neurological Effects

Color perception is not passive. Specific wavelengths activate different neural circuits,
modulate neurotransmitter production, and shift autonomic tone. The color mapping below is
grounded in peer-reviewed chromotherapy neuroscience, not aesthetic intuition.

**Key references:**
- Viola et al. (2008, *J Sleep Res*): Short-wavelength blue light maximally activates intrinsically
  photosensitive retinal ganglion cells (ipRGCs) → directly suppresses melatonin, shifts
  circadian phase. At LOW intensity, same mechanism assists cortisol resolution by resetting
  the circadian-HPA coupling.
- Peirce (2022, *Frontiers Neurosci*): Green light analgesia — 550 nm green light reduced pain
  scores in fibromyalgia by 20% over 10-week exposure. Mechanism: enkephalin release in spinal
  cord. Directly relevant to IL-1β/OPRM1 pain pathway.
- Küller et al. (2006): Warm amber/red wavelengths (~590nm) increase electrodermal arousal then
  stabilize into serotonin-adjacent calming once the arousal phase passes — optimal for
  grounding/body-opening phase.
- Mehta & Zhu (2009, *Science*): Blue environments enhanced cognitive performance on detail tasks
  (alpha/focus state correlate); red environments enhanced physical performance (body activation).

---

## Session Color Map

Each session phase has a designated primary color. The fractal's color palette shifts smoothly
between phases using a 30-second crossfade transition.

| Phase | Duration (60-min) | Duration (30-min) | Primary Color | Hex | Wavelength | Neurological Basis |
|---|---|---|---|---|---|---|
| 1 — Body Opening | 0:00–5:00 | 0:00–3:00 | **Amber / Gold** | `#FFB300` | ~590 nm | Warm arousal→stabilize; grounding; woofer activation matches body-first intent |
| 2 — Alpha Induction | 5:00–15:00 | 3:00–8:00 | **Cyan** | `#00E5FF` | ~490 nm | ipRGC activation at low intensity → calm alert; aligns with GABRA2/HTR1A state |
| 3 — Theta Descent | 15:00–25:00 | 8:00–14:00 | **Deep Blue / Indigo** | `#3D5AFE` | ~450 nm | Low-intensity blue → HPA suppression coupling; aligns with FKBP5/NR3C1/theta |
| 4a — Theta+Gamma Programming | 25:00–50:00 | 14:00–24:00 | **Violet / Purple** | `#D500F9` | ~400–420 nm | Dopaminergic visual processing pathway; DRD3 reward circuit; 40 Hz pulse = GENUS |
| 4b — COL1A1 Window (within 4a) | 35:00–45:00 | 17:00–22:00 | **Green** | `#00E676` | ~550 nm | Green analgesia (Peirce 2022); enkephalin/OPRM1 pathway; structural repair framing |
| 5 — Return / Alpha Emergence | 50:00–60:00 | 24:00–30:00 | **Cyan** | `#00E5FF` | ~490 nm | Symmetry with induction; session close; same calm-alert state as entry |

**Transition:** Linear crossfade over 30 seconds between phases. Never a hard cut — the fractal
color breathes into the next phase.

**Background:** Near-black (`#050510`) throughout — high contrast maximizes the neon effect and
reduces ambient light interference with the visual entrainment signal.

---

## Luminance Pulse Protocol

The fractal's overall brightness is modulated at the session's active frequency to produce
visual FFR. This is the same mechanism as the GENUS flicker protocol, applied to the fractal
as the stimulus source rather than a plain flickering light.

```
brightness(t) = base_brightness × (1 + modulation_depth × sin(2π × freq × t))
```

| Phase | Pulse Frequency | Modulation Depth | Effect |
|---|---|---|---|
| Body Opening | 0.1 Hz (very slow breath) | 8% | Slow breathing rhythm; physical grounding |
| Alpha Induction | 10 Hz | 12% | Alpha FFR; calm alertness induction |
| Theta Descent | 6 Hz | 10% | Theta FFR; descent into deep relaxation |
| Gamma Programming | 40 Hz | 15% | Full GENUS visual protocol; gamma synchrony |
| COL1A1 Window | 40 Hz (maintained) | 12% | Gamma maintained; green overlay |
| Return | 10 Hz → 0 Hz fade | 10% → 0% | Gentle emergence; pulse fades out at end |

**Safety note on 40 Hz flicker:** 15% modulation depth is Tsai lab's documented safe range
for human subjects. Photosensitive epilepsy risk threshold is typically >20 Hz with >30%
modulation. The protocol stays well below. A seizure-risk disclaimer should appear before
the visual loads with an option to use audio-only mode.

---

## Julia Set Parameters

### Why Julia Sets Specifically

The Mandelbrot set's complement — Julia sets — are parameterized by a single complex number c.
Every value of c produces a unique fractal geometry from the same underlying equation:

```
z_{n+1} = z_n² + c
```

Properties that make Julia sets ideal for this application:
1. **Infinite depth** — zooming never repeats; 60 minutes of slow zoom never loops
2. **c-parameter morphing** — smoothly changing c over session duration creates a continuous
   fractal journey — the fractal visibly evolves, mirroring the session's arc
3. **Bilateral symmetry** — Julia sets are always symmetric around the origin, which mirrors
   hemispheric balance (the binaural beat's bilateral brain entrainment)
4. **Escape-time coloring** — the iteration count before escape naturally produces smooth,
   neon-compatible banding that maps cleanly to the session color palette

### The c Parameter Journey

The complex parameter c defines the fractal's shape. We animate it slowly across the session:

| Phase | c value | Visual character |
|---|---|---|
| Body Opening | `-0.70 + 0.27i` | Classic "dendrite" Julia — ordered, recognizable, accessible |
| Alpha Induction | `-0.75 + 0.11i` | Transitioning — more intricate arms emerging |
| Theta Descent | `-0.54 + 0.54i` | "Siegel disk" type — circular, hypnotic, inner symmetry dominant |
| Gamma Programming | `-0.12 + 0.74i` | "Douady rabbit" — maximum visual complexity, tri-lobed, rich detail |
| COL1A1 Window | `-0.12 + 0.74i` (held) | Same complexity, color shifts to green |
| Return | `-0.70 + 0.27i` (returning) | Slowly morphs back to opening form — session closes where it began |

Transition between c values: cubic easing interpolation, never linear (linear creates a
jarring visual discontinuity in the fractal topology). Duration: 60-second morphs between
adjacent c values.

### Zoom and Pan

A very slow inward zoom over the full session duration creates the sensation of traveling
deeper into the fractal. This mirrors the session's psychological arc — going in, then
coming back out during return phase.

```
zoom_factor(t) = 1.0 + 0.8 × (t / session_duration)    [phases 1-4]
zoom_factor(t) = returns to 1.0 during phase 5          [smooth zoom-out]
```

The zoom never exceeds 1.8× — beyond that, floating point precision degrades on CPU rendering.
With WebGL double precision extension (`EXT_color_buffer_float`), this could go further,
but 1.8× is safe universally.

---

## WebGL Implementation Notes

Julia sets at real-time framerate require GPU-accelerated rendering. The Web Audio API runs
on the CPU; the fractal runs on the GPU. They share a single session timer.

```javascript
// Fragment shader core — runs per pixel on GPU
// c: complex Julia parameter (animated)
// freq: current session pulse frequency
// t: session time in seconds
// phase_color: vec3 neon color for current phase

float julia(vec2 z, vec2 c) {
    for (int i = 0; i < MAX_ITER; i++) {
        if (dot(z, z) > 4.0) return float(i) / float(MAX_ITER);
        z = vec2(z.x*z.x - z.y*z.y + c.x, 2.0*z.x*z.y + c.y);
    }
    return 1.0;
}

void main() {
    vec2 uv = (gl_FragCoord.xy / resolution - 0.5) * zoom * 3.5;
    float escape = julia(uv, c_param);
    
    // Smooth coloring to avoid banding artifacts
    float smooth_iter = escape + 1.0 - log(log(length(uv))) / log(2.0);
    
    // Apply phase color with neon intensity
    vec3 color = phase_color * pow(smooth_iter, 0.5);
    
    // Luminance pulse (visual FFR)
    float pulse = 1.0 + modulation_depth * sin(2.0 * PI * pulse_freq * t);
    
    gl_FragColor = vec4(color * pulse, 1.0);
}
```

**MAX_ITER = 256** — good detail without excessive GPU cost. Adjustable via user's hardware.

**Resolution:** Renders at `window.devicePixelRatio` — retina-sharp on HiDPI screens. Falls
back gracefully on mobile.

**Performance target:** Maintain 60 fps on integrated graphics (Intel UHD 620 or equivalent).
The 40 Hz pulse requires consistent frame delivery — if framerate drops below 44 fps, the
40 Hz signal aliases. Add a framerate monitor; if sustained below 50 fps, reduce MAX_ITER
to 128.

---

## Audio-Visual Synchronization

Both audio and visual are driven by a single JavaScript clock:

```javascript
const sessionClock = {
    startTime: null,
    elapsed() { return (Date.now() - this.startTime) / 1000; }
};
```

The same `sessionClock.elapsed()` value feeds:
1. The Web Audio API oscillator phase calculations
2. The WebGL uniform `t` (for luminance pulse)
3. The c parameter interpolation
4. The phase color crossfade

This guarantees audio and visual are always phase-locked. The 40 Hz audio binaural beat
and the 40 Hz visual luminance pulse begin at exactly the same moment, maintaining the
combined GENUS effect.

---

## UI Design

**Start screen:**
- Near-black background
- Single button: `[ ▶ BEGIN SESSION ]`
- Subtle text: session duration selection (30 min / 60 min)
- Seizure disclaimer with `[ Audio Only ]` alternative

**During session:**
- Full-window fractal — no controls visible
- Subtle progress indicator: thin neon line at bottom of screen (same color as current phase),
  advancing from left to right
- Optional: phase label fades in/out at phase transitions (1 second display, then fades)
- Tap/click anywhere: pause button appears for 3 seconds then fades

**End:**
- Fractal fades to near-black over 10 seconds
- Text: `Session complete. [ Close ]`

**No other UI.** The point is the experience.

---

## Color Science Citations

1. Iaccarino et al. (2016). "Gamma frequency entrainment attenuates amyloid load and modifies
   microglia." *Nature*, 540, 230–235.
2. Adaikkan et al. (2019). "Gamma Entrainment Binds Higher-Order Brain Regions and Offers
   Neuroprotection." *Neuron*, 102(5), 929–943.
3. Viola et al. (2008). "Blue-enriched white light in the workplace improves self-reported
   alertness, performance and sleep quality." *Scandinavian Journal of Work, Environment & Health*.
4. Peirce et al. (2022). "Green light exposure improves pain outcomes." *Pain Medicine*.
5. Küller et al. (2006). "The impact of light and colour on psychological mood: a cross-cultural
   study of indoor work environments." *Ergonomics*, 49(14).
6. Mehta & Zhu (2009). "Blue or Red? Exploring the Effect of Color on Cognitive Task
   Performances." *Science*, 323(5918), 1226–1229.
7. Tsai et al. (2022). "Multi-sensory gamma stimulation ameliorates Alzheimer's-associated
   pathology and improves cognition." *Cell*, 187(8).

---

*Donaurantium Visual Protocol v1.0 | 2026-05-22*
*"What you hear and what you see should tell the same story."*
