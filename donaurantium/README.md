# Donaurantium

Open-source acoustic epigenetics research platform.

Eight standalone browser-based session players deliver binaural beats, isochronic tones,
and physical mechanotransduction tones targeting documented genomic pathways for anxiety,
depression, spinal stenosis, and general wellness. No server. No build step. No external
dependencies. Open one HTML file and run a full session.

**Protocols:** Anxiety · Depression · Spinal Stenosis · General Wellness  
**Delivery:** Stereo headphones required (binaural variants) · Any speakers (isochronic variants)  
**Open for replication:** Yes — all code, protocols, and research published openly

---

## Quick Start

1. Clone or download the repo
2. Open any file from `versions/` directly in a browser
3. Read the seizure warning, choose your session length, put on headphones
4. See `docs/DISCLAIMER.md` before first use

No installation. No internet connection required after download.

---

## Project Structure

```
donaurantium/
├── README.md
├── docs/
│   ├── DISCLAIMER.md                          Safety info + mechanism honesty
│   ├── ESTIMATES_OF_POTENTIAL_PROGRESS.md     Research-backed 7/30/60/90-day timeline
│   ├── HTML_IMPLEMENTATION_NOTES.md           Full technical spec for all 8 players
│   ├── claudes-thoughts.md                    Honest reflection on the project
│   ├── ANXIETY_GENOMIC_ACOUSTIC_TARGETS.md
│   ├── ANXIETY_RESEARCH.md
│   ├── SPINE_GENOMIC_ACOUSTIC_TARGETS.md
│   ├── SPINE_NERVE_PAIN_RESEARCH.md
│   ├── DEPRESSION_CALMING_RESEARCH.md
│   ├── GENERAL_HEALTH_RESEARCH.md
│   ├── AUDIO_MECHANOSENSORY_RESEARCH.md
│   ├── AUDIO_TECHNIQUES_REFERENCE.md
│   ├── UNIFIED_PROTOCOL_RESEARCH.md
│   ├── VISUAL_PROTOCOL.md
│   ├── SURGICAL_FREQUENCY_PROTOCOL.md
│   ├── WHAT_WERE_ACTUALLY_BUILDING.txt
│   └── BRAINSTORM_001-006.txt                 Design reasoning papers
└── versions/
    ├── donaurantium-anxiety-headphones.html
    ├── donaurantium-anxiety-stereo.html
    ├── donaurantium-depression-headphones.html
    ├── donaurantium-depression-stereo.html
    ├── donaurantium-spinal-stenosis-headphones.html
    ├── donaurantium-spinal-stenosis-stereo.html
    ├── donaurantium-general-improvement-headphones.html
    └── donaurantium-general-improvement-stereo.html
```

---

## The Science in One Paragraph

Sound waves physically deform cell membranes. PIEZO1 and TRPV4 ion channels open in
response. Calcium floods the cell. Calcium-sensitive kinases activate transcription
factors. Transcription factors enter the nucleus and change which genes are read. mRNA
levels shift. Protein levels change. Cellular behavior changes. This chain is documented
in peer-reviewed literature including a 2025 Nature Communications Biology study
confirming 42–145 differentially expressed genes from acoustic exposure (PMC12003795).
Donaurantium uses this cascade deliberately, with specific frequency targets for specific
genes derived from AlphaGenome RNA-seq data and published research.

---

## What Each Session Delivers

| Feature | Details |
|---|---|
| Binaural beats | L/R channel split → SOC difference tone → FFR cortical entrainment |
| Isochronic tones | Amplitude-gated carrier → CAEP entrainment, works on any speakers |
| Physical mechanotransduction | Sub-bass tones (20–400 Hz) targeting PIEZO1/TRPV4 |
| GENUS protocol | 40 Hz combined audio + visual → PV+ interneuron activation |
| Biological drift | ±3% LFO per layer (56–91s period) — prevents neural habituation |
| Harmonic reinforcement | 1.5× harmonic at 18% amplitude for sub-300 Hz layers |
| WebGL fractal | Julia set phase-locked to session frequency, GPU-rendered |
| Logarithmic fade-in | 90–120s ramp (FKBP5 startle-sensitivity motivated) |
| Intensity slider | 0.5×–1.8× physical layer gain scaling |
| Breath pacing cue | 5/min at theta, 6/min at higher frequencies |
| Session logging | Local CSV via browser download |

---

## Protocol Targets

**Anxiety** — 6 Hz theta, 40 Hz GENUS, pink noise  
Primary: FKBP5 methylation + HPA axis downregulation via sustained theta state

**Depression** — 6 Hz theta + 40 Hz gamma coupling, GENUS  
Primary: DRD3/IL1B/IL6 suppression, theta-gamma coupling for mood circuit entrainment

**Spinal Stenosis** — 10/30/400/800 Hz COL1A1, 90 Hz NP, 40 Hz GENUS  
Primary: COL1A1 collagen synthesis, neuroinflammation reduction, HPA pain modulation  
Note: BDNF (20 Hz) is intentionally excluded — spinal dorsal horn BDNF is pro-nociceptive

**General Wellness** — 6 Hz theta, 40 Hz GENUS, 20 Hz BDNF, pink noise  
Primary: Broad HPA regulation, BDNF upregulation, neuroinflammatory baseline reduction

---

## Mechanism Honesty

Donaurantium is built on a documented design constraint: distinguish what is proven from
what is extrapolated from what is speculative.

- **Confirmed in humans:** FFR/CAEP cortical entrainment, FKBP5 methylation from
  sustained meditation (theta proxy), GENUS protocol early human signals
- **Extrapolated:** Meditation literature standing in for acoustic theta; in-vitro
  mechanotransduction mechanisms applied to headphone delivery
- **Speculative:** Whether headphone SPL is sufficient to drive meaningful PIEZO1
  activation in deep tissue in vivo; structural disc repair at 90 days

See `docs/DISCLAIMER.md` and `docs/ESTIMATES_OF_POTENTIAL_PROGRESS.md` for full detail.

---

## Safety

- Use comfortable, conversational-level volume only
- Headphones variant requires stereo headphones — binaural beats collapse on speakers
- Do not use the visual layer if you have photosensitive epilepsy or seizure history
- Full contraindications list in `docs/DISCLAIMER.md`
- This is not a medical device, treatment, or cure

---

## Status

- [x] Theoretical framework (BRAINSTORM_001–006)
- [x] AlphaGenome genomic panels — anxiety, depression, spine, general
- [x] All 8 session players — fully implemented and audited
- [x] Biological drift, harmonic reinforcement, logarithmic fade-in
- [x] WebGL Julia set fractal renderer
- [x] GENUS 40 Hz audio + visual protocol
- [x] BDNF exclusion from all spinal variants (confirmed clean)
- [x] Full documentation suite
- [x] Personal details stripped — ready for open release
- [ ] Community replication data
- [ ] Biomarker tracking results (90-day)

---

## License

MIT. Provided as-is for research and self-experimentation purposes.
See `docs/DISCLAIMER.md` for full terms.

---

*The Donaurantium Project | 2026-05-23*  
*"Not coding new DNA. Changing which existing DNA gets read."*
