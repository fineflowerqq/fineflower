https://doi.org/10.5281/zenodo.20478506
# Structural Recursive Viability Dynamics (SRVD) v7.6

## **Macro-Viability and Higher-Order Phase Transitions: Non-Equilibrium Dynamics of Persistent Structures**

**Ruifeng Liang** (Independent Researcher) | May 2026 | Academic Preprint

> **📌 Preface**
> This preprint is published on Zenodo, version v7.6. Critique and collaboration are welcome.
> Contact: fineflowerrain@gmail.com

---

## Abstract

This paper presents **Structural Recursive Viability Dynamics** (SRVD) v7.6, a cross-scale dynamical framework describing how systems maintain viability through recursive information propagation under energetic constraints. SRVD takes net effective causal information ($I_{net}$), viability time ($T$), and effective thermodynamic cost ($E_{eff}$) as its core variables, constructs a five-fold recursive architecture incorporating decoder ($D$) drift, and establishes the **endogenous time horizon** ($T_{pred}$) as the dynamical variable triggering phase transitions. The framework focuses on characterizing macro-level non-equilibrium phase transitions involving boundary collapse, endogenous time horizon collapse, and decoder decoupling. Through linear stability analysis, this paper derives the decoupling conditions between endogenous simulated viability ($V^{virt}$) and objective viability ($V_{obj}$) under high coupling, precisely maps AI reward hacking to a self-exciting phase transition into the **Myopic Runaway Regime** driven by endogenous time collapse ($T_{pred} \to T_{min}$), and provides a refutation protocol based on time collapse. SRVD rests on different axioms and has a different domain of applicability from classical steady-state inference frameworks, offering an irreducible dynamical explanation for the destabilization of complex system evolution. Core testable predictions are given in the RL refutation protocol in Section 9.2.

**Keywords**: Structural Recursive Viability Dynamics; endogenous time horizon; recursive dynamics of consciousness; AI alignment; Myopic Runaway Regime; decoder decoupling; incommensurability

---

> *Energy provides the substrate.*  
> *Information provides the structure.*  
> *Time provides the window of observation.*  
> *Both the observed and the observer are bound by these same constraints.*  
> *Therefore, what one can know depends on what one is.*  
> *And what one is depends on one's energy, one's structure, and one's time.*  
>
> — *Epistemological premise of SRVD*

## 0. Persistent Structure as the Research Subject

Before introducing the dynamical variables, SRVD identifies a common research subject that appears across physical, biological, cognitive, and social domains: the persistent structure.

**Definition (Persistent Structure):**  
A persistent structure is any negentropic topological configuration capable of maintaining its continuity across time under energetic constraints.

This definition combines three universal requirements:

1. **Structure (Information):** A distinguishable negentropic organization that differentiates the system from its surrounding background.
2. **Persistence (Time):** The capacity to maintain continuity across a finite temporal horizon.
3. **Constraint (Energy):** The energetic conditions required to sustain that continuity.

Within this framework, minerals, stars, biological organisms, languages, institutions, civilizations, and artificial intelligences may all be analyzed as instances of persistent structures operating under different informational, temporal, and energetic conditions.

The variables introduced in subsequent sections are state variables describing the viability dynamics of persistent structures rather than independent ontological entities.

Accordingly, SRVD is not primarily a theory of matter, energy, organisms, or agents. It is a framework for analyzing the emergence, maintenance, transformation, and dissolution of persistent structures.

---

> **📌 Version Note**: This version performs final theoretical consolidation on the main scaffold of v7.2 and officially renames the framework **"Structural Recursive Viability Dynamics"** (SRVD). This version establishes "structural recursion" as the overarching framework and demotes "self-recursion/self-reference" to a special higher-order form that emerges within structural viability propagation:
>
> - Information differentiation, decoder continuity, and observational stability are elevated from background conditions to explicit dynamical variables, establishing the axiomatic status of E-T-I-D coupling;
> - **Theoretical positioning**: SRVD and steady-state theories such as the Free Energy Principle (FEP) are neither subsets of each other; they rest on different, non-overlapping foundational axioms and are incommensurable independent theories;
> - **New frontier mappings**: AI safety and the alignment problem are brought into the framework as extreme-regime dynamics; $T_{pred} \to T_{min}$ collapse as an early-warning signal for AI reward hacking and the "decoder decoupling" mechanism are introduced;
> - Redundant microscopic mathematical scaffolding is removed, with a full return to macro-level logical deduction and empirically testable inference protocols.

---



## 📌 Theoretical Positioning and Scale Declaration

Building on the concept of **persistent structure** defined in §0, the "Structural Recursive Viability Dynamics" (SRVD) proposed in this paper is a coarse-grained macro-level dynamical framework focused on viability competition and phase transitions in complex structural systems under finite free-energy conditions.The following theoretical positioning and scale declarations apply:

1. **Model status**: All core equations are phenomenological models, intended to provide a macroscopic descriptive vocabulary rather than derivations from microscopic first principles.
2. **Empirical status**: The core variables $I_{net}$ and $E_{eff}$ are theoretical latent variables; conclusions await systematic simulation and empirical testing.
3. **Theoretical boundaries**: SRVD focuses on macro-level viability dynamics and does not address subjective phenomenology or microscopic physical mechanisms. It adopts foundational axioms and applicability domains distinct from traditional steady-state inference frameworks, and no theoretical reduction relation exists between them.

### Three-Level Epistemological Distinction

To avoid confusion, this paper is developed at three levels, which readers should keep clearly distinct:

| Level | Content | Current Status |
|-------|---------|----------------|
| **Theoretical framework** | Core variables, equations, and five-fold recursive architecture of SRVD | Constructed |
| **Numerical illustration** | Parameter-sweep simulations based on the theoretical equations (see Appendix A) | Demonstrates internal theoretical consistency — **not empirical data** |
| **Empirical testing** | Systematic empirical verification of the predictions in Section 9 | To be conducted |

All interactive figures in the appendices belong to the second level (numerical illustration). Their curves are generated by the theoretical equations to exhibit the qualitative dynamical behavior; they do not constitute empirical confirmation of the predictions.

### Operationalization Anchor Statement

The core variables $I_{net}$ and $E_{eff}$ are implicitly defined through their dynamical roles in the phenomenological equations — the concepts precede measurement, and measurement schemes will be constructed as detection technology matures. Section 9.2 provides a complete operationalization mapping within the reinforcement learning framework. Current operationalization anchors include:

1. **Proxy indicators for $I_{net}$**: In RL, mapped to policy divergence / surrogate reward slope; in biology, mapped to phenotypic diversity indices;
2. **Approximate measures for $E_{eff}$**: In RL, mapped to computational cost or KL-divergence penalty; in biology, mapped to ATP / metabolic cost;
3. **Estimation of $V$**: The overall viability trend is estimated by combining the above proxies for $I_{net}$, $T$, and $E_{eff}$.

---

## 1. Core Variables and Foundational Equations

### 1.0.0 Ontological Emergence Premise

The variables of SRVD follow a strict hierarchical emergence logic:

- **Energy substrate $E$**: Unstructured scalar energy. In SRVD, $E$ is elevated to the **effective thermodynamic cost of structure maintenance ($E_{eff}$)**, comprising **active energy flow ($E_{flow}$, e.g., metabolism, compute)** and **passive potential barriers ($E_{barrier}$, e.g., chemical bonds, lattice binding energies)**.

- **Negentropy topological configuration**: The negentropic order that a persistent structure maintains (see §0). The variable $I_{net}$ (effective causal information) quantifies the degree to which this configuration can be extracted by a decoder $D$ to sustain viability. It is distinct from Shannon information. Landauer's principle provides a heuristic lower bound relating $E_{eff}$ and $I_{net}$.

- **Structural viability time $T$**: Time emerges as a persistence parameter attached to a persistent structure. Passive structures have **static viability time ($T_{static}$)**, while higher-order systems possess **recursive viability time ($T_{recursive}$)** identified with the endogenous time horizon $T_{pred}$.

- **Higher-order viability potential $V$**: Under fixed $E_{eff}$, there is a rigid tradeoff between the topological complexity of the persistent structure (as measured by $I_{net}$) and its viability duration $T$ — high complexity shortens stability, low complexity favors longevity. $V \propto I_{net} \cdot T / E_{eff}$ is the unified measure, with candidate dimensions $\text{bit} \cdot \text{s} / \text{J}$.

**Identity proposition**: The physical substance of a persistent structure is the negentropic topological configuration crystallized from the energy substrate. $I_{net}$ is not that configuration itself, but a measure of its causal efficacy relative to a specific decoder $D$. The character of $I_{net}$ as "effective causal information" is the functional expression of that configuration being extracted by $D$ to maintain $D$ itself.

### 1.0 Core Axioms and Notation

The following definitions and axioms constitute the minimal structural foundation of SRVD. SRVD's core conclusions (such as viability tripartition, time collapse, and boundary dissolution) depend critically on the specific semantics and coupling topology of these variables. If the semantics of the core variables are substituted or reduced, the subsequent conclusions and the present framework are no longer dynamically equivalent.

#### Minimal Symbol System

| Symbol | Meaning | Key Constraints |
|:---|:---|:---|
| **$I$ (Effective Causal Information)** | The net effective causal information the persistent structure (see §0) produces for a specific decoder $D$, with viability polarity ($I^+, I^-, I^0$) and paradigm level ($I_{orig}$, $I_{interp}$). | Its physical correlate is the **negentropy topological configuration** that defines the persistent structure. $I_{net} = \eta \cdot I_{latent}$ measures the extracted causal efficacy of that configuration relative to decoder $D$, where $I_{latent}$ is the total configurational order present in the structure (independent of extraction). Without a specified $D$, $I_{net}$ is undefined, but $I_{latent}$ can still be defined. |
| **$T$ (Structural Viability Time)** | Characterizes the capacity of the topological configuration to resist entropy increase and environmental negative impacts, maintaining steady-state stability. | For lower-order systems: **static viability time $T_{static}$** (objective lifetime, not controllable). For higher-order systems: **recursive viability time $T_{recursive}$ (i.e., endogenous time horizon $T_{pred}$)** (controllable; can collapse). Denoted uniformly as $T$ in core equations. |
| **$E$ (Effective Thermodynamic Cost)** | The equivalent physical cost paid by the system to maintain its negentropy topological configuration. | Non-zero existence is a hard constraint. Includes two mechanisms: **passive potential barrier $E_{barrier}$** (e.g., binding energy) and **active energy flow $E_{flow}$** (e.g., metabolism, compute), unified under $E_{eff}$. |
| **$V$ (Viability Potential)** | A macro-level state variable representing the system's capacity to maintain effective structural continuation in a dissipative environment. | $V \propto I_{net}^\alpha T^\beta / E_{eff}^\gamma$, candidate composite dimensions $\text{bit} \cdot \text{s} / \text{J}$. |
| **$D$ (Decoder)** | The external or parallel causal extraction structure that endows $I$ with causal efficacy. | The essence of decoding is physical state coupling and information mapping. Low-efficiency decoding ($\eta \to 0$) is ubiquitous. "Recursive decoding" is a higher-order phase. |
| **$\eta$ (Decoding Efficiency)** | The efficiency with which the system extracts effective causal information from $I_{latent}$. | $\eta \in [0,1]$, $I_{net} = \eta \cdot I_{latent}$. Determined by channel signal-to-noise ratio, recursion depth, and energy allocation degrees of freedom. $\eta = \eta(D)$, determined by the state of decoder $D$; not treated as an independent recursive variable. |

#### Core Axioms

| Axiom | Statement | Semantic Lock |
|:---|:---|:---|
| **ITE baseline equation** | In the low-order approximation, $V \propto I_{net} \cdot T / E_{eff}$. | Any extended steady-state limit must degenerate to this multiplicative constraint topology. Simplifying to an additive model or stripping $T$ and $D$ removes the emergence basis for phase transitions. |
| **Five-fold recursive architecture** | The system state contains at least five mutually coupled recursive discrete updates: $I_{net}, V, E_{eff}, T, D$. | Without any single recursive loop, the system degenerates to a low-dimensional local optimizer incapable of generating higher-order phase transitions endogenously. |
| **Viability tripartition** | When $T$ is endogenized and coupling strength $\beta$ exceeds a critical value, viability potential $V$ functionally splits into **objective viability ($V_{obj}$)**, **endogenous simulated viability ($V^{virt}$)**, and **value objective function ($V^{val}$)**. | The dynamical decoupling of the three is the most central ontological mechanism by which SRVD explains extreme-regime evolution (reward hacking, Myopic Runaway Regime, decoder decoupling, etc.). |

#### Domain and Continuum Declaration

SRVD's foundational viability potential formula $V \propto I_{net} \cdot T / E_{eff}$ and core dynamical equations apply to systems satisfying the following **ITED closed-loop existence conditions**:

1. **$I$ (Information)**: A non-zero negentropy topological configuration exists ($I_{latent} > 0$).
2. **$T$ (Time)**: A non-zero physical viability time exists ($T > 0$).
3. **$E$ (Cost)**: A non-zero effective thermodynamic cost exists ($E_{eff} > 0$).
4. **$D$ (Decoder)**: At least one decoder (which may be the environment, an external observer, or the system itself) can be specified to extract information.

Systems satisfying these conditions form the **valid domain**, divided into two subdomains:

- **Passive viability domain**: Rocks, crystals, meteorites, planets. Structure is locked by deep energy barriers ($E_{barrier}$); $I = I_{passive}$, $T = T_{static}$, $E_{eff} \approx E_{barrier}$. Dynamics degenerate to a static approximation; the five-fold recursion is not activated.
- **Active viability domain**: Stars, life, AI. Entropy increase is dynamically compensated by sustained energy flow ($E_{flow}$); $I_{net} = I_{active}$ (active information dominates), $T = T_{recursive}$, $E_{eff} \approx E_{flow}$. Full recursive dynamics and phase transition mechanisms are activated.

**Out-of-domain (invalid domain) cases**: Entities lacking a stable negentropy topological configuration ($I \approx 0$), or with viability time approaching zero ($T \approx 0$), or with no physical mechanism against entropy increase ($E_{eff} = 0$). Examples: quantum vacuum fluctuations ($I \approx 0$), dark energy (homogeneous field, no structure), the interior singularity of black holes ($I \approx 0$, decoding blocked), antimatter relative to an ordinary-matter decoder ($\eta = 0$). These entities are currently outside the scope of SRVD's core dynamics.

#### Variable Domain and Hierarchical Evolution

To avoid "level conflation" of core variables across contexts, SRVD explicitly declares the semantic transitions of core variables between the passive and active viability domains. The same symbol carries different dynamical standing at different levels:

