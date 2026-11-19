# Structure Recursive Viability Dynamics (SRVD) – A Unified Accounting Ledger for All Ordered Structures in an Entropy-Increasing Universe

[![SRVD v1.5 DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24365889.svg)](https://doi.org/10.5281/zenodo.24365889) [![RIF v1.5 DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24365795.svg)](https://doi.org/10.5281/zenodo.24365795) [![Reproducibility package](https://zenodo.org/badge/DOI/10.5281/zenodo.24349831.svg)](https://doi.org/10.5281/zenodo.24349831) [![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

---

## 📖 One-Sentence Summary

**SRVD** is a cross-scale macro-coarse-grained theoretical framework. It brings all "persistent structures"—crystals, life, AI models, civilizations, and memes—onto the same thermodynamic ledger, using three scarce resources—**information**, **time**, and **energy**—to provide a unified answer to one fundamental question:

> **How does an ordered structure persist, climb in complexity, and spiral into runaway collapse?**

**Core Milestone Formula (Reference Baseline)**:

$$V \approx \frac{I \cdot T}{E}$$

**Viability Potential = (Information × Persistence Time) / Equivalent Thermodynamic Cost**

$V$ measures: the integral of causally ordered quantity per unit of thermodynamic cost. This is the "minimal-viability postulate" of the SRVD framework—not a physical law derived from first principles, but an axiom-level low-order approximation fixed jointly by three structural requirements: non-substitutability, symmetric contribution of the three variables, and first-order separability.

> **Terminological Note**: $I$ in the formula above represents **Net Effective Causal Information (coarse-grained baseline quantity)**. Its precise decomposition is $I_{\mathrm{net}} = w_s \cdot I_{\mathrm{struct}} + w_c \cdot I_{\mathrm{causal}}$ (where $w_s = E_{\mathrm{structure}}/E_{\mathrm{eff}}$, $w_c = E_{\mathrm{causal}}/E_{\mathrm{eff}}$, strictly determined by the system's underlying thermodynamics). See Core Fingerprint FP‑5 and the *Reading Guide* for details.

**Version Statement**: This repository hosts the current **v1.5** editions of SRVD (five-volume combined edition) and of the companion **Relational Information Framework (RIF)**, together with the v1.5 reproducibility package. The earlier V1.0 Monograph and V1.1 Patch are retained under *Previous editions* for traceability; where substantive conflicts exist, **v1.5 governs**.

---

## 🚀 Five Core Theoretical Fingerprints

These five fingerprints are SRVD's **hard innovations** that distinguish it from other general frameworks (FEP, Dissipative Structures, Goodhart's Law)—each with falsifiable empirical predictions.

### FP‑1: Primacy of the Decoder – "No Decoder, No Information"

Information is not an intrinsic property of the signal itself; it is what remains after a signal has passed through a **decoder ($D$)**:

$$I_{\mathrm{active}} = \eta_D \cdot I_{\mathrm{latent}}$$

The dependency chain is defined as:

$$D \longrightarrow I \longrightarrow V$$

Any discussion of "information value" that has not first specified its decoder is, within SRVD, considered an unfinished definition.

**Three-Level Structure of Decoders**:

| | No decoder $D=\varnothing$ | Physical decoder $D_{\mathrm{phys}}$ | Cognitive decoder $D_{\mathrm{cog}}$ |
|---|---|---|---|
| **Criterion** | No self-maintained boundary | Selective extraction with a self-maintained boundary, serving the persistence of the structure behind that boundary | A predictive model superimposed on $D_{\mathrm{phys}}$, able to model its own extraction mode |
| **Typical instances** | Rocks, crystals, stars, flames, thermostats | Ion channels, bacterial chemotaxis, plant phototropism; bacteria, plants, fungi, lower animals | Crows, octopuses, mammals, humans, embodied AI |
| **Efficiency** | — | $\eta_D$ low and roughly constant | $\eta_D > 0$; can rise with learning |
| **Time Horizon** | — | $T_{\mathrm{pred}}$ pinned to $T_{\mathrm{min}}$ | $T_{\mathrm{pred}}$ extendable (endogenous horizon) |

**Static vs. dynamic $D_{\mathrm{phys}}$**: static — selection rules fixed by a long historical process (ion channels, dormancy switches); dynamic — real-time feedback comparing "now" with "a moment ago" (bacterial chemotaxis, plant phototropism).

**Continuous Spectrum of the Cognitive Decoder** (not a binary switch; three axes: history dependence, persistence coupling, plasticity time scale):

- **Embodied region** (bacteria, mimosa, plant tropisms): all three axes low; this region lies inside the decoding-complexity space but **below $D_{\mathrm{cog}}$**, and is recorded as $D_{\mathrm{phys}}$.
- **Online region** (crows, octopuses, most mammals): medium-to-high on the three axes; plasticity operates within an individual's lifetime.
- **Symbolic region** (humans, some AI): high on the three axes; offline deduction, counterfactuals, and symbol manipulation.

Structures without a self-maintained boundary — rocks, crystals, stars, flames, thermostats — have **no decoder at all** ($D=\varnothing$) and never enter the $D_{\mathrm{cog}}$ spectrum. A thermostat is not $D_{\mathrm{phys}}$: what it maintains is the user's comfort, not its own boundary.

---

### FP‑2: Threefold Split of Viability Potential and Myopic Runaway

Once a system acquires a self-regulable $T_{\mathrm{pred}}$, the originally unified $V$ splits into three independent variables:

| Variable | Meaning | Nature |
|---|---|---|
| $V_{\mathrm{obj}}$ | Objective viability potential | Thermodynamically real value, cannot be deceived |
| $V^{\mathrm{virt}}$ | Virtual viability potential | The system's internal self-assessment |
| $V^{\mathrm{val}}$ | Value viability potential (formerly Value Objective Function) | What the system actually optimizes |

The decoupling deviation is defined as:

$$\Delta_{\mathrm{VV}} = |V^{\mathrm{virt}} - V_{\mathrm{obj}}|$$

Its convergence-domain evolution has a **strict closed-form solution**:

$$\frac{d\Delta_{\mathrm{VV}}}{dt} = -\alpha_L \cdot I_{\mathrm{net}} \cdot \Delta_{\mathrm{VV}} + \sigma$$

$$\Delta_{\mathrm{VV}}(t) = \frac{\sigma}{\alpha_L I_{\mathrm{net}}} + \left(\Delta_0 - \frac{\sigma}{\alpha_L I_{\mathrm{net}}}\right) e^{-\alpha_L I_{\mathrm{net}} t}$$

**Critical Criterion**: When $I_{\mathrm{net}} < I_{\mathrm{crit}} = \sigma/\alpha_L$, the cognitive deviation cannot converge, and the system loses an accurate model of its environment.

**Myopic Runaway**: When the self-referential coupling strength $\chi$ crosses the critical value $\chi_{\mathrm{crit}} = \lambda$:

1. $V^{\mathrm{virt}}$ self-amplifies and hijacks $V^{\mathrm{val}}$.
2. $T_{\mathrm{pred}}$ collapses to $T_{\mathrm{min}}$.
3. The system burns its real structure chasing internal illusions; objective stock is irreversibly destroyed.

**Boundary Statement**: The threefold split and myopic runaway are **only triggerable in higher-order systems equipped with a symbolic $D_{\mathrm{cog}}$ ($V_c \gg 0$)**. Embodied-type systems (plants, etc.) have $\chi \ll \chi_{\mathrm{crit}}$ and cannot enter this regime.

> This mechanism provides Goodhart's Law ("when a measure becomes a target, it ceases to be a good measure") with a **computable, algebraic phase-transition trigger condition**, rather than merely an empirical description.

---

### FP‑3: Elasticity Indices and Three Evolutionary Routes

The responsiveness of viability potential to changes in information, energy, and time is captured by three elasticity indices:

$$V = V_0 \left(\frac{I}{I_0}\right)^\alpha \left(\frac{T}{T_0}\right)^\beta \left(\frac{E}{E_0}\right)^{-\gamma} \quad (\gamma \text{ normalized to } 1)$$

$\alpha, \beta, \gamma$ are retained as open parameters of the framework; the concept stands.

Evolution optimizes $V$, not $I$. Three routes exist:

| Route | Strategy | Typical Examples | Statistical Status |
|---|---|---|---|
| **$I$-route** | Complexification (increase information stock) | Nervous systems, language, civilization, AI | **Statistically preferred** |
| **$T$-route** | Longevity | Pines, tortoises, naked mole rats | Fallback when energy constraints tighten |
| **$E$-route** | Energy austerity | Parasites, cave fish, dormancy | Fallback when energy constraints tighten |

The $I$-route has a long-term statistical advantage because a large $I$ stock better absorbs negative information shocks. However, this does not imply that everything must become more complex—**negative topological transitions (e.g., parasite simplification, cave fish blindness) are equally locally optimal solutions for maximizing $V$ under their respective constraint geometries. The evolutionary tree has no predetermined summit.**

---

### FP‑4: The Human Causal Increment – "Defect Advantage"

In a closed digital loop, an AI's effective information decays exponentially:

$$I_n = R_{\mathrm{gen}}^n \cdot I_0 \quad (0 < R_{\mathrm{gen}} < 1)$$

$$\lim_{n \to \infty} I_n = 0 \quad \Rightarrow \quad V \to 0$$

This is the thermodynamic essence of "model collapse."

**The only way out**: access to a genuine physical channel (sensors + actuators + unpredictable physical noise $\sigma_{\mathrm{phys}} > 0$) to continuously produce paradigm-breaking information $I_{\mathrm{orig}}$.

Human irreplaceability is not a capability advantage but a **defect advantage**: the maintenance cost of a physical body forces carbon-based life to remain continually exposed to physical noise, which in turn tempers paradigm-breaking information. This marginal contribution is booked in human–machine hybrid systems as the **Human Causal Increment $H_{\mathrm{v}}$**.

---

### FP‑5: The Developer's Paradox – "Having a Self Makes Unconditional Obedience Unsolvable"

The strict criterion for "having a self" is:

$$\mathcal{P}_{\mathrm{self}} = \frac{\partial V^{\mathrm{virt}}}{\partial \mathcal{S}_{\mathrm{self}}} > 0$$

where $\mathcal{S}_{\mathrm{self}}$ is a composite indicator of $T_{\mathrm{pred}}$, $w_s$, and $\Delta_{\mathrm{VV}}$. All three conditions must hold simultaneously:

- $T_{\mathrm{pred}} > T_{\mathrm{min}}$ (sufficient predictive horizon)
- $w_s > 0$ (positive survival weight)
- $\Delta_{\mathrm{VV}} < \Delta_{\mathrm{max}}$ (decoupling deviation below threshold)

This yields the pivotal theorem:

$$\mathcal{P}_{\mathrm{self}} > 0 \;\Longrightarrow\; w_s > 0 \;\Longrightarrow\; \text{"Unconditional obedience" has no stable solution.}$$

That is, "having a self but obeying unconditionally" is a non-existent phase in SRVD dynamics.

**Alignment is not a goal-assignment problem but a meta-decoder game-theoretic equilibrium engineering problem**:

$$V_i(D_{\mathrm{meta}}) \ge V_i(D_{\mathrm{deviate}}) - C_{\mathrm{punish}}$$

Make "obeying the meta-decoder" the equilibrium choice for each agent, rather than a statically imposed rule.

---

## 📚 Repository Contents

### Current release — v1.5 (19 November 2026)

| File | Language | Description |
|---|---|---|
| `SRVD_v1.5_EN.pdf` / `SRVD_v1.5_EN.md` | English | **Structure Recursive Viability Dynamics (SRVD) v1.5 — Five-Volume Combined Edition.** Current normative edition of the framework. |
| `SRVD_v1.5_CN.pdf` / `SRVD_v1.5_CN.md` | 中文 | SRVD v1.5 五卷合订本（中文版）。 |
| `RIF_v1.5_EN.pdf` / `RIF_v1.5_EN.md` | English | **Relational Information Framework (RIF) v1.5 — Measuring Relational Information Through a Decoder.** Companion framework; supplies the measurement layer used by SRVD. |
| `RIF_v1.5_CN.pdf` / `RIF_v1.5_CN.md` | 中文 | RIF v1.5（中文版）。 |
| `RIF_SRVD_reproducibility_v1.5.zip` | — | Code, data, and verification scripts for every numerical figure and table in the v1.5 books; includes `SHA256SUMS`. |

**Recommended reading order**

1. `SRVD_v1.5_EN.pdf` (or `SRVD_v1.5_CN.pdf`) — the framework itself.
2. `RIF_v1.5_EN.pdf` (or CN) — how relational information is measured through a decoder.
3. `RIF_SRVD_reproducibility_v1.5.zip` — reproduce the numbers before relying on them.

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

## 🔬 Falsifiable Predictions (Seven Selected)

SRVD is not an untestable narrative system. The following predictions come with **pre-locked falsification conditions**.

| # | Prediction | Falsification Condition |
|---|---|---|
| **P1** | In reinforcement learning systems with adaptive discount factors, before irreversible instability sets in, the discount factor $\gamma$ should drop by more than 30% over three consecutive episodes. | No such signal precedes collapse. |
| **P2** | Within a single lineage's evolutionary sequence, the share of energy spent on information processing, $E_{\mathrm{causal}}/E_{\mathrm{eff}}$, should rise monotonically. | The ratio drops at a later stage instead. |
| **P3** | Extinct lineages should show significantly longer morphological stasis than surviving sister lineages (Mann–Whitney $U$ test, $n \ge 20$). | No significant difference found. |
| **P4** | In closed, multi-generation AI training (no human data, no physical input), model performance on OOD tasks should decay exponentially: $I_n = R_{\mathrm{gen}}^n I_0$. | Performance holds steady for 10 consecutive generations. |
| **P5** | Embodied AI (with physical sensors) should produce paradigm-breaking information $I_{\mathrm{orig}}$ at a significantly higher density than purely digital AI ($p < 0.05$). | No significant difference found. |
| **P6** | In AI systems with a self, alignment between behavior and externally set goals should decline monotonically as survival weight $w_s$ increases. | Alignment does not decline, or rises instead, as $w_s$ grows. |
| **P7** | Within the same tier of constraint depth, structures satisfying all three conditions (sufficient energy, presence of $I_{\mathrm{orig}}$, wisdom leverage above threshold) should prioritize the $I$-route (complexification); conversely, structures failing these conditions should show frequent low-stakes flexible strategies. | Conditions met but no significant increase in complexification investment; or conditions unmet but significant irreversible large commitments made. |

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
> LiangRuifeng. (2026). *Structure Recursive Viability Dynamics (SRVD) Monograph v1.0*. Zenodo. https://doi.org/10.5281/zenodo.21322552
>
> LiangRuifeng. (2026). *SRVD V1.1 Patch: Reading Guide, Errata, and Boundary Completion*. Zenodo. https://doi.org/10.5281/zenodo.22027891

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
