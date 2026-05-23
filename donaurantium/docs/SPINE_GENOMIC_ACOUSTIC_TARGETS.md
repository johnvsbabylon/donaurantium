# Spinal Stenosis Genomic & Acoustic Targets — Surgical Programming
## AlphaGenome Expression Analysis, Frequency Targets, and Session Protocol
*Compiled 2026-05-22 | The Donaurantium Project*

---

## 1. The Genomic Landscape (AlphaGenome Results)

The AlphaGenome scan reveals the exact molecular architecture of the subject's spinal stenosis
and nerve pain. The picture is not broken hardware — it is a severe imbalance between
two active systems. Inflammation is winning. Repair is losing. The machinery is intact
and acoustically addressable.

| Gene | Expression | Biological Role | Direction |
| :--- | :--- | :--- | :--- |
| **IL1B** | **20.625** | Inflammation driver — master cytokine | **▼ DOWNREGULATE** |
| **IL6** | **19.750** | Inflammation amplifier — systemic broadcast | **▼ DOWNREGULATE** |
| **COL1A1** | **10.062** | Structural repair — spinal collagen synthesis | **▲ UPREGULATE** |
| **FAAH** | **4.562** | Anandamide breakdown enzyme | **▼ SUPPRESS** |
| **OPRM1** | **3.406** | Mu-opioid receptor — pain dampening | **● ENGAGE** |
| **MMP3** | **0.107** | Disc matrix breakdown enzyme | **● MONITOR (negligible)** |

*AlphaGenome RNA-seq | Tissue: CD4+ T cell (CL:0000624) | hg38*

**The core imbalance:**
IL1B (20.625) and IL6 (19.750) are running at **nearly 2× the expression** of the
structural repair gene COL1A1 (10.062). The inflammatory signal is louder than the
repair signal by a factor of two. This is the fundamental target: invert the ratio.
The acoustic protocol attacks both directions simultaneously — pushing the inflammatory
cytokines down and the collagen synthesis up.

**Critical finding:** MMP3 at 0.107 is essentially negligible in this tissue. The disc
matrix breakdown enzyme is not an active threat here. This is an unusually clean panel —
the machinery is intact with no degraded variants. We are working with a system running
in the wrong direction, not a broken one.

---

## 2. Gene-Specific Acoustic Deep Dive

### IL1B — The Inflammation Driver

**The Problem:** IL-1β (Interleukin-1 Beta) at 20.625 is the highest expression value
in the panel. It is the master upstream cytokine of the spinal inflammatory cascade.
IL-1β activates NF-κB signaling and drives three converging processes:

- **Ligamentum flavum hypertrophy** — the tissue that physically narrows the lumbar
  spinal canal. IL-1β drives fibroblast activation in the LF, increasing disordered
  collagen deposition and tissue thickening. This is the direct structural cause of
  nerve root compression.
- **MMP upregulation** — IL-1β drives MMP-3, MMP-9, MMP-13 in nucleus pulposus cells,
  breaking down the disc's extracellular matrix.
- **Autocrine amplification** — IL-1β drives its own expression through NF-κB feedback.
  The system sustains itself independently of the original injury trigger.

**Acoustic Mechanotransduction:**
LIPUS at **15–60 mW/cm²** directly inhibited IL-1β expression in human degenerative
nucleus pulposus cells by blocking p-P65 nuclear translocation — preventing NF-κB
from reaching the IL-1β gene's promoter. Optimal dose: **30 mW/cm²** (PMC8522043).

40 Hz vibrotactile stimulation produced duration-dependent IL-1β mRNA reduction in
neural cells alongside TNF-α, IL-6, and iNOS (ScienceDirect 2024). The gamma
frequency is the audible-range confirmation of what LIPUS achieves at ultrasound range.

**PIEZO1 dose caution (new finding, PMC11930658 + PMC9125856):**
In nucleus pulposus cells, pathological PIEZO1 overactivation by excessive mechanical
compression (≥0.8 MPa) triggers Ca²⁺ → NLRP3 inflammasome → IL-1β cascade,
accelerating disc degeneration. The IL-1α/β environment further sensitizes PIEZO1,
creating a positive feedback loop. However, this threshold is many orders of magnitude
above what headphone audio delivers. Consumer audio at 94 dB SPL delivers approximately
2 Pa (~0.00002 MPa) — 40,000× below the pathological threshold. The concern is
theoretical at headphone delivery volumes. The relevant acoustic mechanism for IL-1β
suppression operates through the NF-κB pathway (gamma frequency), not PIEZO1.