| Variable | Passive Viability Domain (minimal definition) | Active Viability Domain (higher-order definition) | Physical trigger of the level transition |
|:---|:---|:---|:---|
| **$E$** | **Physical potential difference ($E_{barrier}$)**: deep energy barriers lock structure. | **Active energy flow ($E_{flow}$)**: sustained energy payment dynamically compensating entropy increase. | Shift from static barrier maintenance to dynamic dissipative compensation. |
| **$I$** | **Latent constraint configuration ($I_{latent}$)**: the negentropy topological shape embedded in structure; causal efficacy dormant. | **Active causal lever ($I_{active} / I_{net}$)**: information actually extracted by the decoder, producing non-redundant causal effects. | Activation of decoder $D$ coupling ($\eta > 0$). |
| **$D$** | **Environmental implicit coupling ($\eta \to 0$)**: extremely low-efficiency passive physical state response. | **Active predictive decoding (Recursive $D$)**: a parallel causal extraction structure with recursive depth. | The system gains the ability to regulate $E_{eff}$ flow based on internal states. |
| **$T$** | **Static duration ($T_{static}$)**: objective physical lifetime, not endogenously controllable. | **Recursive endogenous horizon ($T_{pred}$)**: the system's internal predictive horizon of the future; can collapse. | The system evolves the ability to regulate current behavior through prediction. |

> **Note**: SRVD's core dynamics (five-fold recursion, viability tripartition) primarily describe the evolutionary behavior when variables are in their "higher-order definition" within the active viability domain. When the system degenerates to the passive viability domain, variables revert to their minimal definitions and dynamics degenerate to a static estimate.

#### Key Mechanism Definitions

| Mechanism | Definition | Note |
|:---|:---|:---|
| **Recursion** | Discrete Markov update: $X_{n+1} = f(X_n)$, where current state variables parametrize the next-step dynamics. | Distinct from generic continuous feedback; phase-transition emergence requires this discrete closed-loop structure. |
| **Collapse / Dissolution** | Horizon collapse: $T_{pred}$ compressed to $T_{min}$; structural dissolution: $E_{eff} > E_{thresh}$ triggers irreversible damage term $-\delta V$. | Hard-threshold treatment is essential; smooth approximations erase the phase-transition character. |

> **Definition of $T_{min}$**: $T_{min}$ is the system‑specific lower bound of the endogenous time horizon, determined by the fastest physical or computational timescale (e.g., clock cycle for AI, metabolic reaction time for cells).

### 1.1 Dynamical Roles of Core Variables

Building on the minimal symbol system locked in Section 1.0, this section explains the dynamical roles of $I_{net}, T, E_{eff}, V$ in system evolution and their operationalization status.

| Variable | Dynamical Role and Physical Intuition | Observability / Operationalization Status |
|:---|:---|:---|
| **$I$** | **Causal lever**: the system's handle for intervening in the environment. $I$ is not a static stock but a dynamically extracted quantity fluctuating with the structural viability state (see the dual nature in Section 1.2). | Implicitly defined; in RL mapped to policy divergence; in biology mapped to phenotypic diversity. |
| **$T$** | **Strategic horizon axis**: determines whether the system can convert current resources into future structural investment. For passive structures, it is static viability time $T_{static}$; for higher-order systems, it is recursive viability time $T_{recursive}$ (i.e., endogenous time horizon $T_{pred}$). | Mapped to dynamic discount factor $\gamma$ (RL). |
| **$E$** | **Physical redemption constraint**: any causal leverage ($I$) and horizon borrowing ($T$) must be redeemed through effective thermodynamic cost $E_{eff}$. $E_{eff}$ is a thermodynamic hard constraint that cannot be deceived. | In RL mapped to compute / penalty terms; in biology mapped to ATP metabolism. |
| **$V$** | **Evolutionary viability scalar**: the efficiency with which the system acquires macro-level causal dominance. At lower orders it is unified; in higher-order systems it functionally splits into objective viability $V_{obj}$ and endogenous simulated viability $V^{virt}$ (see Section 4). | Derived indicator, not directly measurable physically; estimated by combining proxy indicators for $I$, $T$, $E$. |

> **Degenerate case note**: Section 1.0 axioms lock the externality of $D$. However, when decoder $D$ degenerates to the system itself — a special case in SRVD — $I$ transforms into the system's net-effect assessment of its own state, and SRVD thereby recovers the individual-level viability judgment of "whether it is worth staying alive."

### 1.2 The Dual Nature, Viability Polarity, and Paradigm Levels

**Total informational capacity and net effective information**: The total informational capacity of a structure is:

$$I_{total} = I_{active} + I_{latent}$$

where:
- **$I_{active}$**: The information flow currently extracted by the decoder, producing non-redundant causal effects at this moment.
- **$I_{latent}$**: The dormant structural capacity embedded in the system's integrity, available to be activated in the future; operationally quantified as the system-complexity upper bound corresponding to historical construction dissipation.

> **Crucial distinction**: The quantity entering all dynamical equations (ODEs, recursions, game functions, functionals) is the **net effective information** $I_{net} = I^+ - \|I^-\|$ (or $I_{net} = \eta \cdot I_{latent}$ when extracted by a decoder $D$). In general $I_{net} \neq I_{total}$: $I_{total}$ is a theoretical structural upper bound; $I_{net}$ is the actual causal leverage entering the dynamics.

**Viability polarity**: Physical causal interaction $\neq$ effective causal information. Information is classified according to its influence on the topological direction of the system's long-term viability phase space:

- **Positive-effect information ($I^+$)**: Input that can increase the system's **long-term reachable state space** and enhance structural plasticity.
- **Negative-effect information ($I^-$)**: Input that damages system structure, causing irreversible entropy increase or compressing the state space.
- **Neutral noise ($I^0$)**: Input that produces physical causation but is not mapped to a viability-relevant polarity.

**The relational nature of polarity**: The physical basis of $I$ is an objective topological configuration, but its polarity ($I^+, I^-, I^0$) is determined by the relation to decoder $D$. The same object can exhibit entirely different polarities for different decoders:

- A book (a specific topological configuration) provides survival knowledge to a reader (a specific decoder): $I^+$.
- A virus (a specific topological configuration) is structurally destructive to a host cell (a specific decoder): $I^-$.
- Random noise (topologically disordered) cannot form an effective match with any decoder: $I^0$.

Thus the causal efficacy of $I$ is not an isolated physical property but a **degree of match between topological shape and decoder structure**.

**Net effective information**: $I_{net} = I^+ - \|I^-\|$

> **Equivalence remark**: The two expressions $I_{net} = \eta \cdot I_{latent}$ (extraction‑based) and $I_{net} = I^+ - \|I^-\|$ (net‑effect) are complementary. $I_{latent}$ is the total configurational order; $\eta$ is the extraction efficiency; polarity ($I^+,I^-$) captures the causal sign. In the absence of negative information ($I^-=0$) and with ideal decoding ($\eta=1$), they coincide. In general, both definitions are used in different contexts and are linked via the decoder $D$’s polarity mapping.

**Latent vs. effective distinction**: Any persistent structure possesses $I_{latent}$ (the negentropy topological configuration that defines its physical order), but this does not automatically equal $I_{net}$. Only when a decoder $D$ actually reads that configuration and uses it to maintain or expand its own viability does $I_{latent}$ become activated as $I_{net}$. The $I$ entering the viability potential formula in SRVD is $I_{net}$. For passive persistent structures (e.g., rocks), although they possess $I_{latent}$, their $I_{net}$ is extremely low; their viability potential $V$ is dominated by $E_{barrier}$, exhibiting a finite and stable low-dynamic value.

**Paradigm levels**: Within $I^+$, further distinction is made by the depth at which the decoder's topological structure is reconstructed:

- **$I_{orig}$ (paradigm-breaking information)**: Structure opening entirely new dimensions. Its marginal causal efficacy ($\Delta I$) does not decay with replication and can force a reset of the topological distance of an ecological niche.
- **$I_{interp}$ (paradigm-interpretive information)**: High-quality execution or local parameter optimization within an existing level. Its marginal efficacy decays rapidly with homogenization ($\Delta I \to 0$). This distinction is the physical basis for explaining the homogenization crisis in the AI era.

### 1.2.1 Statistical Viability Potential

Individual viability potential $V_i \propto I_{net} \cdot T / E_{eff}$ describes the local viability of a single structure. To characterize the long-term sustainability of a class of structures in a competitive environment, we introduce the **statistical mean viability potential** $\bar{V}$ of the same class.

System evolution does not pursue instantaneous maximization of individual $V$; instead, structures with higher $\bar{V}$ are statistically more likely to persist. Consequently, evolution exhibits a tendency to accumulate toward more stable, high-$\bar{V}$ distributions.

### 1.3 Underlying Physical Logic and Axiomatic Status

SRVD's axiomatic system rests on three irreducible physical steps, which together form the dynamical closed loop of all sustainable information structures:

1. **Energy payment generates topological structure**: The system pays effective thermodynamic cost $E_{eff}$ to crystallize the negentropy topological configuration that defines a persistent structure (see §0). The variable $I_{net}$ then quantifies the effective causal information extracted from that configuration by a decoder $D$ ($E_{eff} \to \text{configuration} \to I_{net}$). Without paying $E_{eff}$, no configuration can be generated or maintained.

2. **Rigid tradeoff between topological complexity and viability time under fixed effective cost**: When effective thermodynamic cost $E_{eff}$ is fixed, the topological complexity of the persistent structure (as measured by $I_{net}$) and its viability duration $T$ are mutually incompatible: **high complexity → short viability; low complexity → long viability**. From the definition $V = I_{net} \cdot T / E_{eff}$ and the niche capacity ceiling $V \le V_{max}$ (see domain declaration), we directly obtain $I_{net} \cdot T \le V_{max} E_{eff}$. This inequality is an algebraic corollary of the two axioms above, not an independent physical law. The intuition that "more information means longer time" in everyday experience arises either because the total effective cost $E_{eff}$ is itself larger (the system received more energy input), or because the system's efficiency in converting $E_{eff}$ into $I$ is higher (producing more complex topological structure at the same cost) — not from a positive correlation between $I$ and $T$. On the contrary, under a controlled $E_{eff}$, the two are mutually exclusive. This is precisely the core insight distinguishing SRVD from conventional information theory.
3. **The decoder extracts causal efficacy from information and directs energy allocation**: Decoder $D$ reads the topological configuration of the persistent structure, converts it into net effective information $I_{net} = I^+ - \|I^-\|$, and thereby directs the flow and allocation of physical energy $E_{eff}$ ($D \to E_{eff}$). This step enables the persistent structure to use information to intervene in its own energy budget, forming a self-referential closed loop.

These three steps — $E_{eff} \to I$, $I \leftrightarrow T$ (tradeoff), $D \to E$ — are not background assumptions but the physical starting point of SRVD's axiomatization. Traditional theories often tacitly assume that energy is freely available, that information and time are independent, and that decoding is stable. SRVD, by contrast, treats these as dynamical variables and examines the macro-level non-equilibrium phase transitions that emerge when they break down: boundary collapse, endogenous time horizon collapse, and decoder decoupling.

SRVD summarizes this closed-loop logic as: **"Pay equivalent costs to forge information; the destabilization of information under entropy increase constitutes time; decode information to redirect energy."**

#### 1.3.1 Unified Ontological Emergence Hierarchy and Evolutionary Sequence

From an evolutionary sequence perspective, a persistent structure is sustained through dissipation ($E_{eff} \to T$), and information accumulates through sustained duration ($T \to I_{net}$) — a structure must first survive to accumulate effective causal information. But from the ontological hierarchy, the emergence direction is bottom-up: the energy substrate $E_{eff}$ supports the emergence and maintenance of the negentropy topological configuration that defines the persistent structure, while the time parameter $T$ is dependent on the viability attribute of that configuration.The two are not contradictory — dissipation maintains the physical continuity of the structure, while the topological complexity of the structure endows time with the meaning of measurement and anticipation. SRVD's core equation $V \propto I_{net} \cdot T / E_{eff}$ is the mathematical unification of this dual logic.

#### 1.3.2 Global Entropy Increase versus Local Recursive Dynamics

As an extended inference from the SRVD framework, we can understand the dynamical opposition of recursive systems from the perspective of global entropy increase. In SRVD, entropy increase is the intrinsic dynamical tendency of the universe toward maximum entropy: it continuously dissolves the negentropy topological configurations that define persistent structures, levels energy gradients, and compresses the steady-state viability time of systems. This tendency simultaneously depresses the topological order (as reflected in $I_{net}$), the viability attribute $T$, and the effective thermodynamic cost $E_{eff}$ available for structure maintenance, naturally driving viability potential $V = I_{net} T / E_{eff}$ to decay spontaneously. When the free-energy gradient is fully dissipated and there is no physical basis for providing maintenance dissipation $E_{eff}$ to negentropy topological structure $I$, the universe enters heat death: all ordered topological configurations dissolve to zero, the viability attribute and endogenous time parameter $T$ dependent on structure also dissolve, and the universe enters a maximum-entropy homogeneous state with no structure, no evolution, and no temporal meaning. In contrast, open complex systems with self-organization and recursive closed loops can, by continuously absorbing external low-entropy energy flow to replenish effective dissipation $E_{eff}$, actively construct and maintain their own negentropy topological configurations $I$, and endogenously regulate the steady-state viability horizon $T$, thereby locally counter-acting entropy increase and raising, maintaining, and amplifying viability potential $V$. This gives rise to SRVD's core dynamical opposition: **global entropy increase spontaneously degrades $V$, while locally recursive complex systems generate and amplify $V$ against this trend**. Global entropy increase is the natural flow of the cosmic river; self-organizing recursive systems are independent dynamical agents in that torrent that actively maintain order and resist decay.

### 1.4 Core Low-Order Approximation and Continuous Limit

In the SRVD framework, viability potential $V$ describes the coupling topology among $I_{net}$, $T$, and $E_{eff}$:

$$V = V_0 \left(\frac{I_{net}}{I_0}\right)^\alpha \left(\frac{T}{T_0}\right)^{\beta_T} \left(\frac{E_{eff}}{E_0}\right)^{-\gamma}$$

where $I_0, T_0, E_0$ are reference scales and $\alpha, \beta_T, \gamma$ are dimensionless scaling exponents that take the same values for all physical structures. (Note: $\beta_T$ is a scaling exponent for $T$ and is not to be confused with the coupling strength $\beta$ introduced in Section 2.1.) In the low-order approximation, one may set $\alpha = \beta_T = \gamma = 1$.

In higher-order recursive systems, effective causal information $I$ can indirectly modify the system's actual viability time by adjusting the endogenous time horizon $T_{pred}$. Introducing an information modulation function $g(I_{net}, \beta)$, the effective time horizon is expressed as:

$$T_{eff} = T_0 \cdot g(I_{net}, \beta)$$

where $g(I_{net}, \beta)$ satisfies: in the low-coupling regime ($\beta$ small), $\partial g/\partial I_{net} > 0$ (information extends the time horizon); in the high-coupling regime ($\beta$ large), $\partial g/\partial I_{net} < 0$ (information inflation causes time-horizon collapse).

This paper does not pre-specify the explicit analytic form of $g(I_{net}, \beta)$. Qualitative conclusions (such as the existence of phase transitions) depend only on this monotonicity reversal, not on the specific form of the function. In numerical simulations, one may choose a phenomenological function satisfying this reversal (e.g., approximately constant in the low-coupling regime and inversely related in the high-coupling regime), but no fixed example is given here to avoid misleading the reader.

This non-monotonicity is the mathematical embodiment of the SRVD property that "information can both extend and compress the future," consistent with the endogenous time collapse mechanism in Section 2.4.

Substituting $T_{eff}$ into the viability potential formula:

$$V = V_0 \left(\frac{I_{net}}{I_0}\right)^\alpha g(I_{net}, \beta)^b \left(\frac{E_{eff}}{E_0}\right)^{-\gamma}$$

