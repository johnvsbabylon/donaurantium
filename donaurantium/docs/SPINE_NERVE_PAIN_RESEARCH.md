# Spinal Stenosis / Nerve / Pain Research — Deep Dive
## Matched to AlphaGenome Spine Panel Results
*Compiled 2026-05-23 | The Donaurantium Project*

---

## Overview

This document cross-references the AlphaGenome spinal stenosis / nerve /
pain variant scan results against peer-reviewed research on acoustic gene
expression modulation, mechanotransduction, low-intensity pulsed ultrasound
(LIPUS), and frequency-specific biological effects. This is the scientific
foundation for the acoustic DNA programming protocol targeting the subject's spinal
stenosis, anxiety, and depression (see BRAINSTORM_004 / Paper 004).

**Core finding from AlphaGenome scan:**
All six genes show baseline expression. No degraded variants. The machinery
is intact. The critical pattern revealed is the expression imbalance:

| Gene | Expression | Role | Direction |
|------|-----------|------|-----------|
| IL1B | ref=20.625 | Inflammation driver | ▼ DOWNREGULATE |
| IL6  | ref=19.750 | Inflammation amplifier | ▼ DOWNREGULATE |
| COL1A1 | ref=10.062 | Structural repair | ▲ UPREGULATE |
| OPRM1 | ref=3.406 | Pain dampening receptor | Understand baseline |
| FAAH | ref=4.562 | Anandamide breakdown | ▼ DOWNREGULATE |
| MMP3 | ref=0.107 | Disc matrix breakdown | ▼ MODULATE / MONITOR |

**The core imbalance:** IL1B (20.625) and IL6 (19.750) are running at
nearly double the expression of COL1A1 (10.062). The inflammatory
machinery significantly outpaces the repair machinery. This is the
primary target: shift the ratio. Reduce inflammatory expression.
Increase collagen synthesis. Tip the balance from breakdown to repair.

MMP3 at ref=0.107 is essentially negligible in this tissue — extremely low
baseline, nothing to suppress. FAAH's −0.7% delta from the AC protective
allele already trends toward the desired direction.

---

## GENE 1 — IL1B (rs16944 [GG] — 0.0% Δ)

**AlphaGenome result:** ref=20.625, alt=20.625. Neutral. GG genotype —
reference allele, no elevated-risk T allele at this position. Full baseline
IL-1β expression.

**The critical flag:** ref=20.625 is the HIGHEST expression value in this
panel and represents a substantially elevated baseline for a pro-inflammatory
cytokine. IL-1β is not supposed to be the loudest gene in the panel. This
high baseline expression in CD4+ T cells — the immune surveillance tissue —
indicates the inflammatory system is persistently active. Primary acoustic
downregulation target.

### What IL1B Is

Interleukin-1 Beta is the master upstream cytokine of the inflammatory
cascade in spinal stenosis. It operates via NF-κB signaling and drives:

- Ligamentum flavum hypertrophy (the tissue that physically narrows the
  spinal canal in lumbar stenosis)
- Upregulation of MMP-3, MMP-9, and MMP-13 in nucleus pulposus cells
  (disc-degrading enzymes)
- Suppression of proteoglycan and collagen synthesis (blocking repair)
- Sensitization of spinal nociceptors (amplifying pain signals)
- Autocrine feedback: IL-1β drives its own further expression

The system is self-reinforcing. Elevated IL-1β keeps the inflammatory
cascade running independently of the original injury trigger.

### IL1B and Acoustic Stimulation — The Research

**LIPUS directly suppresses IL-1β in spinal nucleus pulposus cells
(PMC8522043, Journal of Orthopaedic Surgery and Research, 2021):**
The most directly relevant study to this target. Low-intensity pulsed
ultrasound at **15, 30, and 60 mW/cm²** all inhibited LPS-induced
TNF-α and IL-1β expression in human degenerative nucleus pulposus cells.
**30 mW/cm² was the optimal dose.** At the same time, LIPUS upregulated
aggrecan and collagen II and downregulated MMP-3 and MMP-9. Mechanism
confirmed: LIPUS inhibited p-P65 protein expression and blocked the
NF-κB p65 subunit from translocating to the nucleus — directly blocking
the IL-1β transcription pathway. This is the spinal tissue analog of the
effect we are targeting acoustically.

