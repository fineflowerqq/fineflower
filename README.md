# Structure Recursive Viability Dynamics (SRVD) – A Unified Accounting Ledger for All Ordered Structures in an Entropy-Increasing Universe

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21322552.svg)](https://doi.org/10.5281/zenodo.21322552) [![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

---

## 📖 One-Sentence Summary

**SRVD** is a cross-scale macro-coarse-grained theoretical framework. It brings all "persistent structures"—crystals, life, AI models, civilizations, and memes—onto the same thermodynamic ledger, using three scarce resources—**information**, **time**, and **energy**—to provide a unified answer to one fundamental question:

> **How does an ordered structure persist, climb in complexity, and spiral into runaway collapse?**

**Core Milestone Formula (Reference Baseline)**:

$$V \approx \frac{I \cdot T}{E}$$

**Viability Potential = (Information × Persistence Time) / Equivalent Thermodynamic Cost**

$V$ measures: the integral of causally ordered quantity per unit of thermodynamic cost. This is the "minimal-viability postulate" of the SRVD framework—not a physical law derived from first principles, but an axiom-level low-order approximation fixed jointly by three structural requirements: non-substitutability, symmetric contribution of the three variables, and first-order separability.

> **Terminological Note**: $I$ in the formula above represents **Net Effective Causal Information (coarse-grained baseline quantity)**. Its precise decomposition is $I_{\mathrm{net}} = w_s \cdot I_{\mathrm{struct}} + w_c \cdot I_{\mathrm{causal}}$ (where $w_s = E_{\mathrm{structure}}/E_{\mathrm{eff}}$, $w_c = E_{\mathrm{causal}}/E_{\mathrm{eff}}$, strictly determined by the system's underlying thermodynamics). See Core Fingerprint FP‑5 and the *Reading Guide* for details.

**Version Statement**: This repository contains the V1.0 Monograph and the V1.1 Patch (Reading Guide, Errata, and Boundary Completions). Where substantive conflicts exist, the patch documents govern.

---

## 🚀 Five Core Theoretical Fingerprints

These five fingerprints are SRVD's **hard innovations** that distinguish it from other general frameworks (FEP, Dissipative Structures, Goodhart's Law)—each with falsifiable empirical predictions.

### FP‑1: Primacy of the Decoder – "No Decoder, No Information"

Information is not an intrinsic property of the signal itself; it is what remains after a signal has passed through a **decoder ($D$)**:

$$I_{\mathrm{net}} = \eta_D \cdot I_{\mathrm{latent}}$$

The dependency chain is defined as:

$$D \longrightarrow I \longrightarrow V$$

Any discussion of "information value" that has not first specified its decoder is, within SRVD, considered an unfinished definition.

**Two-Level Structure of the Decoder**:

| | Physical Decoder $D_{\mathrm{phys}}$ | Cognitive Decoder $D_{\mathrm{cog}}$ |
|---|---|---|
| **Scope** | All persistent structures | Active-phase structures only (life/AI) |
| **Function** | Receives energy flow; extracts no effective causal information | Actively extracts information based on prediction |
| **Efficiency** | $\eta_D \to 0$ | $\eta_D > 0$, continuous spectrum |
| **Time Horizon** | No $T_{\mathrm{pred}}$ | Has $T_{\mathrm{pred}}$ (endogenous time horizon) |

**Continuous Spectrum of the Cognitive Decoder** (not a binary switch):

- **Embodied** (plants/fungi/bacteria): Prediction via DNA-templated biochemical integration and physical-space probing; $V_c \to 0^+$; $T_{\mathrm{pred}}$ pressed against the floor.
- **Online** (crows/octopuses/mammals): Associative learning and online simulation via neural networks; $V_c$ low-to-mid range.
- **Symbolic** (humans/AI): Offline, multi-path counterfactual reasoning; $V_c \gg 0$; $T_{\mathrm{pred}} \gg T_{\mathrm{min}}$.

Strictly zero-cognition systems (rocks, stars, flames) possess **only $D_{\mathrm{phys}}$** and never enter the $D_{\mathrm{cog}}$ spectrum.

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

## 📚 Repository Structure and Reading Guide

# SRVD Repository File Structure

## File Names → Display Names (with word breaks)

| Original Filename (long) | Display Name (with word breaks) |
| ------------------------------------------------------------ | ------------------------------ |
| `Vol_I_SRVD_paper_v7.8_EN`                                   | **Volume I: Theoretical Core**               |
| `Vol_II_SRVD_The_Evolution_of_Persistent_Structures`         | **Volume II: Evolution of Persistent Structures**         |
| `Vol_III_SRVD_Chapters_Compressed_Intelligence_and_Cognitive_Evolution` | **Volume III: Compressed Intelligence and Cognitive Evolution**     |
| `Vol_IV_SRVD_Decoder_Game_Theory_and_Alignment_Engineering`  | **Volume IV: Decoder Game Theory and Alignment Engineering** |

> **Display Rule**: The "File" column in the table retains the long filename (clickable for location), while the "Volume" column uses the display name for a clean reading experience.

## Complete Table

| File                                                         | Volume                             | Description                                                         | Priority         |
| ------------------------------------------------------------ | ------------------------------ | ------------------------------------------------------------ | -------------- |
| SRVD_V1.1_Patch_Reading_Guide                                | **Patch: Reading Guide**                   | Normative entry point for the entire framework. Integrates core fingerprints, clarifications of common misreadings, seven falsifiable predictions, and a version-update comparison table. **Where conflicts with V1.0 Monograph arise, this patch governs.** | ⭐⭐⭐⭐⭐ **Required** |
| SRVD_Monograph_2026_v1.0                                     | **Monograph Collection**                   | Complete five-volume monograph collection; suitable for bulk download or batch reading.             | ⭐⭐⭐⭐⭐Foundation     |
| Vol_I_SRVD_paper_v7.8_EN                                     | **Volume I: Theoretical Core**               | Variable constitution, core dynamics, decoder definition, fivefold recursion, elasticity indices, threefold split and myopic runaway. Source of all symbols in the series. | ⭐⭐⭐⭐ Foundation      |
| `Vol_II_SRVD_The_Evolution_of`<br>`_Persistent_Structures`   | **Volume II: Evolution of Persistent Structures**         | Complexity ascent from crystals to civilizations. Three conditions for topological transitions, energy-dominance transfer sequence, three-axis coordinate system. | ⭐⭐⭐ Applied/Extension   |
| `Vol_III_SRVD_Chapters_Compressed_`<br/>`Intelligence_and_Cognitive_Evolution` | **Volume III: Compressed Intelligence and Cognitive Evolution**     | Offline compiled computation (physical essence of expert intuition), art/science as cross-agent decoder compilers, human causal increment, emergence of self, and the Developer's Paradox. | ⭐⭐⭐ Applied/Extension   |
| `Vol_IV_SRVD_Decoder_Game`<br>`_Theory_and_Alignment_Engineering` | **Volume IV: Decoder Game Theory and Alignment Engineering** | Decoder drift equation, four modes of cross-agent interaction, Nash stability condition for the meta-decoder (DGT.8), AI alignment engineering pathways. | ⭐⭐⭐ Applied/Extension   |
| Vol_Z _SRVD_Equations_and_Narrative                          | **Volume Z: Reality-Mapping Dictionary**      | Reality-mapping narrative.                                                 | ⭐ Further Reading      |
| `v7.6_SRVD_v7.6`                                             | **Manuscript v7.6**                  | Historical manuscript. Distinguishes objective stock from viability-drive rate dimensionally, phase-space constraint inequalities, rigorous classification of four global attractors. | ⭐ Historical Archive     |
| `v7.5_Structural_Recursive`<br>`_Viability_Dynamics`         | **Manuscript v7.5**                  | Historical manuscript. Threefold split and endogenous time collapse as core mechanisms of paranoid recursion/reward hacking; reinforcement learning falsification protocol. | ⭐ Historical Archive     |

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

If this framework inspires your research, you are welcome to cite it:

**Monograph**:
> Liang, R. (2026). *Structure Recursive Viability Dynamics (SRVD) Monograph V1.0*. Zenodo. https://doi.org/10.5281/zenodo.21322552

**Patch: Reading Guide**:
> Liang, R. (2026). *Structure Recursive Viability Dynamics (SRVD) V1.1 Patch: Reading Guide, Errata, and Boundary Completion*. GitHub/Gitee.

**BibTeX**:
```bibtex
@misc{liang_srvd_2026,
  author = {Ruifeng Liang},
  title = {Structure Recursive Viability Dynamics (SRVD) Monograph V1.0},
  year = {2026},
  doi = {10.5281/zenodo.21322552},
  url = {https://github.com/fineflowerqq/fineflower}
}
```

---

**In an entropy-increasing universe, keep every ordered structure on the same ledger.**