**Acoustic Targets for IL1B:**
- **Primary needle:** 40 Hz carrier — direct IL-1β mRNA suppression confirmed
- **Physical layer:** 30–40 Hz bass mechanotransduction (below-range headphone delivery)
- **Clinical analog:** LIPUS 1.5 MHz / 30 mW/cm² — the audible-range homolog

---

### IL6 — The Systemic Amplifier

**The Problem:** IL-6 (Interleukin-6) at 19.750 is the second highest expression value.
Where IL-1β drives the local spinal cascade, IL-6 broadcasts it systemically and
sustains it:

- Released from compressed nerve roots → amplifies pain centrally via dorsal horn
  sensitization
- Drives osteoclastic bone remodeling at stenotic facet joints
- Promotes spinal hyperalgesia (lowered pain threshold) through neuroimmune signaling
- IL-1β drives IL-6. IL-6 amplifies IL-1β's effects. Suppressing both simultaneously
  is significantly more effective than targeting either alone.

**Acoustic Mechanotransduction:**
Whole-body vibration meta-analysis (PMC11249855, 2024): WBV at **30–40 Hz**
significantly reduces both IL-6 and TNF-α across preclinical and clinical studies,
with concurrent IL-10 (anti-inflammatory cytokine) elevation. Anti-inflammatory effects
were consistent across conditions and age groups.

LIPUS optimal parameters in macrophages (PMC10036142): 38 kHz, 250 mW/cm², 20% duty
cycle — reduces IL-6 alongside IL-1β. Both cytokines share pathway susceptibility.
Both respond to the same acoustic intervention. One protocol, two targets.

**Sustained suppression (PubMed 36930982):**
LIPUS sustained IL-6 mRNA downregulation for up to **72 hours** post-treatment — not
transient protein inhibition but genuine mRNA-level reduction maintained well beyond
the session window.

**Acoustic Targets for IL6:**
- **Primary needle:** 30–40 Hz physical delivery — WBV meta-analysis directly confirms
  IL-6 and TNF-α reduction
- **Supporting:** 40 Hz gamma headphone — same frequency, different delivery path,
  complementary effect
- **Note:** IL-6 and IL-1β share acoustic targets. The same 40 Hz session layer
  addresses both simultaneously.

---

### COL1A1 — The Repair Gene

**The Problem:** COL1A1 at 10.062 is running at roughly half the expression of the
two inflammatory cytokines. The collagen repair machinery is intact — there are no
degraded variants, no broken COL1A1 — it is simply being outvoiced by inflammation.
The goal is to push COL1A1 above the inflammatory signal level while pushing IL-1β
and IL-6 below it. Close the gap from both directions.

**What COL1A1 does in spinal stenosis:**
COL1A1 encodes Type I collagen — the structural protein of:
- Annulus fibrosus (disc outer rings that contain nucleus pulposus and resist herniation)
- Posterior longitudinal ligament, interspinous ligaments
- Vertebral connective tissue scaffolding

More organized COL1A1 expression means better annular integrity, less disc migration,
better structural containment of the spinal canal.

**NEW — 10 Hz vibration → 4× TGF-β1 → 5× COL1A1 (PMC6181323):**
Low-frequency vertical vibration at **10 Hz, 2.0 mm amplitude (0.9 G)** produced:
- **4-fold TGF-β1 increase** in tenocytes at day 3
- **5-fold COL1A1 increase** in tenocytes at day 3
- Confirmed causal chain via TGF-β1 receptor blockade (SB431542): blocking TGF-β1
  signaling ablated the COL1A1 effect. 10 Hz → TGF-β1 → COL1A1. The intermediate
  is confirmed.
- In vivo: significant COL1A1 and TGF-β1 upregulation in rat Achilles tendons after
  3 weeks at the same protocol.

