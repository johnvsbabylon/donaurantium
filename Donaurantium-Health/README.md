# Donaurantium Health — Acoustic Neural Entrainment Protocols

A collection of open-source, browser-based acoustic entrainment protocols designed to gently shift neural oscillation states. No installation required. No data collected. No network requests. Runs entirely in the browser.

---

## Protocols

### `donaurantium-weed.html` — Cannabis-State Emulation
Targets the endocannabinoid system's neural signature through theta-modulated gamma entrainment.

- **Primary mechanism**: 4 Hz theta × 40 Hz gamma nesting (theta-gated gamma)
- **Binaural layers**: CB1 4 Hz, cannabinoid 7 Hz, gamma 40 Hz, alpha 10 Hz
- **Physical layers**: 4 Hz bone conduction, 40 Hz skull driver
- **Visual**: Slow Julia-set fractal with warm amber/indigo palette and indicaDrift organic wander
- **Duration options**: 30 min / 60 min
- **Reported effect**: The strongest protocol in this set — deep body relaxation, visual softness, time dilation

---

### `donaurantium-brute-force-anxiety-depression-photonic.html` — Anxiety & Depression Reset
Targets cortisol dysregulation, stress-circuit hyperactivity, and low-gamma deficits common in anxiety and depression.

- **Primary mechanism**: Adey-window 16 Hz ELF (Ca²⁺ efflux from brain tissue) + theta-gamma photonic coupling
- **Binaural layers**: cortisol 4 Hz, GABA 6 Hz, theta 7 Hz, gamma 40 Hz, alpha 10 Hz
- **Physical layers**: 16 Hz Adey window, 40 Hz skull driver
- **Visual**: Julia-set fractal with theta-envelope animation, edge glow, slow indicaDrift on entry/return phases
- **Duration options**: 30 min / 60 min
- **Reported effect**: Quieting of anxious mental chatter; body warmth; mild mood lift

---

### `donaurantium-euphoria.html` — Endorphin & Dopamine Pathway Activation
Targets the endorphin/opioid and dopamine reward circuits via Ca²⁺/CREB-relevant entrainment frequencies.

- **Primary mechanism**: 3.5 Hz delta (PENK/OPRM1 CREB resonance) + 5 Hz anandamide (CB1 warm-body signal) + 4 Hz NAc reward theta
- **Binaural layers**: endorphin 3.5 Hz (60 Hz carrier), anandamide 5 Hz (120 Hz carrier), reward 4 Hz, alpha 10 Hz
- **Physical layers**: 20 Hz body driver, 30 Hz skull resonance
- **Visual**: Warm golden Julia-set fractal with Lissajous indicaDrift; no cool blues
- **4-phase session**: entry → 4-layer peak (240-second sunrise ramp) → hold → gentle return
- **Duration options**: 30 min / 60 min
- **Reported effect**: Mild warmth and mood lift; subtle physical presence in chest/abdomen; strongest with eyes closed and still

---

### `donaurantium-libido.html` — Desire & Oxytocin Entrainment
Targets bonding and arousal circuits through oxytocin-linked 6 Hz theta and bilateral-symmetric fractal visual resonance.

- **Primary mechanism**: 6 Hz oxytocin theta + 7 Hz desire beta + 18 Hz arousal beta
- **Binaural layers**: oxytocin 6 Hz (120 Hz carrier), desire 7 Hz (200 Hz carrier), beta 18 Hz, gamma 40 Hz
- **Physical layers**: 20 Hz body driver, 40 Hz skull resonance
- **Visual**: Bilateral-symmetric Julia-set (Rorschach pattern) with rose-amber palette — bilateral symmetry via `abs(x)` before iteration
- **4-phase session**: body-arrival → desire-build → peak (all 4 layers) → return
- **Duration options**: 30 min / 60 min
- **Reported effect**: Subtle warmth and heightened body awareness; most noticeable with a partner present

---

## Usage

1. **Open any `.html` file in a modern browser** (Chrome/Firefox/Edge recommended)
2. **Put on stereo headphones** — binaural beats require separate ear channels; earbuds work, over-ear cans are better
3. **Select a duration** and click **Start Session**
4. **Lie down or sit still in a dark room** — eyes closed for maximum effect
5. **Volume**: start around 40–50% system volume; the skull-driver layers need to be felt slightly, not just heard

The fractal visual runs automatically. It is designed to be viewed through closed eyelids or with eyes slightly open in a dark room.

---

## Technical Notes

- **All audio generated in-browser via Web Audio API** — no audio files to load
- **Binaural beats**: carrier tones offset by the beat frequency across L/R channels → brain perceives the difference → frequency-following response
- **Physical layers**: monophonic tones in both channels simultaneously → headphone drivers physically vibrate at those frequencies → bone conduction pathway → mechanotransduction
- **WebGL fractal**: Julia-set iterated escape-time algorithm rendered at full screen resolution; `indicaDrift` slowly wanders the Julia `c` parameter for organic movement
- **No cookies, no analytics, no external requests** — fully offline-capable after first load if served locally

---

## Requirements

- Modern browser with Web Audio API and WebGL support (all major browsers since ~2017)
- **Stereo headphones or earbuds** — the binaural beat mechanism breaks with mono output or speakers
- The physical layer (bone conduction) requires headphones to be worn; it does not work through room speakers

---

## See Also

- [`donaurantium-health-disclaimer.md`](donaurantium-health-disclaimer.md) — important safety and scope notes
- [Donaurantium main project](https://github.com/donaurantium) — genomic and epigenetic sister projects