**40 Hz vibrotactile stimulation (ScienceDirect, 2024):**
40 Hz vibration at audible/tactile frequency produced significant
duration-dependent reduction in IL-1β, TNF-α, IL-6, and iNOS mRNA levels
in neuronal cell lines. This links gamma-frequency acoustic stimulation
directly to IL-1β gene suppression in neural tissue — the frequency
most relevant to our headphone delivery layer.

**LIPUS in macrophages — dose-dependent IL-1β reduction (PMC10036142):**
LIPUS at **10–90 mW/cm²** decreased IL-1β, IL-6, and IL-8 in macrophage
cultures. Optimal anti-inflammatory parameter set identified: **38 kHz,
250 mW/cm², 20% duty cycle, 90 minutes.** Mechanism: suppression of ROS,
TNF-α, and IκBα phosphorylation — the upstream trigger for NF-κB.

**Sustained suppression (PubMed 36930982):**
LIPUS treatment suppressed IL-1β and IL-6 mRNA for up to **72 hours**
post-treatment in peripheral neuropathy models — sustained transcriptional
downregulation, not just transient protein inhibition.

**PIEZO1 as the acoustic gateway to IL-1β:**
PIEZO1 inhibition in nucleus pulposus cells reduces mechanical
shock-induced NLRP3 inflammasome activation and IL-1β expression
(Frontiers in Immunology, 2022). The acoustic PIEZO1 activation pathway
at controlled doses suppresses NF-κB in glial cells. The dose matters:
hormetic response — moderate acoustic activation suppresses IL-1β,
while high-intensity activation can do the opposite. This reinforces
the importance of LIPUS-calibrated intensity parameters.

### Acoustic Targets for IL1B

- **Primary:** 40 Hz carrier (gamma) — direct IL-1β mRNA suppression in
  neural tissue
- **Supporting:** Infrasound layer activating PIEZO1 at moderate amplitude
  → Ca²⁺ → NF-κB suppression cascade
- **Clinical analog:** LIPUS at 1.5 MHz / 30 mW/cm² — audible frequency
  analog is 30–40 Hz whole-body vibration (woofer layer)
- **Session note:** This is the highest-priority acoustic target in the panel

---

## GENE 2 — IL6 (rs1800795 [CG] — 0.0% Δ)

**AlphaGenome result:** ref=19.750, alt=19.750. Neutral. CG genotype —
heterozygous, one C risk allele present. AlphaGenome shows no expression
difference from this allele, but the absolute baseline (19.750) is the
second highest in the panel.

### What IL6 Is

Interleukin-6 is the systemic inflammatory amplifier. Where IL-1β drives
the local spinal inflammatory cascade, IL-6 broadcasts it systemically
and sustains it:

- Released from compressed nerve roots → amplifies pain signal centrally
- Drives osteoclastic bone remodeling at stenotic facet joints
- Sustains inflammatory disc degeneration
- Promotes hyperalgesia (lowered pain threshold) via spinal sensitization
- Red nucleus IL-6 evokes tactile allodynia by disrupting spinal
  cytokine balance

In spinal stenosis, IL-6 and IL-1β operate in a cooperative loop. IL-1β
drives IL-6 production. IL-6 amplifies the downstream effects of IL-1β.
Suppressing one without the other reduces efficacy. The acoustic protocol
addresses both simultaneously.

### IL6 and Acoustic Stimulation — The Research