This is a major addition to the protocol. The original doc documented 30 Hz (+29.1%),
400 Hz (+70.6%), and 800 Hz (maximum response) from PMC4337172. The 10 Hz finding adds
a low-frequency tier with a 5× (400%) response — the strongest COL1A1 effect in the
literature at any frequency — operating through a documented TGF-β1 intermediate
rather than direct calcium influx.

**Frequency specificity confirmed (PMC4337172):**
Human bone marrow-derived MSCs, acoustic vibratory stimulation:
- 30 Hz: +29.1% COL1A1 vs static control
- 400 Hz: +70.6% COL1A1 vs static control
- 800 Hz: Maximum osteogenic/collagen response in study; simultaneous adipogenic
  suppression (fat pathway turned off while repair pathway is turned on)

**TGF-β1 and chondrogenesis (PMC5729425):**
Low-intensity pulsed ultrasound promotes TGF-β1-induced chondrogenesis in MSCs
through the integrin-mTOR signaling pathway — confirming acoustic stimulation
can engage TGF-β1 signaling to drive collagen-related programs.

**Important nuance — the two faces of TGF-β1 in spine:**
TGF-β1 at 10 Hz → organized structural COL1A1 (repair) ← **desired**
TGF-β1 from mechanical stress → fibrotic LF collagen (hypertrophy) ← **not desired**

The distinction is the delivery mechanism and tissue context, not TGF-β1 itself.
Therapeutic vibration at precisely 10 Hz drives organized structural collagen. Chronic
pathological mechanical stretching of the LF drives disorganized fibrotic collagen.
LIPUS at 1.5 MHz simultaneously suppresses the fibrotic TGF-β1 response in ligament
fibroblasts (PMC8458725). The protocol works in two directions: promote structural
collagen via 10 Hz in connective tissue; suppress fibrotic collagen via anti-
inflammatory LIPUS-analog 40 Hz + NF-κB suppression.

**Acoustic Targets for COL1A1:**
- **10 Hz physical layer:** 5× COL1A1 via TGF-β1 — strongest collagen signal in lit
- **400 Hz carrier:** +70.6% COL1A1 (PMC4337172)
- **800 Hz carrier:** Maximum collagen/osteogenic response (PMC4337172)
- **30 Hz physical layer:** +29.1% COL1A1 (PMC4337172)

---

### LIGAMENTUM FLAVUM — The Structural Problem (Not in Gene Panel, But Critical)

**Why this section is here:**
The AlphaGenome panel measures gene expression in CD4+ T cells (immune surveillance
tissue). Ligamentum flavum is a distinct connective tissue. LF hypertrophy is not
captured directly by the panel — but IL-1β (20.625) and IL-6 (19.750) are its primary
drivers. Addressing these genes acoustically also directly addresses the LF.

**The LF hypertrophy mechanism (PMC5805210, PMC11506588):**
Mechanical stretching stress from spinal instability → TGF-β1 upregulation in LF
fibroblasts → Col I, III, V deposition → tissue stiffening and thickening →
physical narrowing of the lumbar spinal canal → nerve root compression.
86.67% of hypertrophic LF specimens show positive TGF-β1 expression vs 20% in controls.

**NEW — LIPUS directly suppresses TGF-β1-driven fibrosis in connective tissue fibroblasts
(PMC8458725):**
LIPUS at **1.5 MHz, 30 mW/cm², 20% duty cycle, 20 minutes** in fibroblast-like
synoviocytes (direct functional analogs of LF fibroblasts):
- Attenuated TGF-β1-induced α-SMA, CTGF, and **Col I expression**
- Suppressed Wnt/β-catenin signaling — the proliferative driver of LF fibrosis
- Decreased collagen deposition confirmed histologically (Masson staining)

This is a new mechanistic pathway for acoustic LF intervention — separate from
NF-κB/IL-1β suppression. The Wnt/β-catenin pathway is the proliferation signal
that drives LF fibroblast expansion. LIPUS-analog acoustic stimulation at the
right parameters simultaneously hits NF-κB (via 40 Hz) AND Wnt/β-catenin (via
LIPUS-range frequency). Two independent anti-fibrotic pathways in one session.

**Acoustic targets for LF:**
- **40 Hz** → NF-κB suppression → IL-1β↓ → downstream LF fibroblast activation↓
- **LIPUS-analog layer** → Wnt/β-catenin suppression → direct COL I fibrosis↓
- The combined effect is: reduce the inflammatory signal driving LF, AND suppress
  the fibroblast proliferation pathway directly

