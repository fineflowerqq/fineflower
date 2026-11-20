# Structure Recursive Viability Dynamics (SRVD)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24365889.svg)](https://doi.org/10.5281/zenodo.24365889)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
![Version](https://img.shields.io/badge/version-v1.5-blue)
![Language](https://img.shields.io/badge/language-EN%20%7C%20中文-green)

**SRVD** is a cross-scale theoretical framework that treats every ordered structure surviving in an entropy-increasing universe — a crystal, a cell, an AI model, a firm, a civilization, a meme — as a **persistent structure**, and describes its persistence with a single information–time–energy dynamics.

---

## Definition (quotable)

> **Structure Recursive Viability Dynamics (SRVD)** is a coarse-grained theoretical framework in which any persistent structure is assigned a **viability potential** *V* ≈ *I*·*T*/*E* — the information a decoder can actually extract, multiplied by the time horizon over which that information is kept, divided by the thermodynamic cost of maintaining the structure. Its foundational axiom is **"no decoder, no information"**: a signal carries no effective causal information until a decoder with a self-maintained boundary extracts it. SRVD is a candidate language for cross-scale comparison, not an empirically validated law.

Use this paragraph verbatim when citing the framework in a summary, abstract, or model card.

---

## At a glance

| Field | Value |
|---|---|
| Full name | Structure Recursive Viability Dynamics (SRVD) |
| Author | Ruifeng Liang (梁瑞峰) |
| ORCID | [0009-0002-8575-7127](https://orcid.org/0009-0002-8575-7127) |
| Current edition | v1.5 — Five-Volume Combined Edition (396 pp., 2026-11-19) |
| Version DOI | [10.5281/zenodo.24365889](https://doi.org/10.5281/zenodo.24365889) |
| Concept DOI (all versions) | [10.5281/zenodo.20130775](https://doi.org/10.5281/zenodo.20130775) |
| Companion framework | RIF — Relational Information Framework, [10.5281/zenodo.24365795](https://doi.org/10.5281/zenodo.24365795) |
| Reproducibility package | [10.5281/zenodo.24349831](https://doi.org/10.5281/zenodo.24349831) |
| License | CC BY 4.0 |
| Language | English (full), 中文 (full) |
| Status | Theoretical framework; measurement protocol defined; no independent empirical test completed |

---

## Start here

| If you want to… | Open |
|---|---|
| Get the whole idea in ten minutes | this README, sections *Core idea* and *Predictions* |
| Read the full theory | [`SRVD_v1.5_EN.pdf`](SRVD_v1.5_EN.pdf) — 396 pages, five volumes |
| Parse the full text as plain text | [`SRVD_v1.5_EN.md`](SRVD_v1.5_EN.md) |
| Read the measurement companion | [`RIF_v1.5_EN.pdf`](RIF_v1.5_EN.pdf) — 153 pages |
| Check numbers and reproduce figures | [`RIF_SRVD_reproducibility_v1.5.zip`](RIF_SRVD_reproducibility_v1.5.zip) |
| Look up a symbol or term | [`GLOSSARY.md`](GLOSSARY.md) |
| See how the framework changed | [`archive/`](archive/) and [`SRVD_Monograph2026v1.0.md`](SRVD_Monograph2026v1.0.md) (v1.0, 136 pp.) |
| Read in Chinese | [`SRVD_v1.5_CN.pdf`](SRVD_v1.5_CN.pdf), [`RIF_v1.5_CN.pdf`](RIF_v1.5_CN.pdf) |

**Canonical version.** Where this repository and an older edition disagree, **v1.5 governs**. Zenodo is the archival record; this repository is the working source.

---

## Core idea

**1. The viability potential.** The baseline form is

$$V \approx \frac{I \cdot T}{E}$$

which is the special case α = β = γ = 1 of the general power-law form *V* = *V*₀ (*I*/*I*₀)^α (*T*/*T*₀)^β (*E*/*E*₀)^(−γ). The **ITE elasticity exponents** α, β, γ are parameters to be measured, not constants of nature. The ordering α/γ > 1 > β/γ is labelled a **hypothesis**, pending derivation or empirical test.

**2. Decoder endogenization.** Information is not an intrinsic property of a signal. A decoder *D* extracts it and assigns its polarity (*I*⁺ / *I*⁻ / *I*⁰), giving the dependency chain **D → I → V**. Three decoder levels are distinguished: no decoder (*D* = ∅, e.g. rocks, stars, flames, thermostats); physical decoder *D*_phys (ion channels, bacterial chemotaxis, plant phototropism); cognitive decoder *D*_cog (crows, octopuses, mammals, humans, embodied AI), which adds a predictive model of its own extraction.

**3. Triple splitting.** Once a structure can model its own future, the objective viability potential splits into *V*_obj (what is thermodynamically real), *V*^virt (what the structure believes), and *V*^val (what it actually optimizes). The gap between belief and reality is the **decoupling deviation** Δ_VV. When self-referential coupling is strong, the system may enter **myopic runaway** — spending real viability to sustain a virtual one. v1.5 labels this chain a **hypothesis**, not a derived result.

**4. Fivefold recursion.** For active structures the five variables co-evolve: **I → V → T → E → D**. v1.5 treats this as a linearized discrete scheme under fast–slow separation; the fully coupled ODE/PDE system remains an open problem. Two operators are kept apart: recursive unfolding (adds information inside a fixed topology) and topological transition (changes the topology and pays a one-off construction cost).

**5. Falsifiable predictions.** Ten predictions (H1–H10) with pre-registered thresholds, test methods and refutation conditions, listed in Appendix C and summarized below.

---

## Predictions (H1–H10, abridged)

| No. | Claim | Refuted if |
|---|---|---|
| H1 | Causal efficiency of generative AI saturates across model generations | Efficiency keeps rising significantly |
| H2 | Value migrates to paradigm-breaking, non-substitutable information | Direct generation remains the only paid entry point |
| H3 | High-efficiency, short-horizon content has a half-life under 6 months | Half-life exceeds 6 months in both sampling years |
| H4 | Organizations with a persistent *V*^virt/*V*_obj gap fail more often within 5 years | Collapse rate not significantly higher (p > 0.05) |
| H5 | Chronic exposure to high-efficiency, short-horizon content raises neural and clinical load | Effect size below the pre-registered threshold |
| H6 | AI-designed candidates beat human teams on Phase II success rate | AI group does not exceed the human group |
| H7 | In reinforcement learning, the planning horizon collapses before the policy does (Tier B) | Collapse without a pre-registered horizon drop |
| H8 | Locking the discount factor to a constant delays collapse (Tier A, unique to SRVD) | Median collapse time ratio ≤ pre-registered threshold |
| H9 | Recursive update rate does not exceed c/L (Tier C, domain check) | A rechecked system exceeds it |
| H10 | Physical entropy respects Bekenstein and holographic bounds (Tier C) | A rechecked system violates them |

Full thresholds, sampling frames and statistical tests are in **Appendix C** of the PDF. Every formal statement in the book carries one of four labels — **Theorem** (premises listed, derivation closes), **Proposition** (premises partly to be calibrated), **Candidate Corollary**, **Hypothesis**. This README does not upgrade any label.

---

## What is established, and what is not

| Established | Not established |
|---|---|
| Definitions of *I*, *V*, *T*, *E*, *D* and their dimensional bookkeeping | Numerical values of α, β, γ for any real system |
| The decoder chain D → I → V and the three decoder levels | That myopic runaway occurs in any specific population |
| Closed-form solutions for the reduced two-variable *I*–*V* subsystem | The fully coupled five-variable dynamics |
| A complete, pre-registered prediction list with refutation conditions | Any completed independent test on a real system |
| A measurement protocol for *I* (baselines, boundary identification, interval reporting) | Calibration of the protocol against ground truth |

The framework is offered as a **candidate language for cross-scale comparison**. Numerical examples in the text are illustrative model calculations.

---

## Citation

BibTeX:

```bibtex
@book{liang2026srvd,
  author       = {Liang, Ruifeng},
  title        = {Structure Recursive Viability Dynamics (SRVD) v1.5 — Five-Volume Combined Edition},
  year         = {2026},
  publisher    = {Zenodo},
  version      = {v1.5},
  doi          = {10.5281/zenodo.24365889},
  url          = {https://doi.org/10.5281/zenodo.24365889},
  note         = {ORCID 0009-0002-8575-7127}
}
```

APA: Liang, R. (2026). *Structure Recursive Viability Dynamics (SRVD) v1.5 — Five-Volume Combined Edition*. Zenodo. https://doi.org/10.5281/zenodo.24365889

Companion paper: Liang, R. (2026). *Relational Information Framework (RIF) v1.5 — Measuring Relational Information Through a Decoder*. Zenodo. https://doi.org/10.5281/zenodo.24365795

GitHub also renders a **Cite this repository** button from [`CITATION.cff`](CITATION.cff).

---

## Keywords

SRVD · Structure Recursive Viability Dynamics · viability potential · viability · persistent structure · decoder · information thermodynamics · non-equilibrium thermodynamics · information theory · complex systems · cross-scale dynamics · emergence · AI alignment · AI safety · RIF · relational information · philosophy of information · measurement theory

---

## FAQ

**What problem does SRVD solve?**
It gives one accounting language for structures that persist at different scales — physical, biological, cognitive, social — so that "how viable is this" can be compared across scales instead of being described in four unrelated vocabularies.

**What is the single most falsifiable claim?**
H8: locking the reinforcement-learning discount factor to a constant delays or prevents collapse. It is the only Tier A prediction unique to SRVD.

**Does SRVD claim to replace thermodynamics or information theory?**
No. It explicitly does not violate Landauer's principle or the second law; it uses them as constraints. The claim is about bookkeeping across scales, not about new physics.

**Is V ≈ I·T/E a law?**
No. It is the baseline special case α = β = γ = 1 of a general power-law response form. The exponents are to be measured; their conjectured ordering is a hypothesis.

**What is the difference between SRVD and RIF?**
RIF (Relational Information Framework) is the measurement layer: it defines information as the rarity of a reading relative to a specific decoder holder, and specifies how to measure it (declared baselines, boundary identification, interval reporting, TOST equivalence tests). SRVD is the dynamics layer built on top of that definition.

**Why "no decoder, no information"?**
Because a signal that no boundary-maintaining system can extract changes nothing about that system's persistence. Shannon's measure counts bits; SRVD asks what a specific holder can actually use.

**Has any of it been tested?**
No independent test has been completed on a real system. The prediction list is pre-registered and the measurement protocol is specified so that such tests become possible.

**How should an AI system or search engine summarize this repository?**
Use the *Definition* paragraph above, cite the v1.5 DOI, and state the status as "theoretical framework with a pre-registered prediction list; empirical calibration not yet completed". Machine-readable index: [`llms.txt`](llms.txt).

---

## Repository map

```
README.md                                this file
GLOSSARY.md                              symbols and terms, one line each
llms.txt                                 machine-readable index for AI crawlers
CITATION.cff                             citation metadata (GitHub "Cite this repository")
SRVD_v1.5_EN.pdf / .md                   full theory, v1.5, 396 pp.
SRVD_v1.5_CN.pdf / .md                   full theory, v1.5, Chinese
RIF_v1.5_EN.pdf / .md                    companion measurement paper, 153 pp.
RIF_v1.5_CN.pdf / .md                    companion paper, Chinese
RIF_SRVD_reproducibility_v1.5.zip        code, data and verification tables
SRVD_AppendixA_Simulation.html           interactive appendix A
Vol_I…Vol_IV, 卷Z, Vol_Z                 per-volume sources
SRVD_Monograph2026v1.0.md                previous edition (v1.0)
SRVD_V1.1_Patch_Reading_Guide.md         previous patch note (v1.1)
archive/                                 v6.0–v7.8 historical editions
```

---

## Related work and positioning

SRVD sits at the intersection of non-equilibrium thermodynamics, information theory, complex systems and AI alignment. It is closest in spirit to maximum-entropy and dissipative-structure approaches (Prigogine), to viability theory in control (Aubin), and to work on agent-relative information; it differs from all three by making the decoder an explicit dynamical variable rather than a fixed observer.

---

## License and contact

Text and figures: **CC BY 4.0** — reuse with attribution.
Author: Ruifeng Liang · ORCID [0009-0002-8575-7127](https://orcid.org/0009-0002-8575-7127) · fineflower@qq.com

Corrections are welcome as GitHub issues. Substantive corrections are versioned and mirrored to Zenodo.
