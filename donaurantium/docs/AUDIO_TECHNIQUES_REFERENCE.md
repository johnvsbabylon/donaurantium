# Audio Entrainment Techniques — Coding Reference
## Monroe Institute, Binaural Beats, Isochronic Tones & Acoustic Mechanotransduction
*Compiled 2026-05-23 | The Donaurantium Project*
*For use during development of the acoustic epigenetic programming system*

---

## Overview

This document is the technical coding reference for the audio generation
system. Every section is written to inform actual implementation decisions:
carrier frequencies, beat frequencies, waveform shapes, duty cycles,
amplitude ratios, session timing, and file format choices. Where research
gives a specific number, that number is here.

The three sources this document synthesizes:
1. Monroe Institute / HemiSync published research and practitioner documentation
2. Peer-reviewed binaural beat and brainwave entrainment literature
3. Acoustic mechanotransduction cell biology research

---

## PART 1 — MONROE INSTITUTE: CORE TECHNIQUES

### 1.1 HemiSync Technology — What It Actually Is

HemiSync (Hemispheric Synchronization) is Monroe's patented binaural beat
delivery system (US Patent 5,213,562). Core mechanism: slightly different
frequencies to each ear → medial superior olivary nucleus computes the
difference → brain generates the beat frequency internally.

**Carrier frequency constraint:** Binaural beats only work when carrier
tones are below approximately 1,000–1,500 Hz. Above 3 kHz, no detectable
binaural beat is produced. Practical working range: **100–1,000 Hz**.

**Published Monroe carrier example:**
100 Hz left + 104 Hz right = 4 Hz delta-range beat