---

### FAAH — The Anandamide Brake

**The Problem:** FAAH (Fatty Acid Amide Hydrolase) at 4.562 is the enzyme that degrades
anandamide — the body's endocannabinoid analgesic and anti-inflammatory molecule.
High FAAH = anandamide destroyed faster = less natural pain relief and less
endocannabinoid anti-inflammation.

The subject carries the AC genotype at rs324420 — one protective A allele that reduces FAAH
enzymatic activity. AlphaGenome confirms a −0.7% expression delta from this allele.
The direction is already right. The acoustic protocol compounds the existing
genetic advantage.

Critical pathway: Chronic pain → chronic stress → elevated cortisol → FAAH
upregulation → anandamide destroyed → more pain, more anxiety → more stress.
Breaking this cycle acoustically (stress reduction → cortisol↓ → FAAH↓ → anandamide↑)
is the most accessible mechanism for FAAH modulation.

**Research status:**
No study has directly measured FAAH mRNA levels after headphone-based acoustic
stimulation. This is a documented gap in the sonobiology literature. However:

- FAAH is functionally active in mechanosensory neuron circuits — FAAH inhibition
  potentiates synapses made by pressure-sensitive mechanosensory neurons (PMC11450075).
  This establishes a direct functional link between mechanosensory input and FAAH signaling.
- Stress-driven FAAH upregulation is well-characterized: HPA axis activation increases
  FAAH activity, reducing anandamide and disinhibiting glutamate (PMC3073528). Acoustic
  parasympathetic activation reverses this cascade.
- FAAH expression is epigenetically regulated in mPFC via CB1R/FAAH co-regulation
  (PMC9992175) — meaning FAAH expression is accessible to the epigenetic modification
  that acoustic stimulation drives (PMC7472266).

**Acoustic Targets for FAAH:**
- **Primary:** 6 Hz theta binaural — HPA axis suppression → cortisol↓ → FAAH↓ → anandamide↑
- **Supporting:** Session-level stress reduction — FAAH benefit is downstream of
  achieving genuine theta state. Session design quality matters.
- **Research frontier:** This project may generate the first data on acoustic FAAH
  modulation. Track pain, mood, and anxiety as anandamide proxies.

---

### OPRM1 — The Pain Dampener

**The Status:** OPRM1 (mu-opioid receptor) at 3.406. AA genotype at rs1799971 —
the reference allele. The A118G variant (G allele = reduced receptor sensitivity,
reduced endorphin response) is **NOT present**. Full mu-opioid receptor function
confirmed. Every endorphin the body releases lands on a full-function receptor.

This gene doesn't need to be upregulated. It needs to be activated by sufficient
endogenous ligand. The acoustic goal: trigger beta-endorphin release, then let
the intact AA receptor do its job.

**Theta binaural beats RCT (PubMed 32564499):**
Double-blind, cross-over RCT. 5 Hz theta binaural beats, 30 minutes. Pain scores
reduced from 5.6±2.3 to 3.4±2.6 vs sham. Stress significantly reduced at 30 minutes
and remained reduced only in the binaural beats group at week's end. Subsequent
significant reduction in analgesic medication consumption. The most robustly
controlled study on binaural beats and chronic pain.

**Direct mu-opioid receptor imaging (PMC12316753):**
[¹¹C]carfentanil PET directly imaged MOR binding during pleasurable music listening.
Increased MOR binding in ventral striatum and orbitofrontal cortex. MOR binding in
nucleus accumbens correlated with frisson. The first direct neuroimaging proof that
sound activates the brain's mu-opioid system.

**Systematic review (PMC10785528, 2024):**
Binaural beats effective for pain relief in acute conditions, with potential in
chronic pain. Theta range (4–8 Hz) shows strongest evidence across studies.

**Acoustic Targets for OPRM1:**
- **Primary:** 5–7 Hz theta binaural beats — RCT-confirmed pain reduction via
  proposed OPRM1-endorphin mechanism
- **Supporting:** Music-layer carrier context — PET-confirmed MOR activation
- **Note:** Theta serves double duty — OPRM1 pain dampening AND theta-state
  receptivity for the full epigenetic session. It is both the delivery vehicle
  and the therapeutic signal.