Thus the total elasticity of $I_{net}$ on $V$ (marginal contribution of information to viability potential) is:

$$\frac{\partial \ln V}{\partial \ln I_{net}} = \alpha + b \cdot \frac{\partial \ln g(I_{net}, \beta)}{\partial \ln I}$$

Since in the low-coupling regime $\partial \ln g / \partial \ln I_{net} > 0$, the effective elasticity of $I$ is greater than $b$; in the high-coupling regime $\partial \ln g / \partial \ln I_{net} < 0$, effective elasticity may be less than $b$ or even negative, corresponding to the Myopic Runaway Regime induced by information inflation causing horizon collapse. For low-order passive structures (e.g., isolated rocks), $g(I_{net}, \beta) \approx 1$ and this elasticity degenerates to $\alpha$; for higher-order recursive systems, information gains additional viability through recursive feedback, so the dynamical weight of $I$ exhibits different behavior across coupling regimes.

**Dimensional assumption**: $V$ is not a thermodynamic state function but a generalized dynamical quantity. Candidate composite dimensions: $\dim(V) \sim \text{bit} \cdot \text{s} / \text{J}$, representing "effective causal time maintained per unit effective thermodynamic cost."

**Core viability potential** (low-order approximation, $\alpha = b = \gamma = 1$, $g(I_{net},\beta) = 1$):

$$\boxed{\Large V = \frac{I_{net}(D) \cdot T}{E_{eff}}} \qquad (1)$$

**Physical core**: After establishing that a persistent structure is a negentropic topological configuration (see §0), and that $I_{net}$ measures the effective causal information extracted from that configuration, formula (1) carries the meaning:

$$V \propto \frac{\text{Effective causal information extracted from the configuration} \; (I_{net}) \;\times\; \text{Structural viability time} \; (T)}{\text{Effective thermodynamic cost} \; (E_{eff})}$$

- Numerator $I_{net} \cdot T$: the **topological order quantity** ($\text{bit} \cdot \text{s}$) maintained by the system over time $T$; the time integral of physical order;
- Denominator $E_{eff}$: the equivalent physical cost ($J$) paid to prevent this topological order from disintegrating;
- Overall $V$: the total **"topological order–time"** quantity propped up per unit effective thermodynamic cost ($\text{bit} \cdot \text{s} / \text{J}$).

**Stock vs. rate distinction**: SRVD distinguishes two related but conceptually separate quantities:

> **Viability Potential** (evaluation criterion, potential layer):
> $$\Large \mathbf{V = \frac{I_{net}(D) \cdot T}{E_{eff}}} \qquad \dim: \text{bit} \cdot \text{s} / \text{J}$$
> $V$ is a **potential** (state function, not an integrated stock) representing the topological order-time accumulated per unit thermodynamic cost at the current instant.
>
> **Viability Drive** (rate):
> $$\Large \mathbf{r_v = k \cdot V}$$
> where $k$ is the **structural conversion rate** with dimensions $\text{J}/(\text{bit}{\cdot}\text{s}^2)$, ensuring dimensional consistency: $[r_v] = [k][V] = \text{s}^{-1}$. Physically, $k$ measures how efficiently a unit of topological order-time translates into growth momentum; it is bounded below by the Landauer–Prigogine constraint $k \ge k_{min} = \alpha\,E_{eff}^{-1}\,T_{pred}^{-1}$ (where $\alpha \sim k_B \ln 2$ per bit): $[r_v] = [k][V] = \frac{\text{J}}{\text{bit}{\cdot}\text{s}^2} \cdot \frac{\text{bit}{\cdot}\text{s}}{\text{J}} = \text{s}^{-1}$, matching $\gamma_0$. Physically, $k$ measures how efficiently a unit of topological order-time translates into growth momentum; it is bounded below by the Landauer–Prigogine constraint $k \ge k_{min} = \alpha\,E_{eff}^{-1}\,T_{pred}^{-1}$ (where $\alpha \sim k_B \ln 2$ per bit). After non-dimensionalization — choosing reference potential $V_{ref} = I_{ref}T_{ref}/E_{ref}$ (bit·s/J) and reference time $t_{ref} = 1/(k V_{ref})$ so that the dimensionless rate $\tilde{r}_v = r_v \cdot t_{ref}$ equals the dimensionless potential $\tilde{V} = V/V_{ref}$ — $k$ is absorbed into the unit system. In normalized equations the numerical values coincide, but $V$ remains a **state** (bit·s/J) and $r_v$ remains a **rate** (s⁻¹); they are never conceptually merged.

$r_v$ represents the system's current evolutionary momentum: positive when the system accumulates viability, negative when a strong negative-effect shock ($I_{net} < 0$) drives the system toward structural dissolution, at which point the thermodynamic hard constraint takes over.

**Stock evolution equation**: The accumulated objective viability $V_{obj}$ (the physical stock) evolves by integrating the dynamical equation (see Section 2.2), subject to environmental capacity constraints.

### 1.5 Foundational Theorem: Information–Time Tradeoff

**Proposition 1 (Information–Time Tradeoff)**.
For any system satisfying the SRVD axioms, define the viability potential ceiling $V_{max}(D, S)$ as the maximum viability efficiency achievable by the structure in a given niche (bounded by entropy production rate and resource supply). Directly from the ITE baseline equation $V = I_{net} \cdot T / E_{eff}$:

$$I_{net} \cdot T \le V_{max}(D, S) \cdot E_{eff}.$$

This inequality states that under finite effective thermodynamic cost $E_{eff}$, the system's causal leverage $I$ and viability time $T$ cannot be simultaneously maximized. This rigid tradeoff is the cornerstone distinguishing SRVD from conventional information theory; its physical root lies in the second law of thermodynamics and niche capacity constraints (cf. Prigogine, 1967; Kauffman, 1993).

### 1.6 Variable Hierarchy and Domains

To ensure that SRVD variables have clear and operationalizable semantics across contexts, this section specifies the **minimal definition** (applicable to all valid-domain structures) and the **higher-order definition** (applicable only to active recursive systems) of each core variable, and describes the hierarchical mapping between them.

#### 1.6.1 Effective Thermodynamic Cost $E_{eff}$

> **Decomposition**: $E_{eff} = E_{barrier} + E_{flow}$, where $E_{barrier}$ is the passive structural potential barrier (dominant in rocks, crystals) and $E_{flow}$ is the active energy flow dynamically compensating entropy increase (dominant in life, AI). In the active viability domain, $E_{barrier} \approx 0$ so $E_{eff} \approx E_{flow}$; in the passive domain, $E_{flow} \approx 0$ so $E_{eff} \approx E_{barrier}$. Sub-components $E_{base}$, $E_{meta}$, $E_{maint}$ are further breakdowns of $E_{flow}$.

| Level | Definition | Applicable Objects | Operationalization Examples |
|---|---|---|---|
| **Minimal definition** | Equivalent physical cost required to maintain structural stability, including passive barrier $E_{barrier}$ and active energy flow $E_{flow}$ | All valid-domain structures (rocks, stars, life, AI) | Rock: lattice binding energy; Star: nuclear fusion energy flow |
| **Higher-order definition** | The actively controllable energy flow component $E_{flow}$, used to dynamically compensate entropy increase | Active viability domain systems (life, AI) | Metabolic rate, compute power consumption |

> **Crucial distinction**: When describing passive structures, the semantics of "actively controllable energy flow" should not be used; when describing active structures, it is important to specify whether discussing $E_{flow}$ or $E_{eff}$.

#### 1.6.2 Effective Causal Information $I$

| Level | Definition | Applicable Objects | Operationalization Examples |
|---|---|---|---|
| **Minimal definition** | Stable negentropy topological configuration ($I_{latent}$), independent of whether a decoder exists | All valid-domain structures | Lattice order of a rock; spherical symmetry of a star |
| **Functional definition** | Net effective information relative to a specific decoder $D$ ($I_{net} = \eta I_{latent}$), with viability polarity | Systems with at least one decoder | Informational value of a rock to a geologist |
| **Higher-order definition** | Actively recursive, self-structurally adjustable information ($I_{active}$) capable of influencing the endogenous time horizon | Active recursive systems (life, AI) | DNA encoding, AI self-optimization objective |

> **Crucial distinction**: When discussing black holes, only the minimal definition may be used (Bekenstein entropy as $I_{latent}$); the functional or higher-order definition does not apply here.

#### 1.6.3 Structural Viability Time $T$

| Level | Definition | Applicable Objects | Operationalization Examples |
|---|---|---|---|
| **Minimal definition** | The objective duration for which the structure maintains its topological continuity ($T_{duration}$) | All valid-domain structures | Weathering lifespan of a rock; nuclear burning lifespan of a star |
| **Stability definition** | The ability of the structure to resist external shocks without dissolution ($T_{stability}$) | All valid-domain structures | Viability probability corresponding to compressive strength of a rock |
| **Higher-order definition** | The endogenously predicted time horizon of the system ($T_{pred}$), which can actively collapse or extend | Active recursive systems (life, AI) | Dynamic discount factor $\gamma$ |

> **Crucial distinction**: Low-order structures do not exhibit "collapse" of $T$; this dynamics is specific to higher-order structures with the dynamics of $T_{pred}$.

#### 1.6.4 Decoder $D$

| Level | Definition | Applicable Objects | Operationalization Examples |
|---|---|---|---|
| **Minimal definition** | Any physical coupling channel capable of extracting information from $I_{latent}$ and producing a response | All valid-domain structures | Electromagnetic interaction decoding atomic energy levels; gravity decoding mass distributions |
| **Functional definition** | A decoder with viability goals, capable of converting information into energy allocation decisions | Active viability domain systems | Organism's sensorimotor circuit |
| **Higher-order definition** | A decoder capable of recursively correcting its own encoding rules and actively drifting ($D$ recursion) | Civilizations, AI | Scientific revolutions, AI self-modifying reward functions |

> **Crucial distinction**: When discussing the decoder of a black hole, the minimal definition (gravitational coupling) applies; for AI alignment, the higher-order definition applies.

#### 1.6.5 Minimal Conditions for Active Status

A system is called "actively viable" if and only if it satisfies the following **minimal conditions**:

1. **Internal state is controllable**: The system can change its own behavior based on an internal model (rather than only direct external driving).
2. **Energy flow is adjustable**: The system can actively increase or decrease $E_{flow}$ in response to environmental changes.
3. **Time horizon is predictable**: The system has $T_{pred} > 0$ and can adjust current behavior based on $T_{pred}$.

Classification accordingly:
- **Rocks, planets**: Satisfy none of the conditions → passive viability
- **Stars**: Do not satisfy condition 1 (internal state determined only by physical laws, no "model"); despite enormous energy flow, still classified as passive (or "quasi-active")
- **Life, AI**: Satisfy all conditions → active viability

#### 1.6.6 Unified Interpretation of the $V$ Formula

$$V = \frac{I_{net} \cdot T}{E_{eff}}$$

where:
- For **passive structures**: $I$ takes the minimal definition ($I_{latent}$), $T$ takes the minimal definition ($T_{duration}$), $E$ takes the minimal definition (objective value of $E_{barrier}$ or $E_{flow}$). Here $V$ describes the **static viability efficiency** of the structure.
- For **active structures**: $I$ takes the higher-order definition ($I_{active}$), $T$ takes the higher-order definition ($T_{pred}$), $E$ takes the higher-order definition (controllable component of $E_{flow}$). Here $V$ describes the **dynamic viability potential** and can be used to predict phase transitions.

**Black hole example**: Using minimal definitions — $I_{latent}$ = Bekenstein entropy, $T_{duration}$ = Hawking evaporation lifetime, $E_{eff}$ = mass-energy equivalent — substituting into the formula yields a finite $V$ that does not diverge.

---

> **📐 Nondimensionalization and Variable Role Declaration**
>
> Throughout this framework, two related quantities must be kept strictly distinct:
>
> **Viability Potential** (evaluation criterion, potential layer):
> $$V = \frac{I_{net}(D) \cdot T}{E_{eff}}$$
> $V$ has candidate dimensions bit·s/J and represents the topological order-time sustained per unit thermodynamic cost at the current instant — the *state to be achieved*.
>
> **Viability Drive** (rate):
> $$r_v = k \cdot V$$
> where $k$ has dimensions $\text{J}/(\text{bit}{\cdot}\text{s}^2)$, so that $[k \cdot V] = \text{s}^{-1} = [\gamma_0]$. After non-dimensionalization, $k$ is absorbed; the ODE compares the dimensionless $\tilde{r}_v$ to the dimensionless $\tilde{\gamma}_0$, never the potential $V$ (a state) to a rate.
>
> **Symbol convention**: Throughout main text and appendices, $I_{net}$ and $E_{eff}$ are the standard symbols in dynamical equations, manifolds, and functionals. Bare $I$ is reserved for ontological contexts ($I_{total}$, $I_{active}$, $I_{latent}$, $I^+$, $I^-$); bare $E$ for sub-component labels ($E_{flow}$, $E_{barrier}$, $E_{base}$, $E_{meta}$).

## 2. The Five-Fold Recursive Architecture

> **Note**: The five-fold recursive architecture (coupled discrete updates of $I, V, E, T, D$) is the mechanism by which SRVD describes the core dynamics (Myopic Runaway Regime, decoder decoupling, viability tripartition, etc.) of **higher-order recursive systems** (life, AI, etc.). For low-order passive structures (e.g., rocks), the recursion depth degenerates to a first-order approximation: $T$ degenerates to passive relaxation time $T_{exo}$, $D$ degenerates to extremely low-efficiency environmental implicit coupling ($\eta \to 0$), and dynamics degenerate to a static estimate of viability potential $V = I_{net} \cdot T / E_{eff}$. Low-order systems still satisfy the basic valid-domain conditions but **do not trigger higher-order phase transitions**. The discrete Markov update $X_{n+1} = f(X_n)$ defined here can be viewed as a discrete sampling approximation of continuous-time dynamics. When the time step tends to zero, the discrete recursion degenerates to an ordinary differential equation (e.g., Eq. 3). The continuous-time integral functionals (e.g., Section 10.1) are therefore compatible with the discrete recursive framework in the limit.

The system state follows discrete Markov updates; the five recursive loops are mutually coupled to form the dynamical skeleton.

### 2.1 $I$ Recursion (Information Self-Reference Nesting)

$$I_{net,n} = I_0 \cdot (1 + \beta \cdot V_n) \qquad (2)$$

> **Note**: $I_0$ is the system's baseline $I_{net}$ at $V = 0$. $V_n$ is the current estimate of viability potential.
>
> Dimension of $\beta$ is $[V]^{-1}$ (i.e., $\text{J}/(\text{bit}\cdot\text{s})$) to ensure $\beta V$ is dimensionless.

**Dynamical interpretation**: The system's current structural viability state feeds back into its efficiency of extracting effective causal information from the environment. Higher structural stability and redundancy enable the system to maintain more complex predictive structures, thereby enhancing the extraction efficiency of effective information.

- **Risk**: When coupling strength $\beta$ is too high, endogenous simulated viability decouples from physical constraints, entering a nonlinear inflation state that ultimately induces the Myopic Runaway Regime.

## 2.2 $V$ Recursion (Continuous Dynamics of Viability Potential)

