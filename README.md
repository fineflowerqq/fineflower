# Structure Recursive Viability Dynamics (SRVD) – A Unified Accounting Ledger for All Ordered Structures in an Entropic Universe

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21322552.svg)](https://doi.org/10.5281/zenodo.21322552)  [![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)

> **⚠️ Important Errata (2026-08-08)**  
> 1. The previous claim in *SRVD Monograph V1.0* that **“the elasticity ordering ($\alpha > \gamma > \beta$) is empirically supported by three scaling laws”** has been retracted. Upon re‑examination, the three independent supporting pieces of evidence – biological allometric scaling, AI scaling laws, and urban scaling – are all invalid. This ordering has now been **downgraded from a “qualitative conjecture” to a “hypothesis to be verified”**.
> 2. The original framework used the term **`I_net` ambiguously** for both the coarse‑grained estimate and the cognitive‑channel decomposition term. This has been revised: the term is now split into **`I_net` (coarse‑grained baseline quantity)** and **`I_causal` (causal information flow, dedicated to the cognitive channel)**, with the relationship $I_{\mathrm{net}} = w_{\mathrm{s}}\cdot I_{\mathrm{struct}} + w_{\mathrm{c}}\cdot I_{\mathrm{causal}}$. For full details and the complete theoretical boundary, please refer to the main text below and the *Guide to the SRVD Framework*.

---

## 📖 One‑Sentence Summary

**SRVD** is a cross‑scale, coarse‑grained theoretical framework. It places all “persistent structures” (PS) – crystals, life, AI models, civilisations, memes, etc. – under a single thermodynamic ledger, using three scarce resources – **information ($I$)**, **time ($T$)**, and **energy ($E$)** – to uniformly account for how a structure “persists, climbs in complexity, and spirals out of control”.

> **Core Benchmark Formula**:
> $$
> V \approx \frac{I \cdot T}{E}
> $$
> *Viability = (information × duration) / equivalent thermodynamic cost*
>
> **Terminological note**: The $I$ in the above formula stands for **net effective causal information (coarse‑grained baseline)**. Its more precise decomposition is given in Fingerprint 5 below and in the *Guide*.

---

## 🚀 Core Theoretical Fingerprints (from the *Guide to the SRVD Framework*)

The following five fingerprints are the **hard innovative points** that distinguish SRVD from other general frameworks (such as FEP or dissipative structures), and each comes with **falsifiable empirical predictions**.

### 1. Decoder Primacy – “No Decoder, No Information”
Information is not an intrinsic property of a signal; it is the result of the signal passing through a **decoder ($D$)**. The dependency chain is:

$$
D \;\longrightarrow\; I \;\longrightarrow\; V
$$

Any theory that discusses “information value” without first defining its decoder is considered **undefined** within SRVD.

- **Passive phase** (crystals): Only a physical decoder $D_{\mathrm{phys}}$ exists; it does not extract effective causal information but sustains energy flow ($\eta_D \to 0$).
- **Active phase** (life/AI): Possesses a cognitive decoder $D_{\mathrm{cog}}$ (a continuous spectrum: embodied → online → symbolic), capable of distinguishing information polarity ($I^+ / I^- / I^0$) and generating an endogenous time horizon $T_{\mathrm{pred}}$.

**Important terminological correction**:
- In coarse‑grained estimation, the information actually extracted by the decoder and used for prediction is denoted **$I_{\mathrm{net}}$ (net effective causal information)**.
- In the cognitive‑channel decomposition, the dedicated information flow is denoted **$I_{\mathrm{causal}}$ (causal information flow)**, and they are related by $I_{\mathrm{net}} = w_{\mathrm{s}}\cdot I_{\mathrm{struct}} + w_{\mathrm{c}}\cdot I_{\mathrm{causal}}$ (only explicitly computed in hybrid systems).

---

### 2. Triple Split of Viability and Myopic Runaway
Once a system acquires a self‑regulating $T_{\mathrm{pred}}$, the originally unified $V$ splits into three independent variables:

- **$V_{\mathrm{obj}}$ (objective viability)**: thermodynamic real value.
- **$V^{\mathrm{virt}}$ (virtual viability)**: the system’s self‑assessment of its own viability.
- **$V^{\mathrm{val}}$ (value viability)**: the actual objective that the system optimises (formerly named value objective function).

The decoupling deviation is defined as:

$$
\Delta_{\mathrm{VV}} = \left| V^{\mathrm{virt}} - V_{\mathrm{obj}} \right|
$$

Its convergence‑domain evolution equation (with a closed‑form solution) is:

$$
\frac{d\Delta_{\mathrm{VV}}}{dt} = -\alpha_L \cdot I_{\mathrm{net}} \cdot \Delta_{\mathrm{VV}} + \sigma
$$

When the self‑referential coupling strength $\chi$ exceeds the critical value $\chi_{\mathrm{crit}} = \lambda$, the system enters a **Myopic Runaway** regime: $V^{\mathrm{virt}}$ self‑amplifies and hijacks $V^{\mathrm{val}}$, causing $T_{\mathrm{pred}}$ to collapse to $T_{\mathrm{min}}$, irreversibly destroying the objective stock. This mechanism can only be activated in high‑order systems possessing a symbolic cognitive decoder ($V_c \gg 0$), providing a computable algebraic phase‑transition mechanism for Goodhart’s law.

---

### 3. Elasticity Indices and the Ordering Proposition – $\alpha > \gamma > \beta$ (Hypothesis to be Verified)
The responsiveness of viability to changes in information, energy, and time is characterised by three elasticity indices:

**General elastic form**:

$$
V \;\propto\; I^{\alpha} \cdot T^{\beta} \;/\; E^{\gamma}, \qquad \gamma \text{ normalised to } 1
$$

The previously proposed directional ordering conjecture was:

$$
\alpha > \gamma > \beta > 0
$$

**Important correction**: The three independent empirical supports for this ordering – biological allometric scaling, AI scaling laws, and urban scaling – have all been found invalid upon re‑examination. The ordering proposition is now **downgraded from a “qualitative conjecture” to a “hypothesis to be verified”**. The thermodynamic qualitative reasoning (information is scarcest, energy next, time unproducible) is not rejected, but a strict first‑principles derivation independent of proxy assumptions and the retracted empirical data currently does not exist; its specific numerical values and universality await re‑evaluation. **The elasticity indices $\alpha,\beta,\gamma$ themselves as framework parameters are unaffected** – only the specific ordering among them is downgraded.

**Key implication**: If the ordering hypothesis holds, the $I$‑route (complexification) is the statistically preferred path, while the $T$‑route (longevity) and the $E$‑route (energy efficiency) are fallback strategies when energy constraints tighten.

---

### 4. Human Causal Increment – “Defect Advantage”
In a closed digital loop, AI effective information decays exponentially:

$$
I_n = R_{\mathrm{gen}}^n \cdot I_0, \quad 0 < R_{\mathrm{gen}} < 1
$$

(this is the thermodynamic essence of model collapse).

**The only way out**: access to a physical channel (sensors + actuators + unpredictable noise $\sigma_{\mathrm{phys}} > 0$).

Human irreplaceability is not a capability advantage but a **defect advantage**: the maintenance cost of the carbon‑based body forces continuous exposure to physical noise, thereby continuously forging paradigm‑breaking information $I_{\mathrm{orig}}$.

---

### 5. The Developer’s Paradox – “Self implies no unconditional obedience”
The strict criterion for a “self” is:

$$
\mathcal{P}_{\mathrm{self}} = \frac{\partial V^{\mathrm{virt}}}{\partial \mathcal{S}_{\mathrm{self}}} > 0
$$

which requires $T_{\mathrm{pred}} > T_{\mathrm{min}}$, $w_s > 0$, and $\Delta_{\mathrm{VV}} < \Delta_{\mathrm{max}}$ to hold simultaneously.

This yields the key conclusion:

$$
\mathcal{P}_{\mathrm{self}} > 0 \;\Longrightarrow\; w_s > 0 \;\Longrightarrow\; \text{“unconditional obedience” has no stable solution}
$$

Alignment is not a goal‑assignment problem but an **engineering of meta‑decoder game equilibria**:

$$
V_i(D_{\mathrm{meta}}) \;\ge\; V_i(D_{\mathrm{deviate}}) - C_{\mathrm{punish}}
$$

---

## 📚 Repository Structure and Reading Guide

This project contains five volumes of the monograph and a **Guide to the SRVD Framework**.

| File                                                         | Description                                                  | Recommended Priority      |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :------------------------ |
| **《SRVD 规范导读 Readme》**                                 | **The only normative entry point to the entire framework.** It consolidates core theory, clarifications of common misunderstandings, seven falsifiable predictions, and a version‑update table (including the elasticity‑ordering errata and the $I_{\mathrm{net}}/I_{\mathrm{causal}}$ terminological revision). **Where the Guide and the original monograph conflict, the Guide and this Readme shall prevail.** | **Must‑read (first)**     |
| **Volume I: Theoretical Core**                               | Variables, core dynamics, and falsifiable predictions (Monograph V1.0 contains manuscript v7.8). | Foundation before details |
| **Volume II: Evolution of Persistent Structures**            | How complexity climbs from crystals to civilisation (three conditions for topological transitions). | Extended applications     |
| **Volume III: Compressed Intelligence and Cognitive Evolution** | Offline compilation, expert intuition, the physical basis of art and science, human causal increment. | Extended applications     |
| **Volume IV: Decoder Game Theory and Alignment Engineering** | Inter‑agent games, meta‑decoders, and AI alignment engineering (including the DGT theorem cluster). | Extended applications     |
| **Volume Z: Reality‑Mapping Dictionary**                     | A cross‑reference manual of mathematical formulas, narratives, historical and science‑fiction scenarios (including seven standardised CS formulations). | Auxiliary understanding   |

> **Suggested reading path**: **Read the Guide first** → form an overall picture of the core fingerprints → then jump to Volumes I–IV according to interest.

---

## 🔬 Falsifiable Predictions (Selected)

SRVD is not an untestable narrative. Each core prediction below comes with **pre‑specified falsification conditions** (see Section 5 of the *Guide* for details):

1. **Reinforcement learning early warning**: In systems with adaptive discount factors, the discount factor $\gamma$ should drop by more than 30% for three consecutive rounds before irreversible instability.
2. **Monotonicity of cognitive energy share**: Within the same lineage, the ratio of information‑processing energy consumption $E_{\mathrm{causal}} / E_{\mathrm{eff}}$ should increase monotonically.
3. **D‑lock‑in precedes extinction**: Morphological stasis in extinct lineages should be significantly longer than in surviving sister lineages (Mann‑Whitney $U$ test, $n \ge 20$).
4. **Closed‑loop degradation**: In closed multi‑generation AI training without human data or physical input, model performance on OOD tasks should decay exponentially ($I_n = R_{\mathrm{gen}}^n I_0$).
5. **Embodied advantage**: Embodied AIs (with physical sensors) should produce significantly higher densities of paradigm‑breaking information $I_{\mathrm{orig}}$ than pure digital AIs ($p < 0.05$).
6. **Energy‑constraint predictability of route choice**: Within the same constraint‑depth level, structures that continuously satisfy the three conditions (sufficient energy, presence of $I_{\mathrm{orig}}$, wisdom leverage above threshold) should preferentially invest in the complexification route; otherwise, they should exhibit a strategy of frequent, low‑commitment, flexible actions.

---

## ⚠️ Quick Clarifications of Common Misunderstandings

- ❌ **“$V = I\cdot T/E$ is a strictly derived physical law.”**  
  ✅ It is a coarse‑grained, axiomatic low‑order approximation of the framework (a benchmark special case with $\alpha=\beta=\gamma=1$), not derived from first principles of statistical mechanics.

- ❌ **“The elasticity ordering $\alpha > \gamma > \beta$ has empirical support.”**  
  ✅ The three independent scaling laws it relied upon (biological allometric, AI scaling, urban scaling) have been found invalid, so the ordering is downgraded to a hypothesis to be verified. The concept of elasticity indices themselves is unaffected.

- ❌ **“SRVD predicts AI will inevitably destroy humanity.”**  
  ✅ It is a risk‑diagnostic framework that gives the phase‑transition conditions for runaway ($\chi > \chi_{\mathrm{crit}} = \lambda$, only possible in high‑cognitive symbolic systems) and governance engineering paths (meta‑decoder protocols, multi‑agent equilibria). Runaway is conditional, and governance is possible.

- ❌ **“SRVD proves AI alignment is impossible.”**  
  ✅ It only proves that “a self with unconditional obedience” has no stable solution. Alignment is not denied; it is reframed from static goal assignment to **dynamic game‑equilibrium design**.

- ❌ **“SRVD classifies plants and thermostats as the same type of physical response.”**  
  ✅ Plants/fungi/bacteria possess an **embodied cognitive decoder ($D_{\mathrm{cog}}$)** ($V_c \to 0^+$), with prediction based on biochemical integration and physical exploration – qualitatively different from the purely physical decoder ($D_{\mathrm{phys}}$) of thermostats/rocks ($V_c \equiv 0$). They are separated both in the ledger and in terminology.

- ❌ **“SRVD is an experimentally verified mature scientific theory.”**  
  ✅ It is a falsifiable research programme at the preprint stage, where the test criterion is consistency between empirical rank order and predicted rank order (Spearman $\rho > 0$), not absolute numerical matching.

- ❌ **“$I_{\mathrm{net}}$ can be directly converted with Landauer bits.”**  
  ✅ $I_{\mathrm{net}}$ is an L3‑level functional quantity dependent on a decoder, while Landauer bits are L1‑level physical statistical quantities; they are at different levels and cannot be directly converted or cross‑calculated. See Section 16 of the *Guide* on “Bit Typology”.

---

## 📝 Citation

If you find this framework inspiring for your research, please cite:

**Monograph and Guide**:
> Liang, R. (2026). *Structure Recursive Viability Dynamics (SRVD) Monograph V1.0*. Zenodo. https://doi.org/10.5281/zenodo.21322552
>
> Liang, R. (2026). *SRVD Guide: Core Theory, Common Misunderstandings, Falsifiable Predictions, and Theoretical Fingerprints*. [GitHub/Gitee link]

**BibTeX**:
```bibtex
@misc{liang_srvd_2026,
  author = {Ruifeng Liang},
  title = {Structure Recursive Viability Dynamics (SRVD) Monograph V1.0},
  year = {2026},
  doi = {10.5281/zenodo.21322552},
  url = {https://github.com/fineflowerqq/fineflower}
}