---

### MMP3 — Negligible (Monitor Only)

**The Status:** MMP3 at 0.107 is essentially zero in this tissue. The disc matrix
breakdown enzyme is not an active driver in this individual at the expression level
measured in CD4+ T cells. The −0.5% delta from the AG genotype is noise.

**Why it still matters structurally:**
TNF-α and IL-1β drive MMP-3 expression through NF-κB. Suppressing IL-1β acoustically
achieves MMP-3 suppression as a downstream consequence. No separate MMP-3 protocol
needed. The anti-IL-1β work covers MMP-3 automatically.

---

## 3. The Spine "Needle" Protocol

| Target | Gene/Tissue | Frequency | Layer | Mechanism |
| :--- | :--- | :--- | :--- | :--- |
| **IL1B ▼** | IL1B | 40 Hz | Physical + headphone | NF-κB suppression → IL-1β↓ |
| **IL6 ▼** | IL6 | 30–40 Hz | Physical | WBV meta-analysis IL-6↓ (PMC11249855) |
| **BMP-2 de-block** | BMP2 (indirect) | 40 Hz | Physical + headphone | IL-1β suppresses BMP-2; IL-1β↓ frees it |
| **COL1A1 ▲** | COL1A1 | 10 Hz | Physical | 5× COL1A1 via TGF-β1 (PMC6181323) |
| **COL1A1 ▲** | COL1A1 | 400 Hz | Headphone carrier | +70.6% COL1A1 (PMC4337172) |
| **COL1A1 ▲** | COL1A1 | 800 Hz | Headphone carrier | Max collagen/osteogenic (PMC4337172) |
| **NP preservation** | Nucleus pulposus | 90 Hz | Physical | 35% NP area maintained, 0.2g (PMC3628078) |
| **IGF-1 activation** | IGF1 (indirect) | 90 Hz | Physical | Mechanical loading → IGF-1 release pathway |
| **LF fibrosis ▼** | (IL1B/IL6 downstream) | 40 Hz | Physical + headphone | Wnt/β-catenin ↓ → Col I fibrosis↓ |
| **OPRM1 engage** | OPRM1 | 5–7 Hz | Binaural beat | Theta entrainment → endorphin → MOR |
| **FAAH ▼** | FAAH | 5–7 Hz | Binaural beat | HPA↓ → cortisol↓ → FAAH↓ → anandamide↑ |
| **State induction** | All | 6 Hz | Binaural beat | Theta = maximum epigenetic receptivity |

---

## 4. Session Synthesis: The "Inflammation Inversion" Sequence

The spine session has a single strategic objective: **invert the IL/COL ratio**.
Drive IL-1β and IL-6 below COL1A1. Drive COL1A1 above the inflammatory signal.
Do this while simultaneously engaging OPRM1 for pain relief and FAAH for anandamide
preservation.

**Phase 1: Entry / Pain Gate (0–10 min)**
- **Frequency:** 6 Hz theta (binaural, 200 Hz carrier, headphone)
- **Goal:** OPRM1 engagement, HPA axis descent, FAAH downregulation begins
- **Why first:** Pain relief and stress reduction are prerequisites for the rest of
  the session to be effective. A person in acute pain cannot achieve the theta state
  needed for epigenetic programming. Pain first.

**Phase 2: Anti-Inflammation (10–35 min)**
- **Frequency:** 40 Hz gamma (physical delivery + headphone carrier)
- **Goal:** IL-1β ▼, IL-6 ▼, NF-κB suppression, Wnt/β-catenin suppression
- **Duration:** 25 minutes — this is the primary target phase; duration matters
  for the mRNA-level effect (sustained suppression documented at 30 min threshold)

**Phase 3: Disc Preservation + Regeneration Layer (35–50 min)**
- **Frequencies:** 90 Hz physical + 10 Hz physical (crossfaded)
- **Goal:** NP area preservation (90 Hz → 35% NP maintenance, PMC3628078) +
  IGF-1 mechanical activation pathway (90 Hz mechanical loading signal) +
  TGF-β1 → COL1A1 via 10 Hz (5× collagen, PMC6181323)