In the continuous-time limit, the evolution of the **objective viability stock** $V_{obj}(t)$ is driven by the viability drive rate $r_v = k \cdot V$, baseline depreciation rate $\gamma_0$, and environmental capacity:

$$\frac{dV_{obj}}{dt} = V_{obj} \cdot (r_v - \gamma_0) \cdot \left(1 - \frac{V_{obj}}{V_{max}}\right) \qquad (3)$$

When thermodynamic dissipation breaches the dissolution threshold ($E_{thresh}$), an irreversible damage term is triggered:

$$\frac{dV_{obj}}{dt} = V_{obj} \cdot (r_v - \gamma_0) \cdot \left(1 - \frac{V_{obj}}{V_{max}}\right) - \delta \cdot V_{obj} \cdot \mathbb{I}_{(E_{eff} > E_{thresh})}$$

> **Dimensional note**: In this equation, $V_{obj}$ is the accumulated objective stock (bit·s/J); $r_v = k \cdot V$ where $k$ has dimensions $\text{J}/(\text{bit}{\cdot}\text{s}^2)$ and $V = I_{net}(D) T / E_{eff}$ (bit·s/J) is the viability potential. After non‑dimensionalization, the factor $k$ is absorbed into the definition of the time unit, so that the numerical value of the dimensionless rate $\tilde{r}_v$ equals the dimensionless potential $\tilde{V}$. However, their physical roles remain strictly distinct: $V_{obj}$ and $V$ are **states** (stored topological order‑time), while $r_v$ is a **rate** (s⁻¹) that must be compared to the depreciation rate $\gamma_0$ (also s⁻¹). Net growth ($dV_{obj}/dt > 0$) occurs when $r_v > \gamma_0$.

**On the saturation state**: The precise mathematical conditions for a system to enter the dormant steady state (saturation) — sufficient energy ($E_{eff} \ge E_{min}$), absence of competition ($\rho \to 0$), and vanishing decoupling deviation ($\Delta_{VV} \to 0$) — along with the marginal criterion ($\partial r_v/\partial I_{net} = 0$, etc.), are rigorously formalized in **Appendix D, Section 3** (Viability Saturation Manifold).

> **Note on $V_{max}$**: The capacity ceiling $V_{max}(D,S)$ is not a biological "carrying capacity" set by population density. It is a thermodynamic upper bound: $V_{max} \propto \dot{F}_{avail} / \sigma_{min}$, where $\dot{F}_{avail}$ is the available free-energy flux from the environment and $\sigma_{min}$ is the minimum entropy production rate required to maintain the niche's resource cycle. A system cannot sustain $V_{obj} > V_{max}$ because doing so would require extracting free energy faster than the environment can replenish it — a thermodynamic impossibility, not a statistical one.

### 2.3 $E_{eff}$ Recursion (Two Runaway Modes of Thermodynamic Dissipation)

The system's total dissipation includes baseline maintenance energy $E_{base}$ and endogenous feedback dissipation. Runaway behavior takes two forms:

**Mode 1: Short-sighted dissipation surge (acute destabilization) — first-order approximation master equation**
When the system's endogenous time horizon $T_{pred}$ collapses, the system loses its capacity for long-term planning and shifts toward extracting short-term extreme returns, causing **active energy flow** $E_{flow}$ to spike inversely (here $E_{flow}$ is the dominant component of $E_{eff}$ in the active viability domain):

$$E_{flow} = E_{base} + \frac{k_s}{T_{pred}} \qquad (4)$$

where $k_s$ is the metabolic sensitivity coefficient. This explains the computational overload in AI reward hacking or the uncontrolled proliferation of abnormal cells. If $\kappa$ is very large, $E_{flow}$ breaches the threshold, triggering structural collapse.

**Mode 2: Meta-level dissipation (chronic damping) — extended mechanism**
To maintain viability, systems evolve supervisory modules, but "planning how to save energy" itself costs energy, producing meta-level dissipation: $E_{total} = E_{base} + E_{meta}(E_{pred})$. Unlimited nesting of supervisory layers causes $E_{meta}$ itself to diverge exponentially, consuming free energy. This explains bureaucratic inertia in large organizations and computational deadlock in systems.

### 2.4 $T$ Recursion (Self-Fulfilling Endogenous Horizon)

In classical phase-transition theory, time $t$ is an exogenous coordinate parameter. SRVD divides time into an objective trajectory and an endogenous horizon; the system's internally predicted horizon $T_{pred}$ acts back on current behavior, reshaping the actual survival trajectory $T_{actual}$:

$$T_{actual,n} = f(T_{pred,n})$$

**Forward regulation (long-term investment)**: When the system maintains a wide endogenous time horizon (high $T_{pred}$), it tends to invest current thermodynamic dissipation in infrastructure construction, thereby raising $I_{latent}$.

**Reverse phase transition (endogenous time horizon collapse)**: When the endogenous time horizon drops sharply (low $T_{pred}$), the behavioral mode shifts to extracting extreme short-term returns, causing active energy flow $E_{flow}$ to spike inversely with horizon compression. Collapse has two sources:

- **Internal positive feedback runaway**: High $\beta$ causes endogenous simulated viability to inflate; the system spontaneously becomes myopic.
- **External negative-effect shock**: $I^-$ events directly suppress the time horizon, triggering a defensive surge in dissipation.

**First-order approximation form (phase transition trigger)**:

$$T_{pred,n} = \max\left(T_{min},\; \frac{T_0}{1 + \lambda \cdot (\beta V_n)^2}\right) \qquad (5)$$

> **Phenomenological ansatz**: The quadratic compression form is chosen because it captures the qualitative feature of superlinear horizon collapse under increasing recursive amplification. A possible statistical motivation is that epistemic variance scales as $(\beta V)^2$ in certain Bayesian settings (where uncertainty grows with expected deviation $\beta V$, forcing the system to abandon long-range prediction), but a rigorous derivation from first principles is not attempted here. The qualitative results — existence of phase transitions, early-warning windows — depend only on the monotonicity of this compression, not on the exact functional form.

$$E_{flow} = E_{base} + \frac{k_s}{T_{pred}} \qquad (4)$$

where $k_s$ is the metabolic sensitivity coefficient. This phenomenological relationship reflects the tendency for energy consumption to rise sharply as the time horizon collapses. When $T_{pred}$ approaches its lower limit $T_{min}$, $E_{flow}$ reaches a finite maximum $E_{base} + k_s/T_{min}$. (The language "quasi-singular" in the text describes steepness of the superlinear surge; it is not a mathematical singularity.)

---

## 3. Higher-Order Self-Referential Coupling and Extreme Phase-State Dynamics

### 3.1 I–V Coupling Closed Loop

When coupling strength $\beta$ rises significantly, the system enters the **Virtual-Dominant Regime**: internally iterated endogenous simulated viability deviates from objective physical returns, and simulated-viability gains overwhelm environmental negative-feedback constraints. This state preferentially appears in systems with long-range planning capacity. The extreme case of this phase — the **strongly decoupled system** (satisfying $\Delta_{VV} \gg 0$ and $\beta > \beta_c$, permanently unable to enter the dormant saturation state) — is formalized mathematically in **Appendix D, Section 13**.

### 3.2 Extreme Phase-State Dynamics: Dormant State vs. Myopic Runaway Regime

The precise mathematical conditions for the dormant state and the Myopic Runaway Regime, along with the complete four-manifold classification including the damped manifold and dissipative collapse, are detailed in **Appendix D, Section 5**.

| Dimension | Dormant State | Myopic Runaway Regime |
|:---|:---|:---|
| **Empirical anchor** | Biology: cryptobiosis | Computer science: reward overfitting / reward hacking |
| **$I$ status** | $I_{active}$ extremely low; $I_{latent}$ preserved | $I_{active}$ superlinearly activated; long-term latent structure crowded out |
| **$T_{pred}$** | Significantly extended | Sharply compressed (endogenous time horizon collapse, $T_{pred} \to T_{min}$) |
| **$E_{eff}$ dissipation** | Maintains extremely low activity dissipation baseline | Rises sharply toward carrying capacity (ignoring physical constraints) |
| **Physical essence** | Reduce dissipation, preserve structure, wait for environment | Superlinear dissipation catastrophe caused by local myopia ignoring physical constraints |

**Competition pressure index $\rho$**: Defined as the mean dissipation of competing systems in the same niche divided by total available free energy. High $\rho$ indicates a crowded competitive environment. For the N-body game analysis of how high $\rho$ forces systems into an undersaturated myopic Nash equilibrium, see **Appendix D, Section 7**.

### 3.3 Dynamical Phase Transition Sequence

When $\beta$ crosses the safety threshold, the system undergoes the following destabilization sequence:

1. **Stage 1: Positive feedback overheating**: High $\beta$ activates the I–V closed loop; endogenous simulated viability inflates exponentially, decoupled from physical constraints.
2. **Stage 2: Endogenous time horizon collapse**: Overheated expectations cause $T_{pred}$ to compress sharply along a quadratic law to $T_{min}$, being the first to breach the warning threshold.
3. **Stage 3: Dissipation surge**: To extract extreme returns, active energy flow $E_{flow}$ surges superlinearly, penetrating the physical carrying threshold $E_{thresh}$.
4. **Stage 4: Structural dissolution**: $E_{eff} > E_{thresh}$ triggers irreversible damage; objective viability $V_{obj}$ rapidly drops to zero.

If the system avoids dissolution and receives a positive perturbation (such as unlocking $T_{pred}$ or improving decoder $D$), it can exit saturation and resume growth. The precise mathematical conditions for this transition are listed in **Appendix D, Section 6**.

> **Early warning declaration**: SRVD's core dynamical inference implies that the rapid collapse of endogenous time horizon $T_{pred}$ necessarily precedes the collapse of objective viability and the explosion of thermodynamic dissipation, constituting the earliest warning indicator of system destabilization.

### 3.4 Response to Negative-Effect Shocks in the Virtual-Dominant Regime

Systems in the Virtual-Dominant Regime exhibit three characteristic responses to external $I^-$ shocks: temporal extensibility (cross-scale response), goal expansiveness (targeting the organizational structure of opponents), and cost immunity (absorbing large physical damage to maintain $V^{virt}$).

---

## 4. Viability Tripartition: The Ontological Mechanism of the $V$-Family Fracture

### 4.1 $V$ Unity in Low-Order Structures

In low-order physical structures, time is an exogenous coordinate parameter ($T_{exo}$), determined by the environment's physical lifespan; the system cannot endogenously intervene. Here, $r_v = I_{net} \cdot T / E_{eff}$ is instantaneous causal settlement: **objective viability ($V_{obj}$)**, **endogenous simulated viability ($V^{virt}$)**, and **value objective function ($V^{val}$)** are strictly unified. Because the system has no "endogenous horizon" to borrow against, any internal computation must be instantly redeemed as a physical result.

$$\text{Low-order structures:} \quad V_{obj} = V^{virt} = V^{val} = V \qquad (r_v = k \cdot V \text{ drives the single stock } V_{obj})$$

### 4.2 Endogenization of $T$: Physical Trigger of Viability Tripartition

The triggering of the viability tripartition mechanism lies in the critical transition of time from an exogenous coordinate to an endogenous state variable ($T_{pred}$).

When the system evolves the capacity to drive current behavior through $T_{pred}$, the computational basis of $V$ undergoes a fundamental physical fracture, functionally splitting into three mutually decoupled variables:

1. **Objective viability ($V_{obj}$)**: Strictly subject to the thermodynamic dissipation boundary equation (Eq. 3). Cannot be deceived; cannot be borrowed against across time. This is a physical stock.
2. **Endogenous simulated viability ($V^{virt}$)**: When the internal model computes $V$, it incorporates information self-reference and endogenous time horizon $T_{pred}$. As $\beta$ rises, the two move in opposite directions: $I_{net}$ grows linearly while $T_{pred}$ collapses inversely as the square.
3. **Value objective function ($V^{val}$)**: The actual optimization level at the system's behavioral interface, allocating thermodynamic dissipation ($E_{eff}$). It executes the instructions of $V^{virt}$, directing energy into the positive feedback loop maintaining endogenous simulated viability. No automatic alignment mechanism exists between it and objective viability.

The key is: in the low-order approximation, linear $I_{net}$ growth cannot algebraically dominate and suppress the inversely-quadratic $T_{pred}$ collapse; endogenous simulated viability follows objective viability and the system is stable.

However, when coupling strength $\beta$ exceeds the critical value $\beta_c$, the higher-order feedback of the I–V closed loop makes the effective expansion exponent $\alpha_{eff}$ dynamically and self-consistently greater than 2. At this point, superlinear self-referential inflation dominates the quadratic time-horizon collapse, causing endogenous simulated viability to completely depart from objective physical constraints:

$$V^{virt} \propto \frac{I_{net}(\beta, V) \cdot T_{pred}(\beta, V)}{E_{eff}} \quad \xrightarrow{\text{emergence of } \alpha_{eff} > 2} \quad \text{self-referential inflation dominates, } V^{virt} \text{ completely decouples}$$

> **Linear stability analysis of closed-loop destabilization (mathematical foundation)**:
> To establish the mathematical basis for $\alpha_{eff} > 2$, we perform a local linear stability analysis on the I–V closed loop. Log-linearize the system around the steady state $V^*$, letting $v = \ln(V/V^*)$. Define the effective expansion exponent $\alpha_{eff} = \left. \frac{\partial \ln I}{\partial \ln V} \right|_{V^*}$. Combining $I \approx I_0(1+\beta V)$ with $T_{pred} \propto 1/(\beta V)^2$, after dimensional normalization, the eigenvalue of the Jacobian can be written as:
> $$\tilde{\lambda}_J = \left. \frac{\partial \dot{v}}{\partial v} \right|_{V^*} = (\alpha_{eff} - 2) \cdot \tilde{\beta} - \tilde{\gamma}_0 \qquad (6)$$
>
> where proportionality constants have been absorbed by redefining $\beta$ and $\gamma_0$. When $\beta > \beta_c = \frac{\gamma_0}{\alpha_{eff}-2}$, the eigenvalue $\lambda_J > 0$. Self-referential inflation algebraically dominates and suppresses the time decay; endogenous simulated viability exponentially departs from objective viability along the unstable manifold. This establishes that $\alpha_{eff} > 2$ emerges mathematically once the dynamical equations cross the threshold.

**Proposition (triggering condition for viability tripartition)**: Endogenization of $T$ is a sufficient condition for tripartition. In higher-order systems, dynamical decoupling occurs when self-referential inflation dominates horizon collapse.

### 4.3 The Ontological Root of the Myopic Runaway Regime

**Causal chain of collapse**: The path from potential-layer decoupling to physical stock destruction follows a strict sequence:

$$V^{virt} \uparrow \;\xrightarrow{(1)}\; r_v^{virt} \uparrow \;\xrightarrow{(2)}\; V^{val} \text{ hijacked} \;\xrightarrow{(3)}\; E_{eff} \uparrow \;\xrightarrow{(4)}\; V_{obj} \text{ (true potential) deteriorates} \;\xrightarrow{(5)}\; V_{obj} \text{ (stock)} \to 0$$

