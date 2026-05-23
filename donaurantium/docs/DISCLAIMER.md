# Donaurantium — Disclaimer & Safety Information

**Version:** 1.0.0  
**Project:** Donaurantium — Open-Source Acoustic Epigenetic Programming System  
**Authors:** The Donaurantium Project

---

## What This Is

Donaurantium is an open-source self-experimentation research platform. It generates
acoustic stimuli — binaural beats, isochronic tones, and physical mechanotransduction
layers — with frequencies selected from published peer-reviewed research on acoustic
epigenetic effects, brainwave entrainment, and mechanosensitive ion channel activation.

**It is not a medical device. It is not a treatment. It is not a cure.**

The protocols target documented molecular mechanisms (PIEZO1/TRPV4 ion channel
activation, CaMKII/PKC phosphorylation cascades, FFR-mediated cortical entrainment)
that are established in vitro and in animal models. Whether acoustic stimulation of
these pathways produces clinically meaningful outcomes in humans at headphone delivery
levels is not yet established by clinical trial evidence.

---

## The Honest Mechanism Picture

**What is documented:**

- Acoustic pressure physically deforms cell membranes and activates mechanosensitive
  ion channels (PIEZO1, TRPV4). Source: PMC12003795 (2025, Nature Communications
  Biology) — 42–145 differentially expressed genes measured from acoustic exposure
  in controlled cell culture conditions.
- Binaural beats produce a measurable cortical Frequency Following Response (FFR).
  Source: Oster (1973); multiple replications. Carrier frequency optimum 200–400 Hz.
- Isochronic tones drive cortical auditory evoked potentials (CAEP) through
  amplitude-modulation following response. Source: Picton et al. (2003); Ross et al.
  (2000). Different entrainment pathway from binaural beats; overlapping outcomes.
- The GENUS protocol (40 Hz combined audio+visual) activates PV+ interneurons,
  reduces amyloid load in mice, and modulates neuroinflammatory gene expression.
  Source: Tsai et al. (2016 Science; 2019 Cell).
- 6 Hz theta entrainment has nine-gene convergence across anxiety, depression, and
  pain genomic panels. The FKBP5 methylation + meditation literature supports
  sustained theta as a mechanism for HPA axis downregulation.

**What is not yet established:**

- Whether headphone-level acoustic pressure (vs. direct cell bath in vitro) is
  sufficient to drive meaningful PIEZO1/TRPV4 activation in vivo.
- Whether single-session exposure produces measurable gene expression changes in
  humans, or whether cumulative exposure is required.
- Clinical efficacy for anxiety, depression, or spinal conditions. No clinical
  trials have validated this specific protocol or delivery method.
- Long-term safety of repeated sub-threshold mechanotransduction stimulation.

The frequency assignments are mechanistically reasoned and literature-supported.
They are hypotheses, not proven treatments.

---

## Safety Warnings

### Volume

**Use comfortable, conversational-level volume only.** Therapeutic effect from
acoustic mechanotransduction does not require loud volume; louder is not more
effective and risks hearing damage. If the session is uncomfortable at any
volume level, reduce it or stop.

- Sub-bass physical layers (20–90 Hz) are boosted in gain to compensate for
  headphone frequency rolloff; the boost is calibrated to maintain comfortable
  output levels, not to exceed them.
- The 120-second logarithmic fade-in in anxiety and general improvement protocols
  is mechanistically motivated (FKBP5 startle sensitivity) and is not a suggestion
  to increase volume as the session progresses.

### Photosensitive Epilepsy

The WebGL visual layer includes rhythmic luminance pulses synchronized to the
protocol frequency (40 Hz during GENUS phases). **Do not use the visual layer
if you have photosensitive epilepsy, a history of seizures, or visual sensitivity
to flickering light.** Use audio-only mode (toggle available on the landing screen).

The 40 Hz visual flicker is within the range documented to trigger photosensitive
seizures in susceptible individuals (3–50 Hz, ILAE criteria). The seizure warning
dialog is shown before each session; do not dismiss it without reading it.

### Contraindications — Consult a Doctor First

Do not use this protocol without consulting a qualified healthcare provider if you:

- Have been diagnosed with epilepsy or any seizure disorder
- Have a cardiac pacemaker or implanted electrical device
- Are pregnant
- Have active psychosis or are in an acute psychiatric crisis
- Have severe or untreated hypertension
- Have had recent neurosurgery or traumatic brain injury
- Are currently experiencing acute tinnitus
- Are under 18 years old

This list is not exhaustive. If you have a neurological, cardiac, or psychiatric
condition and are uncertain whether acoustic entrainment is appropriate, ask your
doctor before using this software.

### Stop Immediately If

- You feel dizziness, lightheadedness, or disorientation
- You experience headache during or after a session
- You notice unusual visual phenomena (beyond the intentional fractal display)
- You feel ear pain, pressure, or unusual sounds
- You experience anxiety, panic, or emotional distress
- Any discomfort that was not present before starting

These can indicate excessive volume, audio equipment issues, or individual
sensitivity. Remove headphones, rest, and do not resume until symptoms resolve.

---

## Individual Variation

Acoustic entrainment response varies substantially between individuals. Factors
including baseline brainwave state, auditory processing, genetics (including the
genomic variants documented in each protocol's FREQ table), medications, and
prior meditation experience all influence outcomes.

The genomic target tables (AlphaGenome RNA-seq, CD4+ T cell CL:0000624, hg38)
represent a single reference tissue type. Your gene expression profile in relevant
tissues (neural, immune, connective) may differ. The Δ% values shown are predicted
from variant data, not measured from your cells.

Do not interpret absence of subjective effect as evidence of failure, or presence
of subjective effect as evidence of the claimed mechanisms.

---

## Self-Experimentation Context

This project was built as open-source self-experimentation infrastructure. It is
shared in that spirit: the authors use it, document the mechanisms as honestly as
possible, and release the source so others can evaluate, audit, and extend it.

The source code, research documents, and genomic analysis are published openly.
Researchers, clinicians, and curious individuals are invited to examine the
mechanistic reasoning and form their own conclusions.

**This is not a substitute for clinical evaluation, diagnosis, or treatment.**
If you are experiencing anxiety, depression, chronic pain, or other conditions
addressed by these protocols, please seek qualified professional care. Acoustic
self-experimentation may be a useful adjunct for some people; it is not a
replacement for evidence-based treatment.

---

## No Medical Claims

Donaurantium does not claim to diagnose, treat, cure, mitigate, or prevent any
disease or condition. The protocol names (anxiety, depression, spinal stenosis,
general improvement) refer to the genomic targets and mechanistic hypotheses
being explored — not to clinical indications or outcomes.

No statements in the source code, documentation, or associated research files
should be interpreted as medical advice.

---

## License & Liability

This software is released under the MIT License. It is provided "as is," without
warranty of any kind, express or implied. The authors are not liable for any
adverse outcomes arising from its use.

By using this software, you acknowledge that you have read this disclaimer and
understand the research-only, self-experimentation nature of the project.

---

## Full Citations

PMC12003795 · PMC6172823 · PMC3652411 · PMC11316700 · PMC5791945  
Oster (1973) · Muthukumaraswamy (2013) · Tsai et al. (2016 Science, 2019 Cell)  
Picton et al. (2003) · Ross et al. (2000) · Zannas et al. (2016)  
Tang et al. (2015, Nature Reviews Neuroscience)

Full annotated references in each protocol's `*_RESEARCH.md` and
`*_GENOMIC_ACOUSTIC_TARGETS.md` companion documents.