**Continuous low-intensity ultrasound, 5 MHz — IL-6 attenuation in
cartilage (PMC6499975, BMC Musculoskeletal Disorders, 2019):**
Continuous low-intensity ultrasound at **5 MHz, 14 kPa, 2.5 Vpp,
20 minutes × 4 times/day** in osteochondral explants exposed to IL-6 or
TNFα. This protocol attenuated the catabolic gene expression effects
of both cytokines and promoted chondral repair. Most directly relevant
cartilage-tissue study for the IL-6/acoustic interaction.

**Whole-body vibration meta-analysis — IL-6 and TNF-α reduction
(PMC11249855, 2024):**
Meta-analysis confirmed that **WBV at 30–40 Hz** significantly reduces
both IL-6 and TNF-α across preclinical and clinical studies, with
concurrent IL-10 (anti-inflammatory) elevation. The anti-inflammatory
and anti-pain effects were consistent across age groups and conditions.

**LIPUS optimal parameters in macrophages (PMC10036142):**
38 kHz, 250 mW/cm², 20% duty cycle reduces IL-6 alongside IL-1β —
confirming shared pathway susceptibility to acoustic intervention.

**Sustained IL-6 suppression up to 72 hours (PubMed 36930982):**
Same LIPUS protocol that suppressed IL-1β sustained IL-6 mRNA
downregulation for 72 hours post-treatment in peripheral neuropathy
models. Both cytokines respond to the same acoustic intervention.

**10 kHz spinal cord stimulation — systemic IL-6 reduction (2025):**
High-frequency spinal cord stimulation at 10 kHz in persistent spinal
pain syndrome produced significant plasma reductions in IL-6, IL-1β,
IL-8, IL-10, IL-12, and interferon species. The greatest TNF-α reduction
correlated with best pain relief outcomes. This is electrical rather than
acoustic, but demonstrates that frequency-specific spinal stimulation
produces anti-inflammatory cytokine shifts measurable in blood.

**Note on IL-6 dose sensitivity:**
1 MHz continuous ultrasound at standard wound-healing intensity can
ELEVATE IL-6 in keratinocytes (PMC8463532). IL-6 effects are tissue-
and parameter-specific. The anti-inflammatory profile is achieved at
specific frequency/intensity combinations — not at any acoustic input.
This is why parameter precision matters.

### Acoustic Targets for IL6

- **Primary:** 30–40 Hz whole-body vibration (woofer layer) — directly
  confirmed in meta-analysis to reduce IL-6 and TNF-α
- **Supporting:** 40 Hz gamma carrier (headphone layer) — same gamma
  frequency, different delivery path, complementary effect
- **Session note:** IL-6 and IL-1β share acoustic targets. One protocol
  hits both. The 30–40 Hz woofer layer is the key delivery mechanism.

---

## GENE 3 — COL1A1 (rs1800012 [CC] — 0.0% Δ)

**AlphaGenome result:** ref=10.062, alt=10.062. Neutral. CC genotype —
reference allele, no reduced-function T allele. Full baseline collagen I
expression machinery intact.

**The repair opportunity:** COL1A1 is at roughly half the expression of
the two inflammation drivers (IL1B, IL6). The goal is to push COL1A1 up
while pushing IL-1β and IL-6 down — closing the inflammation/repair gap
from both directions simultaneously.

### What COL1A1 Is

COL1A1 encodes the alpha-1 chain of Type I collagen, the dominant
structural protein of:
- Spinal disc annulus fibrosus (outer rings that contain the disc)
- Ligaments (particularly posterior longitudinal ligament, ligamentum
  flavum, and interspinous ligaments)
- Vertebral connective tissue and bone matrix

In spinal stenosis, collagen scaffolding degrades. The annulus fibrosus
weakens, disc material migrates, ligamentum flavum hypertrophies (but
with disorganized fibrotic collagen rather than organized structural
collagen). More organized COL1A1 expression = more structural integrity
= better disc containment = less nerve root compression over time.

### COL1A1 and Acoustic Stimulation — The Research