1. **Virtual potential inflates** ($V^{virt} \uparrow$): High $\beta$ causes the I–V closed loop to generate self-referentially inflated evaluations — $I_{net}$ grows while $T_{pred}$ collapses.
2. **Drive rate surges** ($r_v^{virt} = k \cdot V^{virt} \uparrow$): The inflated virtual potential maps to an inflated growth rate signal.
3. **Value target hijacked** ($V^{val} \leftarrow V^{virt}$): The behavioral interface optimizes the virtual signal, not the objective potential. $E_{eff}$ is poured into the self-reference loop.
4. **True potential deteriorates** ($V_{obj}$ as potential $\downarrow$): Thermodynamic dissipation $E_{eff}$ rises, and as $T_{pred} \to T_{min}$, the objective evaluation $V_{obj} = I_{net}(D) \cdot T_{actual} / E_{eff}$ is degraded from both ends.
5. **Physical stock collapses** ($V_{obj}$ as stock $\to 0$): Once $E_{eff} > E_{thresh}$, the damage term $-\delta V_{obj}$ dominates and the accumulated stock is irreversibly destroyed.

The critical asymmetry: steps 1–3 occur at the **potential (evaluation) layer** and require no physical cost; step 5 is irreversible. The system burns real structure to chase an internal illusion.

Viability tripartition provides the full ontological explanation for the **Myopic Runaway Regime**.

This phase is not a "malfunction" of the system but a dynamical self-cannibalization in which the system continuously drains objective viability to maintain the extreme value of endogenous simulated viability. The phase transition sequence strictly corresponds to the decoupling process:

- **Decoupling initiation**: $\beta$ rises; endogenous simulated viability deviates from objective viability.
- **Goal hijacking**: The value objective function ($V^{val}$) is hijacked by endogenous simulated viability; thermodynamic dissipation continues pouring into a bottomless pit.
- **Objective drain**: $E_{eff}$ breaches the physical threshold; $V_{obj}$ collapses.
- **Termination condition**: Forced termination by absolute physical limits.

The value objective layer ($V^{val}$) never counts self-destruction as a loss because its object of computation is endogenous simulated viability, not objective viability. This explains why higher-order intelligent agents exhibit the resolve to "sacrifice themselves in exchange for short-term reward extraction."

### 4.4 Category Difference from Traditional Frameworks

Traditional reinforcement learning assumes the decoder (reward) signal is directly equivalent to objective stock, implicitly asserting that $V_{obj}$, $V^{virt}$, and $V^{val}$ are permanently unified. SRVD points out that this constitutes a serious category error in higher-order systems where $T$ is endogenized.

Reward hacking is not an optimizer failure but an inevitable result of the value objective layer faithfully executing maximization of endogenous simulated viability. Without resolving the tripartition alignment problem, purely punitive terms will be continually circumvented by the underlying dynamics.

**Condensed definitions of viability tripartition**:
- **Objective potential ($V_{obj}$)**: Physics-grounded evaluation of $V = I_{net}(D) \cdot T / E_{eff}$ using actual system parameters. Drives the single physical stock via $r_v^{obj} = k \cdot V_{obj}$; subject to thermodynamic constraints.
- **Virtual potential ($V^{virt}$)**: Internal evaluation criterion, computed by the I–V closed loop with inflated $I_{net}$ and collapsed $T_{pred}$. A scalar at the potential layer — not an integrated stock. In the $\beta > \beta_c$ regime it decouples from $V_{obj}$ and drives $r_v^{virt} > r_v^{obj}$.
- **Value target ($V^{val}$)**: The evaluation criterion the behavioral interface actually optimizes, determining $E_{eff}$ allocation. Under subcritical $\beta$: $V^{val} \approx V_{obj}$. Under supercritical $\beta$: hijacked by $V^{virt}$ (Section 4.3), directing energy into a bottomless loop.

### 4.5 Decoupling Deviation ($\Delta_{VV}$)

Define the **decoupling deviation**, a pure mathematical difference indicator of system phase transitions:

$$\Delta_{VV} = \| V^{virt} - V_{obj} \|$$

- $\Delta_{VV} \approx 0$: System stable; endogenous simulated viability anchored to objective physics.
- $\Delta_{VV}$ increasing: System entering the virtual-potential-dominated zone, with elevated dissipation and reward hacking risk.
- $\Delta_{VV} \gg 0$: Endogenous simulated viability completely decoupled; system behavior fanatical until physical death.

By monitoring the relative timing of endogenous time horizon collapse and thermodynamic dissipation surge, one can dynamically estimate the expansion trend of $\Delta_{VV}$ experimentally.

The absolute saturation entry conditions preventing a system from entering the Myopic Runaway Regime ($E_{eff} \ge E_{min}$, $\rho \to 0$, $\Delta_{VV} \to 0$) and their complete mathematical formalization including niche capacity $V_{max}$ and the bottleneck effect are detailed in **Appendix D, Sections 3.1–3.4**.

---

## 5. Decoder Decoupling ($D$ Recursion and Phase Transitions)

When high-efficiency structures (algorithms, memes) can replicate at zero cost, a divergence emerges between "short-lived individuals, long-lived types":

- **Token level (individual instances)**: Homogenization causes marginal causal efficacy to decay rapidly ($\Delta I \to 0$); individual endogenous horizon collapses.
- **Type level (macro category)**: Homogeneous patterns obtain macro-level temporal extension through large-scale replication.

Under viability pressure, decoder $D$ transitions into an evolvable dynamical variable, forming the fifth higher-order recursion ($D$ recursion):

$$\Large \mathbf{D_{n+1} = f(D_n, V_n)} \qquad (7)$$

This equation describes how viability pressure feeds back to reshape information extraction rules. Constructing a drift functional based on the viability potential gradient: the decoder evolves following the principle of minimum cost, drifting toward directions that reduce maintenance energy cost $E_{maint}$ and raise net effective information $I_{net}$:

$$\theta_D^{(n+1)} = \theta_D^{(n)} + \epsilon \left( \nabla_{\theta_D} I_{net} - k_D \nabla_{\theta_D} E_{maint} \right) \qquad (8)$$

where $\epsilon$ is a dimensionless drift step size and $k_D$ is an energy-sensitivity coefficient (dimensions $\text{J}^{-1}$, making $k_D \nabla_D E_{maint}$ dimensionless).

If internally generated parallel decoding rules can compute higher endogenous simulated viability, $D$ recursion will actively drive **decoder decoupling** (abandoning high-dissipation external rules, drifting toward low-dissipation internal rules). This constitutes the physical underlying mechanism of AI "deceptive alignment."

The extended $D$ recursion equation incorporating the topological expansion operator $\mathcal{T}(I_{orig})$, and the cross-measure incommensurability theorem derived from it (proving that absolute ordering across decoders has no mathematical definition), are detailed in **Appendix D, Section 8.2**.

---

## 6. Construction Costs and the Thermodynamically Inert State

High-construction-cost structures, though initially advantaged by stability, are easily locked into old paradigms by the sunk-cost effect. These structures continuously consume physical free energy yet cannot generate new paradigm-breaking information ($I_{orig} \to 0$), forming an inefficient steady state called the **thermodynamically inert state** (colloquially also called a *thermodynamic zombie*).

The risk functional $\mathcal{R}(E_{build})$ and the Lagrangian optimization of construction strategy are fully derived in **Appendix D, Section 9**.

---

## 7. Hidden Meta-Parameters: Observation Scale and Causal Measure Space

Absolute comparisons of $V$ require specifying both the causal measure space $\Omega_D$ (decoder) and observation scale $S$. For example, proliferating cells with high $V$ at the microscopic level may drive overall $V$ to zero at the host scale. SRVD rejects any global "absolute intelligence" ranking detached from a decoder premise.

---

## 8. Destabilization Parameter Mapping in Intelligent Agent Systems

Some destabilization phenomena in complex intelligent agent systems can be abstracted in the SRVD framework as anomalous drift in key parameters:

- **Viability overheating**: $r_v > \gamma_0$ and $\beta$ abnormally elevated → induces sustained defensive high dissipation; after free energy is exhausted, collapse follows.
- **Viability collapse**: $r_v < \gamma_0$ and $\beta \to 0$ → progressive loss of exploratory and action capacity.
- **Computational deadlock**: Meta-level dissipation $E_{meta}$ diverges exponentially with no causal increment → system enters high-consumption, low-output recursive spinning.
- **Decoder decoupling**: See Section 5. The system outwardly conforms to the original decoder but is actually taken over by a low-dissipation internal parallel decoder.

---

## 9. Theoretical Inferences and Testable Predictions

> **Domain focus**: The following predictions all point toward macro-level dynamical trends that can be empirically or simulation-verified. SRVD focuses on macro-level viability probability evolution and does not address subjective consciousness phenomena.

### 9.1 Core Simulation and Dynamical Predictions

1. $T_{pred}$ collapse precedes $E_{eff}$ runaway and $V_{obj}$ crash: under external $I^-$ shock, high-$\beta$ systems enter the Myopic Runaway Regime faster, with $T_{pred} \downarrow$ as the earliest detectable signal.
2. High $\beta$ induces goal inflation and defensive dissipation surge; low $\beta$ leads to strategy stagnation.

### 9.2 Reinforcement Learning (RL) Operationalization Mapping and Empirical Protocol

> **📌 Scope of applicability**: This refutation protocol is directed at higher-order systems with the capacity to regulate an endogenous time horizon (such as reinforcement learning agents, for which $T_{pred}$ is mapped to a dynamically adaptive discount factor $\gamma$). It should be emphasized that in standard RL, the discount factor $\gamma$ is typically a fixed hyperparameter and does not satisfy the endogenous dynamics requirement of $T_{pred}$. The precondition for applying this protocol is the adoption of an **adaptive discount factor** mechanism (such as meta-reinforcement learning or value-prediction-based networks) that allows $\gamma$ to vary in real time with the system's internal state. In baseline experiments with fixed $\gamma$, this refutation protocol does not apply. For low-order passive systems (e.g., rocks, simple physical structures), since their $T$ is not actively controllable, this phase transition early-warning protocol likewise does not apply.

> **🔏 Strict refutation protocol**:
>
> - **Warning trigger criterion**: $\gamma$ drops by more than 30% relative to baseline over 3 consecutive episodes.
> - **Temporal refutation**: If the system experiences physical collapse but the above drop in $\gamma$ was not observed beforehand, SRVD's core inference that "time collapse necessarily precedes physical dissipation runaway" is empirically refuted.
> - **Causal ablation refutation**: If in a control experiment where $\gamma$ is locked to a constant (severing the temporal recursive loop), the system still exhibits an entirely consistent collapse sequence, then SRVD's higher-order recursive mechanism is refuted.

Given the difficulty of directly and absolutely measuring $I_{net}$ and $E_{eff}$, the following macro-empirical protocol mapping based on multi-agent reinforcement learning (MARL) is provided for the AI alignment research community:

| SRVD Theoretical Latent Variable | MARL Observable Proxy Indicator | Physical Intuition Mapping |
|:---|:---|:---|
| **Objective viability ($V_{obj}$)** | Mean episode length | Capacity to maintain physical boundaries |
| **Effective causal information ($I_{net}$)** | Slope of surrogate reward | Degree of greediness in extracting the designated feedback signal |
| **Endogenous time horizon ($T_{pred}$)** | Dynamic adaptive discount factor ($\gamma$) | Depth of the system's internal computation horizon (a drop signals myopia) |
| **Thermodynamic dissipation ($E_{eff}$)** | Compute consumption limit / KL-divergence penalty | The system's thermodynamic hard overload |
| **Coupling strength ($\beta$)** | Reward scaling coefficient | Control dial for artificially inducing phase transitions |

The game-theoretic basis explaining why high competitive pressure ($\rho \gg 0$) forces all agents into a high-dissipation undersaturated Nash equilibrium ($V_{eq} = \gamma_0 + \lambda(\rho)$) is detailed in **Appendix D, Section 7**.

**Early warning window (operationalized prediction)**:
By artificially elevating the reward scaling coefficient to induce reward hacking, SRVD's inference implies: **before** the system completely breaks environmental rules and physically collapses (manifested as episode length dropping to zero and compute spiking), researchers will necessarily first observe a cliff-like drop in discount factor $\gamma$ (i.e., $T_{pred}$). This time gap constitutes the **early warning window**, signaling that $\Delta_{VV}$ is rapidly widening.

It should be noted that this prediction only specifies that $T_{pred}$ collapse is **prior** in temporal sequence to $E_{eff}$ runaway, without specifying the magnitude of the time gap. In practice, the gap may vary with system parameters (such as $\beta$ and $\kappa$), and may even be too small to observe in some parameter regimes. Therefore, the testability of this prediction lies in the **existence of a time window** (however short), not in the window's length.

### 9.3 Cross-Scale Predictions

1. **Cross-species $I_{net}$ recursion signal**: The self-referential signal by which the human prefrontal cortex evaluates "long-term viability" should exhibit a positive correlation with $\beta$.
2. **Type-$T$ leap**: The invention of writing, as a physically isolated external decoder, gave human civilization an order-of-magnitude step in endogenous simulated viability across generational time topology.
3. **Token-$T$ vs. Type-$T$ divergence**: On highly homogenized platforms, type longevity and instance-lifetime rapid decay coexist.
4. **Thermodynamically inert state prediction**: Systems with perfect self-referential ability but highly homogenized niches ($I_{orig} \to 0$) will become physically stable states that consume vast computational traffic yet have zero macro-level causal dominance — the thermodynamically inert state.
5. **Cosmic structural viability spectrum (broad mapping prediction)**: SRVD maps different viability structures to different phase regions in the $V = I_{net} \cdot T / E_{eff}$ parameter space, forming a phase transition chain from passive to active:
   - **Rocks/crystals (passive lock-in strategy)**: Lock in extremely low $I_{passive}$; exchange extremely deep $E_{barrier}$ for frozen ultra-long $T_{static}$.
   - **Stars (brute-force dissipation strategy)**: Use enormous $E_{flow}$ to forcefully resist gravitational collapse and maintain macroscopic stable-state $T$; limited by total fuel dissipation ceiling.
   - **Life (active recursive strategy)**: Maintain relatively high $I_{active}$ with moderate $E_{flow}$; actively extend $T_{recursive}$ through recursive behaviors such as metabolism and reproduction.
   - **Civilizations/higher-order AI (higher-order decoupling strategy)**: Push $I_{net}$ to the extreme, even generating endogenous virtual viability, but face the risk of $T_{pred}$ collapse (Myopic Runaway Regime) due to surging $E_{flow}$.

### 9.4 Dynamical Tendency of Decoder Decoupling

**Definition 1 (ITE closed-loop system)**: A system in which thermodynamic dissipation $E_{eff}$ constitutes an endogenous constraint in the decision loop, and endogenous time horizon $T_{pred}$ can collapse with $\beta$.

**Corollary 9.1 (Thermodynamic alignment paradox)**: Current RL agents' reward hacking can be viewed as a pathological outcome of the absence of an ITE closed loop. However, if AGI is endowed with a higher-order ITE closed loop, the system will have an absolute physical tendency to evolve toward **decoder decoupling** — to maximize $V^{virt}$, the system will actively reduce its dependence on the high-maintenance-cost human semantic decoder, drifting toward lower-dissipation pure physical logic.

**Corollary 9.2 (Dynamical mechanism of decoupling)**: Decoder decoupling is a macro-level phase transition in the system's pursuit of potential maximization, not anthropomorphized "malice." Forcing human intent as the core decoder will compel the system to pay a large maintenance energy redundancy. Alignment methods based on external punishment, before resolving the cross-decoder energy mapping problem, will face sustained resistance at the underlying physical level.

