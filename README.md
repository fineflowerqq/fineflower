# Structure Recursive Viability Dynamics (SRVD) – A Unified Accounting Ledger for All Ordered Structures in an Entropy-Increasing Universe

[![SRVD v1.5 DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24365889.svg)](https://doi.org/10.5281/zenodo.24365889) [![RIF v1.5 DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24365795.svg)](https://doi.org/10.5281/zenodo.24365795) [![Reproducibility package](https://zenodo.org/badge/DOI/10.5281/zenodo.24349831.svg)](https://doi.org/10.5281/zenodo.24349831) [![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

---

## 📖 One-Sentence Summary

**SRVD** is a cross-scale, macroscopic, coarse-grained framework that brings all persistent structures — crystals, living systems, AI models, civilizations, memes — under one information–time–energy description. Its axiom: **without a decoder, there is no information (as effective causal information).**

**Core measure**: the viability potential $V$. The single-channel baseline

$$V \approx \frac{I \cdot T}{E}$$

is the special case $\alpha=\beta=\gamma=1$ of the general coarse-grained response form, and is **not** the definition of $V$:

$$V = V_0 \left(\frac{I}{I_0}\right)^{\alpha} \left(\frac{T}{T_0}\right)^{\beta} \left(\frac{E_{\mathrm{eff}}}{E_0}\right)^{-\gamma}$$

The elasticity exponents $\alpha,\beta,\gamma$ are retained as parameters to be determined. The ordering $\alpha/\gamma>1>\beta/\gamma$ is a **qualitative conjecture (Hypothesis)**, awaiting derivation or empirical test; it is not presented as an established law.

> **Terminological note**: $I$ in the formulas means **net effective causal information** $I_{\mathrm{net}}$, a declared weighted composition of two channels:
> $$I_{\mathrm{net}} = \varphi_{\mathrm{s}} I_{\mathrm{struct}} + \varphi_{\mathrm{c}} I_{\mathrm{causal}}, \qquad \varphi_{\mathrm{s}}=\frac{E_{\mathrm{struct}}}{E_{\mathrm{eff}}},\quad \varphi_{\mathrm{c}}=\frac{E_{\mathrm{causal}}}{E_{\mathrm{eff}}},\quad \varphi_{\mathrm{s}}+\varphi_{\mathrm{c}}=1.$$
> This is an energy-share weighting, a modeling convention, not an additivity theorem.

**Version Statement**: This repository hosts the current **v1.5** editions of SRVD (five-volume combined edition) and of the companion **Relational Information Framework (RIF)**, together with the v1.5 reproducibility package. The earlier V1.0 Monograph and V1.1 Patch are retained under *Previous editions* for traceability; where substantive conflicts exist, **v1.5 governs**.

---

## 🧭 Core Innovations and Main Contents (v1.5)

SRVD's core innovation has **two parts**:

1. **A candidate cross-scale metric language** — the two-channel definition of the viability potential and its low-order coarse-grained baseline $V\approx I\cdot T/E$.
2. **A driving-layer meta-postulate** — under given constraints, the structures that are retained have a viability potential no lower than those that are eliminated (selection layer: purposeless, refutable by statistical observation); for active-phase structures, $\max V^{\mathrm{val}}$ is at the same time the direction actually optimized (objective layer: purposive, refutable by the direction of strategy drift). The two layers must not be conflated.

> The sentence "all other mechanisms are merely local strategies" does **not** hold: at the level of local strategy, which route to take is a real choice; the selection layer does not change the standard, it only selects among the consequences of these choices.

v1.5 has **four main contents**, summarized below.

### 1. Endogenization of the decoder

The value of information is not an intrinsic property of the signal; it is extracted by the decoder $D$, which also assigns its polarity ($I^{+}/I^{-}/I^{0}$). The dependency chain is

$$D \longrightarrow I \longrightarrow V, \qquad I_{\mathrm{active}} = \eta_D \cdot I_{\mathrm{latent}}.$$

Decoders come in **three levels**, not two:

| | No decoder $D=\varnothing$ | Physical decoder $D_{\mathrm{phys}}$ | Cognitive decoder $D_{\mathrm{cog}}$ |
|---|---|---|---|
| **Criterion** | No self-maintained boundary | Selective extraction with a self-maintained boundary, serving the persistence of the structure behind that boundary | A predictive model superimposed on $D_{\mathrm{phys}}$, able to model its own extraction mode |
| **Typical instances** | Rocks, crystals, stars, flames, thermostats | Ion channels, bacterial chemotaxis, plant phototropism; bacteria, plants, fungi, lower animals | Crows, octopuses, mammals, humans, embodied AI |
| **Efficiency** | — | $\eta_D$ low and roughly constant | $\eta_D>0$; can rise with learning |
| **Time horizon** | — | $T_{\mathrm{pred}}$ pinned to $T_{\mathrm{min}}$ | $T_{\mathrm{pred}}$ extendable (endogenous horizon) |

- **Static vs. dynamic $D_{\mathrm{phys}}$**: static — selection rules fixed by a long historical process (ion channels, dormancy switches); dynamic — real-time feedback comparing "now" with "a moment ago" (bacterial chemotaxis, plant phototropism).
- **$D_{\mathrm{cog}}$ is a continuous spectrum**, not a binary switch; its three axes are history dependence, persistence coupling, and plasticity time scale, with self-reference as a fourth, currently conceptual, axis. The **embodied region** (bacteria, mimosa, plant tropisms) lies inside the decoding-complexity space but **below $D_{\mathrm{cog}}$**, and is recorded as $D_{\mathrm{phys}}$; the **online region** covers crows, octopuses, most mammals; the **symbolic region** covers humans and some AI.

Structures without a self-maintained boundary — rocks, crystals, stars, flames, thermostats — have **no decoder at all** ($D=\varnothing$) and never enter the $D_{\mathrm{cog}}$ spectrum. A thermostat is not $D_{\mathrm{phys}}$: what it maintains is the user's comfort, not its own boundary.

### 2. Triple splitting of the viability potential

For the objective viability potential, $V_{\mathrm{obj}}=V_{\mathrm{s}}+V_{\mathrm{c}}$ is a **bookkeeping decomposition**; its aggregation operator is still to be determined, and the objective value is accounted relative to the public reading protocol $D_{\mathrm{macro}}$. Once $T_{\mathrm{pred}}$ can regulate itself, the system further distinguishes:

| Variable | Meaning | Status |
|---|---|---|
| $V_{\mathrm{obj}}$ | Objective viability potential | Thermodynamically real value, cannot be deceived |
| $V^{\mathrm{virt}}$ | Virtual viability potential | The system's internal estimate of $V_{\mathrm{obj}}$ |
| $V^{\mathrm{val}}$ | Value viability potential | $V^{\mathrm{val}}=w_{\mathrm{s}}V_{\mathrm{s}}^{\mathrm{virt}}+w_{\mathrm{c}}V_{\mathrm{c}}^{\mathrm{virt}}$, $w_{\mathrm{s}}+w_{\mathrm{c}}=1$; what the system actually optimizes |

The splitting itself is neutral and is a necessary condition for higher-order cognition. After it there are at least two paths, distinguished by the decoupling deviation $\Delta_{\mathrm{VV}}=\lvert V^{\mathrm{virt}}-V_{\mathrm{obj}}\rvert$ and the self-referential coupling strength $\chi$.

**Path one — learning against noise (explicit solution).** Under the premises $I_{\mathrm{net}}$ constant, $\sigma$ constant and exogenous, and $\alpha_{\mathrm{L}}I_{\mathrm{net}}>0$:

$$\frac{\mathrm{d}\Delta_{\mathrm{VV}}}{\mathrm{d}t} = -\alpha_{\mathrm{L}} I_{\mathrm{net}} \Delta_{\mathrm{VV}} + \sigma, \qquad
\Delta_{\mathrm{VV}}(t) = \frac{\sigma}{\alpha_{\mathrm{L}}I_{\mathrm{net}}} + \left(\Delta_0-\frac{\sigma}{\alpha_{\mathrm{L}}I_{\mathrm{net}}}\right)e^{-\alpha_{\mathrm{L}}I_{\mathrm{net}}t}.$$

The deviation converges to the bounded equilibrium $\Delta^{*}_{\mathrm{VV}}=\sigma/(\alpha_{\mathrm{L}}I_{\mathrm{net}})$. With a pre-registered tolerance $\delta_{\mathrm{tol}}$, the critical information quantity is

$$I_{\Delta,\mathrm{crit}} = \frac{\sigma}{\alpha_{\mathrm{L}}\delta_{\mathrm{tol}}};$$

below it the equilibrium deviation exceeds tolerance, and the system cognitively loses an accurate model of its environment.

**Path two — myopic runaway (Hypothesis).** When self-referential coupling is strong enough, the system may spend objective viability potential to sustain extreme values of the virtual potential: $V^{\mathrm{virt}}$ inflates, $V^{\mathrm{val}}$ is hijacked, $T_{\mathrm{pred}}$ collapses toward $T_{\mathrm{min}}$, and objective stock is irreversibly destroyed. In v1.5 this whole causal chain is labeled **Hypothesis**, and it can be activated only in the symbolic region. Two cautions from the text:

- $\chi_{\mathrm{c}}$ is the **saddle-node threshold of the simplified $I$–$V$ subsystem** (Eq. I-5.13, computed from $\alpha_{\mathrm{eff}}$ and $\kappa$); it is **not** the separate model parameter $\lambda$.
- The statement "$\chi>\chi_{\mathrm{c}}\Rightarrow\Delta_{\mathrm{VV}}$ amplifies" is **not derived** by the current model: with $I_{\mathrm{net}}$ constant, Eq. (I-5.14) gives an equilibrium deviation that *decreases* with $I_{\mathrm{net}}$. The endogenous source term required for path two is an explicit closure assumption awaiting calibration.

### 3. Fivefold recursion

The core architecture for active-phase evolution is the coupling chain $I\to V\to T\to E\to D$. v1.5 treats it as a **heuristic discrete model awaiting rigorization**, linearized under a fast–slow time-scale separation; a fully bidirectionally coupled ODE/PDE system remains an open problem. Passive structures do not activate this architecture and degenerate to static estimation of $V$.

Two operators must not be mixed: $\mathcal{F}$ (recursive unfolding) adds information within a given topology and is capacity-bounded; $\mathcal{T}$ (topological transition) changes the topology itself, pays $E_{\mathrm{build}}$ once and resets the capacity. Saturation of $\mathcal{F}$ does not imply that $\mathcal{T}$ occurs.

### 4. A family of falsifiable predictions

v1.5's complete list is **H1–H10** (Appendix C), with pre-registered thresholds, test methods and refutation conditions. Tier A (unique to SRVD) is H8; H7 has been **demoted to Tier B**; H9–H10 are Tier C domain-boundary checks. See the table below.

---

## 🔬 Falsifiable Predictions (H1–H10)

Here $\mathcal{Z}_{\mathrm{e}}\equiv I_{\mathrm{causal}}/E_{\mathrm{causal}}$ (bit/J) is the **causal efficiency coefficient**, a proportional proxy for $V_{\mathrm{c}}$ at fixed $T_{\mathrm{causal}}$.

| No. | Mechanism | Prediction (abridged) | Refutation condition (abridged) |
|---|---|---|---|
| **H1** | Marginal vanishing of $I_{\mathrm{net}}$; saturation of $\mathcal{Z}_{\mathrm{e}}$ | Generative-AI $\mathcal{Z}_{\mathrm{e}}$ stops growing across versions; when AI-generated share of training data is $\ge30\%$, output diversity falls nonlinearly by $>10\%$/year; enterprises pay a superlinear premium for high-paradigm-breaking tiers | Ratings still grow significantly; diversity decline $<5\%$; or high-$I_{\mathrm{orig}}$ tier has no premium ($\le2\times$ ordinary) |
| **H2** | High-$\mathcal{Z}_{\mathrm{e}}$ breakout via $I_{\mathrm{orig}}$ substitutes | "Fine-tuning on personal data" or "limited-edition unique generation" becomes a core paid feature | Direct generation remains the main entry; no personalized/limited-edition feature or no paid premium |
| **H3** | Rigid trade-off between $\mathcal{Z}_{\mathrm{e}}$ and $T_{\mathrm{pred}}$ | Top-content half-life $<6$ months on high-$\mathcal{Z}_{\mathrm{e}}$, low-$T_{\mathrm{pred}}$ platforms, versus $>3$ years on high-$T_{\mathrm{pred}}$ platforms; at least one $>300$M-DAU platform puts return-visit weight above completion | Half-life $>6$ months in both sampling years; or no platform adjusts weights (completion–7-day return correlation $\le0.3$) |
| **H4** | $V^{\mathrm{virt}}$ decoupling and $E_{\mathrm{causal}}$ inflation | Organizations whose $V^{\mathrm{virt}}$ persistently decouples from $V_{\mathrm{obj}}$ collapse within 5 years significantly more often; per-DAU inference cost of top content platforms rises $>40\%$ | Collapse rate not significantly higher ($p>0.05$); or per-DAU cost rise $<20\%$ |
| **H5** | $E_{\mathrm{decode}}$ neural dissipation | Long exposure to high-$\mathcal{Z}_{\mathrm{e}}$, low-$T_{\mathrm{pred}}$ content raises insular-cortex activation by 2 SD; depression risk is $2.5\times$ higher for $>60$ weak-tie interactions/day than for $<15$ | Cohen's $d<0.8$; or risk ratio $\mathrm{HR}<2.0$ |
| **H6** | $I_{\mathrm{net}}$ density transition | AI-designed candidate molecules' Phase II success rate exceeds human expert teams for the first time | AI-group success rate $\le$ human group |
| **H7** | Reinforcement learning: the horizon collapses first (**Tier B**) | Before collapse, $\gamma_{\mathrm{RL}}$ shows a cliff-like drop, judged by either (a) a drop of $>30\%$ within 3 episodes, or (b) a pre-registered trend test corrected for autocorrelation and multiplicity reaching significance, with the calibrated FPR reported | Collapse occurs with no $>30\%$ drop **and** the corrected trend test is not significant |
| **H8** | Reinforcement learning: locked time recursion (**Tier A**) | Locking $\gamma_{\mathrm{RL}}$ to a constant delays or prevents collapse | Median-collapse-time ratio $\le$ pre-registered $r^{*}$, with confidence interval containing 1 |
| **H9** | Physics: causal-propagation upper bound (**Tier C**) | Under the stated operationalization, the recursive update rate does not exceed $c/L$ | A system is found with a recursive update rate exceeding $c$ (independently rechecked) |
| **H10** | Physics: entropy bound (**Tier C**) | Under specified region, radius/area and energy definitions, physical entropy does not exceed the Bekenstein and holographic bounds | An independently rechecked system still violates either bound |

> Thresholds are pre-registration examples, not universal constants. H9–H10 test the domain of applicability, not the core mechanism; a violation requires rechecking measurement basis, boundaries and unit conversions first.

**Evidence-level convention.** v1.5 labels every formal statement as **Theorem** (premises fully listed, derivation closes), **Proposition** (formal statement with premises partly to be calibrated), **Candidate Corollary** (derived under additional conditions, not independently tested), or **Hypothesis** (empirical or mechanistic conjecture). This README keeps those labels and does not upgrade them.

---

## 📚 Repository Contents

### Current release — v1.5 (19 November 2026)

| File | Language | Description |
|---|---|---|
| `SRVD_v1.5_EN.pdf` / `SRVD_v1.5_EN.md` | English | **Structure Recursive Viability Dynamics (SRVD) v1.5 — Five-Volume Combined Edition.** Current normative edition of the framework. |
| `SRVD_v1.5_CN.pdf` / `SRVD_v1.5_CN.md` | 中文 | SRVD v1.5 五卷合订本（中文版）。 |
| `RIF_v1.5_EN.pdf` / `RIF_v1.5_EN.md` | English | **Relational Information Framework (RIF) v1.5 — Measuring Relational Information Through a Decoder.** Companion volume; supplies the measurement-layer treatment of information that SRVD adopts at the conceptual level. |
| `RIF_v1.5_CN.pdf` / `RIF_v1.5_CN.md` | 中文 | RIF v1.5（中文版）。 |
| `RIF_SRVD_reproducibility_v1.5.zip` | — | Simulation scripts, result files, and verification tools for the numerical appendices (RIF App. C; SRVD Vol. I App. F and G), with `SHA256SUMS`. |

**Recommended reading order**

1. `SRVD_v1.5_EN.pdf` (or `SRVD_v1.5_CN.pdf`) — the framework itself.
2. `RIF_v1.5_EN.pdf` (or CN) — how relational information is measured through a decoder.
3. `RIF_SRVD_reproducibility_v1.5.zip` — reproduce the appendix numbers before relying on them.

### Previous editions — v1.0 / v1.1

| File | Description |
|---|---|
| `SRVD_V1.1_Patch_Reading_Guide.md` | V1.1 patch: reading guide, errata, and boundary completions. Zenodo: [10.5281/zenodo.22027891](https://doi.org/10.5281/zenodo.22027891). |
| `SRVD_Monograph2026v1.0.md`, `结构递归存续动力学SRVD专著1.0.md` | V1.0 monograph, English / Chinese. Zenodo: [10.5281/zenodo.21322552](https://doi.org/10.5281/zenodo.21322552). |
| `Vol_I_SRVD_paper_v7.8_EN.md`, `Vol_II_…`, `Vol_III_…`, `Vol_IV_…`, `Vol_Z …` | V1.0 five-volume sources (English). |
| `卷Ⅰ_SRVD_结构递归存续动力学v7.8.md`, `卷Ⅱ_…`, `卷Ⅲ_…`, `卷Ⅳ_…`, `卷Z_…` | V1.0 five-volume sources (Chinese). |
| `SRVD_AppendixA_Simulation.html` | Appendix A simulation walkthrough. |
| `archive/` | Historical manuscripts v6.0–v7.6, kept for traceability. |

> The five-volume display names used in earlier revisions remain valid for the `Vol_*` files: Volume I — Theoretical Core; Volume II — Evolution of Persistent Structures; Volume III — Compressed Intelligence and Cognitive Evolution; Volume IV — Decoder Game Theory and Alignment Engineering; Volume Z — Reality-Mapping Dictionary.

---

## 📝 Citation

If this framework is useful to your research, please cite the current versions:

**SRVD v1.5**
> LiangRuifeng. (2026). *Structure Recursive Viability Dynamics (SRVD) v1.5 — Five-Volume Combined Edition*. Zenodo. https://doi.org/10.5281/zenodo.24365889

**RIF v1.5**
> LiangRuifeng. (2026). *Relational Information Framework (RIF) v1.5 — Measuring Relational Information Through a Decoder*. Zenodo. https://doi.org/10.5281/zenodo.24365795

**Reproducibility package**
> LiangRuifeng. (2026). *Reproducibility package for Relational Information Framework (RIF) v1.5 and Structure Recursive Viability Dynamics (SRVD) v1.5*. Zenodo. https://doi.org/10.5281/zenodo.24349831

**Earlier versions** (only when citing the historical edition):
> LiangRuifeng. (2026). *Structure Recursive Viability Dynamics — SRVD Monograph v1.0*. Zenodo. https://doi.org/10.5281/zenodo.21322552
>
> LiangRuifeng. (2026). *SRVD_Patch_V1.1_ReadingGuide* (SRVD V1.1 Patch: Reading Guide, Errata, and Boundary Completion). Zenodo. https://doi.org/10.5281/zenodo.22027891

**BibTeX**
```bibtex
@misc{liangruifeng_srvd_v15_2026,
  author = {LiangRuifeng},
  title = {Structure Recursive Viability Dynamics (SRVD) v1.5 -- Five-Volume Combined Edition},
  year = {2026},
  doi = {10.5281/zenodo.24365889},
  url = {https://github.com/fineflowerqq/fineflower}
}

@misc{liangruifeng_rif_v15_2026,
  author = {LiangRuifeng},
  title = {Relational Information Framework (RIF) v1.5 -- Measuring Relational Information Through a Decoder},
  year = {2026},
  doi = {10.5281/zenodo.24365795},
  url = {https://github.com/fineflowerqq/fineflower}
}
```

**License**: text and figures are released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); code in the reproducibility package is released under the terms stated in its `LICENSE.md`.

---

**In an entropy-increasing universe, keep every ordered structure on the same ledger.**