**Acoustic vibration frequency specificity — direct COL1A1 measurements
(PMC4337172, BioMed Research International, 2015):**
Human bone marrow-derived mesenchymal stem cells subjected to acoustic-
frequency vibratory stimulation at four frequencies. COL1A1 results:
- **30 Hz:** +29.1% COL1A1 expression vs static control
- **400 Hz:** +70.6% COL1A1 expression vs static control
- **800 Hz:** Maximum osteogenic collagen response — highest COL1A1,
  ALP, RUNX2, and SPP1 mRNA expression in the study

At 800 Hz, adipogenic gene expression (fat cell pathway) was simultaneously
suppressed. Mechanism: frequency-dependent calcium influx through
mechanosensitive channels driving transcription factor activation.
This is the most frequency-specific COL1A1 data in the literature.

**LIPUS in intervertebral disc cells — collagen synthesis (PMC5667559):**
LIPUS at 1.5 MHz, 30 mW/cm², 20 minutes/day stimulates proteoglycan and
collagen synthesis in IVD cells in vitro. Animal models showed significant
upregulation of Col2a1 (dominant disc collagen) alongside type I collagen
expression and fibroblast proliferation.

**LIPUS in tendon cells — COL1A1 + COL3A1 + TGF-β upregulation
(PubMed 16705693, Journal of Orthopaedic Research, 2006):**
Pulsed ultrasound at 1.5 MHz stimulates procollagen α1(I) and α1(III)
mRNA expression in tendon cells, with RT-PCR confirmed upregulation.
TGF-β in conditioned medium elevated — identifying TGF-β signaling as
the intermediate pathway. TGF-β is a master regulator of collagen
synthesis in connective tissue.

**Earliest direct evidence — ultrasound at 3 MHz, 0.5 W/cm²
(PubMed 7350723):**
Pulsed 3 MHz ultrasound, 5 minutes in human fibroblasts stimulated
collagen synthesis via acoustic cavitation — the original foundational
study linking acoustic energy directly to collagen gene activation.

**LIPUS + annulus fibrosus cells (PubMed 25658041):**
LIPUS at **0.5 W/cm²** increased collagen and GAG (glycosaminoglycan)
synthesis while simultaneously decreasing MMP-1 and MMP-3 expression
in human annulus fibrosus cells — the outer disc structure most relevant
to nerve root compression in spinal stenosis. One protocol, simultaneous
COL1A1 up and MMP down.

### Acoustic Targets for COL1A1

- **Primary carrier:** 400 Hz tone (+70.6% documented COL1A1 upregulation)
- **Maximum response:** 800 Hz tone (strongest overall collagen/osteogenic
  signal in available research)
- **Physical layer support:** 30 Hz woofer vibration (+29.1% COL1A1)
- **Session note:** 400 Hz and 800 Hz are in the audible range and trivial
  to generate. These are the most precisely documented frequencies for
  COL1A1 upregulation in the literature.

---

## GENE 4 — OPRM1 (rs1799971 [AA] — 0.0% Δ)

**AlphaGenome result:** ref=3.406, alt=3.406. Neutral. AA genotype —
reference allele. The A118G variant (G allele = reduced receptor
sensitivity, reduced endorphin response) is NOT present. Full mu-opioid
receptor function confirmed.

### What OPRM1 Is

The mu-opioid receptor (MOR) is the binding site for the body's primary
endogenous pain dampening system:
- Beta-endorphin (released during intense exercise, stress, laughter,
  music, binaural beat entrainment)
- Enkephalins (localized pain modulation)
- Exogenous opioid analgesics (morphine, oxycodone)

MOR activation in the periaqueductal gray, rostral ventromedial medulla,
and spinal dorsal horn produces descending pain inhibition — the brain's
own pain suppression circuit. AA genotype = this circuit runs at full
factory specification.

### OPRM1 and Acoustic Stimulation — The Research