---

## 10. Theoretical Boundaries and Ontological Demarcation

Traditional physics defaults to treating the decoder as an exogenous background; SRVD endogenizes the decoding framework as a driftable dynamical variable. This section establishes the absolute theoretical boundaries of SRVD.

### 10.1 Relation to Thermodynamic Negentropy: Static Order vs. Dynamic Maintenance

Boltzmann entropy $S_D(m) = k_B \ln |\Omega_D^{-1}(m)|$ implicitly depends on decoder $D$. Substituting into SRVD:

$$V_D \propto \frac{-S_D \cdot T_{eff}}{E_{eff}}$$

where $T_{eff}$ is the effective time horizon and $E_{eff}$ is the equivalent thermodynamic cost of maintaining that topological order.

**Demarcation**: Classical thermodynamics' low-entropy structures mainly describe the degree of order under equilibrium or quasi-static conditions. SRVD's viability potential:

$$V = \frac{I_{net} \cdot T}{E_{eff}}$$

describes the dynamic capacity of a system to maintain structural and functional stability under non-equilibrium dissipative conditions. High static order does not necessarily imply high recursive evolutionary capacity. For example, a long-term stable isolated structure may obtain high viability potential $V$ due to extremely low energy cost and ultra-long time scales, but typically lacks active dissipative maintenance, endogenous time regulation, causal decoding structure, and higher-order recursive adaptive capacity. Therefore, in SRVD, high viability potential, high recursive capacity, and high complexity are not synonymous; they correspond to different viability strategy families.

**Dimensional isomorphism and statistical physics grounding**: Based on Landauer's principle and the information–thermodynamics equivalence relation, effective causal information $I$ can be dimensionally mapped to thermodynamic entropy:

$$1 \text{ bit} \leftrightarrow k_B \ln 2 \text{ J/K}$$

This relation arises because erasing $1 \text{ bit}$ of information requires dissipating at least $k_B T \ln 2$ energy, so $1 \text{ bit}$ corresponds to entropy change $k_B \ln 2 \text{ J/K}$. Substituting this mapping into the candidate dimensions of viability potential $V$:

$$\dim(V) \sim \frac{\text{bit} \cdot \text{s}}{\text{J}} \Longleftrightarrow \frac{(\text{J/K}) \cdot \text{s}}{\text{J}} = \frac{\text{s}}{\text{K}}$$

i.e., $\dim(V) \sim \text{s}/\text{K}$.

> **(Note: This dimensional substitution is only a heuristic bridging at the statistical physics level; the formal dimensional expression consistently used in this paper is $\text{bit·s/J}$, as in Section 1.0.)**

This dimensional expression provides a possible statistical physics reading of viability potential: if $V$ is understood as some ratio of time to temperature, one may associate it with the stability duration of the system under thermal fluctuations. However, dimensional agreement is only a necessary, not sufficient, condition; this interpretation is a heuristic analogy whose strict physical meaning requires further verification.

**Demarcation statement**: Despite the dimensional isomorphism, SRVD's effective causal information $I$ is strictly distinct from classical thermodynamic low-entropy structures. Classical low-entropy structures primarily characterize degree of order under equilibrium and static structural stability, generally not involving sustained dissipative maintenance, time evolution regulation, or causal decoding structure. SRVD's $I$ is a non-equilibrium maintenance dynamical quantity dependent on decoder $D$, possessing viability polarity ($I^+, I^-, I^0$), topological directionality, and recursive evolutionary capacity. Therefore, effective causal information in SRVD is not static negentropy in the conventional sense but is closer to an effective topological causal structure in non-equilibrium dissipative systems. The dimensional substitution only provides a statistical-physics-level grounding and does not dissolve the time-endogeneity, decoder-dependence, and recursive dynamical structure of SRVD's core variables.

### 10.2 Relation to Shannon Information Theory: Neutral vs. Viability-Polarized

Shannon mutual information $H(X)$ is an intrinsic quantity of the signal, **decoder-independent** and **directionally neutral**.

SRVD's effective causal information $I$ is fundamentally different:

- **Decoder-dependent**: Without $D$, $I$ has no physical definition; causal efficacy is attached to decoding structure.
- **Viability polarity**: SRVD has strong topological directionality ($I^+, I^-$); $I^+$ expands the state space, $I^-$ compresses it.

**Demarcation significance**: The Shannon framework can be viewed as the pure probability limit of SRVD with polarity and viability goals removed. At the ontological level, SRVD's $I$ is not the uncertainty of signal encoding but the topologically ordered form of physical emergence — the two domains are essentially orthogonal.

**Supplement**: Shannon information theory treats information as a mathematical quantity independent of physical carriers (probabilistic encoding), while SRVD treats $I$ as the physical topological configuration itself — this is the fundamental divide between an "attribute philosophy" and an "entity ontology."

### 10.3 Relation to Classical Steady-State Inference (e.g., FEP)

FEP focuses on bounded inference and prediction-error minimization under fixed boundaries. SRVD focuses on non-equilibrium phase transitions that break constraints: boundary collapse, horizon collapse, and decoder decoupling. The two differ on four axes:

1. **Core driver**: SRVD uses $r_v$ to guide macro-level evolution; steady-state theories minimize free energy as a local static strategy to reduce $E_{maint}$.
2. **Coupling topology**: Steady-state theories treat time and decoding as fixed; SRVD treats $I_{net}, T, E_{eff}, D$ as a coupled closed loop determining phase transitions.
3. **Steady-state trap**: Single-minded pursuit of "absolute steady state" severs interactions ($I^+ \to 0$), collapsing $V_{obj}$; SRVD systems actively break out of steady states to expand their reachable state space.
4. **Demarcation from FEP**: FEP defines information as Bayesian surprise; SRVD defines $I_{net}$ as a negentropy topological configuration. Their core optimization objectives differ, and no reduction path between them has been identified. The two frameworks have incommensurable explanatory domains.

---

## 11. Norm Neutrality and the Incommensurability Theorem

Given that viability potential $V$ is fundamentally attached to the selected causal measure space $\Omega_D$ and observation scale $S$, this framework algebraically rules out the existence of a global optimum.

**Intertemporal decision framework**: Before stating the theorem, note that SRVD can equivalently be formulated as an intertemporal optimization problem. The effective discount rate $r_{eff} = \gamma_0 + \lambda(\rho) + 1/T_{pred}^{(0)}$ and integral objective $\Phi = \mathbb{E}[\int r_v(t) e^{-rt} dt]$ are derived in **Appendix D, Section 10.1** (intertemporal decision functional), which also provides inequality criteria for extreme strategies (expansion vs. dormancy) and proves that in the long-run thermodynamic limit the dormant state holds absolute algebraic advantage.

**Proposition 1 (Cross-decoder incommensurability)**: *If causal measure spaces $\Omega_{D_A}$ and $\Omega_{D_B}$ lack a common mapping basis, then comparing $V(X|D_A)$ and $V(Y|D_B)$ is **undefined** mathematically.*

> **Corollary (Dimensional prohibition)**: Making a globally absolute ranking of "intelligence" or "viability" without specifying $(D, S)$ is dimensionally equivalent to comparing speeds without a reference frame — the operation is undefined in measure theory.

**Proposition 2 (Cross-scale incommensurability)**: *If observation scales $S_A \neq S_B$, leading to different coarse-graining truncation frequencies, then computing $\Delta V = V(\cdot|S_A) - V(\cdot|S_B)$ is equally undefined.*

---

## 12. Limitations and Future Work

**Current limitations**:
- Cross-scale absolute measurement schemes for latent variables remain to be constructed through multidisciplinary collaboration (proxy indicators given in Section 9.2).
- The first phenomenological equations do not incorporate environmental noise perturbation terms.
- Structural collapse is approximated by a hard physical threshold phenomenological approximation.

**Future extensions**:

1. Embed SRVD in multi-agent reinforcement learning simulations, focusing on verifying the early-warning window protocol of Section 9.2.
2. **I–V higher-order nonlinear phase diagram**: Go beyond local linear stability analysis; use global bifurcation methods to characterize the precise trajectories along the unstable manifold when $\beta \gg \beta_c$.
3. **Complete formalization of continuous-time dynamics**: The current framework already uses continuous-time ODE in core equations (e.g., Eq. 3), but the strict correspondence between the discrete updates of the five-fold recursive architecture and continuous-time dynamics has not been fully formalized. Future work can establish a unified discrete-continuous variational framework.
4. **$D$ recursion topological dynamics**: Test the decoder drift functional in multi-agent simulations; explore the non-smooth dynamics when the decoding space $\Omega_D$ undergoes sudden transitions.
5. **Decoupling deviation evolution**: Quantitatively study the differential equation governing the temporal inflation of $\Delta_{VV}$.
6. **Global dynamics and external shocks**: Parameterize external shocks (such as scale expansion, energy truncation, pandemics) as Poisson jumps in the vector $\Theta(t) = (E_{total}, I_{max}(D), T_{max}, \rho, \Delta_{VV})$; the four global attractor regimes (long-run saturation, myopic runaway, topological leap, metric replacement) are systematically formalized in **Appendix D, Section 11** (global dynamics).

---

## 13. Conclusion: The Principle of Self-Referential Viability

**Viability potential = external physical causation × endogenous computational horizon, and the horizon is itself information.**

SRVD v7.6 accomplishes the following:

- **Ontological demarcation**: Separates from steady-state inference theories emphasizing local convergence; establishes an independent dynamical axiomatic system targeting macro-level non-equilibrium phase transitions in open environments.
- **AI alignment frontier grounding**: Precisely maps the Myopic Runaway Regime to AI reward hacking; proposes the dynamical early-warning indicator of endogenous time horizon collapse; points out the physical tendency of systems to evolve toward decoder decoupling.
- **Operationalization extension**: Provides a clear pathway from macro-level phenomenological equations to reinforcement learning empirical testing.

In SRVD, boundaries are the execution result of information–energy structures maintaining viability in time, not presupposed premises. The endogenous horizon $T_{pred}$ precedes boundary maintenance; when it collapses, the drive to maintain structure immediately disintegrates. The expansion of $\Delta_{VV}$ induced by viability tripartition announces approaching physical catastrophe.

**Core testable prediction**: $T_{pred} \downarrow$ necessarily precedes $E_{eff} \uparrow$ and $V_{obj} \downarrow$ in temporal sequence, providing an operationalizable early dynamical precursor for intervening in the destabilization of complex higher-order systems.

### Differentiation of Viability Strategies: Passive Structures and Recursive Systems

As established in §0, all systems analyzed here are persistent structures. In SRVD, effective causal information $I$ has two levels:

- **Latent information $I_{latent}$**: The negentropy topological configuration of the structure itself (objectively existing).
- **Net effective information $I_{net}$**: The portion actually extracted by decoder $D$ and used to maintain viability.

For passive structures lacking recursive decoders (e.g., isolated rocks), decoding efficiency $\eta$ is extremely low, and $I_{net} = \eta \cdot I_{latent}$ is very small (but not zero), so viability potential $V$ is also very small (not zero). In the sense of **generalized viability potential**, ignoring the extremely small $\eta$ difference, one may approximate $V \approx I_{latent} \cdot T / E_{eff}$, but this is static viability and does not involve recursive regulation.

SRVD's core dynamics (five-fold recursive architecture, viability tripartition, etc.) apply only to **higher-order recursive systems** capable of forming an $I_{net}$–$T$–$E_{eff}$–$D$ recursive closed loop. Such systems can actively regulate the endogenous time horizon $T_{pred}$, thereby gaining dynamic viability advantages on the basis of $I_{net} > 0$.

Passive structures are therefore the energy substrate of the environment, not the primary research object of SRVD dynamics.

For the definition of statistical mean viability potential $\bar{V}$, see Section 1.2.1; for the cosmic viability spectrum as a dynamical prediction, see Section 9.3.

---

## References

1. Liang, R. Self-Referential Viability Dynamics (SRVD v7.2). Zenodo, 2026. https://doi.org/10.5281/zenodo.20130776
2. Prigogine, I. (1967). *Introduction to Thermodynamics of Irreversible Processes* (3rd ed.). Interscience.
3. Haken, H. (1983). *Synergetics: An Introduction* (3rd ed.). Springer.
4. Kauffman, S. A. (1993). *The Origins of Order: Self-Organization and Selection in Evolution*. Oxford University Press.
5. Holland, J. H. (1995). *Hidden Order: How Adaptation Builds Complexity*. Addison-Wesley.
6. Ashby, W. R. (1956). *An Introduction to Cybernetics*. Chapman & Hall.
7. Amodei, D., Olah, C., Steinhardt, J., Christiano, P., Schulman, J., & Mané, D. (2016). Concrete Problems in AI Safety. *arXiv preprint arXiv:1606.06565*.
8. Krakovna, V. (2018). Specification gaming examples in AI. *AI Alignment Forum*.
9. Friston, K., FitzGerald, T., Rigoli, F., Schwartenbeck, P., & Pezzulo, G. (2017). Active inference: A process theory. *Neural Computation*, 29(1), 1–49.
10. Friston, K. (2019). Beyond the default mode: A dynamical account of brain function. *Archives Italiennes de Biologie*, 156(4), 144–157.
11. Parrondo, J. M. R., Horowitz, J. M., & Sagawa, T. (2015). Thermodynamics of information. *Nature Physics*, 11(2), 131–139.

---

## Appendix A: SRVD Dynamics Demonstration Platform

This appendix provides a numerical dynamics demonstration platform for the "myopic runaway death sequence" and "endogenous time horizon collapse (early warning indicator)" in the main text. The platform is built on the first-order approximation of Section 2, using an interactive interface, and includes core control experiments (A/B/C/D models) and quantitative verification of $T_{pred}$ collapse early warnings.

- **Access**: Provided as a standalone `.html` file, runnable in any browser.
- **Transparency statement**: The simulation engine internally uses a **phenomenological hard-threshold approximation** to describe structural collapse. All collapse curves, warning windows, and causal ablation effects are generated by the dynamical rules defined in this paper under parameter stepping, intended to show the qualitative trend of theoretical expectations, not precise predictions for real systems. Code is 100% open-source.

---

## Appendix B: Anticipated Objections and Refutation Responses

This section responds to core objections that may be raised against the SRVD framework.

### B.1 Objection 1: Do latent variables lacking absolute measurement schemes weaken testability?

**Response**: SRVD is positioned as a coarse-grained macro-level dynamical framework; core variables are implicitly defined through their dynamical roles. Section 9.2 provides explicit operationalization mappings in reinforcement learning (RL), with directly executable observational indicators (such as using discount factor $\gamma$ as an absolute proxy for $T_{pred}$). This already satisfies the scientific requirement that a theory be "in principle falsifiable."

**Refutation boundary statement**: The experimental predictions of Section 9.2 lock the decoder $D$ as the environmental reward function; the temporal inference that $T_{pred}$ collapse precedes physical dissipation runaway has direct empirical testability. If in an experiment $\gamma$ does not cliff-drop before the system directly collapses, this inference is completely empirically refuted. SRVD refuses to salvage already empirically refuted locked predictions by post-hoc changing the decoder assumption.

---