**Monroe audio layer composition (what's in the actual files):**
- Primary binaural beat signal
- Pink noise base (defined by Monroe as "white noise equalized for human
  hearing" — technically 1/f spectral distribution)
- Natural ambient sounds (surf, rain, forest — varies by product)
- Music (in many tracks)
- Multiple simultaneous beat frequencies layered for complex states

### 1.2 Focus Levels — States and Target Frequencies

Monroe deliberately avoided publishing exact Hz values to prevent
untrained replication. The values below come from third-party FFT analysis
of Monroe materials, CIA Gateway assessment documentation, and practitioner
measurement.

| Focus Level | Monroe Description | Approx Beat Freq | Brainwave Band |
|-------------|-------------------|-----------------|----------------|
| Focus 10 | Mind awake, body asleep | 7–10 Hz | Alpha/Theta border |
| Focus 12 | Expanded awareness | 10–12 Hz | Alpha |
| Focus 15 | No-Time / void / pure potential | 4–6 Hz | Theta |
| Focus 21 | Edge of time-space continuum | ~2–4 Hz | Deep theta |

**Numbers do not equal Hz directly** — Monroe named these numerically to
avoid religious/metaphysical associations. Focus 10 is not 10 Hz.

### 1.3 The Gateway Experience — Full Protocol Structure

**Structure:**
- 8 Waves (Wave I Discovery through Wave VIII Prospecting)
- Each Wave: 6–8 audio exercises
- Total: ~36–48 exercises, completed sequentially
- Do not skip ahead — each exercise builds on the prior state

**Wave progression:**
- Wave I (Discovery): Focus 10 introduction — body asleep, mind awake
- Wave II (Threshold): Focus 10 deepening, Focus 12 introduction
- Wave III (Freedom): Focus 12 consolidation, Free Flow Focus 12
- Wave IV (Adventure): Focus 15 introduction
- Wave V (Exploring): Focus 21 introduction
- Waves VI-VIII: Advanced OBE, contact states, exploration

**Timing:**
- Home program: one exercise per day recommended; replay each until
  comfortable before advancing
- Residential Gateway Voyage (on-site): 6 days, multiple sessions per day
- Per exercise session length: **30–45 minutes**

### 1.4 Resonant Tuning — The Vocal Technique

Introduced in Wave I. Practitioner hums audibly along with the HemiSync
audio, matching pitch instinctively.

**What it does:**
- Creates physical bone and chest cavity vibration (direct mechanotransduction)
- Reduces internal mental chatter / quiets default mode network
- Builds energetic arousal before descending to deeper states
- Mild breath control modulates CO2/O2 balance — hypocapnia shifts
  consciousness state

**Technical analog:** Singing bowl entrainment — mechanical tissue
resonance + auditory feedback loop. Vocal fundamental and harmonics
interact with carrier tones, creating sum/difference frequencies in the
0–20 Hz range as subjective sensation.

**No specific pitch prescribed.** Practitioners vary naturally. Humming
continues several minutes, then fades as the session deepens.

**Coding note:** A resonant tuning phase can be implemented as the
session opening — 2–3 minutes of a prominent single tone (e.g., 200 Hz)
at moderate volume before the binaural layer begins. This gives the
subject something to vocally match and creates a defined transition into
the listening state.

### 1.5 Monroe's OBE Induction via Audio

**Route:** Focus 21 (deep theta / epsilon border, ~2–4 Hz beat).
Monroe found that theta + maintained consciousness enables hypnagogic
imagery, and at the deep theta/epsilon border (~2 Hz), dissociative
experiences reliably occur in trained subjects.

**Lambda/Epsilon connection (Jeffery Thompson research):**
- Lambda: 100–200 Hz brainwave frequency — observed in advanced
  meditators during ecstatic states
- Epsilon: below 0.5 Hz — observed in suspended animation / advanced
  yogi states
- Hypothesis: lambda and epsilon may be harmonically related extremes —
  very fast and very slow states sharing phenomenological qualities
- Practical production: 0.1–0.4 Hz isochronic pulse rate on any carrier

---

## PART 2 — BINAURAL BEAT TECHNICAL RESEARCH

### 2.1 Neural Pathway — How the Beat Actually Forms

```
Ear (L) at f_carrier         Ear (R) at f_carrier + beat_freq
         ↓                              ↓
   Cochlear nucleus              Cochlear nucleus
         ↓                              ↓
    Medial Superior Olivary Complex (MSO)
    ← First bilateral nucleus
    ← Phase-locked neurons fire at beat_freq
    ← This is where the beat is COMPUTED, not heard
         ↓
    Inferior Colliculus
         ↓
    Medial Geniculate Body (thalamus)
         ↓
    Primary Auditory Cortex → FFR at beat frequency
```

**Key fact:** The binaural beat is a subcortical illusion. It does not
exist acoustically — it is computed by the brainstem. This is why:
- Headphones are mandatory (room speakers mix channels before MSO)
- Binaural beats fail above ~1,500 Hz carrier (MSO phase-lock ceiling)
- The effect is real but subtle at the cortical EEG level

### 2.2 Frequency Following Response (FFR)

FFR is cortical EEG shifting toward the dominant stimulus frequency.
Effect is real, effect sizes are moderate, individual variation is high.

**Key eNeuro 2020 study findings (PMC7082494):**
- Carrier tested: 396.5 Hz (L) + 403.5 Hz (R) = 7 Hz theta beat
- Carrier tested: 380 Hz (L) + 420 Hz (R) = 40 Hz gamma beat
- Both binaural and monaural beats produced FFR at beat frequency
- **Monaural beats produced stronger cortical ASSR than binaural beats**
- Cross-frequency coupling: theta beats elicited gamma activity; gamma
  beats elicited alpha — suggests layering produces non-linear effects
- No significant subjective relaxation from acute single session

**Implication:** Monaural (isochronic) beats entrain the cortex more
reliably. Combining both (binaural for subcortical + isochronic for
cortical) is theoretically strongest.

### 2.3 Optimal Carrier Frequencies — The Oster Curve

Gerald Oster (1973, Scientific American) mapped binaural beat perception
strength vs. carrier frequency. Maximum beat perception: **200–400 Hz**.

**Specific coding values:**
```
Target beat frequency    → Recommended carrier range
Delta (0.5–4 Hz)         → 100–300 Hz carrier
Theta (4–8 Hz)           → 250–400 Hz carrier
Alpha (8–13 Hz)          → 200–400 Hz carrier
Beta (13–30 Hz)          → 200–500 Hz carrier
Gamma (40 Hz)            → 400 Hz carrier (eNeuro 2020 used 380/420 Hz)
Mechanotransduction      → 440 Hz (documented in gene expression studies)
```

**Below 100 Hz carrier:** Beat detection degrades
**Above 1,000 Hz carrier:** Beat detection disappears
**Sweet spot: 250–400 Hz for all target bands**

### 2.4 Beat Frequencies and Documented Effects

**Delta (0.5–4 Hz)**
- 0.8 Hz: Slow oscillation entrainment during sleep (50ms tones); enhanced delta EEG and memory consolidation
- 2–3 Hz: Surgical pain reduction protocols; deep tissue repair during sleep
- 3 Hz: Tested in clinical pain settings
- General delta: Growth hormone release, glymphatic clearance, immune function, deep cell repair

**Theta (4–8 Hz)**
- 4 Hz: Deep meditation, OBE-adjacent states, hippocampal memory transfer
- 5 Hz: Verbal recall improvement (15 min sessions 2x/day × 15 days); theta power increase
- **6 Hz: PRIMARY THERAPEUTIC FREQUENCY**
  - Chronic pain protocol: 20 min/day × 14 days → significant depression
    subscale improvement and pain reduction
  - ANS: parasympathetic shift confirmed
  - 1-month daily protocol (10 min/day): P300 and N200 amplitude increases
    each visit across all 3 monthly assessment points — cumulative
  - Anxiety and depression improvement in multiple trials
- 7 Hz: EEG theta entrainment in eNeuro 2020; near Schumann resonance
- 7.83 Hz: Schumann resonance fundamental (see Part 8)

**Alpha (8–13 Hz)**
- 8–10 Hz: Strongest anxiety reduction evidence; cortisol reduction; HRV improvement
- **10 Hz: Best single relaxation frequency; heart rate and BP reduction in 20-min session**
- 10–12 Hz: Monroe Focus 12; pattern recognition; creative states
- 12–13 Hz: SMR (sensorimotor rhythm); attentive relaxation; pain modulation

**Beta (13–30 Hz)**
- 15–20 Hz: Working memory, attention accuracy, cognitive performance
- **25 Hz: Strongest HRV/ANS parasympathetic shift in ANS study** (counter-intuitive — beta frequency produced most pronounced relaxation markers; p<0.01)
- Upper beta (20–30 Hz): Avoid for anxiety targets — can increase arousal

**Gamma (30–100 Hz)**
- **40 Hz: Primary neuroprotective/neurogenesis target** (see full GENUS section below)
- 34–38 Hz: Some studies show stronger entrainment than 40 Hz exactly
- 40 Hz: Activates parvalbumin-positive (PV+) fast-spiking interneurons;
  restores E/I balance; enhances cerebral blood flow

### 2.5 Waveform — CRITICAL FOR MECHANOTRANSDUCTION

**For binaural carrier tones:** Sine wave is standard. No research shows
waveform shape affects binaural beat perception (the beat is computed
from phase relationships).

**For mechanotransduction gene expression (PMC5791945 — PLOS One 2017):**
This is the most important waveform finding in the literature:

| Waveform | Gene Expression Effect |
|----------|----------------------|
| **Sine** | **Maximum suppression of target genes (COX-2, CTGF, Tenascin-C)** |
| Triangle | Intermediate effect |
| **Square** | **Almost no effect** |

**Use sine waves for all carriers.** Square waves are ineffective for
acoustic mechanotransduction even at identical frequency and pressure.
Triangle waves are a compromise but inferior to sine.

### 2.6 Volume / SPL

```
Recommended clinical level:    50–70 dB SPL
Standard clinical trials used: 60 dB SPL
Safe maximum for extended use: 75 dB SPL
Hearing damage threshold:      85 dB SPL (do not exceed)
Mechanotransduction in vitro:  76–94 dB SPL (cell culture; tissue
                               resonance compensates at lower SPL in vivo)
Optimal mix ratio:             Pink noise at 30 dB : binaural carrier at
                               60 dB (from sleep/ASMR study)
```

**Code normalization target:** Normalize output to **-3 dBFS peak**.
This leaves 3 dB headroom below clipping across all platform playback
levels.

### 2.7 Stereo Separation Requirements

- Closed-back over-ear headphones required (circumaural)
- Channel separation: 40+ dB
- Impedance: 32–80 Ω for direct device connection
- No crossfeed circuits (defeats binaural effect)
- No EQ or bass boost (alters carrier balance)
- Frequency response: 20 Hz – 20 kHz flat (±3 dB)
- **Open-back headphones allow acoustic crosstalk — avoid**

### 2.8 Duration, Onset, and Persistence

```
First measurable EEG change:     ~6 minutes
Significant cortical FFR:        ~15–20 minutes
Optimal session length:          20–40 minutes
Long attention/focus sessions:   30–60 minutes
Cumulative EEG plateau:          By session 3 (theta); maintain thereafter
Post-session persistence:        Minutes (not hours) — transient carry-over
```

**One-month theta protocol outcome:** 10 min/day at 6 Hz for 30 days
→ significant improvements at each monthly assessment visit (cumulative,
not just acute). Evidence of progressive neural adaptation to the stimulus.

**For memory improvement:** Shorter is better. 30 minutes at 7 Hz theta
actually *decreased* verbal recall in one study. 15 minutes optimal.

### 2.9 Individual Variation

- Not universal: some individuals are low/non-responders to FFR
- Age: older adults need higher stimulus intensity for equivalent entrainment
- Baseline EEG state: high-alpha subjects entrain more readily to alpha
- Personality: emotional reactivity level correlates with susceptibility
- Takeaway: design for moderate responders; allow volume/session-length
  adjustment in the user-facing config

---

## PART 3 — ISOCHRONIC TONES

### 3.1 What They Are and Why They're Important

Isochronic tones: a single tone pulsed on/off at the target brainwave
frequency. Monaural (identical in both channels). The amplitude modulation
rate creates a rhythmic pulse the auditory cortex entrains to.

**Why superior to binaural for cortical entrainment:**
- Monaural beats produce stronger ASSR than binaural (eNeuro 2020)
- Do not require headphones
- Perceived as distinct rhythmic pulse vs. subtle phantom beat
- Modulation depth: up to 50 dB (vs. ~3 dB for binaural)

**Why binaural still matters:**
- Subcortical entrainment (MSO level) — isochronic doesn't reach this
- The combined approach (both simultaneously) hits both pathways

### 3.2 Technical Parameters — Coding Specifications

**Duty cycle:** Percentage of each cycle the tone is "on"
```
Standard:         50% (equal on/off)
Percussive/sharp: 20–30% (shorter pulse, more rhythmic pop)
Smooth/sustained: 70–80% (longer tone, softer rhythm)
Recommended:      50% starting point; test 30% for gamma (40 Hz)
```

**Gate (amplitude envelope) shape:**
```
Square gate:         Instant on/off — maximum modulation, click artifacts
Cosine gate:         Smooth ramp — recommended; eliminates click artifacts
Linear gate:         Compromise; less smooth than cosine
```

**Cosine gate numpy implementation:**
```python
def isochronic_envelope(t, pulse_rate, sample_rate, duty_cycle=0.5):
    cycle_length = sample_rate / pulse_rate
    position = (t * sample_rate) % cycle_length
    on_samples = cycle_length * duty_cycle
    envelope = np.zeros(len(t))
    # Cosine fade in/out within on-period
    fade = int(on_samples * 0.1)  # 10% of on-period for fade
    for i, pos in enumerate(position):
        if pos < on_samples:
            if pos < fade:
                envelope[i] = 0.5 * (1 - np.cos(np.pi * pos / fade))
            elif pos > on_samples - fade:
                envelope[i] = 0.5 * (1 - np.cos(np.pi * (on_samples - pos) / fade))
            else:
                envelope[i] = 1.0
    return envelope
```

### 3.3 Combining Isochronic + Binaural — The Strongest Approach

Layer both on the same carrier:
```python
# Binaural layer (requires headphones)
left  = amplitude * np.sin(2 * np.pi * f_carrier * t)
right = amplitude * np.sin(2 * np.pi * (f_carrier + beat_freq) * t)

# Isochronic envelope (same target frequency, no headphone requirement)
iso_env = isochronic_envelope(t, beat_freq, sample_rate, duty_cycle=0.5)

# Apply isochronic gate to binaural pair
left  = left  * iso_env
right = right * iso_env
```

This produces a signal that is simultaneously:
- A binaural beat (subcortical entrainment via MSO)
- An isochronic tone (cortical entrainment via ASSR)
Both operating at the same target frequency.

---

## PART 4 — SOLFEGGIO FREQUENCIES

### 4.1 Historical Basis (Plain Truth)

Modern "solfeggio frequencies" are **not** from Gregorian chant. They were
devised by Dr. Joseph Puleo (~1974) by applying Pythagorean reduction to
Numbers 7 in the Old Testament. Medieval musicology confirms these specific
Hz values cannot be traced to historical sacred music. The concert pitch
standard of A=440 Hz was only established internationally in 1939 — earlier
music had no universal Hz reference.

**What this means for coding:** These frequencies have no ancient sacred
basis. Several (particularly 432 Hz and 528 Hz) do have some modern
research interest. Use them as carrier options with appropriate framing.

### 4.2 The Two Frequencies with Actual Research

**432 Hz (vs 440 Hz tuning):**
- Double-blind crossover study: 432 Hz music → lower mean heart rate vs 440 Hz
- University of Florence dental study: 432 Hz group had lower anxiety
  (salivary markers) and stronger left prefrontal alpha
- Sleep in spinal cord injury patients: 432 Hz improved sleep quality vs 440 Hz
- EEG: stronger left prefrontal alpha during 432 Hz playback
- **Verdict:** Effect is real but modest. Mechanism: subjective harmonic
  preference affecting ANS arousal, not special 432 Hz biological resonance.
- **Coding use:** 432 Hz as carrier is a reasonable option; add as config flag

**528 Hz (claimed "DNA repair frequency"):**
- 2017 cell culture study (ResearchGate): 528 Hz reduced cell death and ROS
  production in astrocytes treated with ethanol; ~20% increased cell viability;
  up to 100% ROS reduction
- The widely circulated "DNA repair" claim: original paper difficult to
  verify; not reproduced in independent studies
- **Verdict:** Preliminary in vitro evidence of reduced oxidative stress.
  Not confirmed DNA repair in living organisms. The frequency falls within
  the optimal 500 Hz carrier range — usable on that basis.
- **Coding use:** 528 Hz as a carrier option is not contradicted; sits just
  above the optimal 400–500 Hz range

**Full solfeggio list:** 174, 285, 396, 417, 432, 528, 639, 741, 852, 963 Hz
— only 432 and 528 have any peer-reviewed research. The others have no
specific biological evidence beyond the historical narrative.

---

## PART 5 — FREQUENCY-SPECIFIC TARGET REFERENCE

### 5.1 Complete Frequency Map for Our Three Target Conditions

**ANXIETY:**
```
Primary target:    6–8 Hz theta binaural beat, 250–400 Hz carrier
Entry state:       10 Hz alpha, 300 Hz carrier (start here, descend)
ANS support:       25 Hz beta (paradoxically produces strongest
                   parasympathetic HRV shift in ANS study)
OPRM1 engage:      6 Hz theta (endorphin release documented)
FAAH suppress:     6 Hz theta (stress reduction → HPA ↓ → FAAH ↓)
Duration:          20–30 min/session; twice daily if possible
```

**DEPRESSION:**
```
BDNF upregulation: 20 Hz woofer layer (PMC11316700 — best frequency tested)
Neurogenesis:      40 Hz gamma carrier (MIT GENUS: TCF4, dentate gyrus)
Neural repair:     40 Hz, 60 min/day, daily (GENUS clinical protocol)
Plasticity support: 6 Hz theta (hippocampal memory consolidation)
Duration:          40 Hz layer: 60 min ideally; minimum 20 min
```

**SPINAL STENOSIS:**
```
COL1A1 upregulate: 400 Hz tone (+70.6%); 800 Hz tone (maximum osteogenic)
                   30 Hz woofer (+29.1%)
IL1B downregulate: 40 Hz woofer/carrier (direct IL-1β mRNA suppression)
IL6 downregulate:  30–40 Hz woofer (meta-analysis confirmed)
OPRM1 engage:      6 Hz theta binaural (chronic pain RCT confirmed)
FAAH compound:     6 Hz theta (anandamide preservation via HPA suppression)
MMP3 (monitor):    Negligible baseline — IL-1β suppression handles it
Duration:          30–60 min; daily for cumulative collagen effect
```

**THE THREE-CONDITION OVERLAP (one session, simultaneous):**
```
Theta binaural (6 Hz):  Hits anxiety + pain + FAAH + OPRM1 simultaneously
40 Hz carrier:          Hits depression neurogenesis + IL-1β suppression
30–40 Hz woofer:        Hits IL-6 + COL1A1 + physical PIEZO1/TRPV4 activation
20 Hz woofer:           Hits BDNF (depression)
400/800 Hz tones:       Hits COL1A1 upregulation specifically
```

### 5.2 Schumann Resonance as a Target (7.83 Hz)

The Schumann fundamental (7.83 Hz) sits at the theta/alpha border.

**Research:**
- Randomized double-blind PEMF study at 7.83 Hz: subjects fell asleep
  faster, slept longer, improved polysomnography quality vs control
- Cell proliferation: 7.83 Hz PEMF → 2.8× cell proliferation increase;
  enhanced wound migration
- **As audio binaural beat:** Functional analog to the EM frequency —
  targets same EEG range (theta/alpha border), not literal EM entrainment

**Coding use:** 7.83 Hz binaural beat on 300 Hz carrier as the
Schumann-analog theta target. Falls between 6 Hz (primary) and 10 Hz
(alpha entry). Can be used as a secondary beat layer or as the primary
when a slightly shallower theta state is preferred.

### 5.3 Delta for Sleep-Phase Repair

```
0.8 Hz:   Slow oscillation entrainment (50ms tones at 0.8 Hz pulse rate);
          enhances endogenous slow oscillations and memory consolidation
2–3 Hz:   Deep tissue repair, glymphatic clearance, growth hormone release
          Used as session terminus for sleep-oriented sessions
Production: Isochronic pulse at 0.8–3 Hz on 100–200 Hz carrier
           OR amplitude modulation of continuous tone at target rate
```

---

## PART 6 — INFRASOUND AND WHOLE BODY VIBRATION

### 6.1 Infrasound Effects by Frequency

Infrasound is felt, not heard. Delivered via woofer displacement as
physical pressure waves.

| Hz | Effect | Notes |
|----|--------|-------|
| 2–4 Hz | Near organ resonance; nausea, spatial disorientation possible | Use with caution |
| 4–8 Hz | Thoracic cavity resonance; breathing rhythm interference | |
| 8–12 Hz | Heart resonance range; cardiac rhythm effects | Keep amplitude low |
| 18–19 Hz | Eye resonance — visual smearing, anxiety, cortisol spike | **AVOID** |
| ~19 Hz | Salivary cortisol increase; irritability; music sounds "more sad" | 2026 Frontiers study |

**Vic Tandy finding (Coventry, ~1998):** 18.98 Hz standing wave generated
by extractor fan caused: peripheral vision disturbance, intense depression,
cold shivers, feeling of presence. Confirmed in reportedly haunted locations.
The eyeball resonance at 18–19 Hz is the proposed mechanism.

**Coding rule:** Do NOT generate infrasound near 18–19 Hz. This is the
one infrasound range with documented aversive physiological effects.
The safe infrasound range for therapeutic use: **below 15 Hz**.

**Recommended infrasound targets:**
```
0.5–4 Hz:  Body entrainment / delta analog (felt as very slow pulse)
5–10 Hz:   Autonomic influence, PIEZO1/TRPV4 whole-body activation
10–15 Hz:  Physical alpha-range entrainment via body surface
Avoid:     16–22 Hz (organ/eye resonance danger zone)
```

### 6.2 Whole Body Vibration — Parameters for Spinal Safety

**Safe therapeutic WBV for spinal conditions:**
```
Frequency:     20–30 Hz (optimal for bone; 30 Hz = peak transmissibility)
Magnitude:     < 1g (low magnitude essential for spinal safety)
High frequency (>33 Hz) drops transmissibility to 40–50%
Very high magnitude (>1g) at any frequency: can WORSEN spinal conditions
WBV > 60 Hz: linked to occupational low back pain in extended exposure
```

**Woofer delivery vs. WBV platform:**
Consumer woofer speakers generate airborne pressure waves and some
structural vibration through the floor, not the controlled contact
vibration of a WBV platform. Energy transfer to deep spinal tissue
is lower but whole-body PIEZO1/TRPV4 activation via skin/surface
contact is still documented at audible and near-audible frequencies.

### 6.3 Mechanosensory Activation — The Woofer Layer's Function

For the spinal stenosis protocol, the woofer layer's primary role is
PIEZO1/TRPV4 activation across the body surface via the acoustic
mechanotransduction cascade. Not WBV-level direct bone/disc stimulation.

**Effective woofer delivery frequencies:**
```
20–40 Hz:   Physically felt as low rumble; PIEZO1/TRPV4 activation
            Overlaps with documented anti-inflammatory WBV range (30–40 Hz)
40 Hz:      Gamma frequency; dual function — anti-inflammatory + GENUS
80–100 Hz:  Audible but felt throughout body; structural resonance
400 Hz:     COL1A1 upregulation (PMC4337172 — strongest direct evidence)
800 Hz:     Maximum COL1A1 osteogenic response (same study)
```

---

## PART 7 — NOISE COLORS: TECHNICAL SPECS

### 7.1 Spectral Definitions

```
White noise:  Flat spectrum (equal energy per Hz)        — hissy, full
Pink noise:   1/f spectrum (equal energy per OCTAVE)     — balanced, natural
              Power drops -3 dB per octave (-10 dB/decade)
Brown noise:  1/f² spectrum                             — deep, bass-heavy
              Power drops -6 dB per octave (-20 dB/decade)
Blue noise:   Rising spectrum (+3 dB/octave)             — very bright
```

**Monroe's choice:** Pink noise. Human hearing is logarithmic (octave-
based) so pink noise sounds perceptually balanced — equal energy per
musical interval. This is why it sounds natural rather than harsh or
tubby.

### 7.2 Evidence by Color

**Pink noise (best-evidenced):**
- Memory consolidation and sleep quality (multiple studies)
- Slow oscillation (0.8 Hz) embedded in pink background → enhances delta EEG
- Improved memory recall in older adults
- One study found overnight pink noise *may impair* sleep-dependent insight
  — not uniformly beneficial; short-session use is safe

**White noise:**
- Best for masking environmental disruption
- Stochastic resonance: can enhance weak signal detection in neural systems

**Brown noise:**
- Anecdotally preferred for deep focus and anxiety suppression
- Enhanced working memory in one study vs. other conditions
- Less peer-reviewed evidence overall
- **Subjective preference for anxiety:** many users prefer brown over pink
  for sustained session use; offer as config option

### 7.3 Stochastic Resonance — Why Noise Helps

Neurons are threshold detectors. A sub-threshold signal that would not fire
a neuron can, with appropriate noise added, sometimes push it over threshold
and improve signal transmission. Adding the right amount of noise to a weak
binaural beat signal can actually *enhance* entrainment — this is stochastic
resonance.

**Optimal noise:** Colored noise (pink) superior to white for neural signal
detection (PMC3954722).

**Practical ratio (from sleep/ASMR study):**
```
Binaural carrier:  -12 dBFS (0 dB reference)
Pink noise:        -18 to -24 dBFS (6–12 dB quieter than carrier)
```
The noise should be audible but clearly below the carrier tone level.

### 7.4 Numpy Pink Noise Generation — Voss-McCartney Algorithm

```python
def pink_noise(num_samples, sample_rate=44100):
    """Generate pink noise using Voss-McCartney algorithm."""
    num_columns = 16
    array = np.full((num_samples, num_columns), np.nan)
    array[0, :] = np.random.random(num_columns)
    array[:, 0] = np.random.random(num_samples)
    
    n = num_samples
    cols = np.random.geometric(0.5, n)
    cols[cols >= num_columns] = 0
    rows = np.random.randint(0, n, n)
    array[rows, cols] = np.random.random(n)
    
    df = pd.DataFrame(array)
    df.fillna(method='ffill', axis=0, inplace=True)
    total = df.sum(axis=1)
    total = (total - total.mean()) / total.std()
    return total.values * 0.5

# Alternative: FFT-based (simpler, accurate)
def pink_noise_fft(num_samples):
    white = np.random.randn(num_samples)
    fft = np.fft.rfft(white)
    freqs = np.fft.rfftfreq(num_samples)
    freqs[0] = 1  # avoid div by zero
    fft = fft / np.sqrt(freqs)
    return np.fft.irfft(fft, num_samples)
```

---

## PART 8 — TECHNICAL AUDIO ENGINEERING

### 8.1 Binaural Beat Generation — Core Numpy Pattern

```python
import numpy as np
import soundfile as sf

def generate_binaural_beat(
    carrier_freq,     # Hz — the carrier tone (200–500 Hz)
    beat_freq,        # Hz — the beat frequency (4–40 Hz)
    duration,         # seconds
    amplitude=0.5,    # 0.0 to 1.0
    sample_rate=44100
):
    t = np.linspace(0, duration, int(sample_rate * duration), endpoint=False)
    left  = amplitude * np.sin(2 * np.pi * carrier_freq * t)
    right = amplitude * np.sin(2 * np.pi * (carrier_freq + beat_freq) * t)
    # Phase difference accumulates naturally from frequency difference
    return left, right

# Example: 6 Hz theta on 300 Hz carrier
left, right = generate_binaural_beat(300, 6, duration=1200)  # 20 min
stereo = np.column_stack([left, right])
sf.write('theta_6hz.wav', stereo, 44100)
```

### 8.2 Fade Envelopes

No published standard timing, but practitioner consensus and Monroe
protocol timing:

```python
def cosine_fade(length_samples, fade_in_samples, fade_out_samples):
    envelope = np.ones(length_samples)
    # Fade in
    t_in = np.linspace(0, np.pi, fade_in_samples)
    envelope[:fade_in_samples] = 0.5 * (1 - np.cos(t_in))
    # Fade out
    t_out = np.linspace(0, np.pi, fade_out_samples)
    envelope[-fade_out_samples:] = 0.5 * (1 + np.cos(t_out))
    return envelope

# Recommended fade times:
# Delta/theta sessions:  60s fade in, 60s fade out
# Alpha sessions:        30s fade in, 30s fade out
# State transitions:     120s crossfade between beat frequencies
```

### 8.3 State Transition — Frequency Sweep

When shifting brain states mid-session (e.g., alpha to theta descent),
interpolate beat frequency smoothly rather than stepping:

```python
def frequency_sweep(f_start, f_end, duration, carrier, sample_rate=44100):
    """Sweep beat frequency from f_start to f_end over duration seconds."""
    t = np.linspace(0, duration, int(sample_rate * duration), endpoint=False)
    beat_freq = np.linspace(f_start, f_end, len(t))
    # Instantaneous phase of right channel
    right_phase = 2 * np.pi * np.cumsum(carrier + beat_freq) / sample_rate
    left_phase  = 2 * np.pi * carrier * t
    left  = np.sin(left_phase)
    right = np.sin(right_phase)
    return left, right

# Example: alpha to theta descent over 5 minutes
left_sweep, right_sweep = frequency_sweep(10, 6, 300, 300)
```

### 8.4 Layering Multiple Frequency Targets

When layering multiple binaural frequencies (e.g., theta + gamma), use
**separate carrier frequencies** to prevent the carriers from beating
against each other at an audible frequency.

```python
# Layer 1: 6 Hz theta on 300 Hz carrier
l_theta = 0.5 * np.sin(2 * np.pi * 300 * t)
r_theta = 0.5 * np.sin(2 * np.pi * 306 * t)

# Layer 2: 40 Hz gamma on 400 Hz carrier
l_gamma = 0.3 * np.sin(2 * np.pi * 400 * t)
r_gamma = 0.3 * np.sin(2 * np.pi * 440 * t)

# Layer 3: 400 Hz mechanotransduction tone (mono, both channels)
col1a1_tone = 0.2 * np.sin(2 * np.pi * 400 * t)  # COL1A1 upregulation

# Mix and normalize
left  = l_theta + l_gamma + col1a1_tone
right = r_theta + r_gamma + col1a1_tone
peak  = max(np.max(np.abs(left)), np.max(np.abs(right)))
left  = left  / peak * 0.85   # -3 dBFS headroom
right = right / peak * 0.85
```

**Rule:** Two carriers at frequencies X and Y produce an audible beat
at |X−Y| Hz. Keep carriers spaced far enough apart that |X−Y| is either
inaudible or intentional.

### 8.5 File Format

```
Generation output:     44,100 Hz or 48,000 Hz sample rate; 16-bit WAV
Distribution:          320 kbps MP3 minimum; FLAC for lossless
Avoid:                 MP3 < 192 kbps (carrier smearing risk)
Never:                 MP3 < 128 kbps for binaural content (artifacts)
Channel count:         2 (stereo) for all headphone content
                       1 (mono) for woofer/infrasound track
```

### 8.6 GENUS 40 Hz Protocol — Full Clinical Specification

The MIT/Tsai Lab protocol for reference:

```
Audio:       40 Hz sinusoidal tone (pure sine wave)
             Closed-eye condition → strongest prefrontal response
             34–38 Hz showed stronger entrainment than 40 Hz in some tests
Light:       40 Hz flickering, 400–700 cd/m² luminance
             Red/white light > green/blue for entrainment
             (Light not relevant for audio-only sessions)
Session:     1 HOUR per session
Frequency:   DAILY (skipping breaks cumulative effect)
Duration:    Phase 1: 10 days for acute effect
             Phase 2A: 3 months for clinical cognitive benefit
             4–6 months for neuroprotection
Mechanism:   PV+ interneuron activation → E/I balance restoration
             → enhanced cerebral blood flow
             → microglial modulation
             → amyloid plaque reduction ~50% in mouse models
             → hippocampal/amygdala entrainment confirmed
Safety:      Generally well-tolerated; minor dizziness/tinnitus in subset
```

**For our sessions:** 40 Hz sine tone on 400 Hz carrier (headphone layer)
+ 40 Hz isochronic woofer layer simultaneously. Run for as close to
60 minutes as practical. Daily.

---

## PART 9 — COMPLETE SESSION ARCHITECTURE

### 9.1 Standard 30-Minute Session (Anxiety + Depression + Spine)

```
TIME      LAYER                         CONTENT
────────────────────────────────────────────────────────────────────────
00:00     Pink noise only               Fade in over 90 seconds
01:30     Woofer layer begins           20 Hz (BDNF) + 30 Hz (IL-6/COL1A1)
02:00     Alpha binaural begins         10 Hz beat, 300 Hz carrier, fade in
05:00     Alpha holds                   10 Hz theta binaural + woofers
07:00     Theta sweep begins            10 Hz → 6 Hz over 3 minutes
10:00     Theta holds                   6 Hz binaural (300 Hz carrier)
10:00     Gamma layer begins            40 Hz beat, 400 Hz carrier, fade in
10:00     COL1A1 carrier adds           400 Hz pure tone at low amplitude
10:00–25:00  PROGRAMMING PHASE         6 Hz theta + 40 Hz gamma + 400 Hz
                                        + 20 Hz woofer + 30–40 Hz woofer
                                        + pink noise background
25:00     Theta → alpha return          6 Hz → 10 Hz over 2 minutes
27:00     Alpha → SMR                  10 Hz → 13 Hz over 1 minute
28:00     Binaural fade out            Carriers fade over 60 seconds
29:00     Pink noise only               Final fade to silence over 60 seconds
30:00     End
────────────────────────────────────────────────────────────────────────
```

### 9.2 Extended 60-Minute Session (Full GENUS + Spine)

```
TIME      LAYER                         CONTENT
────────────────────────────────────────────────────────────────────────
00:00     Pink noise + woofer prep     20 Hz + 30 Hz woofer; pink noise
02:00     Alpha entry                  10 Hz binaural, 300 Hz carrier
06:00     Theta descent                10 → 6 Hz sweep over 4 minutes
10:00     PROGRAMMING PHASE BEGINS
          ├─ Theta binaural             6 Hz, 300 Hz carrier (sustained)
          ├─ Gamma binaural             40 Hz, 400 Hz carrier (sustained)
          ├─ COL1A1 carrier             400 Hz + 800 Hz sine tones (low amp)
          ├─ 20 Hz woofer              BDNF upregulation
          ├─ 30–40 Hz woofer           IL-1β/IL-6 suppression + COL1A1
          └─ Pink noise                Stochastic resonance substrate
10:00–55:00  SUSTAINED PROGRAMMING    45-minute core phase
55:00     Return sweep                 6 → 10 → 13 Hz over 3 minutes
58:00     Carriers fade                60 second fade
59:00     Pink noise                   Final 60 second fade to silence
60:00     End
────────────────────────────────────────────────────────────────────────
```

### 9.3 Output File Structure

```
session_[name]_[date]/
├── woofer.wav           Mono. 20 Hz + 30 Hz + 40 Hz sine layers.
│                        Plays through Quasar SW372 speakers.
├── headphones_L.wav     Left ear. All binaural carriers (left side).
├── headphones_R.wav     Right ear. All binaural carriers (right side).
├── headphones_stereo.wav  Combined L+R stereo. Main headphone file.
├── session_manifest.txt  Hz targets, gene targets, timing, rationale.
└── (optional) combined_mix.wav  Everything bounced to stereo reference.
```

### 9.4 Volume Balance Between Layers

```
Pink noise:         -18 dBFS (quietest layer — background only)
Woofer tones:       -12 dBFS (felt more than heard; drive speakers hard)
Binaural carrier:   -6 dBFS (primary audible layer)
Pure tones (400 Hz, 800 Hz): -15 dBFS (present but not distracting)
40 Hz gamma:        -9 dBFS (audible; slightly below primary theta carrier)
Final peak:         Normalize output to -3 dBFS
```

---

## PART 10 — QUICK REFERENCE CARD

```
══════════════════════════════════════════════════════════════════════
FREQUENCY TARGETS
══════════════════════════════════════════════════════════════════════
0.8 Hz    Delta slow oscillation (sleep; memory consolidation)
2–3 Hz    Deep delta (tissue repair; GH release)
6 Hz      Theta primary (pain + anxiety + depression; OPRM1; FAAH)
7.83 Hz   Schumann resonance analog (theta/alpha border)
10 Hz     Alpha entry / return state
13 Hz     SMR (waking return; session exit)
20 Hz     BDNF upregulation (depression; PMC11316700)
25 Hz     ANS parasympathetic shift (strongest HRV effect)
30 Hz     COL1A1 +29%; IL-6 suppression (woofer)
40 Hz     GENUS neuroprotection; IL-1β suppression (GENUS + woofer)
400 Hz    COL1A1 +70.6%; optimal binaural carrier; mechanotransduction
800 Hz    Maximum COL1A1 osteogenic response; mechanotransduction

══════════════════════════════════════════════════════════════════════
CARRIER FREQUENCIES
══════════════════════════════════════════════════════════════════════
200–300 Hz   Delta binaural carrier
250–400 Hz   Theta binaural carrier (300 Hz standard)
200–400 Hz   Alpha binaural carrier (300 Hz standard)
400 Hz       Gamma binaural carrier; COL1A1 mechanotransduction
432 Hz       Alternate carrier (modest ANS evidence)
528 Hz       Alternate carrier (in vitro oxidative stress evidence)

══════════════════════════════════════════════════════════════════════
WAVEFORM RULES
══════════════════════════════════════════════════════════════════════
ALL carriers:          SINE WAVE ONLY
Square wave:           Ineffective for mechanotransduction
Triangle wave:         Inferior to sine; avoid
Isochronic gate:       Cosine curve (not square) to eliminate clicks

══════════════════════════════════════════════════════════════════════
AVOID
══════════════════════════════════════════════════════════════════════
18–19 Hz infrasound    Eye resonance; cortisol spike; anxiety induction
>85 dB SPL             Hearing damage risk
Square wave carriers   No mechanotransduction effect
MP3 < 192 kbps         Carrier smearing risk for binaural content
Carrier > 1,500 Hz     Binaural beat perception fails

══════════════════════════════════════════════════════════════════════
TIMING
══════════════════════════════════════════════════════════════════════
Session length:        20–30 min (standard); 60 min (GENUS protocol)
Fade in/out:           60s for deep states; 30s for alpha
State transitions:     2–3 min sweep (never step abruptly)
First EEG change:      ~6 minutes in
Cumulative plateau:    By session 3
Monthly results:       6 Hz theta × 30 days → P300/N200 enhancement
══════════════════════════════════════════════════════════════════════
```

---

*Sources:*
- [HemiSync patent US5213562](https://patents.google.com/patent/US5213562A/)
- [Monroe Institute Focus Levels](https://www.monroeinstituteuk.org/focus-levels/)
- [The Gateway Experience Manual (Archive.org)](https://archive.org/details/the-gateway-experience-manual)
- [Binaural beats auditory pathway — PMC7082494](https://pmc.ncbi.nlm.nih.gov/articles/PMC7082494/)
- [Binaural beats review — PMC11367212](https://pmc.ncbi.nlm.nih.gov/articles/PMC11367212/)
- [Isochronic tones — Wikipedia](https://en.wikipedia.org/wiki/Isochronic_tones)
- [Cumulative theta effects — ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S1746809418300296)
- [6 Hz theta 1-month protocol — Scientific Reports 2024](https://www.nature.com/articles/s41598-024-68628-9)
- [ANS binaural beat regulation — PMC12145584](https://pmc.ncbi.nlm.nih.gov/articles/PMC12145584/)
- [Parametric binaural investigation — Scientific Reports 2025](https://www.nature.com/articles/s41598-025-88517-z)
- [Acoustic gene expression — PMC12003795](https://pmc.ncbi.nlm.nih.gov/articles/PMC12003795/)
- [Waveform specificity COX-2/CTGF — PMC5791945](https://pmc.ncbi.nlm.nih.gov/articles/PMC5791945/)
- [Sonobiology and mechanotransduction review — PMC11735818](https://pmc.ncbi.nlm.nih.gov/articles/PMC11735818/)
- [40 Hz GENUS review — PMC9797689](https://pmc.ncbi.nlm.nih.gov/articles/PMC9797689/)
- [Schumann resonance sleep — PMC9189153](https://pmc.ncbi.nlm.nih.gov/articles/PMC9189153/)
- [Infrasound cortisol/mood — Frontiers 2026](https://www.frontiersin.org/journals/behavioral-neuroscience/articles/10.3389/fnbeh.2026.1729876/full)
- [Pink noise memory — PMC10722168](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10722168/)
- [Stochastic resonance colored noise — PMC3954722](https://pmc.ncbi.nlm.nih.gov/articles/PMC3954722/)
- [432 Hz health effects — ScienceDirect](https://www.sciencedirect.com/science/article/abs/pii/S1550830718302763)
- [Vic Tandy infrasound research — Wikipedia](https://en.wikipedia.org/wiki/Vic_Tandy)
- [Binaural beats pain systematic review — PMC10785528](https://pmc.ncbi.nlm.nih.gov/articles/PMC10785528/)
- [Resonant Tuning — Monroe Institute](https://www.monroeinstitute.org/blogs/blog/how-resonant-tuning-helps-you-connect-more-easily-with-higher-states)