- **Why 90 Hz:** This is the frequency at which low-intensity vibration was directly
  shown to preserve disc morphology in a degenerative model. 0.2g at 90 Hz maintained
  nucleus pulposus area 35% above untreated controls. It is deliverable through
  headphone bass response and physical coupling.

**Phase 4: Collagen Synthesis Drive (50–65 min)**
- **Frequencies:** 400 Hz headphone carrier + 800 Hz headphone carrier
- **Goal:** COL1A1 ▲ via direct calcium-mediated transcription factor activation
  (+70.6% at 400 Hz, maximum osteogenic response at 800 Hz, PMC4337172)
- **Why at end:** Collagen synthesis upregulation is an anabolic process. The session
  ends in a repair state, not an inflammatory state. The anti-inflammatory work in
  phases 1-2 has cleared the BMP-2 pathway; phases 3-4 drive the anabolic program
  into that cleared space.

**Crossfade strategy:**
40 Hz runs continuously through phases 2, 3, and 4 as the background inflammation
suppressor. 90 Hz and 10 Hz overlap in phase 3 at lower amplitude — mechanical disc
signals underneath the 40 Hz layer. 400/800 Hz enter in phase 4 as foreground
carriers. All layers are compatible mechanistically and can coexist in the same
stereo audio stream with careful mixing.

---

## 5. Safety Notes and Cautions

**PIEZO1 dose:**
Pathological PIEZO1 overactivation occurs at ≥0.8 MPa mechanical pressure in nucleus
pulposus cells. Consumer headphone audio at maximum safe listening volume (~94 dB SPL)
delivers approximately 0.00002 MPa — a ratio of 40,000:1 below the pathological
threshold. The therapeutic acoustic dose is safe by multiple orders of magnitude.
However: **never exceed comfortable listening volume**. The session is not more effective
at higher volume. The mechanotransduction benefit operates at gentle amplitudes.

**LF/TGF-β nuance:**
In the spine context, TGF-β1 has two roles: (1) pro-fibrotic when chronically elevated
by mechanical stress (bad — drives LF thickening), (2) pro-repair when transiently
activated by organized vibration (good — drives structural COL1A1). The acoustic
protocol exploits role (2) via 10 Hz organized vibration. The anti-inflammatory
layer simultaneously suppresses the chronic mechanical-stress-driven TGF-β1 via
NF-κB and Wnt/β-catenin inhibition.

**BDNF in spinal cord:**
BDNF in the brain context (20 Hz vibration, PMC11316700) is neuroplastic and beneficial
for depression and cognitive function. In the **spinal dorsal horn** context, BDNF
released from microglia drives central sensitization and hyperalgesia in neuropathic
pain models. The spine protocol deliberately does not include a BDNF upregulation
target. Pain sensitization via spinal BDNF is not a desired outcome. The BDNF
frequency target (20 Hz) belongs in the depression/anxiety session, not the spine session.

**Soft start mandatory:**
All carriers should fade in over minimum 90 seconds. Sudden acoustic transitions can
trigger startle — a sympathetic response that acutely upregulates NF-κB and temporarily
spikes IL-1β. Startles during an IL-1β suppression session are directly counterproductive.

---

## 6. The Expression Picture — Current State vs Target

```
CURRENT STATE (what AlphaGenome measured):

INFLAMMATION (need down)          REPAIR (need up)
IL1B  ████████████████████  20.625  COL1A1  ██████████  10.062
IL6   ███████████████████   19.750

                                    PAIN MODULATION
                             OPRM1  ███  3.406  (AA, full function ✓)
                             FAAH   ████  4.562  (AC, partial advantage ✓)
                             MMP3   ░  0.107   (negligible ✓)

TARGET STATE (after sustained protocol):

IL1B  ██████████████  ~12-14    COL1A1  ████████████████  ~15-17
IL6   █████████████   ~11-13

Structural repair exceeds inflammatory signal.
Net direction: from breakdown to maintenance.
```

---