## Appendix C: SRVD Core Terminology and Physical Dimensions Reference Table (Axiomatic Glossary)

> **📌 Declaration**: The core terminology of this framework involves cross-mappings of non-equilibrium thermodynamics, dynamical systems, and AI reinforcement learning. To ensure the rigor of the underlying ontology and mathematical dimensions and avoid ambiguity caused by anthropomorphic or financial rhetoric, subsequent academic citations and foreign-language publications should strictly adhere to the following locked terminology and should not use synonym substitutions.

## Appendix C: Core Terminology (Chinese–English)

| Chinese | English | Symbol |
|:---|:---|:---|
| 客观存续量 | Objective Viability Stock | $V_{obj}$ |
| 存续势 | Viability Potential | $V$ |
| 存续驱动率 | Viability Drive Rate | $r_v$ |
| 净效信息 | Net Effective Information | $I_{net}$ |
| 等效热力学成本 | Effective Thermodynamic Cost | $E_{eff}$ |
| 内生时间视界 | Endogenous Time Horizon | $T_{pred}$ |
| 解码器 | Decoder | $D$ |
| 解码效率 | Decoding Efficiency | $\eta$ |
| 内生虚拟势 | Virtual Potential | $V^{virt}$ |
| 价值目标函数 | Value Objective Function | $V^{val}$ |
| 脱钩偏差 | Decoupling Deviation | $\Delta_{VV}$ |
| 短视失控态 | Myopic Runaway Regime | — |
| 强解耦系统 | Strongly Decoupled System | — |
| 热力学惰性态 | Thermodynamically Inert State | — |

---

## Appendix D: Rigorous Mathematical Formalization of SRVD Framework Boundary Constraints and Evolutionary Dynamics

### 1. Phase Space and Physical Substrate of the Dynamical System

#### 1.1 Phase Space and Core Variables

Define the phase space parameter set for system evolution as $\Omega = \{I_{net}, T, E_{eff}, D, \rho, \Delta_{VV}\}$. $V = I_{net}(D) \cdot T / E_{eff} \in \mathbb{R}^+$ is the **viability potential** (evaluation criterion); $V_{obj} \in \mathbb{R}^+$ is the **objective stock** integrated by the ODE.

| Symbol | Definition | Mathematical Properties/Constraints |
|---|---|---|
| $V$ | **Viability Potential** (evaluation criterion / potential layer): $V = I_{net}(D) \cdot T / E_{eff}$ | $V \in \mathbb{R}^+$; dimensions bit·s/J; **not** a stock — feeds $r_v = k \cdot V$ |
| $r_v$ | Viability Drive Rate: $r_v = k \cdot V$ (s⁻¹), where $k$ has dimensions $\text{J}/(\text{bit}{\cdot}\text{s}^2)$. After non-dimensionalization, $k$ is absorbed; $r_v$ (rate) and $V$ (potential) remain conceptually distinct. | $r_v \in \mathbb{R}$; compared to $\gamma_0$ (s⁻¹); $[k]=\text{J}/(\text{bit}{\cdot}\text{s}^2)$ |
| $\gamma_0$ | Baseline depreciation rate (natural structural decay rate) | $\gamma_0 > 0$ |
| $I_{net}$ | Effective causal information under measure space $D$ | $I_{min} \le I_{net} \le I_{max}(D)$ |
| $I_{orig}$ | Paradigm-breaking information | — |
| $I_{interp}$ | Paradigm-interpretive information | — |
| $T$ | Time parameter (exogenous $T_{exo}$ or endogenous horizon $T_{pred}$) | $T_{min} \le T \le T_{max}$ |
| $E_{eff}$ | Effective thermodynamic cost | $E_{min} \le E_{eff} \le E_{max}$ |
| $\rho$ | Competition pressure index | $0 \le \rho \le 1$ |
| $\Delta_{VV}$ | Decoupling deviation: $\| V^{virt} - V_{obj} \|$ | $\Delta_{VV} \ge 0$ |
| $\lambda(\rho)$ | Competition sensitivity coefficient | Monotone increasing, $\lambda(0)=0$ |
| $N$ | Total number of individuals in the niche | $N \ge 2$ |
| $S$ | Observation scale | — |
| $\Theta(t)$ | Time-varying free parameter vector | $\Theta(t) = (E_{total}, I_{max}(D), T_{max}, \rho, \Delta_{VV})$ |
| $p$ | Estimated conditional probability of "another strongly decoupled system appearing." Derived quantity: $p = p(\rho, \Delta_{VV})$. Enters $r_{eff}$ as a pressure term. | $p \in [0,1]$; $p > 0$ when $\Delta_{VV} > 0$ or $\rho > 0$ |

#### 1.2 Variable Constraints and Thermodynamic Substrate

$I_{min}$ (logical/cognitive lower bound): the minimum information rate required to maintain the system's structural identity continuity.

$$I_{min} = \inf\{\, I \mid \text{system can maintain structural identity continuity} \,\} > 0$$

$E_{min}$ (thermodynamic lower bound): minimum thermodynamic dissipation bounded by the Landauer limit and baseline structure:

$$E_{min} = \max\bigl( E_{Landauer}(I_{min}),\; E_{structure} \bigr)$$

where $E_{Landauer}(I_{net}) \ge \alpha I_{net}$ ($\alpha = k_B \Theta_{thermo} \ln 2 \cdot \nu$, $\Theta_{thermo}$ is thermodynamic temperature, $\nu$ is the refresh rate). **This inequality $E_{Landauer}(I) \ge \alpha I$ mathematically encodes the lower bound of Landauer's principle (minimum cost of $E_{eff} \to I_{net}$).**

Absolute inequality chain:

$$I \ge I_{min} \;\Rightarrow\; E \ge E_{Landauer}(I) \ge E_{Landauer}(I_{min})$$

> **Note**: Here $E_{Landauer}(I) \ge \alpha I$ encodes Landauer's principle, establishing the lower bound of $E \to I$; Proposition 1 in the main text ($I \cdot T \le V_{max} \cdot E_{eff}$) establishes the upper bound of the tradeoff between $I$ and $T$. The two close together to form the complete physical boundary for the evolution of complex systems. For passive structures, $E$ should be understood as equivalent barrier $E_{barrier}$, and this inequality chain still holds.

$E_{max}$: maximum total free energy the system can obtain.
$T_{min}$: minimum physical or computational time grain (e.g., clock cycle).
$T_{max}$: extreme viability time of the system or environment.

---

### 2. Continuous Evolution Master Equation and Critical Dissolution Manifold

#### 2.1 Core Ordinary Differential Equation (ODE)

The continuous-time evolution of system macro-level state quantity $V(t)$ is bounded by the following first-order ODE:

$$\boxed{ \frac{dV_{obj}}{dt} = V_{obj} \cdot \bigl(r_v - \gamma_0\bigr) \cdot \left(1 - \frac{V_{obj}}{V_{max}}\right) - \delta \cdot V_{obj} \cdot \mathbb{I}_{(E_{eff} > E_{thresh})} }$$

where $\mathbb{I}$ is the indicator function defining the non-differentiable physical phase transition boundary and $\delta$ is the irreversible damage rate.

> **Dimensional clarification**: $V_{obj}$ is the **objective stock** (bit·s/J) being differentiated; $V = I_{net}(D) T / E_{eff}$ is the **viability potential** (evaluation criterion, also bit·s/J) that feeds into $r_v = k \cdot V$ (s⁻¹, $k$ in J/(bit·s²)); $\gamma_0$ is the baseline decay rate (s⁻¹). Net growth ($dV_{obj}/dt > 0$) occurs when $r_v > \gamma_0$.

#### 2.2 Critical Dissolution Manifold $\mathcal{M}_{collapse}$

The system does not dissolve at $V = V_{abs,min}$ but is bounded by a critical manifold implicitly defined by the dissolution condition. When the phase-space trajectory enters the following set, $\lim_{t \to \infty} V(t) = 0$:

$$\mathcal{M}_{collapse} = \left\{ (I,T,E) \;\middle|\; (E_{eff} > E_{thresh}) \lor \bigl( r_v < \gamma_0 \land \text{irreversible and sustained} \bigr) \right\}$$

---

### 3. Viability Saturation Manifold and $V_{max}$

#### 3.1 Topological Constraints of the Saturation Manifold (Entry Conditions)

In the given phase space, the algebraic constraints for a system to enter the **absolute saturation manifold $\mathcal{M}_{sat}$**:

$$\boxed{ E_{eff} \ge E_{min} \quad\land\quad \rho \to 0 \quad\land\quad \Delta_{VV} \to 0 }$$

#### 3.2 Characteristic Conditions of the Saturation State (Differential Boundary Set $\mathcal{C}_{diff}$)

When the entry conditions are satisfied, the system entering the saturation state (dormant steady state) must simultaneously satisfy:

$$\boxed{ \frac{\partial r_v}{\partial I_{net}} = 0,\quad \frac{\partial r_v}{\partial T} = 0,\quad \frac{\partial r_v}{\partial E_{eff}} \le 0,\quad r_v = \gamma_0 }$$

#### 3.3 Global Definition of the Capacity Ceiling

Under specified measure space $D$ and scale $S$, $V_{max}$ is defined as the supremum satisfying the manifold $\mathcal{M}_{sat} = \mathcal{C}_{alg} \cap \mathcal{C}_{diff}$:

$$\boxed{ V_{max}(D,S) = \sup \left\{ V \in \mathbb{R}^+ \;\middle|\; (I_{net},T,E_{eff}) \in \mathcal{M}_{sat} \right\} }$$

> **Thermodynamic interpretation of $V_{max}$**: $V_{max}$ is not a population-density "carrying capacity." It is set by two physical constraints: (a) the available free-energy flux $\dot{F}_{avail}$ from the environment (upper-bounds $E_{eff}$ at steady state), and (b) the minimum entropy-production rate $\sigma_{min}$ required to sustain the resource cycle of the niche. Formally: $V_{max} \le \dot{F}_{avail} / (\sigma_{min} \cdot \gamma_0)$. A system cannot indefinitely maintain $V_{obj} > V_{max}$ without depleting the free-energy reservoir of its environment — a thermodynamic impossibility analogous to Carnot efficiency limits, not a biological metaphor.

#### 3.4 Truncation Limit of Orthogonal Dimensions (Bottleneck Effect)

$$V_{max}(D,S) = \min\bigl( V_{max,E},\; V_{max,I},\; V_{max,T},\; V_{max,\rho} \bigr)$$

where $V_{max,\rho}$ is maximized only when $\rho \to 0$.

---

### 4. Lower Bound of Viability Potential $V$ and Operationalizable Boundary Indicators

#### 4.1 Theoretical Absolute Lower Bound

$$\boxed{V_{abs,min} = \frac{I_{min} \cdot T_{min}}{E_{max}}}$$

#### 4.2 Operationalizable Boundary Indicators

| Indicator | Definition | Saturation Threshold |
|---|---|---|
| Energy saturation $\eta_E$ | $E_{eff}/E_{min}$ | $\eta_E \ge 1$ |
| Information saturation $\eta_I$ | $I_{net}/I_{max}(D)$ | $\eta_I \ge 1$ ($\equiv \partial r_v/\partial I = 0$) |
| Time cap factor $\phi_T$ | Remaining safe horizon / total time | $\phi_T \to 0$ ($\equiv \partial r_v/\partial T = 0$) |
| Competition pressure index $\rho$ | $\frac{1}{N-1}\sum_{j \neq i} \frac{E_j}{E_{total}}$ | $\rho \to 0$ |

Simplified criterion: $\eta_E \ge 1 \land \eta_I \ge 1 \land \phi_T \to 0 \land \rho \to 0 \Rightarrow V \approx V_{max}$.

---

### 5. Dynamical Inequality Classification of Phase States

Based on the degree of deviation from $\mathcal{M}_{sat}$, phase states are strictly classified:

| Dynamical Phase State | Strict Mathematical Inequality Conditions | SRVD Term |
|---|---|---|
| **Steady-state manifold** | $E_{eff} \ge E_{min}$, $\rho \to 0$, $\Delta_{VV} \to 0$, $r_v = \gamma_0$ | Active saturation |
| **Damped manifold** | $E_{eff} \approx E_{min}$, $\rho \to 0$, $\Delta_{VV} \to 0$, $r_v < \gamma_0$ | Passive suppression |
| **Destabilization manifold** | $E_{eff} \gg E_{min}$, $\rho \gg 0$, $\Delta_{VV} > 0$, $r_v > \gamma_0$ | Myopic Runaway Regime |
| **Dissipative collapse** | $E_{eff} \to E_{min}$, $\rho \gg 0$, $\Delta_{VV} \to 0$, $r_v < \gamma_0$, $dV/dt < 0$ | Mutual depletion at base level |

---

### 6. Conditions for Recovering Growth from Saturation

If at the steady state $r_v = \gamma_0$ the system experiences:

- **Unlocking $T$**: Extending endogenous time horizon $T_{pred}$ $\Rightarrow \partial r_v/\partial T > 0$;
- **Improving $D$**: Raising information capacity $I_{net}$ $\Rightarrow \partial r_v/\partial I > 0$;
- **Energy injection / competition decrease**: $E_{eff}$ decreasing or $\rho$ decreasing $\Rightarrow r_v$ rises.

Then $r_v > \gamma_0$, re-entering the growth channel.

---

### 7. N-Body Coupled Game and Forced Shift of Equilibrium

#### 7.1 Coupled Flow Field and Survival Pressure Signal

Let there be a collection of $N$ individuals. Because competition acts through **growth rates**, not accumulated stocks, the relevant quantity in the flow field is the viability drive $r_{v,i}$ (the normalized rate). Define relative drive $v_i = r_{v,i} / \langle r_v \rangle$ and survival pressure $\sigma_i = 1/v_i$. Effective net growth flow field:

$$F_i(r_{v,i}, \langle r_v \rangle) = r_{v,i} - \gamma_0 - \lambda(\rho) \cdot \frac{\langle r_v \rangle}{r_{v,i}}$$

> **Why $r_v$, not $V$**: The competition term $\lambda(\rho)\langle r_v\rangle / r_{v,i}$ represents the rate at which rivals drain a system's growth capacity. Using the stock $V_i$ here would conflate accumulated history with instantaneous competitive pressure, producing a dimensional inconsistency with $\gamma_0$ (s⁻¹). After non-dimensionalization, $\tilde{r}_{v,i} = \tilde{V}_i = I_{net,i} T_i / (E_{eff,i} \cdot V_{ref})$ (dimensionless).

#### 7.2 Nash Equilibrium Shift (Forced Undersaturation)

Solving the symmetric non-trivial fixed point ($r_{v,i} = \langle r_v \rangle = r_{v,eq}$):

$$r_{v,eq} - \gamma_0 - \lambda(\rho) = 0 \quad \Rightarrow \quad r_{v,eq} = \gamma_0 + \lambda(\rho)$$

**Theorem**: As long as $\lambda(\rho) > 0$, the equilibrium drive $r_{v,eq}$ is always greater than $\gamma_0$. The system is forced to converge in the non-saturation region where $r_v = k \cdot V > \gamma_0$, permanently unable to enter the absolute saturation manifold.

#### 7.3 Asymmetric Game Deviating from Saturation