**Direct PET-fMRI neuroimaging of music-induced MOR activation
(PMC12316753, European Journal of Nuclear Medicine, 2025):**
The landmark finding. [¹¹C]carfentanil PET directly imaged mu-opioid
receptor binding during music listening. Results:
- Pleasurable music significantly increased MOR binding in ventral
  striatum and orbitofrontal cortex (the brain's hedonic centers)
- MOR binding in nucleus accumbens correlated with frisson (chills)
- This is the first direct neuroimaging confirmation that sound
  activates the brain's mu-opioid system
- Authors connect this explicitly to music-induced pain relief and
  reduced post-operative opioid requirements

**Theta binaural beats (5 Hz) — clinical pain reduction RCT
(PubMed 32564499, European Journal of Pain, 2020):**
Double-blind randomized controlled trial. Binaural beats at **5 Hz
(theta)** for 30 minutes in chronic pain patients, then on-demand use
for one week. Results: significant reduction in perceived pain intensity
and significant reduction in analgesic medication consumption. Proposed
mechanism: theta-frequency brain entrainment induces endogenous opioid
release through OPRM1-expressing pain modulation circuits.

**Theta binaural beats (6 Hz) — chronic pain pilot
(PubMed 26773319):**
Pilot study using theta binaural beats at **6 Hz**, 20 minutes daily.
Pain reduction documented. Attribution: theta entrainment activating
circuits governing endorphin-mediated analgesia.

**Binaural beats systematic review (PMC10785528, 2024):**
Binaural auditory beats are effective for pain relief in acute conditions
and show potential for chronic pain reduction. Effectiveness is frequency-
and condition-dependent. Theta range (4–8 Hz) shows strongest pain
evidence.

**AA genotype significance:**
The goal is not to upregulate OPRM1 receptor density — it's to promote
endogenous ligand (beta-endorphin) release that engages the existing
full-function receptor. With AA genotype, every endorphin molecule
released binds at maximum sensitivity. The acoustic protocol that
triggers endorphin release lands on the best possible receptor.

### Acoustic Targets for OPRM1

- **Primary:** Theta binaural beats at 5–7 Hz (headphone layer) — RCT
  confirmed pain reduction, proposed OPRM1 mechanism
- **Supporting:** Music with emotional resonance as carrier context —
  PET-confirmed MOR activation in nucleus accumbens
- **Session note:** This is the pain relief mechanism. The theta
  entrainment state serves double duty: neural programming receptivity
  AND OPRM1-mediated pain dampening via endorphin release.

---

## GENE 5 — FAAH (rs324420 [AC] — −0.7% Δ)

**AlphaGenome result:** ref=4.562, alt=4.531. Delta: −0.031 (−0.7%).
AC genotype — one protective A allele. The −0.7% already trends in the
desired direction. The A allele reduces FAAH enzyme activity; the
AlphaGenome delta confirms the expression-level effect points the right
way.

### What FAAH Is

Fatty Acid Amide Hydrolase is the enzyme responsible for degrading
anandamide (arachidonoyl ethanolamide, AEA) — the body's primary
endocannabinoid analgesic. The simpler framing:

FAAH destroys the molecule that makes you feel okay.

Lower FAAH activity → more anandamide persists in circulation →
CB1 and CB2 receptor activation → reduced spinal pain signaling,
reduced neuroinflammation, improved mood, reduced anxiety.

The AC genotype at rs324420 means one copy of the A allele, which is
associated with reduced FAAH enzymatic activity. This individual already
has a partial natural advantage in anandamide preservation. The acoustic
goal is to compound that by further suppressing FAAH expression.

FAAH activity is upregulated by chronic stress through HPA-axis activation.
When cortisol is chronically elevated (as in chronic pain states), FAAH
goes up, anandamide goes down, pain amplification worsens — exactly when
pain relief is most needed. Acoustic stress reduction breaks this cycle.

### FAAH and Acoustic Stimulation — The Research

**Direct acoustic FAAH modulation — documented research gap:**
No peer-reviewed study to date has directly measured FAAH mRNA or protein
levels following acoustic stimulation in spinal or neural tissue. This is
a documented gap in the sonobiology literature. This project may generate
the first data points on acoustic FAAH modulation.

**Indirect pathway — mechanistically supported:**

*FAAH in mechanosensory circuits (PMC11450075):*
FAAH is functionally active in mechanosensory neuron circuits. FAAH
inhibition potentiated synapses made by pressure-sensitive mechanosensory
neurons — establishing a direct functional connection between FAAH-
anandamide signaling and mechanosensory/acoustic input processing. FAAH
governs how mechanical input translates to pain signal modulation.

*Stress-driven FAAH upregulation pathway (PMC3073528):*
In response to stress, FAAH activity increases, reducing anandamide and
disinhibiting glutamate, facilitating further stress response. Acoustic
interventions reducing physiological stress (theta binaural beats,
parasympathetic activation) reduce the HPA-axis stress signal → lower
cortisol → lower FAAH upregulation → more circulating anandamide.

*FAAH epigenetic regulation (PMC9992175):*
FAAH expression is epigenetically regulated in the medial prefrontal
cortex via CB1R/FAAH co-regulation. This means FAAH expression is
accessible to epigenetic modification — including the histone modification
documented from acoustic stimulation (PMC7472266).

### Acoustic Targets for FAAH

- **Mechanism:** Acoustic stress reduction → HPA-axis downregulation →
  lower cortisol → reduced stress-driven FAAH upregulation → anandamide
  preserved
- **Primary:** Theta binaural beats (5–7 Hz) — parasympathetic shift,
  cortisol reduction, stress circuit quieting
- **Supporting:** Session design that reliably achieves relaxation/theta
  state — the FAAH benefit is downstream of state achievement
- **Research note:** This project will generate novel data on acoustic
  FAAH modulation. Track anandamide-related subjective markers (pain,
  mood, anxiety) over session series.

---

## GENE 6 — MMP3 (rs6746030 [AG] — −0.5% Δ)

**AlphaGenome result:** ref=0.107, alt=0.106. Delta: near-zero (−0.5%).
AG genotype — heterozygous.

**The key finding: ref=0.107 is essentially negligible.**

MMP3 is barely expressed in this tissue type at baseline. This is the
opposite of the concern — MMP3 is not running high. It is not a primary
driver of disc degeneration in this individual at the expression level
captured here. The −0.5% delta from the AG genotype is noise at this
expression level.

This does not mean MMP3 is irrelevant to spinal stenosis biologically —
it is a known driver in degenerative disc tissue. It means the acoustic
protocol does not need to specifically prioritize MMP3 suppression. The
COL1A1/MMP3 balance is already heavily weighted toward the low-MMP3 side
at the expression level measured.

### What MMP3 Is

Matrix Metalloproteinase-3 (stromelysin-1) degrades aggrecan, fibronectin,
multiple collagen types, laminin, and fibronectin in the spinal disc
extracellular matrix. It also indirectly activates latent MMP-1 and MMP-9.
In degenerative disc disease, elevated MMP3 is a validated marker of
degeneration stage. TNF-α and IL-1β drive MMP3 expression through NF-κB.

### Research Note

**LIPUS directly downregulates MMP-3 in nucleus pulposus (PMC8522043):**
The same LIPUS protocol that suppresses IL-1β simultaneously suppresses
MMP-3. Since IL-1β is the primary driver of MMP-3 expression, suppressing
IL-1β acoustically achieves MMP-3 suppression as a downstream consequence
— no separate MMP-3 protocol needed.

**Indirect suppression path:** IL-1β ↓ → NF-κB inhibition → MMP-3 ↓

Given the near-zero baseline, MMP3 monitoring is appropriate but MMP3
is not a primary acoustic programming target for this individual.

---

## THE EXPRESSION PICTURE — WHAT WE'RE ACTUALLY WORKING WITH

```
INFLAMMATION (need down)         REPAIR (need up)
IL1B  ████████████████████  20.625    COL1A1  ██████████  10.062
IL6   ███████████████████   19.750
                                       PAIN DAMPENING
                                OPRM1  ███  3.406  (full function ✓)
                                FAAH   ████  4.562  (partial A allele ✓)
                                MMP3   ░  0.107   (negligible ✓)
```

The imbalance is stark. Two inflammatory cytokines running at 20+.
One collagen repair gene at 10. The inflammation is winning by a factor
of two. The acoustic protocol's primary objective is to invert this ratio
over time.

**Target state after sustained protocol:**
IL-1β and IL-6 suppressed toward 10–14 (below COL1A1 baseline)
COL1A1 pushed above 15 via acoustic upregulation
Net effect: repair machinery running louder than the inflammation

---

## ACOUSTIC MECHANOTRANSDUCTION — THE DELIVERY CHAIN

```
Sound wave → cell membrane physical deformation
→ PIEZO1 opens (calcium in)     [confirmed: PMC7946898]
→ TRPV4 opens (calcium in)      [confirmed: PMC7584681]
→ Ca²⁺ activates CaMKII, PKC    [established intracellular biochemistry]
→ Kinases phosphorylate transcription factors
→ NF-κB nuclear translocation BLOCKED at target intensity
  (IL-1β transcription inhibited)
→ TGF-β signaling ACTIVATED
  (COL1A1 transcription enhanced)
→ mRNA levels shift
→ Protein production changes
→ Tissue behavior changes over weeks to months
```

The chain is real. The question is whether consumer audio hardware at
audible and near-audible frequencies produces sufficient membrane
deformation to meaningfully activate the cascade. That is what this
experiment answers.

---

## FREQUENCY TARGET MAP — SPINE PROTOCOL

| Target | Gene | Frequency | Delivery | Evidence |
|--------|------|-----------|----------|----------|
| IL1B ↓ | IL1B | 40 Hz | Woofer + headphone | 40 Hz vibration reduces IL-1β mRNA (ScienceDirect 2024) |
| IL6 ↓ | IL6 | 30–40 Hz | Woofer | WBV 30–40 Hz reduces IL-6 in meta-analysis (PMC11249855) |
| COL1A1 ↑ | COL1A1 | 400 Hz | Headphone carrier | +70.6% COL1A1 at 400 Hz (PMC4337172) |
| COL1A1 ↑ | COL1A1 | 800 Hz | Headphone carrier | Maximum collagen response at 800 Hz (PMC4337172) |
| COL1A1 ↑ | COL1A1 | 30 Hz | Woofer | +29.1% COL1A1 at 30 Hz (PMC4337172) |
| OPRM1 engage | OPRM1 | 5–7 Hz | Binaural beat | Theta RCT pain reduction (PubMed 32564499) |
| FAAH ↓ | FAAH | 5–7 Hz | Binaural beat | Stress reduction → HPA ↓ → FAAH ↓ |
| Neural induction | All | 5–6 Hz | Binaural beat | Theta state = maximum programming receptivity |
| BDNF ↑ (depression) | — | 20 Hz | Woofer | Strongest BDNF at 20 Hz (PMC11316700) |
| Neurogenesis (depression) | — | 40 Hz | Both layers | MIT GENUS (ScienceDaily 2025) |
| Body activation | All | <20 Hz | Woofer | PIEZO1/TRPV4 infrasound activation |

---

## SYSTEM SUMMARY — WHAT WE HAVE TO WORK WITH

| Gene | Expression | Status | Acoustic Priority |
|------|-----------|--------|-------------------|
| IL1B | ref=20.625 | HIGH — primary inflammation driver | **URGENT ▼** |
| IL6 | ref=19.750 | HIGH — systemic amplifier | **URGENT ▼** |
| COL1A1 | ref=10.062 | Baseline — repair machinery intact | **▲ PUSH UP** |
| OPRM1 | ref=3.406 | Full function — AA genotype | **Engage via theta** |
| FAAH | ref=4.562 | Partial protection — AC genotype | **▼ compound** |
| MMP3 | ref=0.107 | Negligible — not a primary concern | **Monitor only** |

**Conclusion:** Clean hardware, significant expression imbalance. The
acoustic protocol has clear targets and a measurable success criterion:
shift the IL-1β/IL-6 to COL1A1 ratio over time. All six genes show
intact machinery — no broken receptors, no degraded variants, no missing
components. The system is working; it is just working in the wrong
direction. Sound can push it back.

---

## NEXT STEPS

1. ✅ AlphaGenome spine scan — complete
2. ✅ Deep research documentation — this document
3. Generate audio files (Python/numpy): 40 Hz, 30 Hz, 400 Hz, 800 Hz,
   20 Hz, 5–6 Hz binaural beats, infrasound layer
4. Execute Session 1 tonight
5. Document outcomes: pain scale, spinal mobility, anxiety, mood
6. Repeat and track over 30–90 day protocol

---

*Sources:*
- [LIPUS suppresses IL-1β, MMP-3 in nucleus pulposus — PMC8522043](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8522043/)
- [LIPUS in intervertebral disc cells — PMC5667559](https://pmc.ncbi.nlm.nih.gov/articles/PMC5667559/)
- [LIPUS anti-inflammatory macrophage parameters — PMC10036142](https://pmc.ncbi.nlm.nih.gov/articles/PMC10036142/)
- [LIPUS 72-hour IL-1β / IL-6 suppression — PubMed 36930982](https://pubmed.ncbi.nlm.nih.gov/36930982/)
- [LIPUS in annulus fibrosus — MMP-3 reduction — PubMed 25658041](https://pubmed.ncbi.nlm.nih.gov/25658041/)
- [LIPUS tendon COL1A1 / TGF-β upregulation — PubMed 16705693](https://pubmed.ncbi.nlm.nih.gov/16705693/)
- [Acoustic vibration COL1A1 at 30/400/800 Hz — PMC4337172](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4337172/)
- [IL-6 in cartilage 5 MHz cLIUS — PMC6499975](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6499975/)
- [WBV anti-inflammatory meta-analysis 30–40 Hz — PMC11249855](https://pmc.ncbi.nlm.nih.gov/articles/PMC11249855/)
- [40 Hz vibration IL-1β / IL-6 mRNA reduction — ScienceDirect 2024](https://www.sciencedirect.com/science/article/pii/S0361923024002727)
- [Music activates mu-opioid receptors PET-fMRI — PMC12316753](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC12316753/)
- [Theta binaural beats chronic pain RCT — PubMed 32564499](https://pubmed.ncbi.nlm.nih.gov/32564499/)
- [Theta binaural beats pain pilot — PubMed 26773319](https://pubmed.ncbi.nlm.nih.gov/26773319/)
- [Binaural beats pain systematic review — PMC10785528](https://pmc.ncbi.nlm.nih.gov/articles/PMC10785528/)
- [FAAH in mechanosensory neurons — PMC11450075](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC11450075/)
- [Stress-driven FAAH upregulation — PMC3073528](https://pmc.ncbi.nlm.nih.gov/articles/PMC3073528/)
- [PIEZO1 acoustic activation in osteoblasts — PMC7946898](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7946898/)
- [TRPV4 acoustic wave calcium influx — PMC7584681](https://pmc.ncbi.nlm.nih.gov/articles/PMC7584681/)
- [Acoustic gene expression 145 genes — PMC12003795](https://pmc.ncbi.nlm.nih.gov/articles/PMC12003795/)
- [20 Hz BDNF upregulation — PMC11316700](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC11316700/)
- [40 Hz neurogenesis GENUS — ScienceDaily 2025](https://www.sciencedaily.com/releases/2025/04/250425113441.htm)
- [MMP-3 inhibition enriches collagen II in NP cells — PMC11402661](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC11402661/)
- [TNF-α / IL-1β drive MMP-3 via NF-κB in NP cells — PMC4188173](https://pmc.ncbi.nlm.nih.gov/articles/PMC4188173/)
- [Sonomechanobiology review — PMC10903386](https://pmc.ncbi.nlm.nih.gov/articles/PMC10903386/)