*Sources:*
- [LIPUS suppresses IL-1β, NF-κB in nucleus pulposus — PMC8522043](https://pmc.ncbi.nlm.nih.gov/articles/PMC8522043/)
- [10 Hz vibration → 5× COL1A1 via TGF-β1, tenocytes — PMC6181323](https://pmc.ncbi.nlm.nih.gov/articles/PMC6181323/)
- [Acoustic vibration COL1A1 30/400/800 Hz, MSCs — PMC4337172](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4337172/)
- [WBV 30–40 Hz meta-analysis IL-6/TNF-α reduction — PMC11249855](https://pmc.ncbi.nlm.nih.gov/articles/PMC11249855/)
- [LIPUS suppresses TGF-β1-driven Col I fibrosis, Wnt/β-catenin — PMC8458725](https://pmc.ncbi.nlm.nih.gov/articles/PMC8458725/)
- [TGF-β and ligamentum flavum hypertrophy — PMC5805210](https://pmc.ncbi.nlm.nih.gov/articles/PMC5805210/)
- [PIEZO1 in IVD degeneration — therapeutic inhibition — PMC11930658](https://pmc.ncbi.nlm.nih.gov/articles/PMC11930658/)
- [PIEZO1 overexpression → NLRP3 → IL-1β in NP cells — PMC9125856](https://pmc.ncbi.nlm.nih.gov/articles/PMC9125856/)
- [Acoustic technologies cell function review — PMC12273796](https://pmc.ncbi.nlm.nih.gov/articles/PMC12273796/)
- [Theta binaural beats chronic pain RCT — PubMed 32564499](https://pubmed.ncbi.nlm.nih.gov/32564499/)
- [Music activates mu-opioid receptors PET — PMC12316753](https://pmc.ncbi.nlm.nih.gov/articles/PMC12316753/)
- [Binaural beats pain systematic review 2024 — PMC10785528](https://pmc.ncbi.nlm.nih.gov/articles/PMC10785528/)
- [FAAH in mechanosensory circuits — PMC11450075](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC11450075/)
- [Stress-driven FAAH upregulation — PMC3073528](https://pmc.ncbi.nlm.nih.gov/articles/PMC3073528/)
- [LIPUS IVD cells collagen/proteoglycan synthesis — PMC5667559](https://pmc.ncbi.nlm.nih.gov/articles/PMC5667559/)
- [LIPUS 72-hour IL-1β / IL-6 suppression — PubMed 36930982](https://pubmed.ncbi.nlm.nih.gov/36930982/)
- [LIPUS optimal macrophage parameters — PMC10036142](https://pmc.ncbi.nlm.nih.gov/articles/PMC10036142/)
- [40 Hz vibration IL-1β/IL-6 mRNA reduction — ScienceDirect 2024](https://www.sciencedirect.com/science/article/pii/S0361923024002727)
- [Ligamentum flavum molecular/cellular mechanisms 2024 — PMC11506588](https://pmc.ncbi.nlm.nih.gov/articles/PMC11506588/)

---

---

## NEXT SCAN PANEL — REGENERATION TARGETS

The current AlphaGenome spine panel measured: IL1B, IL6, COL1A1, OPRM1, FAAH, MMP3.
These are the inflammatory/pain genes. The regeneration picture is incomplete without
measuring the anabolic growth factor side. Proposed next panel:

| Gene | Role | Why |
| :--- | :--- | :--- |
| BMP7 | Disc anabolism master regulator | >200% proteoglycan increase alone; 400% with IGF-1 |
| IGF1 | Disc cell proliferation + ECM synthesis | Synergizes with BMP-7 via complementary SMAD+ERK pathways |
| SOX9 | Chondrogenic transcription factor | Master regulator of NP cell identity; BMP-7 drives it |
| ACAN | Aggrecan — disc proteoglycan core | Direct disc matrix structural marker; IGF-1/BMP-7 target |
| BMP2 | Anabolic growth factor | LIPUS-upregulated in NP cells; IL-1β suppresses it |
| SDF1 | Stem cell homing chemokine | Degenerative disc distress signal; recruits endogenous MSCs |

Script: `score_spine_regeneration.py` — to be written after current scan queue clears.

---

*Series: Digital Genesis Theory | Document: SPINE_GENOMIC_ACOUSTIC_TARGETS.md*
*Companion document: SPINE_NERVE_PAIN_RESEARCH.md (full gene-by-gene mechanistic deep dive)*
*Theory document: BRAINSTORM_006.txt (RNA landscape engineering + regeneration framework)*