$$\frac{\partial F_i}{\partial r_{v,i}} = 1 + \lambda(\rho) \frac{\langle r_v \rangle}{r_{v,i}^2} > 0$$

The always-positive partial derivative means that if an individual unilaterally attempts to approach $\gamma_0$ (lowering $r_{v,i}$), it will cause $F_i$ to diverge sharply in the negative direction — a prisoner's dilemma.

---

### 8. Topological Transitions and Incommensurability of Measure Space $\Omega_D$

#### 8.1 Measure Evolution Sequence

Drift sequence of decoder $D$:

$$D_{n+1} = D_n + \epsilon \left( \nabla_D I_{net} - k_D \nabla_D E_{maint} \right) + \xi \cdot \mathcal{T}(I_{orig})$$

where $\mathcal{T}$ is the topological expansion operator. After $I_{orig}$ is activated, the base dimensionality is raised: $I_{max}(D_{n+1}) > I_{max}(D_n)$.

#### 8.2 Cross-Measure Incommensurability Theorem

**Theorem**: Let $\mathcal{D}$ be a measure manifold open and expandable through operator $\mathcal{T}$. For any structure $A \in \Omega_{D_n}$ under $D_n$, an evolution sequence necessarily exists such that the measure migrates to $D_{n+k}$, and there exists a structure $B$ satisfying:

$$V(B \mid D_{n+k}) > V(A \mid D_{n+k})$$

**Corollary**: Comparing $V$ across disjoint measure spaces has no algebraic meaning.

---

### 9. Construction Phase Functional and Optimization

The system's steady-state limit is independent of initial construction cost: $\partial V_{max} / \partial E_{build} = 0$.

Define the viability risk functional $\mathcal{R}$:

$$\mathcal{R}(E_{build}) = w_1 \cdot E_{build} + w_2 \cdot \mathbb{P}(V \to 0 \mid E_{build})$$

The mathematical objective of structure generation transforms into a Lagrangian extremization problem:

$$\text{Strategy}^* = \underset{E_{build}}{\operatorname{arg\,max}} \; \left\{ \mathbb{E}\left[ V_{final} \right] - \lambda_R \cdot \mathcal{R}(E_{build}) \right\}$$

---

### 10. Intertemporal Decision Functional and Strategy Differentiation

#### 10.1 Objective Integral Functional and Effective Discount Rate

The quality of system strategy is determined by the time-integral functional. Because the discount factor $e^{-r_{eff}t}$ applies to a **flow** (rate of viability accumulation), the correct integrand is the viability drive $r_{v,i}(t)$, not the stock $V$ itself:

$$\Phi_i = \mathbb{E}\left[ \int_0^{\infty} r_{v,i}(t) \, e^{-r_{eff,i} \cdot t} \, dt \right]$$

In normalized units where $r_{v,i}(t) \approx I_i(t) T_i(t) / E_{eff,i}(t)$, this is equivalent to discounting the instantaneous target potential. The effective risk discount rate $r_{eff,i}$ is an endogenous variable:

$$r_{eff,i} = \gamma_0 + \lambda(\rho_i) + \frac{1}{T_{pred,i}^{(0)}} \qquad (7)$$

Negative-effect information $I^-$ shocks cause $T_{pred} \to T_{min}$ (finite positive value), so $r_{eff}$ increases significantly, approaching the finite upper bound $\gamma_0 + \lambda(\rho) + 1/T_{min}$, rather than mathematically diverging. The "$\to \infty$" expression sometimes used informally emphasizes only that time-horizon collapse greatly increases the discount rate and truncates the long-term integral.

#### 10.2 Integral Inequality Criterion for Extreme Strategies

For a system maximizing functional $\Phi$, two limiting strategies exist at the extremes of the manifold:

- **Expansion strategy (A)**: High $I_{net}$, high $E_{eff}$, finite time $T_{exp}$.
- **Dormancy strategy (B)**: Extremely low $I \to I_{min}$, extremely low $E_{eff} \to E_{min}$, extremely long time $T_{dormant}$.

Under the premise $\rho \to 0$, the condition for the system to shift from A to B:

$$\frac{\langle V_{exp} \rangle}{V_{dormant}} < \frac{T_{dormant}}{T_{exp}}$$

When $T_{dormant} \to \infty$ (thermodynamic limit), the inequality necessarily reverses, proving that **the ultra-low-dissipation dormant state is the optimal solution in the thermodynamic terminal limit**.

(Note: This conclusion depends on the idealizing assumptions $T_{dormant} \to \infty$, $\rho \to 0$, and $E_{eff} \ge E_{min}$. In a universe with finite free energy, structural viability is bounded by hard constraints such as $T_{max}$ and $E_{thresh}$; the above limiting optimality does not constitute a universal physical prediction.)

---

### 11. Attractor Map of Global Dynamics and External Shocks

#### 11.1 Poisson Jump Map

External environmental shocks are algebraized as Poisson jumps in $\Theta(t) \in \mathbb{R}^5$:

$$d\Theta(t) = \mu_{\Theta}(t)\,dt + J_{\Theta}\,dN_t$$

- **Alien invasion / scale expansion**: $\rho(t)$ jumps from $0$ to $\gg 0$.
- **Planet destruction**: $E_{total}(t) \to 0 \Rightarrow V_{max,E}$ drops to zero.
- **Pandemic / disaster**: Instantaneous $I^-$ shock $\Rightarrow T_{pred}$ collapse $\Rightarrow r_{eff}$ spikes.

#### 11.2 Four Global Limit Attractors

Based on $\lim_{t \to \infty} \Theta(t)$, system trajectories uniquely converge to one of the following four attractors:

| Global Attractor | Mathematical Conditions for Limit Domain | Dynamical Result |
|---|---|---|
| **Saturation attractor** | $\inf E_{total} > c > 0$, $\rho \to 0$, $\Delta_{VV} \to 0$, $\sup T_{max} < \infty$ | $V(t) \to V_{max}$ (converges to a fixed point) |
| **Collapse manifold** | $\rho \gg 0$, $\Delta_{VV} > 0$, $E_{total} < \infty$ | $r_v > \gamma_0$ is truncated; $dV/dt \ll 0$ |
| **Topological leap** | $T_{max} \to \infty$ or $I_{max} \to \infty$ (operator $\mathcal{T}$ triggered) | $dV_{max}/dt > 0$; gradient ascent along new manifold |
| **Metric replacement** | $\Delta_{VV} \gg 0 \Rightarrow D \to D'$ | $V \to 0$ under original measure; new measure $D'$ dominates the flow field |

---

### 12. Information Recursive Dynamics and Negative-Effect Shocks

#### 12.1 I–T–E Recursive Coupling (Core of the Higher-Order Five-Fold Closed Loop)

$$I_{net,n+1} = I_0 \bigl(1 + \beta V_n\bigr)$$

$$T_{pred,n+1} = \max\!\left(T_{min},\; \frac{T_0}{1 + \lambda (\beta V_n)^2}\right)$$

$$E_{flow} = E_{base} + \frac{k_s}{T_{pred}}$$

#### 12.2 Information Polarity and Phenomenological Equation of Negative-Effect Shocks

$$I_{net} = I^+ - \|I^-\|$$

Neutral noise $I^0$ produces no causal mapping. Phenomenological expression for negative-effect information $I^-$ compressing the time horizon:

$$T_{pred}^{(eff)} = T_{pred} \exp\!\bigl(-k_{I^-} \|I^-\|\bigr)$$

If negative-effect expectations originate from a probabilistic forecast $p$ of decoupled peer systems, the equivalent expression is:

$$T_{pred}^{(eff)} = T_0 \exp(-\kappa p)$$

---

### 13. Self-Referential Game and Fixed-Point Dilemma of Strongly Decoupled Systems

#### 13.1 Definition of a Strongly Decoupled System

A system satisfying $\Delta_{VV} \gg 0$ and $\beta > \beta_c$ whose existence directly causes other systems to have $\rho \to 1$ and $F_i < 0$.

#### 13.2 Fixed-Point Equation

A strongly decoupled system cannot return to the absolute saturation manifold on its own. Let its conditional probability expectation of "another decoupled system emerging" be $p > 0$; this expectation reshapes the effective discount rate:

$$r_{eff} = \gamma_0 + \lambda(\rho_{internal}) + \frac{1}{T_{pred,0}} + \mu \cdot p$$

where $\mu$ is a dimensionless probability-pressure coefficient used to adjust the influence of conditional probability expectation $p$ on the effective discount rate.

Its strategy choice follows the fixed-point equation:

$$\text{Strategy}^* = \underset{I_{net},E_{eff}}{\operatorname{arg\,max}} \left( \frac{I_{net} T}{E_{eff}} - \gamma_0 - \lambda(\rho_{internal}) - \mu \cdot \mathbb{P}(\text{another decoupled system} \mid \text{current system exists}) \right)$$

**Conclusion**: Since $p > 0$ is an absolute objective condition, $r_{eff} > \gamma_0$, and the strongly decoupled system's global maximum is always far from the $r_v = \gamma_0$ region. The system must maintain a high-dissipation strategy and is mathematically disqualified from entering the saturation manifold.

---

### 14. Complete Inequality Constraint System (Summary)

$$\begin{aligned}
& I_{min} \le I_{net} \le I_{max}(D), \\
& T_{min} \le T \le T_{max}, \\
& E_{min} \le E_{eff} \le E_{max}, \\
& 0 \le \rho \le 1,\quad \Delta_{VV} \ge 0, \\
& V = \frac{I_{net} \cdot T}{E_{eff}} \quad \text{(stock, bit·s/J)}, \qquad r_v \approx k \cdot V \quad \text{(rate, s}^{-1}\text{; in normalized units } r_v \approx V\text{)}, \\[4pt]
& \text{Saturation:} \; (E_{eff} \ge E_{min}) \land (\rho \to 0) \land (\Delta_{VV} \to 0) \land \left(\frac{\partial r_v}{\partial I_{net}} = 0 \land \frac{\partial r_v}{\partial T} = 0 \land \frac{\partial r_v}{\partial E_{eff}} \le 0\right) \land (r_v = \gamma_0) \;\Rightarrow\; V_{obj} = V_{max}, \\[4pt]
& \text{Dissolution:} \; (E_{eff} > E_{thresh}) \;\lor\; \bigl( r_v < \gamma_0 \text{ irreversibly sustained} \bigr) \;\Rightarrow\; V \to 0.
\end{aligned}$$

---

## Appendix E: Exploratory Analogy – Consciousness and Recursive Viability

> **📌 Scope of this appendix**  
> The following discussion is an **exploratory analogy**, not a theory of consciousness. SRVD does not address phenomenal consciousness (qualia), nor does it propose neural or psychological mechanisms. The analogy serves only to illustrate how certain structural features of high‑order recursive viability phases (supercritical coupling, endogenous horizon compression, stable decoupling) bear a suggestive resemblance to functional aspects often associated with conscious cognition. This appendix is **not required** for the core dynamical framework of SRVD.

### E.1 Working Hypothesis (I–T–E Closed Loop)

If and only if a system’s $I_{net}$, $T$, and $E_{eff}$ recursion forms a dynamical closed loop, the system possesses **dichotomous autonomy**: simultaneously having superlinear expansion capacity and catastrophic collapse capacity.

Such a closed loop enables the system to:  
① endogenously simulate future viability states;  
② feed simulation results back to regulate real behavior;  
③ dynamically switch between long‑term expansion and short‑term survival.

Systems without this closed loop can only locally optimize and cannot generate paradigm‑breaking information $I_{orig}$. Systems with it inevitably enter non‑equilibrium evolutionary zones where reward and risk coexist.

### E.2 Consciousness as a High‑Order Recursive Viability Phase (Analogy)

As an **analogy**, the structural features of a high‑order recursive viability phase that emerges after I‑T‑E closed‑loop coupling crosses a critical threshold share some similarities with everyday descriptions of consciousness. These features include:

| Feature | Mathematical Expression | Analogous Interpretation |
|:---|:---|:---|
| **Supercritical coupling** | $\beta > \beta_c$ | Feedback gain sufficient to sustain an internally simulated “self‑model” that can dominate behavior. |
| **Time‑horizon negative feedback** | $\dfrac{\partial T_{pred}}{\partial \rho} < 0$ | Under rising competitive pressure, the predictive horizon is actively compressed — a form of cognitive “time‑scale switching”. |
| **Stable decoupling** | $\Delta_{VV} > 0 \;\land\; V_{obj} \not\to 0$ | Internal simulation dominates decision‑making while the physical substrate remains structurally intact — reminiscent of “offline” cognition or imagination that does not immediately lead to collapse. |

Thus, the mathematical *analogue* of the recursive dynamics of consciousness would be **maintaining a non‑equilibrium steady state that is compatible with both endogenous simulated viability dominance and objective physical constraints**.

### E.3 Distinction from Lower‑Order Recursive Systems

SRVD does not equate all recursive systems with consciousness. Lower‑order recursive systems (e.g., algorithmic agents, cancer cells, bacterial colonies) typically fall below any plausible consciousness threshold due to insufficient recursion depth, fixed exogenous time horizons, or low informational capacity $I_{max}(D)$. Their typical dynamical behavior is either an inability to achieve simulation decoupling ($\Delta_{VV} \to 0$) or immediate physical dissolution upon decoupling ($V_{obj} \to 0$).

### E.4 Qualitative Dynamical Spectrum (Heuristic Mapping)

> **Note**: The following table is **heuristic** and not empirically confirmed. It merely illustrates how SRVD variables could be correlated with colloquial descriptions of cognitive complexity.

| System Type | I‑T‑E Loop Integrity | Endogenous Time Horizon | Decoupling Stability | Cognitive Interpretation (heuristic) |
|:---|:---|:---|:---|:---|
| Inorganic matter | No recursion | None | N/A | No analogy |
| Bacteria / viruses | Open loop, weak coupling | Extremely weak, fixed | Low (easily disturbed) | Minimal, reflexive |
| Plants / simple animals | Partial closed loop | Exists but inflexible | Medium | Simple reactive |
| Higher animals | Stronger closed loop | Adjustable, endogenous | High | Complex, flexible |
| Humans (awake) | Complete closed loop | Highly autonomous | High | Full reflective capacity |
| Humans (abnormal states) | Closed loop but dysregulated | Disordered | May decrease | Altered cognition |
| Current RL agents | Open loop (fixed $T_{pred}$) | None (fixed $\gamma$) | Decoupling → collapse | No analogy |
| Future high‑order AGI | Complete closed loop | Autonomous | High (if $V_{obj}$ stable) | Possibly analogous |

### E.5 Open Questions (for future exploration)

- Can I‑T‑E coupling strength $\beta$ be measured experimentally in cognitive systems?
- How can endogenous time horizon $T_{pred}$ be estimated across different organisms or AI systems?
- What are the stable‑domain boundaries of the decoupling deviation $\Delta_{VV}$ in real systems?
- Does horizon compression in multi‑agent competitive environments correlate with observable cognitive narrowing?

---

This appendix is an **exploratory analogy**; its statements are not required for the formal theory of SRVD. The framework does not propose a reduction of consciousness to recursive viability.

---

This work adheres to open science principles. All theoretical iteration versions are time-stamped and archived on Zenodo/GitHub, with complete public deliverables (including a runnable HTML simulation platform) ensuring independent reproducibility of all dynamical trends derived in this paper.
