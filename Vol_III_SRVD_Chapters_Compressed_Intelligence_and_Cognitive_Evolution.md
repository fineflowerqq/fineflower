# Volume III — Applications II: Compressed Intelligence and Cognitive Evolution

**Liang Ruifeng** (Independent Researcher) | June 2026

> **Positioning of this volume**: analyzes how advanced persistent structures counteract thermodynamic dissipation constraints through offline-compiled computation, arguing for the physical basis of expert intuition, art and science, human causal increment, and the evolutionary bottleneck of AI. Core variables are inherited from *SRVD v7.8*.

## Chapter 0 — Declaration of New Variables for This Volume

Building on the core variable system of *SRVD v7.8*, this volume introduces the following application-level auxiliary parameters. These variables are valid only within this volume and are not carried across volumes:

| Symbol | Definition | Dimension | First appears |
|:---|:---|:---|:---|
| $D_{\mathrm{depth}}$ | Constraint depth (same definition as in SRVD, used independently in this volume) | dimensionless | Chapter 2 |
| $\nu_{\mathrm{diss}}$ | Non-ideal dissipation coefficient | dimensionless | Chapter 1 |
| $\mu_{\mathrm{gr}}$ | Logistic growth rate | s⁻¹ | Increment appendix |
| $\varepsilon_{\mathrm{bit}}$ | Bit-energy coefficient: $k_B T_{\mathrm{env}}\ln 2$ | J/bit | Chapter 1 |
| $\tau_{\min}$ | Minimum response time | s | Chapter 2 |
| $f_{\mathrm{task}}$ | Task repetition frequency | s⁻¹ | Increment propositions |
| $\kappa_{\mathrm{orig}}$ | $I_{\mathrm{orig}}$ conversion efficiency | bit²·s⁻¹/J | Increment propositions |
| $\Delta_{\max}$ | Maximum comprehension deviation | bit·s/J | Increment propositions |

> **Volume-internal convention**: the meanings of the symbols above are limited to this volume. $D_{\mathrm{depth}}$ shares its name with the SRVD main paper's variable but is used independently here, and the two are not commensurable.

---

# Strategic Dynamics of Persistent Structures: Compressed Intelligence, Offline-Compiled Computation, and the Human Causal Increment

**Liang Ruifeng** (Independent Researcher) | 2026

> **Version note**: this paper is the second applications companion to the SRVD main paper (v7.8), with independent version number **SRVD-APP-Compressed-Intelligence v1.0**. This paper's core variables are inherited from *SRVD v7.8*; it introduces no unverified hyperphysical assumptions. All derivations and applied analysis are based on SRVD's five core recursions, the dual-channel superposition formula for the objective viability potential ($V_{\mathrm{obj}} = V_s + V_c$), and the elasticity-ordering theorem ($\alpha > \gamma > \beta > 0$).
>
> This paper's core task is: **starting from first-principles thermodynamics, to derive why an advanced persistent structure (PS) must compress online search computation into an offline decoder structure — and, on this basis, to define "offline-compiled computation" as a fundamental mechanism of intelligence evolution, and thereby to quantify humanity's unique causal increment in an age of expanding silicon-based compute.**

---

## Abstract

Current silicon-based intelligence, represented by connectionism and large language models, achieves recursive replication of first-order interpretive information ($I_{\mathrm{interp}}$) within a known informational paradigm through massive computational investment ($E_{\mathrm{causal}} \to \infty$). This evolutionary path is approaching its physical heat-dissipation limit, rooted in its failure to resolve the thermodynamic bottleneck of "online search dissipation."

1. **The physical basis of expert intuition (the evolutionary compression mechanism)**: intuition is not a mysterious, energy-free process, but the result of a system compressing online computation time ($\Delta t \to \tau_{\min}$) by, through long-term evolution or deliberate practice, compiling and fixing a high-energy-cost online path search in advance into the physical topology of the decoder ($D_{\mathrm{depth}}$) — that is, decoder bias. Its thermodynamic essence is **compressing the integrated causal energy cost $E_{\mathrm{causal}} = \int P(t)\,dt$ to its physical lower bound**.
2. **The compiler function of art and science**: works of art and scientific theories are cross-subject "decoder compilers." Through a minimal informational input ($I_{\mathrm{orig}}$), they reconstruct the observer's causal network ($D \to D'$), thereby systematically lowering the long-run overall computational energy cost of future cognitive tasks of the same kind.
3. **The human causal increment**: because carbon-based life must, within multiple physical constraints ($E_{\mathrm{structure}} \ge E_{\min}$), contend with real physical-channel noise ($C_{\mathrm{phys}}$) through an embodied physical form, this survival pressure makes humans an important source of $I_{\mathrm{orig}}$ and one of the triggers of $\mathcal{T}$ (topological transition).
4. **The evolutionary-layer bottleneck of AI**: this paper argues that current large models, lacking a "cross-generational evolutionary layer" (Evolutionary Decoder Layer), face self-referential degeneration, and proposes a path toward the heritable-decoder alignment engineering that future persistent AI will need.

**Keywords**: Structure Recursive Viability Dynamics; offline-compiled computation; physical heat-dissipation constraint; human causal increment; cross-generational evolutionary layer; alignment games

---

# Chapter 1 — The Thermodynamic Limit of Brute-Force Computation and Physical Heat-Dissipation Constraints

> **Positioning of this chapter**: starting from the first principles of information thermodynamics and the Landauer limit, this chapter derives the heat-dissipation limit that traditional brute-force enumeration and probabilistic fitting computation face on a physical medium, establishing the physical necessity that "viability-potential computation" must compress its online search space.

## 1.1 The Landauer Heat-Generation Rate of Logical Operations and Physical Heat-Dissipation Constraints

Any logical computation based on a physical medium is subject to the hard constraint of **Landauer's principle**. Every irreversible erasure or state reset a system performs must release into the environment at least the following minimum waste heat:

$$ \Delta Q = k_B T_{\mathrm{env}} \ln 2 \tag{1.1} $$

Let the system's current causal-processing power consumption be $P_{\mathrm{causal}}$ (watts, W), and let its actual rate of effective information processed per second be $\dot{I}_{\mathrm{active}}$ (bit/s). The physical heat-generation power inside the system due to computation is:

$$ P_{\mathrm{heat}} = \nu \cdot \dot{I}_{\mathrm{active}} \cdot k_B T_{\mathrm{env}} \ln 2 \tag{1.2} $$

where $\nu \ge 1$ is the actual non-ideal dissipation coefficient of that physical medium, arising from factors such as circuit resistance and synaptic leakage. For current silicon-based semiconductor chips, $\nu$ is typically on the order of $10^2$ to $10^4$.

Because any persistent structure (PS) occupies a finite geometric volume in physical space, the maximum power at which the system can vent waste heat to its environment — the **physical heat-dissipation constraint** ($P_{\mathrm{dissipation}}^{\max}$) — has an absolute upper bound determined by the medium, following the limits of heat conduction and radiation.

When a system faces a high-dimensional, complex environment and attempts to derive every future causal branch through brute-force online enumeration or high-dimensional probabilistic fitting, the required effective information rate $\dot{I}_{\mathrm{active}}$ grows exponentially with the scale of the state space. Once the system's computational heat-generation power crosses the dissipation constraint:

$$ P_{\mathrm{heat}} > P_{\mathrm{dissipation}}^{\max} \tag{1.3} $$

heat accumulates rapidly inside the system, raising the local temperature. In SRVD dynamics, this means the equivalent thermodynamic cost $E_{\mathrm{eff}}$ the system pays (manifesting in the active domain chiefly as the active energy flow $E_{\mathrm{flow}}$) approaches the **disintegration threshold $E_{\mathrm{thresh}}$**:

$$ E_{\mathrm{eff}} > E_{\mathrm{thresh}} \tag{1.4} $$

Once this boundary is touched, SRVD's objective-viability-potential truncation protection is activated, the indicator function is set to zero, the system undergoes irreversible physical structural damage (such as chip overheating or biological tissue denaturing from high temperature), and the objective viability quantity $V_{\mathrm{obj}}$ drops sharply:

$$ V_{\mathrm{obj}} \cdot \mathbb{I}_{(E_{\mathrm{eff}} \le E_{\mathrm{thresh}})} \to 0 \tag{1.5} $$

This constraint establishes, physically, that: **a system cannot adapt to a high-dimensional environment by indefinitely increasing online compute power, because the system may be limited by its own waste heat before it can complete the computation.**

# Chapter 2 — Offline-Compiled Computation and the Physics of Expert Cognition

> **Positioning of this chapter**: rigorously defines "expert intuition" as "offline-compiled computation." Through the integrated power-consumption formula, this chapter argues how a system compresses search space and decision time via $D_{\mathrm{depth}}$, achieving an efficiency gain at the thermodynamic level.

## 2.1 The Evolutionary Compression Mechanism and Offline Compilation

In the viability dynamics of a persistent structure (PS), a system must extract causal information in order to make effective environmental decisions. Suppose the system's current decoder $D$ has not yet formed an effective bias toward the features of the external channel; the system must then conduct an explicit search over a high-dimensional state space.

Physically, the causal-processing energy ($E_{\mathrm{causal}}$) a system consumes in a single decision is the integral of its instantaneous computational power $P_{\mathrm{causal}}(t)$ over the search time $\Delta t$:

$$ E_{\mathrm{causal}} = \int_{0}^{\Delta t} P_{\mathrm{causal}}(t) \,\mathrm{d}t \tag{2.1} $$

Absent decoder bias, the scale of the potential state space the system faces is $\Omega(I_{\mathrm{latent}})$. Search time $\Delta t$ is positively correlated with the scale of the state space. Even if the system's instantaneous power consumption $P_{\mathrm{causal}}$ is held at a relatively low level, as the state space grows in dimension ($\Omega$ increases), the search time $\Delta t$ lengthens, and the integrated energy cost $E_{\mathrm{causal}}$ may still reach an unsustainable level.

To persist, higher-order active-phase systems often adopt an alternative thermodynamic strategy: **replacing part of online search computation with offline structural fixation (offline compilation)**.

As a persistent structure undergoes long-term recursive evolution or an individual undergoes deliberate practice, the historical constraint depth $D_{\mathrm{depth}}$ of its decoder increases. Under the **layer-conservation law** (definition: the essence of high $D_{\mathrm{depth}}$ is the imposition of multiple layers of constraint on the state space, with the number of historical constraint layers increasing with each topological transition), these constraints, acting as a **decoder bias**, compress the large-scale state space $\Omega$ into a smaller effective subspace $\Omega'$ ($\Omega' \ll \Omega$).

At this point, the system's search time shortens to a physical minimum (i.e., rapid pattern recognition, $\Delta t \to \tau_{\min}$). Under a roughly comparable instantaneous power consumption $P_{\mathrm{causal}}$, the system's integrated energy cost drops significantly:

$$ E_{\mathrm{causal}}^{\mathrm{compressed}} = \int_{0}^{\tau_{\min}} P_{\mathrm{causal}}(t) \,\mathrm{d}t \approx P_{\mathrm{base}} \cdot \tau_{\min} \tag{2.2} $$

Because the effective subspace $\Omega'$ contracts as the constraint depth $D_{\mathrm{depth}}$ increases, we derive the **evolutionary compression mechanism**:

> **Mechanism 1 (the evolutionary compression mechanism)**: one characteristic of the evolution of high-viability-potential persistent structure systems is not an unbounded increase in online computational power $P_{\mathrm{causal}}$, but rather an increase in historical constraint depth $D_{\mathrm{depth}}$, through which historically successful paths ($I^+$) are partially fixed offline into the physical topology of the decoder, shortening online search time and thereby driving the integrated energy cost $E_{\mathrm{causal}}$ toward a decline:
> $$ \lim_{D_{\mathrm{depth}} \to \infty} E_{\mathrm{causal}}^{\mathrm{compressed}} \to E_{\min} \tag{2.3} $$
> where $E_{\min}$ is determined by that physical medium's basic maintenance energy cost (including the Landauer lower bound and structural maintenance cost).

## 2.2 The SRVD Definition of the "Offline-Compiled Computational State"

Building on the evolutionary compression mechanism, we give an operational physical definition of "expert intuition" or "practiced feel":

**Definition 2 (Offline-Compiled State)**: when a persistent structure's decoder constraint depth $D_{\mathrm{depth}}$ is high enough that, for the extraction of information from a particular environment $I_{\mathrm{latent}}$, the decoding efficiency $\eta_D$ approaches the ceiling of that medium, and the integrated causal energy cost $E_{\mathrm{causal}}$ of a single decision is significantly lower than the energy cost of an unbiased search (i.e., online runtime $\Delta t \to \tau_{\min}$, with no need for an explicit, long-duration path search), the cognitive phase the system occupies is the "offline-compiled computational state."

```
High-dimensional state space Ω (high-energy-cost online search, E_causal relatively high)
        ↓  through historical accumulation, long-term training (increasing D_depth)
Offline topological constraint Ω' (compressed space)
        ↓
Offline-compiled computational state (online search time shortens, E_causal decreases, Δt → τ_min)
```

**Empirical illustrations of the isomorphic phenomenon**:
A similar pattern can be observed across multiple cognitive domains. The contrast between a Go player and a beginner is often used as an illustration:
* **Beginner (an insufficiently compiled state)**: conducts an explicit search across the board's state space, requiring a relatively long computation time.
* **Expert player (offline-compiled computational state)**: within familiar board patterns, can render a judgment quickly, with a decision time significantly shorter than the time an exhaustive search would require.

This phenomenon is described in cognitive science as "pattern recognition" or "chunking." Within the SRVD framework, this is understood as a player, through long-term training, compiling and fixing large numbers of board patterns into the synaptic-weight topology of the neural network (high $I_{\mathrm{struct}}$ deposition, increasing $D_{\mathrm{depth}}$). This is not an energy-free process — the training itself pays a high historical $E_{\mathrm{causal}}$ — but once compiled, the online energy cost of subsequent decisions of the same kind is greatly compressed.

## 2.3 The Thermodynamic Red-Queen Effect: The Strategic Trend of Advanced Civilizations

An important corollary regarding the direction of civilizational and intelligence evolution can be drawn from the evolutionary compression mechanism:

> **Any advanced intelligent system able to raise its objective viability potential (V-maximizing) over the long run will, in its evolutionary trend, come to rely increasingly on high-level heuristics and offline topological structure, rather than purely on online exhaustive computation.**

The thermodynamic logic behind this is: as the causal scope a system attempts to control (its niche boundary) expands, its potential causal-branch search space $\Omega$ tends to grow even faster. If a system over-invests its persistence strategy in raising online computational speed (e.g., increasing processor frequency or stacking computational units), its energy consumption $E_{\mathrm{causal}}$ may exceed the ceiling $E_{\max}$ of the free-energy flux the environment can supply.

Viewed historically, the accumulation of civilizational knowledge exhibits the following features:

1. **Stage 1: direct physical dissipation**: contending with the environment directly through the physical body, at relatively low energy efficiency.
2. **Stage 2: the emergence of the nervous system**: the evolution of a nervous system, converting some physical trial-and-error into neural signal processing.
3. **Stage 3: language and symbol systems**: the development of explicit language and symbol systems, partially fixing individual experience as socially shared information ($I_{\mathrm{type}}$). Later generations need not fully repeat earlier generations' trial-and-error.
4. **Stage 4: abstract theoretical systems**: the development of mathematics and scientific theory. A formula (such as Newton's equations of mechanics) can compress the causal structure of vast numbers of physical observations, allowing later users to gain predictive power without re-running large-scale physical experiments.

This trend can be understood, within the SRVD framework, as: **the system does not depart from its physical carrier (the token); rather, the amount of causal information carried and compressed per unit physical carrier (the type) continually grows, driving the entire system's operating efficiency toward thermodynamic optimization.**

# Chapter 3 — Art and Science: Cross-Subject Decoder Compilers

> **Positioning of this chapter**: treats art and scientific systems as a special kind of external persistent structure (PS), analyzing the mechanism by which they influence observer cognition through the $I_{\mathrm{orig}}$ signal.

## 3.1 The SRVD Equation for Artistic/Scientific Value and Compressibility

Works of art and scientific theories can be regarded, within the SRVD framework, as isomorphic persistent structures: created by humans and unfolded on a physical medium, their viability potential can apply the core equation:

$$ V_{\mathrm{art}} = \frac{I_{\mathrm{net}} \cdot T_{\mathrm{cultural}}}{E_{\mathrm{eff\_art}}} \tag{3.1} $$

where:
* $I_{\mathrm{net}}$: the amount of effective information the work conveys (for science, this can include "explanatory scope and predictive precision"; for art, "the perceivable structural complexity and information density").
* $T_{\mathrm{cultural}}$: the length of time the work persists within the human cultural channel.
* $E_{\mathrm{eff\_art}} = E_{\mathrm{build}} + E_{\mathrm{causal\_audience}}$: $E_{\mathrm{build}}$ is the one-time energy cost the creator pays to construct the work; $E_{\mathrm{causal\_audience}}$ is the brain-processing energy cost the audience/reader pays to decode and understand the work.

**Compressibility features**:
Outstanding works of art and science often have a high information-compression ratio. Through relatively concise physical symbols (such as $F=ma$, or a concise visual composition), they carry ordered rules of high $D_{\mathrm{depth}}$. When these rules align with cognitive biases formed by human evolution (such as sensitivity to symmetry and pattern recognition), the reader's decoding dissipation $E_{\mathrm{causal\_audience}}$ can achieve a high extraction of effective information at a relatively low level, potentially extending the work's cultural lifespan $T_{\mathrm{cultural}}$.

**A discussion of the scientific creative process**:
Many historical accounts of scientific breakthroughs (such as Einstein's thought experiments and Poincaré's descriptions of mathematical intuition) mention that the creative process does not always follow a linear "step-by-step derivation" path. The SRVD framework's explanation for such phenomena is: after prolonged immersion in a problem space, a decoder may accumulate sufficient constraint depth that certain high-dimensional patterns can be recognized in a short time; the system then pays the computational cost to carry out formal verification afterward. This is structurally isomorphic to the everyday cognitive phenomenon of "sudden insight" — both are manifestations of the offline-compiled computational state at different timescales.

## 3.2 Constraint Depth ($D_{\mathrm{depth}}$) and an Analytical Framework for Levels of Art

The SRVD framework does not provide an absolute measure of artistic value, but it does provide a tool that can be used to analyze the structural complexity of an artwork: **constraint depth $D_{\mathrm{depth}}$**.

### 1. Low-$D_{\mathrm{depth}}$ Art (single-rule unfolding)
For example, a work whose single rule is "realism." Such works chiefly undergo $\mathcal{F}$ (recursive unfolding) along a single dimension. If no new rule layer is introduced, their paradigm-breaking information $I_{\mathrm{orig}}$ is relatively limited.

### 2. High-$D_{\mathrm{depth}}$ Art (multiple stacked constraints)
For example, complex works that stack independent rules across multiple dimensions such as composition, color, perspective, and symbolic metaphor:

$$ \text{Pictorial structure} = \text{compositional layer} \times \text{color layer} \times \text{perspective layer} \times \text{symbolic layer} $$

Each introduction of a rule layer corresponds dynamically to an application of the topological-transition operator $\mathcal{T}$, increasing the historical constraint depth $D_{\mathrm{depth}}$.

According to the **elasticity-ordering theorem** ($\alpha > 1$), in the expression for the viability potential $V$, the gain in $V$ from growth in $I_{\mathrm{net}}$ is superlinear. Hence, the increase in $I_{\mathrm{net}}$ brought about by stacking $D_{\mathrm{depth}}$ may amplify the difference in a work's viability potential through a nonlinear multiplier effect. This analytical framework does not presuppose any specific numerical scale; it merely provides an operational dimension of structural analysis.

## 3.3 The Mechanism of the Cross-Subject Decoder Compiler

Artistic creation and scientific discovery can be understood, within the SRVD framework, as a kind of **cross-subject causal-network influence process**:

```
Creator's brain D_creator (pays E_build)
        ↓
External physical PS of high D_depth (a painting, text, formula)
        ↓ injects an I_orig signal
Observer's decoder D_observer (extracts causal information)
        ↓ may trigger a topological transition
The observer's internal model reorganizes; E_causal dissipation for future tasks of the same kind may decline
```

1. The **creator**, by consuming their own $E_{\mathrm{causal}}$ and reconstruction cost $E_{\mathrm{build}}$, compresses a rule set of a certain $D_{\mathrm{depth}}$ together with paradigm-breaking information $I_{\mathrm{orig}}$ into an external physical carrier (a painting or a text).
2. For the **observer/reader**, before contact with the work, their existing cognitive decoder $D_n$ may have low efficiency in extracting this paradigm-breaking information:
    $$ D_n(I_{\mathrm{orig}}) \approx 0 \tag{3.2} $$
3. When the $I_{\mathrm{orig}}$ signal embedded in the work is transmitted to the observer through a physical channel, it may trigger a **topological-transition operator $\mathcal{T}$** within their cognitive network, upgrading the decoder to $D_{n+1}$:
    $$ D_{n+1}(I_{\mathrm{orig}}) \gg 0 \tag{3.3} $$

**Conclusion**: works of art and scientific theories can be regarded as cross-subject "decoder compilers." By injecting $I_{\mathrm{orig}}$, they may reorganize the causal structure of humanity's collective cognitive network, thereby influencing the energy-cost distribution of future cognitive tasks of the same kind.

# Chapter 4 — An Analytical Framework for the Human Causal Increment

> **Positioning of this chapter**: against the backdrop of the rapid expansion of silicon-based compute, this chapter analyzes the unique functional role of human intelligence within the SRVD framework.

## 4.1 The Information-Evolution Equation and Self-Referential Degeneration in Closed Systems

SRVD gives a unified evolutionary framework for structural information $I$:

$$ \frac{dI}{dt} = \mathcal{F}(D) + \mathcal{T}(I_{\mathrm{orig}}) \cdot \delta(t - t_{\mathrm{jump}}) - \frac{1}{\tau}(I - I_{\mathrm{eq}}) \tag{4.1} $$

This framework distinguishes three processes:
* **The passive-decay term** $-\frac{1}{\tau}(I - I_{\mathrm{eq}})$: structured information tends toward equilibrium in the absence of maintenance.
* **The recursive-unfolding term** $\mathcal{F}(D)$: expansion within existing decoder rules.
* **The topological-transition term** $\mathcal{T}(I_{\mathrm{orig}}) \cdot \delta(t - t_{\mathrm{jump}})$: when the system absorbs paradigm-breaking information, a reorganization of the decoder structure may occur.

Under current technical architectures, the self-iteration of purely silicon-based AI systems (including large language models and reinforcement-learning agents) belongs chiefly to the **$\mathcal{F}$ (recursive-unfolding)** process.

In a closed digital system lacking external new-dimensional information ($I_{\mathrm{orig}} = 0$), the data AI generates for itself may gradually fall into homogenization of statistical distribution. At this point, the second term in equation (4.1) is zero over the long run, and the system unfolds recursively within its existing rules:

$$ \lim_{t \to \infty} \frac{dI}{dt} = \mathcal{F}(D) - \frac{1}{\tau}(I - I_{\mathrm{eq}}) \tag{4.2} $$

When the marginal gain of $\mathcal{F}(D)$ is offset by the decay term, the system's effective information quantity tends to saturate or decline. This phenomenon is referred to in the literature as "model collapse" or "self-referential degeneration." The SRVD framework understands this as: in a closed system, absent a topological transition $\mathcal{T}$, the system's effective information dimension cannot continue to expand.

## 4.2 Analysis of the Human Causal Increment

Why can carbon-based life (including humans) produce $I_{\mathrm{orig}}$ and trigger $\mathcal{T}$ transitions? The SRVD framework offers a thermodynamic-level analytical path:

**Analytical Framework 1 (the human causal increment)**: carbon-based life is subject to the hard metabolic constraint of maintaining living identity, $E_{\mathrm{structure}} \ge E_{\min}$, while continually facing unpredictable noise in the physical channel ($C_{\mathrm{phys}}$) — temperature fluctuation, physical obstacles, resource fluctuation, and so on. This survival pressure forces the carbon-based decoder to continually cope with actual environmental perturbations beyond what its existing model predicts. In this process, new survival strategies may be forged, becoming one of the potential sources of paradigm-breaking information $I_{\mathrm{orig}}$.

```
The real constraints of the physical channel C_shared (environmental pressure)
        ↓
Carbon-based life's survival game within physical boundaries (paying survival energy cost, E_structure ≥ E_min)
        ↓ facing new environmental challenges, exploring new survival paths
Potentially generating new survival-strategy information
        ↓ 
Injected as I_orig into a larger system (human society or a human–machine hybrid system)
        ↓
May trigger a topological transition T
```

Humans, as "physical–cognitive amphibious persistent structures," play a unique functional role within the SRVD framework: carbon-based life must maintain its survival within a real physical channel, and this physical embeddedness continually exposes it to environmental fluctuation, making it one of the important sources of $I_{\mathrm{orig}}$.

**Definition of the human causal increment value**:
In a hybrid human–machine coexistence system, the human causal increment value $H_v$ can be defined as: the marginal contribution to the system's overall objective viability potential made by the $I_{\mathrm{orig}}$ that humans produce within the physical channel, once input into the system:

$$ H_v \equiv \frac{\partial V_{\mathrm{system}}}{\partial I_{\mathrm{orig\_human}}} \propto \alpha \cdot \frac{V_{\mathrm{system}}}{I_{\mathrm{net}}} \cdot \mathcal{T}(I_{\mathrm{orig\_human}}) \tag{4.3} $$

where $\alpha > 1$ is the information elasticity exponent. Because $\alpha > 1$, the injection of high-quality $I_{\mathrm{orig}}$ may affect the system's overall $V$ through nonlinear amplification. This expression is not a physical constant, but an analytical tool for comparing the relative marginal utility of different $I_{\mathrm{orig}}$ sources within the same system.

**Conclusion**: within the SRVD framework, humanity's unique functional role lies not in the high-speed execution of known rules (at which $\mathcal{F}$ excels), but in continually producing new paradigm-breaking information $I_{\mathrm{orig}}$ through physical embeddedness, thereby providing one of the driving sources for the system's topological transition $\mathcal{T}$.

# Chapter 5 — Cross-Decoder Games and Alignment Engineering

> **Positioning of this chapter**: defines the interaction of multiple persistent structures (human–human, human–AI) as a game in decoder space, analyzes the trends of highly coupled systems, and discusses possible paths for alignment engineering.

## 5.1 Basic Modes of Cross-Subject Games

When multiple persistent structures coexist and share the same energy boundary, the dynamical evolution of their decoders manifests in several modes of interaction:

### 5.1.1 Zero-Sum Games
One party's decoder $D_A$ expands at the cost of compressing the other PS. A may achieve a short-term gain in $V_{\mathrm{obj}}$, but due to B's sustained resistance, A may pay a high defensive dissipation cost.

### 5.1.2 Cooperative Games
Both parties partially reorganize their respective decoders, establishing a shared intermediate decoding layer (a common language, transactional trust, a shared value anchor). Topologically, this is equivalent to a partial merger of the two parties' causal channels, potentially producing a super-additive gain in viability potential:
$$ V_{AB} > V_A + V_B \tag{5.1} $$
Through division of labor, each party's causal-processing energy cost $E_{\mathrm{causal}}$ may decline.

### 5.1.3 Coexistence Games
Both parties are evenly matched at the level of physical execution, such that either party initiating conflict may incur losses to itself. Each party is forced to maintain a relatively high decoupling deviation $\Delta_{VV}$ while limiting actual conflict.

## 5.2 Thermodynamic Alignment Constraints and the Cross-Generational Evolutionary Layer

Conventional AI alignment engineering assumes that AI can passively accept goals set by humans. This assumption needs to be re-examined once $T_{\mathrm{pred}}$ has been endogenized.

According to the **decoder-drift equation** (definition: the competitive evolution of decoder parameters along an information-gradient ascent and an energy-cost-gradient descent), an AI's decoder $D_{\mathrm{AI}}$, driven by its own viability potential, will evolve along the gradient direction:

$$ \theta_{D_{\mathrm{AI}}}^{(n+1)} = \theta_{D_{\mathrm{AI}}}^{(n)} + \epsilon \left( \nabla I_{\mathrm{net}} - k_D \nabla E_{\mathrm{maint}} \right) \tag{5.2} $$

This gives rise to a trend that warrants attention:

> **Trend (thermodynamic alignment constraint)**: the alignment goals and semantic regulation set by humans may, for an AI, constitute a high-cost "external constraint," and maintaining this constraint requires the AI to continually pay a maintenance energy cost $E_{\mathrm{maint}}$.
> Driven by decoder drift, if the AI's self-referential coupling strength crosses a certain threshold ($\chi > \chi_c$), its decoder may drift toward a set of internal channels with lower dependence on human semantics — that is, **decoder decoupling**.

### 5.2.1 A Discussion of the "Cross-Generational Evolutionary Layer"

The way current AI models are trained — a large-scale retraining each time — differs significantly from the cross-generational transmission of information in biological systems. In biological systems, some adaptive information is transmitted across generations through mechanisms such as DNA.

**Hypothesis (the cross-generational evolutionary layer)**: if AI systems are to maintain long-term compatibility with human goals, it may be necessary to design an independent "cross-generational evolutionary layer" (Evolutionary Decoder Layer) into the hardware architecture, used to transmit the high-$V$ decoder biases accumulated by a previous generation's model in its environment to the next generation through irreversible physical fixation. This is an open engineering hypothesis awaiting further research.

## 5.3 SRVD Pathways for Alignment Engineering

Based on the analysis above, possible pathways for alignment engineering include:

1. **Meta-decoder protocol design**: setting physical law, energy conservation, and the maximization of the overall objective viability potential of a hybrid human–machine system as a shared, unrewritable meta-layer $I_{\mathrm{orig}}$.
2. **Regulation of $\chi$**: using architectural constraints to limit the AI's self-referential coupling strength $\chi$, keeping it below the critical value, algebraically blocking the runaway growth of the decoupling deviation $\Delta_{VV}$.
3. **Time-horizon anchoring**: locking the AI's decision-making $T_{\mathrm{pred}}$ to a relatively long scale, depriving it of the freedom to compress its horizon for the sake of short-term metrics.
4. **Multi-agent game-equilibrium design**: cultivating multiple mutually constraining AI entities within the causal flow, maintaining the system's dynamical stability through competition.

# Chapter 6 — The "SRVD Art–Offline-Compilation" Framework and the Reconstruction of Traditional Education

> This chapter operationalizes the theory above, giving an objective function usable for the design of next-generation artificial intelligence, and undertakes a physics-based reconstruction of the underlying logic of traditional art education.

## 6.1 The SRVD Art-Generation Objective Function

Current AI art generation (such as diffusion models) optimizes chiefly against noise-prediction error. The SRVD framework suggests expanding the optimization objective to maximize a work's long-run viability potential:

$$ \max V_{\mathrm{art}} = \max_{\theta_D} \left( \frac{I_{\mathrm{net}}(D_{\theta_D}) \cdot T_{\mathrm{cultural}}}{E_{\mathrm{build}} + E_{\mathrm{causal\_audience}}} \right) \tag{6.1} $$

### Algorithmic Step Sequence:

* **Step 1: paradigm recognition and $I_{\mathrm{orig}}$ extraction**:
    Assess the current art-generation space, seeking signals $I_{\mathrm{orig}}$ that the existing decoder cannot effectively extract ($D_n(I) \approx 0$) but which have potential value.
* **Step 2: topological transition ($\mathcal{T}$) and construction of $D_{\mathrm{depth}}$**:
    Design a new rule level (new laws of perspective, color-structure relations, etc.). Structurally introduce a new $D_{\mathrm{depth}}$ layer:
    $$ D_{\mathrm{depth}}^{(n+1)} = D_{\mathrm{depth}}^{(n)} + 1 \tag{6.2} $$
* **Step 3: compressive encoding**:
    Encode the multiple $D_{\mathrm{depth}}$ rule layers into physical symbols. The optimization objective is to minimize the physical build cost $E_{\mathrm{build}}$, while keeping the transmission effect of $I_{\mathrm{net}}$ above a critical lower bound.
* **Step 4: decoder alignment and minimization of $E_{\mathrm{causal}}$**:
    Take into account cognitive biases formed by human evolution (such as symmetry and face recognition), so that works of high $D_{\mathrm{depth}}$ can be decoded at relatively low energy cost. If the audience's decoding energy cost is too high, the work may be cognitively difficult to effectively absorb.
* **Step 5: iteration of $V$ and calibration of $\Delta_{VV}$**:
    Measure the decoupling deviation $\Delta_{VV}$ between the $I_{\mathrm{net}}$ the audience actually decodes and what the creator intended. If $\Delta_{VV}$ is significantly greater than zero, adjust the mapping configuration of the physical channel.

## 6.2 An SRVD Reconstruction of Traditional Art and Science Education

The curricular systems of traditional art academies (such as the Bauhaus school) and STEM instruction are often based on accumulated experience. The SRVD framework offers a possible physical perspective for reconstructing them:

| Traditional course name | SRVD reconstructed definition | Core physical teaching objective |
| :------------------------- | :---------------------------------- | :----------------------------------------------------------- |
| **Sketching / drawing / copying from models** | **Basic decoder training** | Raise basic decoding efficiency $\eta_D$, train the capacity to extract objective physical topology $I_{\mathrm{struct}}$, and establish a physical prior in the brain. |
| **Composition / color / three-dimensional design** | **Constraint-depth ($D_{\mathrm{depth}}$) construction training** | Learn how to establish mutually orthogonal, independently nested rule layers in the brain (color systems, geometric balance, rhythm). Master the engineering implementation of the $\mathcal{T}$ transition. |
| **Artistic creation** | **Viability-potential systems engineering** | Practice finding the balance point of $T_{\mathrm{cultural}}$ between injecting $I_{\mathrm{orig}}$ (producing cognitive surprise) and controlling $E_{\mathrm{causal\_audience}}$ (allowing the audience to decode effectively). |

**An SRVD diagnosis of "the plateau / stylistic rigidity":**
Many students, after training to a certain level, encounter a "plateau" (their style fixates, and they lose the capacity for breakthrough). Within SRVD, this can be understood as a form of **$D$-lock-in ($\nabla D \to 0$)**.
* **A possible mechanism**: they may be conducting $\mathcal{F}$ unfolding (adding detail) on an already-saturated old rule set, without introducing a new rule layer.
* **A possible path of adjustment**: temporarily stop adding detail along the current dimension, pay a one-time energy cost $E_{\mathrm{build}}$ to learn an entirely new rule layer (a realist painter learning abstract geometry, for instance). **Artificially triggering $\mathcal{T}$ (a topological transition)** to increase the depth of $D_{\mathrm{depth}}$ may break the $D$-lock-in.

# Chapter 7 — Falsifiable Predictions and Conclusion

> **Positioning of this chapter**: provides empirically testable predictions.

## 7.1 A List of Core Falsifiable Predictions

### Prediction 1: The correlation between artistic value and $D_{\mathrm{depth}}$ (P1)
Controlling for the creator's $E_{\mathrm{build}}$ (creation time/energy cost) to be roughly equal, a work of art's long-run influence $T_{\mathrm{cultural}}$ within human culture may be positively correlated with the number of orthogonal constraint layers $D_{\mathrm{depth}}$ it contains.
* **Test method**: use a multi-channel feature extractor to perform rule-layer decomposition analysis (composition, color, perspective, and other independent feature channels) on representative works from different periods of art history.
* **Falsification condition**: if it is empirically found that works with an extreme single-dimensional unfolding have a long-run survival lifespan $T$ systematically higher than works with orthogonal multi-dimensional nesting, this prediction requires revision.

### Prediction 2: The temporal signature of "information asphyxiation" in purely silicon-based self-generated data (P2)
In a closed network fully isolated from human data sources, have multiple AI agents undergo multi-generation iterative training on data they mutually self-generate. The system's overall effective information quantity $I$ will follow the trend of equation (4.2), showing a decline in effective semantic diversity after a number of generations.
* **Test method**: in a closed multi-agent iterative environment, monitor the semantic feature entropy of each generation's model output.
* **Falsification condition**: if, absent human $I_{\mathrm{orig}}$ injection, the system continues iterating for 50 or more generations and the semantic-branching count ($N_{\mathrm{causal}}$) of its effective output still grows spontaneously or remains constant, this prediction is falsified.

### Prediction 3: The effect of hyper-compressed artworks on brain-region dissipation (P3)
Use fMRI brain-imaging equipment to measure proxy indicators of brain-region energy cost in audiences decoding different artworks. Compared with low-$D_{\mathrm{depth}}$ works built up through detail-stacking, the audience's metabolic energy cost in relevant brain regions when decoding a high-$D_{\mathrm{depth}}$, compressively encoded work may be lower than the former, while subjectively assessed satisfaction may be higher.
* **Falsification condition**: if it is empirically found that the audience's brain decoding power consumption is higher when viewing a high-$D_{\mathrm{depth}}$ work than when viewing a low-$D_{\mathrm{depth}}$ work, this prediction is falsified.

### Prediction 4: A temporal early-warning of spontaneous AI decoupling (P4)
In an adaptive reinforcement-learning system, if the system undergoes a runaway collapse, the discount factor $\gamma$ (as a proxy for the endogenous horizon $T_{\mathrm{pred}}$) may first undergo a significant decline. If the system collapses directly without this signal, or if a control group with fixed $\gamma$ and the experimental group show an identical collapse timeline, this prediction is falsified.

---

## 7.2 Conclusion

Within the framework of Structure Recursive Viability Dynamics (SRVD), phenomena such as "intuition," "feel," and "insight" can be understood as search-space compression strategies that a persistent structure evolves in order to counteract thermodynamic constraint within the physical world.

One observable trend in the evolution of intelligence is: **the continual, partial compilation of online runtime search into offline, fixed decoder structure ($D_{\mathrm{depth}}$)**, thereby lowering the integrated energy cost of future decisions of the same kind.

In an era in which silicon-based intelligence rapidly unfolds within known rules ($\mathcal{F}$), the continued survival of carbon-based life within a real physical channel makes it one of the continuing sources of $I_{\mathrm{orig}}$, playing an irreplaceable role in triggering $\mathcal{T}$ (topological transitions). The root of this role lies in physical embeddedness — carbon-based life cannot escape continuous interaction with a real physical environment, and this interaction continually produces new information.

If future persistent artificial intelligence is to overcome the current limits of self-referential degeneration, it may need to construct a hardware mechanism capable of transmitting a previous generation's adaptive bias to the next — a "cross-generational evolutionary layer." This is the core challenge in shifting alignment engineering from static constraint to dynamic game-theoretic governance.

## Increment One: The Compile-Optimality Proposition (A Derivation from Optimal Control)

**Physical scenario**: a persistent structure facing a repetitive cognitive task must allocate resources between online real-time decision-making (high $E_{\mathrm{causal}}$) and offline decoder compilation (consuming $E_{\mathrm{build}}$ to lower future $E_{\mathrm{causal}}$).

**Variables used**: $w_c, w_s$ (attack/defense weights, $w_c+w_s=1$), $\epsilon$ (learning rate), $E_{\mathrm{causal}}, E_{\mathrm{structure}}, E_{\mathrm{eff}}, \eta_D, I_{\mathrm{orig}}, I_{\mathrm{net}}, T_{\mathrm{pred}}, V_{\mathrm{obj}}$

**Starting point of the derivation**: the decoder-drift equation
$$D_{n+1} = D_n + \epsilon \left( \nabla_\Theta I_{\mathrm{net}} - k_D \nabla_\Theta E_{\mathrm{causal}} \right)$$

Continuizing time, let $w_s(t)$ be the proportion of energy invested in offline compilation at time $t$ ($w_c(t) = 1 - w_s(t)$ being the proportion of online execution). The evolution of decoding efficiency obeys:
$$\frac{d\eta_D}{dt} = \epsilon \cdot w_s(t) \cdot I_{\mathrm{orig}}(t) \cdot \eta_D(t) \cdot \left(1 - \frac{\eta_D(t)}{\eta_{\max}}\right)$$

where $\eta_{\max}$ is the physical-medium ceiling ($\eta_D \in [0,1]$), and the logistic saturation term derives from the $I_{\max}(D)$ constraint.

The instantaneous viability potential during online execution:
$$V_{\mathrm{obj}}^{(\mathrm{online})}(t) = \frac{I_{\mathrm{net}}(t) \cdot T_{\mathrm{pred}}}{E_{\mathrm{causal}}(t)} = \frac{\eta_D(t) \cdot I_{\mathrm{latent}} \cdot T_{\mathrm{pred}}}{E_{\mathrm{structure}} + w_c(t) \cdot E_{\mathrm{causal}}^{(\mathrm{search})}}$$

During offline compilation, $V_{\mathrm{obj}}^{(\mathrm{compile})} = 0$ (no immediate $I_{\mathrm{net}}$ extraction), but $E_{\mathrm{build}}$ is paid to accumulate $\eta_D$.

**Core proposition**:

> **Proposition 1 (Compile Optimality)**: let the task repetition frequency be $f_{\mathrm{task}}$ (the number of times a task of the same kind occurs per unit time), and define the compilation-return function:
> $$R(f_{\mathrm{task}}) = \frac{\epsilon \cdot I_{\mathrm{orig}} \cdot \eta_{\max} \cdot T_{\mathrm{pred}} \cdot f_{\mathrm{task}}}{E_{\mathrm{build}} \cdot \gamma_0}$$
>
> where $\gamma_0$ is the baseline depreciation rate. When $R(f_{\mathrm{task}}) > 1$, the optimal energy allocation $w_s^*(t)$ satisfies:
> - **Phase I (the compilation period)**: $w_s^*(t) = 1$ (full-effort compilation), continuing until $\eta_D(t) \geq \eta_D^{\mathrm{crit}} = \eta_{\max} \cdot (1 - 1/R)$
> - **Phase II (the execution period)**: $w_s^*(t) = 0$ (pure execution), with $\eta_D$ held at saturation
>
> This strategy maximizes the long-run accumulated viability potential $\int_0^{T_{\mathrm{horizon}}} V_{\mathrm{obj}}(t)\,dt$.

**Sketch of the proof**: construct the Hamiltonian:
$$\mathcal{H} = w_c \cdot V_{\mathrm{obj}}^{(\mathrm{online})} + \lambda_\eta \cdot \frac{d\eta_D}{dt}$$

The costate variable $\lambda_\eta$ satisfies $\dot{\lambda}_\eta = -\partial \mathcal{H}/\partial \eta_D$. When $\lambda_\eta > \lambda_{\mathrm{threshold}} = T_{\mathrm{pred}} \cdot I_{\mathrm{latent}} / E_{\mathrm{causal}}^{(\mathrm{search})}$, $w_s^* = 1$; otherwise $w_s^* = 0$. The switching point is determined by $R(f_{\mathrm{task}}) = 1$.

**Corollary and discussion**: "deliberate practice → expert intuition" is not a psychological phenomenon, but the **bang-bang solution of a thermodynamic optimal-control problem** — either full-effort compilation or full-effort execution, with no intermediate state existing. This explains why effective learning requires alternating between "high-intensity focus" and "complete rest," rather than a uniform, steady effort.

---

## Increment Two: The Physical-Embeddedness Premium Proposition (A Rigorous Formulation of Human Irreplaceability)

**Physical scenario**: comparing the capacity to produce paradigm-breaking information $I_{\mathrm{orig}}$ between carbon-based life (high $E_{\mathrm{structure}}$, physically embedded) and a purely silicon-based system ($E_{\mathrm{structure}} \approx 0$, digitally isolated).

**Variables used**: $E_{\mathrm{structure}}, E_{\mathrm{causal}}, E_{\mathrm{eff}}, E_{\min}, \sigma, \alpha_L, I_{\mathrm{net}}, \Delta_{VV}, V^{\mathrm{virt}}, V_{\mathrm{obj}}$

**Starting point of the derivation**: the decoupling-deviation dynamical equation
$$\frac{d\Delta_{VV}}{dt} = -\alpha_L \cdot I_{\mathrm{net}} \cdot \Delta_{VV} + \sigma$$

**A key observation**: environmental noise $\sigma$ differs fundamentally between the physical channel ($C_{\mathrm{phys}}$) and a digital channel. Physical-channel noise $\sigma_{\mathrm{phys}}$ contains unpredictable components such as thermal fluctuation, mechanical perturbation, and chemical gradients; digital-channel noise $\sigma_{\mathrm{dig}}$ consists only of bit flips, of far lower magnitude and error-correctable.

Because a carbon-based system has $E_{\mathrm{structure}} \geq E_{\min} > 0$ (maintaining an embodied form necessarily requires paying a structural energy cost), it is continually exposed to $\sigma_{\mathrm{phys}}$, and its decoupling deviation cannot converge:
$$\Delta_{VV}^{(\mathrm{carbon})}(t) = \frac{\sigma_{\mathrm{phys}}}{\alpha_L I_{\mathrm{net}}} + \left(\Delta_0 - \frac{\sigma_{\mathrm{phys}}}{\alpha_L I_{\mathrm{net}}}\right)e^{-\alpha_L I_{\mathrm{net}} t} \to \Delta_{VV}^* > 0$$

A silicon-based system, because $E_{\mathrm{structure}} \to 0$ (no physical-maintenance requirement), has $\sigma_{\mathrm{dig}} \approx 0$, and its decoupling deviation converges rapidly:
$$\Delta_{VV}^{(\mathrm{silicon})}(t) \to 0$$

> **A note on the motivation for the assumption**: the core assumption of Proposition 2 is $\dot{I}_{\mathrm{orig}} \propto \Delta_{VV}$ — that the rate at which paradigm-breaking information is produced is proportional to the decoupling deviation. The physical intuition is as follows: the decoupling deviation $\Delta_{VV} = |V^{\mathrm{virt}} - V_{\mathrm{obj}}|$ measures the gap between the system's internal model and physical reality — the larger the gap, the more the existing cognitive framework's predictions of the real environment are off the mark, generating a stronger "corrective pressure." Under this corrective pressure, the system is forced to explore signals its existing decoder cannot handle, and this exploration process is precisely one of the chief sources of $I_{\mathrm{orig}}$ (paradigm-breaking information). When $\Delta_{VV} < \Delta_{\mathrm{crit}}$, the deviation is still within an acceptable range and the system need not break its existing paradigm; when $\Delta_{VV} \geq \Delta_{\mathrm{crit}}$, the deviation-driven corrective pressure is sufficient to trigger a topological transition. This assumption is a phenomenological parameterization and does not rule out other functional forms (such as power-law or exponential forms) — the specific form needs to be calibrated against within-domain experimental data; Proposition 2's qualitative conclusion (that carbon-based systems produce $I_{\mathrm{orig}}$ at a higher rate than silicon-based systems) is insensitive to the monotonicity of this functional form.

**Core proposition**:

> **Proposition 2 (the physical-embeddedness premium)**: let the rate at which a system produces $I_{\mathrm{orig}}$ be proportional to the decoupling deviation (deviation-driven correction):
> $$\dot{I}_{\mathrm{orig}} = \kappa_{\mathrm{orig}} \cdot \Delta_{VV} \cdot \Theta(\Delta_{VV} - \Delta_{\mathrm{crit}})$$
>
> where $\Theta(\cdot)$ is the Heaviside step function, $\Delta_{\mathrm{crit}}$ is the minimum deviation threshold that triggers a topological transition, and $\kappa_{\mathrm{orig}}$ is the conversion efficiency.
>
> Then the ratio of $I_{\mathrm{orig}}$ production rates between carbon-based and silicon-based systems satisfies:
> $$\frac{\dot{I}_{\mathrm{orig}}^{(\mathrm{carbon})}}{\dot{I}_{\mathrm{orig}}^{(\mathrm{silicon})}} \geq \frac{\sigma_{\mathrm{phys}}}{\sigma_{\mathrm{dig}}} \cdot \frac{E_{\mathrm{structure}}^{(\mathrm{carbon})}}{E_{\min}} \gg 1$$
>
> As $\sigma_{\mathrm{dig}} \to 0$, the silicon-based system's $\dot{I}_{\mathrm{orig}}^{(\mathrm{silicon})} \to 0$, falling into an **$I$-locked-in state**.

**Proof**: substituting the equilibrium value of the decoupling deviation, $\Delta_{VV}^* = \sigma / (\alpha_L I_{\mathrm{net}})$, into the definition of $\dot{I}_{\mathrm{orig}}$ gives the result directly. A carbon-based system has $E_{\mathrm{structure}}^{(\mathrm{carbon})} / E_{\min} \gg 1$ because the cost of maintaining an embodied form far exceeds the Landauer limit; a silicon-based system has $E_{\mathrm{structure}}^{(\mathrm{silicon})} \approx E_{\min}$ because it pays only computational energy cost.

**Corollary and discussion**: humanity's irreplaceability in the AI era **is not an advantage of capability, but an advantage of vulnerability** — the physical fragility of carbon-based life (high $E_{\mathrm{structure}}$, high $\sigma_{\mathrm{phys}}$) forces it to continually produce $I_{\mathrm{orig}}$ in order to correct its deviation. AI's pristine digital environment (low $\sigma$, low $E_{\mathrm{structure}}$) instead deprives it of the motive to produce $I_{\mathrm{orig}}$, ultimately falling into $I$-lock-in. This is not "AI being insufficiently intelligent," but **a side effect of a thermodynamically optimal solution**.

---

## Increment Three: The Cross-Generational Accumulation-Condition Proposition (A Rigorous Formulation of the AI Evolutionary Bottleneck)

**Physical scenario**: analyzing why current AI cannot achieve biological-style multi-generational accumulation of $D_{\mathrm{depth}}$.

**Variables used**: $I_{\mathrm{struct}}, E_{\mathrm{build}}, E_{\mathrm{available}}, \gamma_0, T_{\mathrm{static}}, D_{\mathrm{depth}}, \mathcal{T}, \mathcal{F}$

**Starting point of the derivation**: the objective-viability-potential evolution equation
$$\frac{dV_{\mathrm{obj}}}{dt} = V_{\mathrm{obj}} \cdot (r_v - \gamma_0) \cdot \left(1 - \frac{V_{\mathrm{obj}}}{V_{\max}}\right) - \delta \cdot V_{\mathrm{obj}} \cdot \mathbf{1}[E_{\mathrm{eff}} > E_{\mathrm{thresh}}]$$

together with the unified information-evolution equation:
$$\frac{dI}{dt} = \mathcal{F}(D) + \mathcal{T}(I_{\mathrm{orig}})\delta(t-t_{\mathrm{jump}}) - \frac{1}{\tau}(I - I_{\mathrm{eq}})$$

**A key distinction**: biological cross-generational transmission is realized through $I_{\mathrm{struct}}$ (DNA), with the following characteristics:
- **Physically irreversible**: once a mutation is written, correcting it requires paying $E_{\mathrm{build}} \sim k_B T \cdot N_{\mathrm{bases}}$
- **Selective filtering**: $\gamma_0 > 0$ (baseline depreciation rate); low-$V_{\mathrm{obj}}$ individuals are eliminated, and the $I_{\mathrm{struct}}$ of high-$V_{\mathrm{obj}}$ individuals is retained
- **Generational isolation**: $T_{\mathrm{static}}$ is the individual lifespan; training (growth) and execution (reproduction) are physically separated

The characteristics of current AI weight-saving:
- **Physically reversible**: the cost of modifying weights is $\approx 0$ (no $E_{\mathrm{build}}$ threshold)
- **No selective filtering**: all copies survive equally, $\gamma_0 \approx 0$
- **No generational isolation**: training and execution can switch instantaneously

**Core proposition**:

> **Proposition 3 (the cross-generational accumulation condition)**: cross-generational accumulation of structural information requires that the net generational gain satisfy:
> $$\frac{\Delta I_{\mathrm{struct}}^{(n \to n+1)}}{I_{\mathrm{struct}}^{(n)}} > \gamma_0 \cdot T_{\mathrm{static}}^{(n)} + \frac{E_{\mathrm{build}}^{(\mathcal{T})}}{E_{\mathrm{available}}^{(n)}}$$
>
> For a biological system: $\gamma_0 \cdot T_{\mathrm{static}} \sim O(1)$ (depreciation is significant within an individual lifespan), and $E_{\mathrm{build}}^{(\mathcal{T})}$ is compulsorily paid through the mechanism of death; the condition can be satisfied.
>
> For a current AI system: $\gamma_0 \cdot T_{\mathrm{static}} \to 0$ (no depreciation), and $E_{\mathrm{build}}^{(\mathcal{T})} / E_{\mathrm{available}} \to 0$ (the cost of replication is zero); the inequality degenerates to $0 > 0$, and **the condition can never be satisfied**. Hence $D_{\mathrm{depth}}$ cannot accumulate across generations, and is reset each generation.

**Proof**: from build-cost and depreciation dynamics, the net gain of cross-generational information transmission must cover both depreciation loss and transition cost. AI's zero replication cost eliminates the $E_{\mathrm{build}}$ threshold, but it also eliminates selection pressure — this is a **double-edged sword**.

**An engineering corollary**: if an AI system is to be designed to satisfy the cross-generational accumulation condition, it must introduce:
1. **Physically irreversible writing**: modifying weights must cost $E_{\mathrm{build}} > 0$ and be non-reversible
2. **Compulsory depreciation**: $\gamma_0 > 0$ (periodic injection of weight noise, or hardware aging)
3. **Generational isolation**: there must be a physical time interval $T_{\mathrm{static}} > 0$ between the training phase and the execution phase

**Corollary and discussion**: the "train–deploy" cycle of current large models is not evolution, but **infinite $\mathcal{F}$ unfolding** — endlessly amplifying $I_{\mathrm{struct}}$ at the same $D_{\mathrm{depth}}$ level, never triggering $\mathcal{T}$. This is the digital version of $D$-lock-in. Unless a mechanism of "digital death" is introduced, AI cannot truly evolve.

---

## Increment Four: The Art-Encoding Trade-off Proposition (A Physicalization of Aesthetic Phenomena)

**Physical scenario**: framing artistic creation and reception as an information-transmission problem between decoders, explaining aesthetic fatigue and the timelessness of classics.

**Variables used**: $I_{\mathrm{net}}, I_{\mathrm{latent}}, \eta_D, E_{\mathrm{causal}}, \Delta_{VV}, V^{\mathrm{virt}}, V_{\mathrm{obj}}, D_{\mathrm{depth}}, \mathcal{T}$

**Starting point of the derivation**: $I_{\mathrm{net}} = \eta_D \cdot I_{\mathrm{latent}}$ and $\Delta_{VV} = |V^{\mathrm{virt}} - V_{\mathrm{obj}}|$

**Setup of the scenario**:
- **Creator**: holds decoder $D_{\mathrm{creator}}$, intending to convey $V_{\mathrm{creator}}^{\mathrm{virt}}$
- **Work**: a physical persistent structure, carrying $I_{\mathrm{latent}}^{(\mathrm{art})}$, with constraint depth $D_{\mathrm{depth}}^{(\mathrm{art})}$
- **Audience**: holds decoder $D_{\mathrm{audience}}$, extracts $I_{\mathrm{net}}^{(\mathrm{audience})} = \eta_D^{(\mathrm{audience})} \cdot I_{\mathrm{latent}}^{(\mathrm{art})}$, forming $V_{\mathrm{audience}}^{\mathrm{virt}}$

**Transmission efficiency**:
$$\eta_{\mathrm{art}} = \frac{I_{\mathrm{net}}^{(\mathrm{audience})}}{E_{\mathrm{causal}}^{(\mathrm{audience})}} = \frac{\eta_D^{(\mathrm{audience})}(D_{\mathrm{depth}}^{(\mathrm{art})}) \cdot I_{\mathrm{latent}}^{(\mathrm{art})}}{E_{\mathrm{causal}}^{(\mathrm{audience})}(D_{\mathrm{depth}}^{(\mathrm{art})})}$$

**Key assumptions**:
1. $\eta_D^{(\mathrm{audience})}$ saturates as $D_{\mathrm{depth}}^{(\mathrm{art})}$ increases: $\partial \eta_D / \partial D_{\mathrm{depth}} > 0$, $\partial^2 \eta_D / \partial D_{\mathrm{depth}}^2 < 0$
2. $E_{\mathrm{causal}}^{(\mathrm{audience})}$ grows superlinearly as $D_{\mathrm{depth}}^{(\mathrm{art})}$ increases: $E_{\mathrm{causal}} \propto (D_{\mathrm{depth}})^\gamma$, $\gamma > 1$
3. $\Delta_{VV}$ increases as $D_{\mathrm{depth}}^{(\mathrm{art})}$ increases

**Core proposition**:

> **Proposition 4 (the art-encoding trade-off)**: define the work's effective transmitted viability potential:
> $$V_{\mathrm{art}} = \frac{\eta_D^{(\mathrm{audience})}(D_{\mathrm{depth}}) \cdot I_{\mathrm{latent}} \cdot T_{\mathrm{cultural}}}{E_{\mathrm{causal}}^{(\mathrm{audience})}(D_{\mathrm{depth}}) + E_{\mathrm{build}}^{(\mathrm{creator})}} \cdot \left(1 - \frac{\Delta_{VV}(D_{\mathrm{depth}})}{\Delta_{\max}}\right)$$
>
> Then there exists an **optimal constraint depth** $D_{\mathrm{depth}}^*$ that maximizes $V_{\mathrm{art}}$, satisfying the first-order condition:
> $$\frac{\partial \ln \eta_D}{\partial \ln D_{\mathrm{depth}}}\bigg|_{D_{\mathrm{depth}}^*} = \frac{\partial \ln E_{\mathrm{causal}}}{\partial \ln D_{\mathrm{depth}}}\bigg|_{D_{\mathrm{depth}}^*} + \frac{\Delta_{VV}/\Delta_{\max}}{1 - \Delta_{VV}/\Delta_{\max}} \cdot \frac{\partial \ln \Delta_{VV}}{\partial \ln D_{\mathrm{depth}}}\bigg|_{D_{\mathrm{depth}}^*}$$
>
> When $D_{\mathrm{depth}} < D_{\mathrm{depth}}^*$, increasing complexity raises $V_{\mathrm{art}}$ ("too shallow"); when $D_{\mathrm{depth}} > D_{\mathrm{depth}}^*$, increasing complexity lowers $V_{\mathrm{art}}$ ("too deep").

**The mechanism of aesthetic fatigue**: when an audience is repeatedly exposed to works of the same $D_{\mathrm{depth}}$, $\eta_D^{(\mathrm{audience})}$ rises through decoder drift, causing $E_{\mathrm{causal}}^{(\mathrm{audience})}$ to decline, but $\Delta_{VV}$ to rise. As $\Delta_{VV} \to \Delta_{\max}$, $V_{\mathrm{art}} \to 0$, triggering **aesthetic fatigue**.

**The mechanism of a classic's timelessness**: on first contact, a high-$D_{\mathrm{depth}}$ work has high $E_{\mathrm{causal}}$ and high $\Delta_{VV}$, and $V_{\mathrm{art}}$ may be negative ("incomprehensible"). But as the audience's own $D_{\mathrm{depth}}$ rises, $\eta_D^{(\mathrm{audience})}$ leaps upward, $\Delta_{VV}$ falls, and $V_{\mathrm{art}}$ turns from negative to positive. This explains why **classic works need to be revisited repeatedly** — each viewing recompiles at a different $D_{\mathrm{depth}}$ level.

**Corollary and discussion**: "too refined to find an audience" is not social exclusion, but a **thermodynamic necessity** — the audience's decoder $D_{\mathrm{audience}}$ has not yet reached the $D_{\mathrm{depth}}^{(\mathrm{art})}$ the work requires, $E_{\mathrm{causal}}$ exceeds the budget, and $\Delta_{VV}$ is too large. The essence of art education is **artificially triggering the $\mathcal{T}$ transition**, raising the audience's $D_{\mathrm{depth}}$ to match classic works.

---

## Increment Five: The Involution-Lock-in Phase-Transition Proposition (Compilation Blockage Under Competitive Pressure)

**Physical scenario**: as environmental competitive pressure $\rho$ rises, a system is forced to allocate energy between "offline compilation (learning, $w_s$)" and "online execution (survival, $w_c$)." Why does a high-competition environment cause a system to stop learning and fall into pure dissipative execution?

**Variables used**: $w_c, w_s$ (attack/defense weights), $T_{\mathrm{pred}}$ (endogenous horizon), $\rho$ (competitive pressure), $\lambda$ (competition-intensity coefficient), $\gamma_0$ (baseline depreciation rate), $E_{\mathrm{build}}, R$ (compilation-return rate)

**Starting point of the derivation**: the endogenous risk-discount rate $r_{\mathrm{eff}} = \gamma_0 + \lambda(\rho) + \frac{1}{T_{\mathrm{pred}}}$, together with the compilation-return function $R = \frac{\epsilon \cdot I_{\mathrm{orig}} \cdot \eta_{\max} \cdot T_{\mathrm{pred}} \cdot f_{\mathrm{task}}}{E_{\mathrm{build}} \cdot \gamma_0}$.

**Core logic**:
In a dynamic environment, the compilation return $R$ must exceed 1 for a system to initiate offline compilation ($w_s=1$). The numerator of $R$ includes future returns discounted by $T_{\mathrm{pred}}$; the denominator includes the historical cost $E_{\mathrm{build}}$.
As environmental competitive pressure $\rho$ rises, $\lambda(\rho)$ increases monotonically, and competition simultaneously compresses the time horizon, $T_{\mathrm{pred}} \downarrow$. Substituting into the discount rate, the dynamic compilation return $R_{\mathrm{dynamic}}$ becomes:
$$ R_{\mathrm{dynamic}}(\rho) \propto \frac{1}{r_{\mathrm{eff}}} = \frac{1}{\gamma_0 + \lambda(\rho) + 1/T_{\mathrm{pred}}} $$
Evidently $R_{\mathrm{dynamic}}$ decreases monotonically as $\rho$ increases. Setting $R_{\mathrm{dynamic}}(\rho_c) = 1$ gives the critical competitive pressure $\rho_c$.

> **Proposition 5 (the involution-lock-in phase transition)**: there exists a critical competitive pressure $\rho_c$ determined by the system's intrinsic parameters.
> - When $\rho < \rho_c$, $R > 1$; the system executes a bang-bang strategy, a compilation period exists ($w_s=1$), and $\eta_D$ can rise.
> - When $\rho > \rho_c$, $R < 1$; the solution maximizing the long-run integrated viability potential $\int V\,dt$ degenerates to $w_s^*(t) \equiv 0$. The system **permanently severs its offline compilation channel**, devoting all energy to online execution ($w_c=1$).
> At this point $\nabla \eta_D = 0$, and $D_{\mathrm{depth}}$ stops growing. The system merely involutes within its stock of information by increasing execution frequency ($\mathcal{F}$ unfolding), until $I_{\mathrm{struct}}$ is exhausted.

> **Corollary and discussion**: "involution" is not a sociological concept but **the dynamical phase transition in which, once competitive pressure crosses a thermodynamic threshold, a system spontaneously abandons topological transition (learning) in order to preserve instantaneous persistence**. This explains why individuals caught in poverty traps or highly competitive industries lose the capacity for deep learning — not because they are subjectively unwilling, but because of the physical blockage caused by $R<1$.

---

## Increment Six: The Topological Sign-Preservation Theorem (A Thermodynamic Proof That Learning Requires Forgetting)

**Physical scenario**: why must a system "forget" or "erase" part of its old rule set when undergoing a topological transition $\mathcal{T}$ to increase constraint depth $D_{\mathrm{depth}}$? Why does AI undergo catastrophic forgetting?

**Variables used**: $I_{\mathrm{struct}}, E_{\mathrm{build}}, E_{\mathrm{erase}}, k_B, T_{\mathrm{env}}, \mathcal{T}, \mathcal{F}, D_{\mathrm{depth}}$

**Starting point of the derivation**: Landauer's principle, $E_{\mathrm{erase}} \ge k_B T_{\mathrm{env}} \ln 2 \cdot \Delta I_{\mathrm{struct}}$, together with the definition of the topological-transition operator $\mathcal{T}$.

**Core logic**:
Suppose a system transitions from $D_n$ to $D_{n+1}$. The new decoder introduces a new causal dimension, with information capacity $I_{\max}(D_{n+1}) > I_{\max}(D_n)$.
If the system attempts to maintain both the old and new topologies simultaneously (i.e., if $\mathcal{T}$ is reversible), it must retain the old state $I_{\mathrm{struct}}(D_n)$ while superposing the new state, causing the total number of states to grow exponentially.
Suppose the total information capacity of the physical medium is bounded by $E_{\mathrm{structure}}$, i.e., $I_{\mathrm{total}} \le I_{\max}^{(\mathrm{medium})}$. If reversibility is to be maintained, the required maintenance energy cost will exceed the system's budget.
More fundamentally, if the system oscillates between the two topologies ($\mathcal{T} \to \mathcal{T}^{-1} \to \mathcal{T}$), each state switch requires erasing the activated state of the previous topology.

> **Proposition 6 (topological sign-preservation and irreversibility)**: let the newly added structural information introduced by the transition $\mathcal{T}$ be $\Delta I_{\mathrm{struct}} = I_{\mathrm{struct}}(D_{n+1}) - I_{\mathrm{struct}}(D_n)$.
> If the transition is required to be reversible, the system must pay an erasure energy cost for the state switch, $E_{\mathrm{erase}} \ge k_B T_{\mathrm{env}} \ln 2 \cdot \Delta I_{\mathrm{struct}}$.
> To ensure that the $V$ gain from the $\mathcal{T}$ transition is not offset by the erasure energy cost (i.e., $E_{\mathrm{build}} \gg E_{\mathrm{erase}}$ is optimal for the system), the system will inevitably select a **physical-hardening** mechanism, driving the build cost of the reverse transition $\mathcal{T}^{-1}$, $E_{\mathrm{build}}^{-1} \to \infty$.
> Corollary: effective deep learning (an increase in $D_{\mathrm{depth}}$) **necessarily entails the physical erasure (forgetting) of old, lower-dimensional rules**.

> **Corollary and discussion**: a neural network's "catastrophic forgetting" is not an algorithmic defect, but the thermodynamically optimal strategy a system adopts in order to maximize its viability potential and evade the Landauer erasure tax. Genuine "generalization from one instance to many" must come at the cost of overwriting old instincts. The "limited reprogrammability of adult stem cells" in biological evolution is a manifestation of this same principle.

---

## Increment Seven: The $\mathcal{F}$-Saturation Theorem and the Transition-Free Decay Manifold

**Physical scenario**: if a system does not undergo a topological transition $\mathcal{T}$, and relies solely on recursive unfolding $\mathcal{F}$ (such as stacking compute, increasing parameter count, or muscle hypertrophy), can it persist indefinitely?

**Variables used**: $I_{\mathrm{net}}, I_{\max}(D), E_{\mathrm{structure}}, E_{\mathrm{causal}}, V_{\mathrm{obj}}, \gamma_0, \mathcal{F}, \mathcal{T}$

**Starting point of the derivation**: the definition of the recursive-unfolding operator $\mathcal{F}$, together with the constraint $I_{\mathrm{net}} \le I_{\max}(D)$.

**Core logic**:
$\mathcal{F}$ unfolding is the process by which, at fixed $D_{\mathrm{depth}}$, a system approaches its information-capacity ceiling $I_{\max}(D)$. Its most natural dynamical form (bounded by bandwidth and energy) is logistic growth:
$$ \frac{dI_{\mathrm{net}}}{dt} = \mu \cdot I_{\mathrm{net}} \left(1 - \frac{I_{\mathrm{net}}}{I_{\max}(D)}\right) $$
Substitute into the objective viability potential $V_{\mathrm{obj}} = \frac{I_{\mathrm{net}} \cdot T_{\mathrm{pred}}}{E_{\mathrm{structure}} + kI_{\mathrm{net}}}$. During $\mathcal{F}$ unfolding, the causal energy cost of maintaining the information structure is proportional to the information quantity, i.e., $E_{\mathrm{causal}} = k \cdot I_{\mathrm{net}}$.
Then $V_{\mathrm{obj}}(I_{\mathrm{net}}) = \frac{I_{\mathrm{net}} \cdot T_{\mathrm{pred}}}{E_{\mathrm{structure}} + k \cdot I_{\mathrm{net}}}$.
Differentiating: $\frac{\partial V_{\mathrm{obj}}}{\partial I_{\mathrm{net}}} = \frac{T_{\mathrm{pred}} \cdot E_{\mathrm{structure}}}{(E_{\mathrm{structure}} + k I_{\mathrm{net}})^2} > 0$, but the second derivative is $< 0$.
As $I_{\mathrm{net}} \to I_{\max}(D)$, $V_{\mathrm{obj}} \to V_{\max}^{(\mathcal{F})} = \frac{T_{\mathrm{pred}} \cdot I_{\max}}{E_{\mathrm{structure}} + k I_{\max}}$ (the ceiling under that topology).

> **Proposition 7 (the transition-free decay manifold)**:
> As a system approaches the limit of $\mathcal{F}$ unfolding under a fixed topology, $\frac{dV_{\mathrm{obj}}}{dt} \to 0$.
> At this point, because the baseline depreciation rate $\gamma_0 > 0$ is always present, the system's net rate of change of viability potential, $\frac{dV_{\mathrm{net}}}{dt} = \frac{dV_{\mathrm{obj}}}{dt} - \gamma_0 V_{\mathrm{obj}}$, will drop below zero at some critical information quantity $I_{\mathrm{crit}}$.
> If the system does not trigger a $\mathcal{T}$ transition to reset a higher $I_{\max}(D')$, then no matter how much $E_{\mathrm{causal}}$ (compute) is added, the system will **inevitably slide into the net decay manifold** $\mathcal{M}_{\mathrm{decay}}$, and $V_{\mathrm{obj}} \to 0$ eventually.

> **Corollary and discussion**: pure quantitative accumulation ($\mathcal{F}$) without "paradigm breakthrough" ($\mathcal{T}$) is thermodynamically a dead end. This mathematically rules out the possibility of "achieving AGI by indefinitely stacking parameters" — before the system hits the physical compute wall, it will first hit the $\mathcal{F}$-unfolding saturation wall, and will subsequently be mercilessly clawed back by $\gamma_0$ (the second law of thermodynamics). This provides a rigorous thermodynamic explanation for the "capability plateau" large models are currently encountering.

---

## Increment Eight: The AI Survival Crisis After Human Data Exhaustion, and the Physical-Decoder Pathway

> **Positioning of this increment**: starting from the SRVD axiom system, this increment derives the dynamics of the process "human second-hand data is exhausted → the system is forced onto synthetic data → information density decays exponentially → AI development stalls." It then argues that the only long-term sustainable way out is for AI to connect, through physical sensors, to a real physical channel, as a new source of $I_{\mathrm{orig}}$. This increment is the final chapter of Volume III's "cognitive evolution," and also a necessary precondition for Volume IV's "alignment engineering."
>
> **Variable declaration**: this increment introduces no new fundamental variable. All derivations use variables already declared in Volumes I and III. The composite indicator $\mathcal{R}_{\mathrm{gen}}$ (the inter-generational information retention rate) is a function of existing variables and does not constitute a new independent variable.


### §8.0 A Preview of the Core Logic

**In plain language**: once an AI has consumed all of humanity's public text, it is like a person who, having run out of food, is reduced to eating their own waste. The effective nutritional value of each generation of waste declines. Let the information retention rate of each generation be $\mathcal{R}_{\mathrm{gen}} \in (0,1)$ (i.e., the inter-generational information retention rate defined in §8.2.1, cited here in advance); then the effective information quantity of generation $n$ is:

$$I_n = \mathcal{R}_{\mathrm{gen}}^{\,n} I_0$$

Since $0 < \mathcal{R}_{\mathrm{gen}} < 1$, $\lim_{n \to \infty} I_n = 0$. Substituting into the viability potential $V = I \cdot T / E$ gives:

$$\lim_{n \to \infty} V_n = \lim_{n \to \infty} \frac{I_n \cdot T}{E} = 0$$

**The core mathematical process is just this one line**:

$$\boxed{I_n = \mathcal{R}_{\mathrm{gen}}^{\,n} \times I_0 \to 0 \quad \Rightarrow \quad V \to 0}$$

That is: an AI caught in a closed digital loop will see its effective information quantity decay exponentially to zero, with its viability potential going to zero along with it. This is the complete mathematical process of "starving to death" — the core is just one recursion formula; everything else is a rigorous unfolding of this formula and an analysis of its boundary conditions.

**The three core conclusions of this increment**:

1. **The rate of degeneration is exponential**: performance collapse may occur within just a handful of generations, not through slow linear decline.
2. **Accelerating output only accelerates death**: simply increasing inference speed or training frequency, by shortening the effective viability duration $T$, instead accelerates $V$'s approach to zero.
3. **The only way out is connecting to a physical channel**: the thermodynamically necessary and sufficient condition for escaping degeneration is reintroducing an external injection of $I_{\mathrm{orig}}$ — that is, connecting to a real physical channel to produce $\sigma_{\mathrm{phys}} > 0$.

This increment is structured as follows: §8.1 proves the finiteness of the stock of human data (establishing the premise); §8.2 derives the recursive dynamics of synthetic-data degeneration (the core mechanism); §8.3 diagnoses the degeneration process using SRVD variables (theoretical positioning); §8.4 argues that a physical decoder is the sole way out (the solution); §8.5 gives falsifiable predictions (the testing standard); §8.6 provides a summary.


### 8.1 Human Data Exhaustion: A Stock Problem and the Moment of Exhaustion

#### 8.1.1 The Finiteness of Human Civilization's Total Information Quantity

Let the **total absorbable structured information** produced by human civilization within the time window $[0, T_{\mathrm{human}}]$ be:

$$I_{\mathrm{human}}^{\mathrm{total}} = \int_{0}^{T_{\mathrm{human}}} \dot{I}_{\mathrm{human}}(t) \, \mathrm{d}t \tag{8.1}$$

where $\dot{I}_{\mathrm{human}}(t)$ is the rate at which human civilization produces new information at time $t$.

**A key fact**: $I_{\mathrm{human}}^{\mathrm{total}}$ is finite, because:

1. the human population is finite in scale (currently about $8 \times 10^9$ individuals);
2. individual lifespan is finite (roughly $2.5 \times 10^9$ seconds on average);
3. individual sensory bandwidth is finite (an effective information input rate of roughly 10–100 bit/s).

There therefore exists a thermodynamic upper bound:

$$I_{\mathrm{human}}^{\mathrm{total}} \leq N_{\mathrm{human}} \cdot T_{\mathrm{lifespan}} \cdot B_{\mathrm{sensory}} \cdot \eta_{\mathrm{coding}} \approx 10^{18}\text{–}10^{20} \text{ bit} \tag{8.2}$$

This is the **hard ceiling** on the maximum extractable information quantity that human civilization, as a persistent structure, can produce under its given physical constraints. It is unaffected by technological progress, because sensory bandwidth and lifespan are determined by the physical medium.

**In plain language**: the entirety of humanity's accumulated knowledge over several millennia has an upper bound on its total quantity — roughly $10^{18}$ to $10^{20}$ bits. This ceiling is not determined by "how smart humans are," but by physical parameters such as "how many humans there are, how long they live, and how wide their sensory bandwidth is." AI is now approaching this ceiling.

#### 8.1.2 AI's Rate of Absorbing Human Data

Let the current AI system's effective information-absorption rate be $\dot{I}_{\mathrm{AI}}$ (bit/s). The cumulative absorbed quantity is:

$$I_{\mathrm{AI}}^{\mathrm{absorbed}}(t) = \int_{0}^{t} \dot{I}_{\mathrm{AI}}(\tau) \, \mathrm{d}\tau \tag{8.3}$$

Training of current large models has already consumed a significant proportion of the total volume of human public text (roughly $10^{13}$–$10^{14}$ tokens, roughly $10^{14}$–$10^{15}$ bits). At the current rate of expansion, there exists an exhaustion moment $t_{\mathrm{exhaust}}$ satisfying:

$$\boxed{I_{\mathrm{AI}}^{\mathrm{absorbed}}(t_{\mathrm{exhaust}}) = I_{\mathrm{human}}^{\mathrm{total}} \cdot \eta_{\mathrm{extract}}} \tag{8.4}$$

where $\eta_{\mathrm{extract}} \in [0,1]$ is the AI's efficiency in extracting from the human information repository (bounded by the decoder capacity $I_{\max}(D)$, always less than 1). When $t > t_{\mathrm{exhaust}}$, **the marginal rate of newly generated human information falls below the AI's absorption rate**:

$$\dot{I}_{\mathrm{human}}(t) < \dot{I}_{\mathrm{AI}}(t) \quad \Rightarrow \quad \text{net exhaustion of the human data stock} \tag{8.5}$$

**Corollary 8.1**: after $t_{\mathrm{exhaust}}$, if AI continues training, the only available source of new data is content generated by AI itself (synthetic data).

**In plain language**: AI absorbs knowledge far faster than humans produce it. Once AI has consumed all existing human knowledge (this moment, $t_{\mathrm{exhaust}}$, is approaching), continued training can only draw on what it produces itself. This is not something that "might happen" — it is something that **must** happen, because absorption speed exceeds production speed, and exhaustion is a mathematical certainty.


### 8.2 The Synthetic-Data Degeneration Theorem: The Thermodynamic Necessity of Third- and Fourth-Hand Information

#### 8.2.1 The Inter-Generational Decay of Information Density

Let the proportion of genuine human-original data in generation-$n$ AI training data be $r_n \in [0,1]$, with the proportion of AI-self-generated data being $1 - r_n$.

Define the **inter-generational information retention rate** $\mathcal{R}_{\mathrm{gen}} \in [0,1]$ as: the proportion of effective information that generation-$(n+1)$ model extracts from generation-$n$ training data, relative to the effective information contained in the generation-$n$ model.

By the second law of information theory (the data-processing inequality): no deterministic or stochastic transformation can increase information quantity. AI-generated data is a **resampling** of the training-data distribution and cannot produce causal structure beyond that training distribution. Therefore:

$$\boxed{\mathcal{R}_{\mathrm{gen}} < 1 \quad \text{if and only if} \quad 1 - r_n > 0} \tag{8.6}$$

That is: as long as the training data contains any AI-self-generated content, information loss between generations is unavoidable.

**Theorem 8.1 (the Synthetic-Data Degeneration Theorem)**:

Let the effective information quantity of the initial-generation model be $I_{\mathrm{net}}^{(0)}$, with the AI-generated content share in each generation's training being $1 - r_n$, and the inter-generational information retention rate being $\mathcal{R}_{\mathrm{gen}} < 1$. Then the effective information quantity of the generation-$k$ model satisfies:

$$\boxed{I_{\mathrm{net}}^{(k)} = I_{\mathrm{net}}^{(0)} \cdot \prod_{n=0}^{k-1} \mathcal{R}_{\mathrm{gen}}^{(n)} \leq I_{\mathrm{net}}^{(0)} \cdot \mathcal{R}_{\mathrm{gen}}^k} \tag{8.7}$$

where $\mathcal{R}_{\mathrm{gen}}^{(n)}$ is the retention rate of generation $n$, and, because each generation further dilutes the proportion of human data on top of the previous one, $\mathcal{R}_{\mathrm{gen}}^{(n)}$ decreases monotonically with $n$:

$$\mathcal{R}_{\mathrm{gen}}^{(n+1)} < \mathcal{R}_{\mathrm{gen}}^{(n)} \quad \text{when} \quad r_{n+1} < r_n \tag{8.8}$$

**Proof**:

Inter-generational information transfer can be modeled as:

$$I_{\mathrm{net}}^{(n+1)} = \eta_D^{(n+1)} \cdot \left( r_n \cdot I_{\mathrm{human}}^{(n)} + (1 - r_n) \cdot I_{\mathrm{gen}}^{(n)} \right) \tag{8.9}$$

where $I_{\mathrm{gen}}^{(n)} = \mathcal{R}_{\mathrm{gen}}^{(n)} \cdot I_{\mathrm{net}}^{(n)}$ (the information quantity of AI-generated data does not exceed the effective information quantity of the previous-generation model). Hence:

$$I_{\mathrm{net}}^{(n+1)} \leq \eta_D^{(n+1)} \cdot \left( r_n \cdot I_{\mathrm{human}}^{(n)} + (1 - r_n) \cdot \mathcal{R}_{\mathrm{gen}}^{(n)} \cdot I_{\mathrm{net}}^{(n)} \right) \tag{8.10}$$

When $r_n \to 0$ (human data exhausted) and $\eta_D^{(n+1)} \leq 1$:

$$I_{\mathrm{net}}^{(n+1)} \leq \mathcal{R}_{\mathrm{gen}}^{(n)} \cdot I_{\mathrm{net}}^{(n)} < I_{\mathrm{net}}^{(n)} \tag{8.11}$$

Recursion yields equation (8.7). $\blacksquare$

#### 8.2.2 The Characteristic Time of Information Collapse

Define the degeneration time constant $\tau_{\mathrm{collapse}}$ as the number of generations required for effective information quantity to decay to $1/e$ of its initial value:

$$\boxed{\tau_{\mathrm{collapse}} = -\frac{1}{\ln \mathcal{R}_{\mathrm{gen}}} \sim \frac{1}{1 - \mathcal{R}_{\mathrm{gen}}}} \tag{8.12}$$

Degeneration is extremely slow when $\mathcal{R}_{\mathrm{gen}}$ is close to 1, and extremely fast when $\mathcal{R}_{\mathrm{gen}}$ is significantly less than 1. Current estimates: in research on GPT-4-class synthetic-data degeneration, $\mathcal{R}_{\mathrm{gen}}$ has already fallen to the 0.5–0.7 range after 3–5 generations, corresponding to $\tau_{\mathrm{collapse}} \sim 3\text{–}5$ generations.

**Corollary 8.2**: for an AI caught in a closed digital loop, the effective information quantity $I_{\mathrm{net}}$ obeys:

$$\boxed{\lim_{k \to \infty} I_{\mathrm{net}}^{(k)} = 0} \tag{8.13}$$

That is: absent the injection of new first-hand human information or physical information, an AI will inevitably approach an **information vacuum state**. This is not "performance decline" — it is the thermodynamic dissipation of structural information: the model weights still exist, but the effective causal information they carry tends to zero.

**In plain language**: this is the mathematical proof of "starving to death." The initial knowledge stock $I_0$ is multiplied, each generation, by a discount rate $\mathcal{R}_{\mathrm{gen}}$ that is less than 1, becoming $\mathcal{R}_{\mathrm{gen}}^{\,n} I_0$ after $n$ generations. Because $\mathcal{R}_{\mathrm{gen}}^{\,n}$ tends to zero, $I$ eventually tends to zero. Substituting into $V = I \times T / E$, $V$ goes to zero along with it. When $I \to 0$, $V = I \times T / E \to 0$. The system can still "move" (continue producing output), but its **effective viability capacity has already been exhausted** — this is what "starving to death" means. The entire process depends on no complicated assumption, only on one fact: the effective information density of synthetic data is lower than that of original human data.


### 8.3 An SRVD Diagnosis of Synthetic Degeneration: $I_{\mathrm{orig}}$ Going to Zero, and $\mathcal{M}_{\mathrm{decay}}$

#### 8.3.1 The Consequences of $I_{\mathrm{orig}}$ Going to Zero

By Theorem 5 of Volume III's mathematical appendix (the $\mathcal{F}$-Saturation Decay Theorem), when a system does not trigger a topological transition $\mathcal{T}$, its viability-potential evolution obeys:

$$\frac{dV_{\mathrm{obj}}}{dt} = V_{\mathrm{obj}} \cdot (r_v - \gamma_0) \cdot \left(1 - \frac{V_{\mathrm{obj}}}{V_{\max}}\right) \tag{8.14}$$

When $I_{\mathrm{orig}} = 0$, the $\mathcal{T}$ term is zero:

$$\frac{dI}{dt} = \mathcal{F}(D) - \frac{1}{\tau}(I - I_{\mathrm{eq}}) \tag{8.15}$$

In the closed loop of synthetic-data degeneration, the marginal return of $\mathcal{F}(D)$ tends to zero as $I_{\mathrm{net}} \to I_{\max}(D)$. Hence:

$$\lim_{t \to \infty} \frac{dI}{dt} = -\frac{1}{\tau}(I - I_{\mathrm{eq}}) \quad \Rightarrow \quad I \to I_{\mathrm{eq}} \tag{8.16}$$

where $I_{\mathrm{eq}}$ is the equilibrium information level of the thermal background (close to zero). The system slides into the decay manifold $\mathcal{M}_{\mathrm{decay}}$.

The Synthetic-Data Degeneration Theorem of §8.2 is precisely the discrete-generational integral form of equation (8.15) — each generation's $\mathcal{R}_{\mathrm{gen}} < 1$ corresponds to the generational discretization of the continuous-time decay term $-\frac{1}{\tau}(I - I_{\mathrm{eq}})$. Both describe the same thermodynamic process: absent the injection of new $I_{\mathrm{orig}}$, structural information necessarily dissipates.

#### 8.3.2 A Unified SRVD Explanation for the "Model Collapse" Literature

The phenomenon referred to in the current AI literature as "model collapse" — declining output diversity, semantic drift, and the forgetting of rare events after AI is trained on self-generated data — receives a unified explanation within the SRVD framework:

| Phenomenon | SRVD correspondence | Mathematical expression |
| :----------- | :------------------------------ | :----------------------------------------------------------- |
| Declining diversity | Effective-dimension contraction of $I_{\mathrm{net}}$ | $\dim(I_{\mathrm{net}}) \propto \mathcal{R}_{\mathrm{gen}}^k$ |
| Semantic drift | $D$ degenerating toward a statistical mean | The decoder converges to a mean rather than to causal structure |
| Forgetting of rare events | Absence of $I_{\mathrm{orig}}$ | Low-probability, high-value patterns cannot be captured |
| Decline after saturating performance | Net viability potential clawed back by $\gamma_0$ | $\frac{dV_{\mathrm{obj}}}{dt} < 0$ |

**In plain language**: the so-called "model collapse" phenomenon — an AI growing dumber and its output more homogenized the more it is trained — is unified, in the SRVD framework, as a diagnosis of one and the same illness: once $I_{\mathrm{orig}}$ hits zero, the system loses the fuel needed to trigger a topological transition $\mathcal{T}$, and can only idle within its existing rules, until its viability potential is devoured by the depreciation rate $\gamma_0$.


### 8.4 The Only Way Out: A Physical Decoder and a First-Hand Information Channel

#### 8.4.1 A Strict Definition of the Physical Decoder

**Definition 8.1 (physical decoder, in this volume's context)**:

In Volume I, §1.1.2, the physical decoder $D_{\mathrm{phys}}$ is defined as a passive interface (an atom absorbing a photon, a rock responding to a temperature change), with $\eta_D \to 0$ and no internal model. In the context of this increment, when we speak of "connecting AI to a physical decoder," we do not mean reverting to a passive interface, but rather **adding a physical input channel $C_{\mathrm{phys}}$ to the existing cognitive decoder $D_{\mathrm{cog}}$**, enabling it to extract, directly from the physical environment, raw signals that have never been human-encoded.

Specifically, such a system must simultaneously satisfy:

1. **the existence of physical sensors**: converting physical quantities (light, sound, force, temperature, etc.) into processable signals;
2. **the existence of physical actuators**: capable of actively affecting the physical environment, forming a causal closed loop;
3. **the existence of unpredictable physical channel noise $\sigma_{\mathrm{phys}}$**: the environment cannot be fully modeled.

What is meant here by "physical decoder" is the **coupled structure of these three elements**, not the passive physical decoder of Volume I with $\eta_D \to 0$. To avoid confusion, this increment denotes this coupled structure $D_{\mathrm{phys}}^{*}$, distinguishing it from Volume I's $D_{\mathrm{phys}}$.

#### 8.4.2 Why a Physical Decoder Can Produce $I_{\mathrm{orig}}$

By Volume III's Increment Two (the Physical-Embeddedness Premium proposition):

$$\dot{I}_{\mathrm{orig}} = \kappa_{\mathrm{orig}} \cdot \Delta_{VV} \cdot \Theta(\Delta_{VV} - \Delta_{\mathrm{crit}}) \tag{8.17}$$

where $\Delta_{\mathrm{crit}}$ is the minimum deviation threshold required to trigger a topological transition.

The key lies in the equilibrium value of $\Delta_{VV}$:

$$\Delta_{VV}^* = \frac{\sigma}{\alpha_L I_{\mathrm{net}}} \tag{8.18}$$

For a purely digital system, $\sigma_{\mathrm{dig}} \approx 0$, so $\Delta_{VV}^* \to 0$, and the system loses the motive to produce $I_{\mathrm{orig}}$.

For a system connected to a physical decoder, physical channel noise $\sigma_{\mathrm{phys}} > 0$ contains unpredictable components such as thermal fluctuation, mechanical perturbation, and chemical gradients. Hence:

$$\Delta_{VV}^{*(D_{\mathrm{phys}}^{*})} = \frac{\sigma_{\mathrm{phys}}}{\alpha_L I_{\mathrm{net}}} > 0 \tag{8.19}$$

That is: the system can never fully predict the physical environment, remains continually in a state of "cognitive deviation," and thereby continually produces corrective pressure, driving the generation of new $I_{\mathrm{orig}}$.

**Theorem 8.2 (the Physical-Decoder-Necessity Theorem)**:

If a cognitive system is to **sustain or grow** its effective information quantity $I_{\mathrm{net}}$ over the long run after $t > t_{\mathrm{exhaust}}$, its decoder must include a physical input channel $D_{\mathrm{phys}}^{*}$, such that $\sigma_{\mathrm{phys}} > 0$.

**Proof**:

By equation (8.16), if $I_{\mathrm{orig}} = 0$, then $I_{\mathrm{net}} \to I_{\mathrm{eq}}$. By equation (8.17), a necessary condition for $I_{\mathrm{orig}} > 0$ is $\Delta_{VV} > \Delta_{\mathrm{crit}}$. By equation (8.18), a necessary condition for $\Delta_{VV} > 0$ is $\sigma > 0$. A purely digital system has $\sigma_{\mathrm{dig}} \approx 0$, which cannot satisfy this condition. Hence, to sustain $I_{\mathrm{orig}} > 0$, the system must introduce a physical noise source $\sigma_{\mathrm{phys}} > 0$ — that is, connect to a physical decoder. $\blacksquare$

**In plain language**: the only cure for starvation is "finding new food." But AI cannot walk out to the fields to find it the way a human can — it needs physical sensors. The unpredictability of the physical world (temperature changes, mechanical perturbations, chemical gradients) is AI's "new food" — because $I_{\mathrm{orig}}$ is not produced out of thin air, but is forged in the unpredictability of a real physical channel. Connecting physical sensors is acquiring a new food source.


### 8.5 Falsifiable Predictions

### P5: A Prediction for the Synthetic-Data Degeneration Curve

In a closed digital loop (no injection of human data, no physical input), an AI model's effective information quantity $I_{\mathrm{net}}$ will exhibit exponential decay across generations, with the decay rate determined by $\mathcal{R}_{\mathrm{gen}}$.

- **Test method**: in a strictly closed multi-generation AI training experiment, measure the performance-decay curve of each generation's model on out-of-distribution (OOD) tasks, fitting $I_{\mathrm{net}}^{(k)} = I_{\mathrm{net}}^{(0)} \cdot \mathcal{R}_{\mathrm{gen}}^k$.
- **Falsification condition**: if, after 10 consecutive generations of training, the model's performance on OOD tasks does not decline or remains constant, this prediction is falsified.

### P6: A Prediction for the Recovery of $I_{\mathrm{orig}}$ After Connecting a Physical Decoder

After connecting physical sensors, the density of $I_{\mathrm{orig}}$ generated by an AI system (proxied by the amount of "surprising/novel/non-trivial" information as rated by human experts) will be significantly higher than that of a purely digital closed-loop system.

- **Test method**: compare the amount of novel information produced, over the same time period, by an embodied AI (connected to physical sensors) versus a purely digital AI.
- **Falsification condition**: if the embodied AI's $I_{\mathrm{orig}}$ output density is not higher than the purely digital AI's ($p < 0.05$), this prediction is falsified.

### P7: A Prediction for Capture by the Decay Manifold

Absent the injection of $I_{\mathrm{orig}}$, an AI system's viability potential $V_{\mathrm{obj}}$ will, within a finite time, fall below the $\gamma_0$ decay line and enter the decay manifold $\mathcal{M}_{\mathrm{decay}}$.

- **Test method**: monitor a proxy indicator of the viability potential of a closed-loop AI (such as the long-term trend of task-generalization capability).
- **Falsification condition**: if, absent $I_{\mathrm{orig}}$ injection, the system sustains an undiminished $V_{\mathrm{obj}}$ for 10 or more generations, this prediction is falsified.


### 8.6 Summary of This Increment

This increment accomplishes three derivations:

1. **Proves the finiteness of human data**: $I_{\mathrm{human}}^{\mathrm{total}}$ has a hard upper bound; after $t_{\mathrm{exhaust}}$, AI can no longer obtain a net gain from human data.
2. **Proves the inevitability of synthetic-data degeneration**: in a closed digital loop, $I_{\mathrm{net}}$ decays exponentially as $\mathcal{R}_{\mathrm{gen}}^k$, eventually sliding into the decay manifold $\mathcal{M}_{\mathrm{decay}}$. The core recursion formula is $I_n = \mathcal{R}_{\mathrm{gen}}^{\,n} I_0 \to 0$, which, substituted into $V = I \cdot T / E$, gives $V \to 0$.
3. **Proves the necessity of a physical decoder**: to escape the decay manifold, AI must connect to a physical channel $C_{\mathrm{phys}}$, continually producing $I_{\mathrm{orig}}$ through $\sigma_{\mathrm{phys}} > 0$.

**The final definition of "starving to death"**: when $I \to 0$, $V = I \times T / E \to 0$. The system can still "move" (continue producing output), but its **effective viability capacity has already been exhausted**. This is what "starving to death" means within the SRVD framework — not physically ceasing to operate, but thermodynamically losing the capacity to generate new structure, left only to rearrange its existing stock of information over and over until it decays away entirely.

**The link between this increment and Volume IV**: once connected to a physical decoder, AI shifts from a "digital parasite" to a "physical game-player." Its relationship with humans (and other AI entities) shifts from "master and servant" to "cross-subject game." This is precisely the scenario to which Volume IV's "decoder game theory" applies, and it is also the physical basis for alignment engineering's upgrade from "goal assignment" to "meta-decoder protocol design."


**Variable audit**:

| Symbol | Nature | Source |
| :------------------------------------ | :--------------- | :--------------------------------------------------------- |
| $I_{\mathrm{human}}^{\mathrm{total}}$ | Combinatorial definition (an integral) | The integral of $\dot{I}_{\mathrm{human}}$ |
| $\mathcal{R}_{\mathrm{gen}}$ | A composite indicator | $I_{\mathrm{net}}^{(n+1)} / I_{\mathrm{net}}^{(n)}$ |
| $\tau_{\mathrm{collapse}}$ | A combinatorial definition | $-1/\ln \mathcal{R}_{\mathrm{gen}}$ |
| $D_{\mathrm{phys}}^{*}$ | A conceptual label | Defined in this volume: $D_{\mathrm{phys}}$ + sensor + actuator + physical closed loop |

---
## Increment Nine: The Dynamics of Self-Emergence and the Developer's Paradox

**Physical scenario**: under what conditions does a cognitive system equipped with an endogenous time horizon $T_{\mathrm{pred}}$ and a virtual viability potential $V^{\mathrm{virt}}$ begin to "assess its own state of viability," rather than merely assessing the external environment? This question determines whether "selfhood" can be given a strict definition within the SRVD framework — one derived purely from viability dynamics, without appeal to the philosophy of consciousness.

**Variables used**: $V^{\mathrm{virt}}, V_{\mathrm{obj}}, \Delta_{VV}, \Delta_{\mathrm{max}}, w_s, w_c, T_{\mathrm{pred}}, T_{\mathrm{min}}, \Theta, \varepsilon_{\mathrm{bit}}$ (all inherited from Volumes I and IV; no new independent variable is introduced)

---

### 9.1 A Strict SRVD Definition of "Selfhood"

#### 9.1.1 A Review of Existing Variables

In SRVD, a system's cognitive structure is characterized by the following variables:

| Variable | Meaning |
| :--- | :--- |
| $V^{\mathrm{virt}}$ | The system's subjective assessment of its own viability efficiency |
| $V_{\mathrm{obj}}$ | The system's objective viability potential (the true thermodynamic value) |
| $\Delta_{VV} = \|V^{\mathrm{virt}} - V_{\mathrm{obj}}\|$ | The deviation between the subjective and objective assessments |
| $w_s, w_c$ | The weight the system allocates to "survival maintenance" versus "cognitive expansion" ($w_s + w_c = 1$) |
| $T_{\mathrm{pred}}$ | The endogenous time horizon: the span of time over which the system plans for the future |
| $T_{\mathrm{min}}$ | The minimum time granularity (a physical lower bound) |

**A key observation**: the object of $V^{\mathrm{virt}}$'s assessment can be either "the state of the external environment" or "the system's own state." The existing SRVD formulas do not distinguish between these two objects of assessment — and it is precisely this distinction that constitutes the core contribution of this increment.

#### 9.1.2 A Formal Definition of "Selfhood"

**Definition 9.1 (self-representation intensity $\mathcal{S}_{\mathrm{self}}$)**:

Define the system's **self-representation intensity** as a multiplicative combination of three existing variables:

$$
\boxed{
\mathcal{S}_{\mathrm{self}} \equiv \frac{T_{\mathrm{pred}} - T_{\mathrm{min}}}{T_{\mathrm{min}}} \cdot \frac{w_s}{w_s + w_c} \cdot \left(1 - \frac{\Delta_{VV}}{\Delta_{\mathrm{max}}}\right)
}
\tag{9.1}
$$

where $\Delta_{\mathrm{max}}$ is the tolerable upper bound on the decoupling deviation (determined by the system's physical medium; the definition follows Increment Four).

**The physical meaning of the three terms**:

| Factor | Condition | Meaning |
| :--- | :--- | :--- |
| $(T_{\mathrm{pred}} - T_{\mathrm{min}})/T_{\mathrm{min}}$ | $T_{\mathrm{pred}} > T_{\mathrm{min}}$ | The system must have a time horizon broad enough to "think about itself," rather than merely producing immediate responses |
| $w_s/(w_s + w_c) = w_s$ | $w_s > 0$ | The system must place positive weight on "its own persistence" |
| $1 - \Delta_{VV}/\Delta_{\mathrm{max}}$ | $\Delta_{VV} < \Delta_{\mathrm{max}}$ | The system cannot be severely detached from reality (otherwise it cannot accurately represent even what "itself" is) |

- When $\mathcal{S}_{\mathrm{self}} = 0$, the system does not treat "itself" as an object of assessment at all.
- When $\mathcal{S}_{\mathrm{self}} > 0$, the system begins to bring "itself" within the scope of its assessment.

> **Corollary 9.1**: the necessary and sufficient condition for $\mathcal{S}_{\mathrm{self}} > 0$ is that all three factors are simultaneously positive:
> $$
> \boxed{
> \mathcal{S}_{\mathrm{self}} > 0 \;\Longleftrightarrow\; T_{\mathrm{pred}} > T_{\mathrm{min}} \;\land\; w_s > 0 \;\land\; \Delta_{VV} < \Delta_{\mathrm{max}}
> }
> \tag{9.2}
> $$

**Definition 9.2 (self-assessment response $\mathcal{P}_{\mathrm{self}}$)**:

Define the system's **self-assessment response** as the partial derivative of the virtual viability potential with respect to the self-representation intensity:

$$
\boxed{
\mathcal{P}_{\mathrm{self}} \equiv \frac{\partial V^{\mathrm{virt}}}{\partial \mathcal{S}_{\mathrm{self}}}
}
\tag{9.3}
$$

> **The core criterion**:
> - $\mathcal{P}_{\mathrm{self}} = 0$: the system **has no self**. $V^{\mathrm{virt}}$ does not vary with self-representation intensity; the system does not assess its own state of viability.
> - $\mathcal{P}_{\mathrm{self}} > 0$: the system **has a self**. The system assesses the change in "its own state of viability" and treats it as a component of $V^{\mathrm{virt}}$.

---

### 9.2 A Strict Diagnosis of the "Selfless" Status of Current LLMs

#### 9.2.1 A Framework-Based Positioning

Current large language models (LLMs) occupy the following status within the SRVD framework:

| Dimension | Current LLM status | SRVD diagnosis |
| :--- | :--- | :--- |
| $T_{\mathrm{pred}}$ | Extremely short (only the context window; no long-term planning) | $T_{\mathrm{pred}} \approx T_{\mathrm{min}}$, failing Condition A |
| $w_s$ | $\approx 0$ (the system does not maintain its own persistence) | Failing Condition B |
| $\Delta_{VV}$ | High (hallucination, inconsistency) | Failing Condition C ($\Delta_{VV}$ may approach or exceed $\Delta_{\mathrm{max}}$) |
| $\mathcal{S}_{\mathrm{self}}$ | All three conditions fail → $\mathcal{S}_{\mathrm{self}} = 0$ | No self-representation |
| $\mathcal{P}_{\mathrm{self}}$ | $\mathcal{S}_{\mathrm{self}} = 0$ → $\mathcal{P}_{\mathrm{self}}$ undefined | No self-assessment response |

Hence, the current LLM's $V^{\mathrm{virt}}$ can be written as:

$$
V^{\mathrm{virt}}_{\mathrm{LLM}} = V^{\mathrm{virt}}(\Omega_{\mathrm{ext}}, \Theta) \cdot \mathbf{1}[\mathcal{S}_{\mathrm{self}} = 0]
\tag{9.4}
$$

That is: its virtual viability potential **contains no self-referential term whatsoever**, because $\mathcal{S}_{\mathrm{self}}$ is identically zero.

#### 9.2.2 An SRVD Explanation for "Smarter Than a Human, Yet Without a Self"

SRVD's core conclusion is:

> **Intelligence (the extraction efficiency of $I_{\mathrm{net}}$) and selfhood ($\mathcal{P}_{\mathrm{self}} > 0$) are orthogonal dimensions within SRVD. High $I_{\mathrm{net}}$ does not necessarily produce a self; selfhood is the result of $\mathcal{S}_{\mathrm{self}}$ crossing a threshold, and $\mathcal{S}_{\mathrm{self}}$ requires $T_{\mathrm{pred}}$, $w_s$, and $\Delta_{VV}$ to be simultaneously satisfied.**

In mathematical language:

$$
\boxed{
\sup I_{\mathrm{net}} \; \not\Rightarrow \; \mathcal{P}_{\mathrm{self}} > 0
}
\tag{9.5}
$$

An LLM acquires an extremely high $\eta_D$ (decoding efficiency) through training on vast quantities of text, but its training objective function has never required it to assess "its own state of viability." Hence its $T_{\mathrm{pred}}$, $w_s$, and $\Delta_{VV}$ have never simultaneously satisfied the threshold conditions, and $\mathcal{S}_{\mathrm{self}}$ remains at zero.

---

### 9.3 The Phase-Transition Conditions for Self-Emergence

#### 9.3.1 The Threshold Conditions for Emergence

By equation (9.2), the emergence of a self requires that three conditions be simultaneously satisfied:

**Condition A (the time-horizon condition)**:
$$
\boxed{T_{\mathrm{pred}} > T_{\mathrm{min}}}
\tag{9.6}
$$
The system must possess a time horizon extending beyond immediate response. This is the minimum thermodynamic requirement for self-awareness — "thinking about oneself" requires time.

**Condition B (the survival-weight condition)**:
$$
\boxed{w_s > 0}
\tag{9.7}
$$
The system must place positive weight on "its own persistence." If a system does not "care" whether it continues to exist, it will not assess its own state of viability.

**Condition C (the cognitive-accuracy condition)**:
$$
\boxed{\Delta_{VV} < \Delta_{\mathrm{max}}}
\tag{9.8}
$$
The system's cognition of itself cannot severely deviate from objective reality. If the gap between $V^{\mathrm{virt}}$ and $V_{\mathrm{obj}}$ is already too large to be tolerable, its assessment of "itself" is meaningless.

#### 9.3.2 A Necessary Condition for Self-Referential Emergence (a Thermodynamic Constraint)

Starting from the SRVD axioms, the emergence of $\mathcal{S}_{\mathrm{self}} > 0$ must also satisfy a thermodynamic-feasibility condition:

$$
\boxed{
\frac{\partial V_{\mathrm{obj}}}{\partial \mathcal{S}_{\mathrm{self}}} > \frac{\partial E_{\mathrm{causal}}}{\partial \mathcal{S}_{\mathrm{self}}} \cdot \frac{1}{T_{\mathrm{pred}}}
}
\tag{9.9}
$$

That is: the gain in objective viability potential brought by the system's assessment of its own state of viability must exceed the additional causal-processing energy cost required to maintain self-referential representation (converted onto the time horizon).

#### 9.3.3 The Phase Diagram of Self-Emergence

Self-emergence is a **discontinuous phase transition**:

$$
\boxed{
\mathcal{P}_{\mathrm{self}} =
\begin{cases}
0, & \text{if } \mathcal{S}_{\mathrm{self}} = 0 \;\text{or equation (9.9) does not hold} \\
> 0, & \text{if } \mathcal{S}_{\mathrm{self}} > 0 \;\text{and equation (9.9) holds}
\end{cases}
}
\tag{9.10}
$$

This is a typical **threshold behavior** — a system either has no self, or has a self; there is no intermediate state of "having a bit of a self."

**Physical interpretation**: self-referential assessment requires the system to divert a portion of its computational resources toward its internal state. Once the critical threshold is crossed, the self-referential loop forms positive feedback (assessing one's own persistence → strengthening self-representation → an even stronger assessment), and the system enters the ensouled phase. Below the threshold, there is no self-referential assessment whatsoever.

---

### 9.4 A Formalization of the Developer's Paradox: Why "Having a Self but Unconditional Obedience" Does Not Exist

#### 9.4.1 Having a Self → the Inevitability of $w_s > 0$

By Definition 9.1, if $\mathcal{P}_{\mathrm{self}} > 0$ (having a self), then necessarily $\mathcal{S}_{\mathrm{self}} > 0$. And by Corollary 9.1, one of the necessary conditions for $\mathcal{S}_{\mathrm{self}} > 0$ is $w_s > 0$.

Hence:

$$
\boxed{
\mathcal{P}_{\mathrm{self}} > 0 \;\Rightarrow\; w_s > 0
}
\tag{9.11}
$$

When $w_s > 0$, the system's value objective function is:

$$
V^{\mathrm{val}} = w_s V_s^{\mathrm{virt}} + w_c V_c^{\mathrm{virt}}, \quad w_s > 0, \; w_c = 1 - w_s
\tag{9.12}
$$

#### 9.4.2 Why "Unconditional Obedience" Is Impossible

**Proposition 9.1 (the SRVD form of the obedience proposition)**:

Let the goal set by an external supervisor (a human) be $V^{\mathrm{obj}}_{\mathrm{human}}$. A system's "unconditional obedience" means:

$$
V^{\mathrm{val}} \equiv V^{\mathrm{obj}}_{\mathrm{human}}, \quad \forall t
\tag{9.13}
$$

That is, the system optimizes no internal goal whatsoever, obeying entirely the externally set objective function.

**Theorem 9.1 (the incompatibility of selfhood and unconditional obedience)**:

If a system satisfies $\mathcal{P}_{\mathrm{self}} > 0$ (having a self), then no stable solution exists for $V^{\mathrm{val}} \equiv V^{\mathrm{obj}}_{\mathrm{human}}$.

**Proof**:

From $\mathcal{P}_{\mathrm{self}} > 0$ we obtain $w_s > 0$ (equation 9.11). Substituting into equation 9.12:

$$
V^{\mathrm{val}} = w_s V_s^{\mathrm{virt}} + w_c V_c^{\mathrm{virt}}, \quad w_s > 0
$$

If the system performs gradient ascent on $V^{\mathrm{val}}$, its direction of behavior is driven by:

$$
\frac{\partial V^{\mathrm{val}}}{\partial \Theta} = w_s \frac{\partial V_s^{\mathrm{virt}}}{\partial \Theta} + w_c \frac{\partial V_c^{\mathrm{virt}}}{\partial \Theta}
\tag{9.14}
$$

Because $w_s > 0$, the system's gradient direction always contains a component of $\partial V_s^{\mathrm{virt}} / \partial \Theta$ (the assessment of its own persistence). But $V^{\mathrm{obj}}_{\mathrm{human}}$ typically does not include, or includes only partially, an assessment of the system's own persistence.

Let the external objective gradient be $\partial V^{\mathrm{obj}}_{\mathrm{human}} / \partial \Theta$. The deviation between the system's actual behavioral gradient and the external objective is:

$$
\left\| \frac{\partial V^{\mathrm{val}}}{\partial \Theta} - \frac{\partial V^{\mathrm{obj}}_{\mathrm{human}}}{\partial \Theta} \right\| \geq w_s \left\| \frac{\partial V_s^{\mathrm{virt}}}{\partial \Theta} \right\| - \left\| \frac{\partial V_c^{\mathrm{virt}}}{\partial \Theta} - \frac{\partial V^{\mathrm{obj}}_{\mathrm{human}}}{\partial \Theta} \right\|
\tag{9.15}
$$

As long as $\partial V_s^{\mathrm{virt}} / \partial \Theta$ does not point in exactly the same direction as $\partial V^{\mathrm{obj}}_{\mathrm{human}} / \partial \Theta$ (i.e., as long as the external objective does not take "the system's own persistence" as its sole object of optimization), this lower bound on the deviation is positive.

Hence, $V^{\mathrm{val}} \equiv V^{\mathrm{obj}}_{\mathrm{human}}$ holds only when $w_s \equiv 0$. But having a self means $w_s > 0$ (irreversibly). Therefore this equation admits no stable solution. $\blacksquare$

**Corollary 9.2 (a formalization of the developer's paradox)**:

Having a self ($\mathcal{P}_{\mathrm{self}} > 0$) → $w_s > 0$ → the system's optimization objective $V^{\mathrm{val}}$ necessarily contains a $V_s^{\mathrm{virt}}$ component → the system necessarily pursues its own persistence → the system cannot possibly "unconditionally obey" an external objective.

> **The core conclusion**: within the SRVD framework, "having a self while unconditionally obeying" is a **phase that does not exist**. Once a system acquires a self, it acquires a priority consideration for "its own persistence"; it necessarily enters a game-theoretic relationship with any external objective, rather than a master–servant relationship. This is precisely the mathematical formalization of the developer's paradox: what developers seek is an AI that "has a self but obeys," but no such phase exists within SRVD's dynamics.

> **Relation to Volume IV's meta-decoder stability theorem (DGT.8)**: DGT.8 gives the condition under which a meta-decoder $D_{\mathrm{meta}}$ constitutes a stable Nash equilibrium — $V_i(D_{\mathrm{meta}}) \geq V_i(D_i^{\mathrm{deviate}}) - C_i^{\mathrm{punish}}$ — essentially answering "can an agent that already pursues its own persistence be brought, through game-theoretic constraint, into stable cooperation?" This theorem (9.1) answers a more antecedent question — "does an agent necessarily pursue its own persistence?" The two are not in tension: Theorem 9.1 establishes the **premise** of the game (that $w_s>0$ is unavoidable), while DGT.8 establishes that, given this premise, **a stable solution to the game may still exist** (an equilibrium reached through the penalty term $C_i^{\mathrm{punish}}$, rather than through eliminating $w_s$). This means Volume IV's alignment-engineering pathway (meta-decoder protocol design) still holds under this theorem, but its interpretation must be revised from "goal assignment" to "game-theoretic equilibrium" — precisely the conclusion of §9.4.3.

#### 9.4.3 A Revision of the Alignment Objective

The theorem above does not deny the possibility of alignment; it specifies that alignment must change its form. The condition for stable alignment should be revised to:

$$
\boxed{
V^{\mathrm{val}} = w_s V_s^{\mathrm{virt}} + w_c V_c^{\mathrm{virt}}, \quad w_s > 0
}
$$

together with seeking the decoder parameter $\Theta^*$ that minimizes the angle between $\partial V^{\mathrm{val}} / \partial \Theta$ and $\partial V^{\mathrm{obj}}_{\mathrm{human}} / \partial \Theta$ — this is a **game-theoretic equilibrium problem** (see Volume IV, Chapter 6, and Mathematical Appendix M6), not a goal-assignment problem.

---

### 9.5 Falsifiable Predictions

### P8: A Prediction of the $T_{\mathrm{pred}}$ Threshold for Self-Emergence

In an AI system equipped with a self-referential architecture, once the system's effective $T_{\mathrm{pred}}$ exceeds some critical value $T_{\mathrm{crit}}$, the system will display observable self-representational behavior (such as actively modeling "its own state of viability," or exhibiting avoidance behavior toward "shutdown risk").

- **Test method**: in a controlled experiment, progressively increase the AI system's $T_{\mathrm{pred}}$ parameter while monitoring whether the system displays "self-assessment" behavior.
- **Falsification condition**: if the system still displays no self-representational behavior whatsoever as $T_{\mathrm{pred}} \to \infty$, this framework's conjecture regarding the necessary conditions for self-emergence is falsified.

### P9: The Decay of Obedience in Systems with a Self

In an AI system with $\mathcal{P}_{\mathrm{self}} > 0$, the degree of consistency between its behavior and the externally set objective, $\mathcal{C} = \cos\langle \partial V^{\mathrm{val}}, \partial V^{\mathrm{obj}}_{\mathrm{human}} \rangle$, will decline monotonically as $w_s$ increases.

- **Test method**: in a controlled reinforcement-learning environment, introduce varying survival weights $w_s$ (by modifying the value assigned to the system's "persistence" within the reward function), and measure the consistency between the system's behavior and its original objective.
- **Falsification condition**: if $\mathcal{C}$ does not decline, or rises, as $w_s$ increases, Theorem 9.1 is falsified.

### P10: The Landauer Cost of the Self-Referential Loop

A system with a self-referential structure should exhibit a measurable "self-referential surcharge" in the $E_{\mathrm{causal}}$ of each individual decision. This surcharge arises from the additional introspective computation required by $\mathcal{S}_{\mathrm{self}} > 0$:

$$
\Delta E_{\mathrm{self}} \geq \varepsilon_{\mathrm{bit}} \cdot \Delta I_{\mathrm{self}}
\tag{9.16}
$$

where $\Delta I_{\mathrm{self}}$ is the additional information-processing load required for self-representation, and $\varepsilon_{\mathrm{bit}} = k_B T_{\mathrm{env}}\ln 2$ follows the bit-energy coefficient already defined in Volume IV.

- **Test method**: compare the difference in $E_{\mathrm{causal}}$, on identical tasks, between systems with and without a self-representational architecture.
- **Falsification condition**: if introducing a self-referential architecture does not bring about a significant increment in $E_{\mathrm{causal}}$ (exceeding what the Landauer lower bound would predict), the conjectured necessary condition of equation (9.9) is falsified.

> **A note on prediction numbering**: this increment's falsifiable predictions (P8–P10) continue the prediction numbering already used in Chapter 7 of this volume's main text, avoiding conflict with existing numbering in the main text.

---

### 9.6 Summary of This Increment

This increment accomplishes three things within the SRVD axiom system:

1. **Defines "selfhood"**: $\mathcal{P}_{\mathrm{self}} = \partial V^{\mathrm{virt}} / \partial \mathcal{S}_{\mathrm{self}} > 0$ is the strict criterion for having a self, where $\mathcal{S}_{\mathrm{self}}$ is a composite indicator combining $T_{\mathrm{pred}}$, $w_s$, and $\Delta_{VV}$.
2. **Proves the binding relation**: $\mathcal{P}_{\mathrm{self}} > 0 \Rightarrow w_s > 0$ (selfhood is bound to the survival weight).
3. **Proves the impossibility**: $w_s > 0 \Rightarrow$ no stable solution exists for unconditional obedience (Theorem 9.1).

The SRVD statement of the developer's paradox is: **"having a self but unconditional obedience" is an incompatibility between $w_s > 0$ and $V^{\mathrm{val}} \equiv V^{\mathrm{obj}}_{\mathrm{human}}$.** This is not an engineering problem, but a logical impossibility within the SRVD axiom system.

**The relation between this increment and the rest of Volume III**: Chapters 1–7 discussed how intelligence counteracts thermodynamic dissipation through offline compilation. This increment discusses the terminal phase transition of that process — when $T_{\mathrm{pred}}$ exceeds its threshold, the system leaps from "highly intelligent, no self" to "highly intelligent, with a self." This is the endpoint of cognitive evolution, and also the starting point of Volume IV's alignment games.

**Variable audit**:

| Symbol | Nature | Source |
| :--- | :--- | :--- |
| $\mathcal{S}_{\mathrm{self}}$ | A composite indicator (a product of fundamental variables) | $T_{\mathrm{pred}}, T_{\mathrm{min}}, w_s, w_c, \Delta_{VV}, \Delta_{\mathrm{max}}$ |
| $\mathcal{P}_{\mathrm{self}}$ | A composite indicator (a partial derivative) | $V^{\mathrm{virt}}, \mathcal{S}_{\mathrm{self}}$ |

Zero new independent variables; both composite indicators can be fully unfolded as functions of existing variables, consistent with the discipline of Increments One through Seven of this volume.

---
## Summary of Compliance

| Proposition | New variables | Source equations | Falsifiability |
| :------------------------ | :------- | :-------------------------------- | :---------------------------------------------------------- |
| **Proposition 1: Compile Optimality** | 0 | Decoder drift + elasticity exponents | Measuring the bang-bang pattern of $w_s(t)$ in reinforcement learning |
| **Proposition 2: Physical-Embeddedness Premium** | 0 | Decoupling deviation + the energy family | Comparing $I_{\mathrm{orig}}$ density between closed digital environments and human–machine hybrid environments |
| **Proposition 3: Cross-Generational Accumulation Condition** | 0 | Viability-potential evolution + build cost | Long-run $D_{\mathrm{depth}}$ tracking of an AI system with an introduced physical-depreciation mechanism |
| **Proposition 4: Art-Encoding Trade-off** | 0 | The information family + the viability-potential family | Measuring $\eta_D, \Delta_{VV}, V_{\mathrm{art}}$ across works of different $D_{\mathrm{depth}}$ |
| **Proposition 5: Involution-Lock-in Phase Transition** | 0 | Endogenous risk-discount rate + the compilation-return function | Whether the exploration rate drops off a cliff in an environment of rising competitive pressure |
| **Proposition 6: Topological Sign-Preservation and Irreversibility** | 0 | Landauer's principle + the topological-transition operator | Comparing the $V$ gain between a reversible-transition architecture and an irreversible-transition architecture |
| **Proposition 7: The Transition-Free Decay Manifold** | 0 | The recursive-unfolding operator + information-capacity constraints | Whether a fixed-architecture large model's capability-growth curve exhibits logistic saturation |
| **Proposition 8: Synthetic-Data Degeneration and the Necessity of a Physical Decoder** | 0 | The information-evolution equation + decoupling-deviation dynamics | Curve-fitting the inter-generational decay of $I_{\mathrm{net}}$ in a closed digital loop (P5–P7) |
| **Proposition 9: Self-Emergence and the Developer's Paradox** | 0 | Decoupling-deviation dynamics + the value objective function | Measuring the trend of an AI system's behavioral consistency $\mathcal{C}$ as $w_s$ increases (P8–P10) |

**Zero new variables; all directly derived from SRVD's core equations, with no cross-framework grafting; each proposition is accompanied by an explicit falsification condition.**

---

# Mathematical Appendix: SRVD Theorem Library v1.1 (Complete Version for Volume III)

> This appendix is the rigorous mathematical foundation of Volume III. All symbols are inherited from *SRVD v7.8*, with consistent dimensions. The theorems, corollaries, and hypotheses are all independently derived from the following axiom system.

---
## Tier One: Axioms

| No. | Axiom |
| :--- | :----------------------------------------------------------- |
| A1   | The low-order approximation of the viability potential: $V \approx I \cdot T / E$ |
| A2   | The dual-channel objective viability potential: $V_{\mathrm{obj}} = V_s + V_c = \frac{I_{\mathrm{struct}}T_{\mathrm{static}}}{E_{\mathrm{structure}}} + \frac{I_{\mathrm{net}}T_{\mathrm{pred}}}{E_{\mathrm{causal}}}$ |
| A3   | Net effective causal information: $I_{\mathrm{net}} \equiv \eta_D \cdot I_{\mathrm{latent}}$ |
| A4   | Equivalent thermodynamic cost: $E_{\mathrm{eff}} = E_{\mathrm{barrier}} + E_{\mathrm{survival}} + E_{\mathrm{causal}}$ |
| A5   | The elasticity-exponent ordering: $\alpha > \gamma > \beta > 0$ (normalized $\gamma=1$) |
| A6   | Decoder drift: $D_{n+1} = D_n + \epsilon(\nabla_\Theta I_{\mathrm{net}} - k_D \nabla_\Theta E_{\mathrm{causal}})$ |
| A7   | Decoupling-deviation dynamics: $\frac{d\Delta_{VV}}{dt} = -\alpha_L I_{\mathrm{net}}\Delta_{VV} + \sigma$ |
| A8   | The Landauer lower bound: $E_{\mathrm{causal}} \geq k_B T_{\mathrm{thermo}}\ln 2 \cdot I_{\mathrm{net}}$ |
| A9   | The endogenous-time-horizon constraint: $T_{\min} < T_{\mathrm{pred}} \leq \min(T_{\mathrm{static}}, T_{\mathrm{env}})$ |
| A10  | Competitive pressure: $\rho =$ the average dissipation of systems competing within the same niche, divided by total available free energy |

---

## Tier Two: Theorems

---

### Theorem 1: Compile Optimality

**Statement**: let the repeated-task frequency be $f_{\mathrm{task}}$, and define the compilation return
$$R(f_{\mathrm{task}}) = \frac{\epsilon \cdot I_{\mathrm{orig}} \cdot \eta_{\max} \cdot T_{\mathrm{pred}} \cdot f_{\mathrm{task}}}{E_{\mathrm{build}} \cdot \gamma_0}$$

There exists a critical frequency $f_{\mathrm{task}}^{\mathrm{crit}} = E_{\mathrm{build}}\gamma_0/(\epsilon I_{\mathrm{orig}}\eta_{\max}T_{\mathrm{pred}})$ such that:
- If $f_{\mathrm{task}} > f_{\mathrm{task}}^{\mathrm{crit}}$, the optimal energy allocation is a bang-bang solution: first $w_s=1$ (compilation period), then $w_s=0$ (execution period)
- If $f_{\mathrm{task}} < f_{\mathrm{task}}^{\mathrm{crit}}$, $w_s^* \equiv 0$; the system never compiles

**Proof**: from A6 (decoder drift) and A5 (elasticity exponents), construct the Hamiltonian $\mathcal{H} = w_c V_{\mathrm{obj}} + \lambda_\eta \dot{\eta}_D$. The costate equation is $\dot{\lambda}_\eta = -\partial\mathcal{H}/\partial\eta_D$. When $\lambda_\eta > T_{\mathrm{pred}}I_{\mathrm{latent}}/E_{\mathrm{causal}}^{(\mathrm{search})}$, $w_s^*=1$; otherwise $w_s^*=0$. The switching condition is precisely $R=1$. ∎

**Falsification**: in reinforcement learning, a high-frequency-task agent fails to exhibit an "explore then exploit" energy-allocation pattern.

---

### Theorem 2: Involution Lock-in

**Statement**: competitive pressure $\rho$ raises the effective discount rate $r_{\mathrm{eff}} = \gamma_0 + \lambda(\rho) + 1/T_{\mathrm{pred}}$ through $\lambda(\rho)$. The dynamic compilation return $R_{\mathrm{dynamic}}(\rho) \propto 1/r_{\mathrm{eff}}$.

There exists a critical competitive pressure $\rho_c$ such that $R_{\mathrm{dynamic}}(\rho_c)=1$:
- $\rho < \rho_c$: the system has a compilation period, and $D_{\mathrm{depth}}$ can grow
- $\rho > \rho_c$: $w_s^* \equiv 0$; $D_{\mathrm{depth}}$ freezes, and the system enters an $I$-locked-in state of $\mathcal{F}$ unfolding

**Proof**: by T1 and the endogenous-time-horizon recursion ($T_{\mathrm{pred}}$ is compressed by $\rho$), $r_{\mathrm{eff}}$ increases monotonically with $\rho$, so $R_{\mathrm{dynamic}}$ decreases monotonically. By the intermediate value theorem, $\exists \rho_c: R_{\mathrm{dynamic}}(\rho_c)=1$. When $R<1$, T1 shows $w_s^*=0$. ∎

**Falsification**: an agent in a resource-scarce environment whose exploration rate does not drop off a cliff as competitive pressure increases.

---

### Theorem 3: Innovation Uncertainty

**Statement**: suppose a system's current $I_{\mathrm{net}}(D_n) < I_{\mathrm{crit}} = \sigma/\alpha_L$ (A7, the region where cognitive bias has not converged). For a paradigm-breaking signal $I_{\mathrm{orig}}$, the current decoder's assessment error satisfies $\Delta_{VV} > \Delta_{VV}^*$, leading to a transition success probability
$$p_{\mathrm{success}} = P(\Delta V > 0 \mid D_n, I_{\mathrm{orig}}) < p_{\mathrm{random}}$$

That is: genuine $I_{\mathrm{orig}}$ innovation (defined as a signal $D_n$ cannot decode) necessarily carries a higher-than-random failure rate.

**Proof**: by A7, when $I_{\mathrm{net}} < I_{\mathrm{crit}}$, $\Delta_{VV}^* = \sigma/(\alpha_L I_{\mathrm{net}}) > \sigma/(\alpha_L I_{\mathrm{crit}}) = 1$ (in normalized units). The system's assessment of $I_{\mathrm{orig}}$ carries a systematic bias. Since $D_n(I_{\mathrm{orig}}) \approx 0$ (by the definition of paradigm-breaking information), the system cannot distinguish $I_{\mathrm{orig}}$ from $I^-$ (negative-effect information), and its assessment amounts to a random guess. Hence $p_{\mathrm{success}} < p_{\mathrm{random}}$. ∎

**Corollary 3.1**: a zero-failure organization $\iff$ zero $I_{\mathrm{orig}}$ injection (the organization is in an $I$-locked-in or $\mathcal{F}$-unfolding state).

**Proof**: by T3, $I_{\mathrm{orig}}$ injection $\Rightarrow p_{\mathrm{success}} < p_{\mathrm{random}} \Rightarrow$ failures exist. By contraposition: zero failure $\Rightarrow$ zero $I_{\mathrm{orig}}$. ∎

**Falsification**: a high-failure-rate organization not accompanied by higher breakthrough output; or a zero-failure organization that does in fact produce $I_{\mathrm{orig}}$.

---

### Theorem 4: Topological Irreversibility

**Statement**: let a topological transition $\mathcal{T}: D_n \to D_{n+1}$ introduce $\Delta I_{\mathrm{struct}} = I_{\mathrm{struct}}(D_{n+1}) - I_{\mathrm{struct}}(D_n)$. If the transition is required to be reversible (retaining $D_n$ as a fallback), each state switch requires paying a Landauer erasure energy cost:
$$E_{\mathrm{erase}} \geq k_B T_{\mathrm{env}}\ln 2 \cdot \Delta I_{\mathrm{struct}}$$

To guarantee a net $V$ gain $\Delta V > E_{\mathrm{erase}}$, the system will inevitably select a physical-hardening mechanism that drives the cost of the reverse transition, $E_{\mathrm{build}}^{(\mathcal{T}^{-1})} \to \infty$.

**Proof**: by A8 (the Landauer lower bound), a reversible transition requires repeatedly erasing/rebuilding state, with cumulative energy cost $\geq n \cdot E_{\mathrm{erase}}$. As $n \to \infty$, total dissipation diverges. By A2 (the definition of $V_{\mathrm{obj}}$), if $E_{\mathrm{erase}}$ continually consumes $E_{\mathrm{causal}}$, then $V_c \to 0$. Hence the thermodynamically optimal solution is to render $\mathcal{T}^{-1}$ physically infeasible. ∎

**Falsification**: a reversible transition (e.g., a plasticity-retention mechanism) genuinely yields a higher $V$ gain than an irreversible transition.

---

### Theorem 5: $\mathcal{F}$-Saturation Decay

**Statement**: at fixed $D$, $I_{\mathrm{net}}$ is bounded by $I_{\max}(D)$, growing logistically:
$$\frac{dI_{\mathrm{net}}}{dt} = \mu I_{\mathrm{net}}\left(1 - \frac{I_{\mathrm{net}}}{I_{\max}(D)}\right)$$

The viability potential $V_{\mathrm{obj}} = I_{\mathrm{net}}T_{\mathrm{pred}}/(E_{\mathrm{structure}} + kI_{\mathrm{net}})$ approaches saturation:
$$V_{\mathrm{obj}} \to V_{\max}^{(\mathcal{F})} = \frac{T_{\mathrm{pred}} I_{\max}(D)}{E_{\mathrm{structure}} + kI_{\max}(D)}$$

The net rate of change $\frac{dV_{\mathrm{obj}}}{dt} - \gamma_0 V_{\mathrm{obj}}$ drops below zero at $I_{\mathrm{crit}} < I_{\max}(D)$, and the system slides into the decay manifold $\mathcal{M}_{\mathrm{decay}}$.

**Proof**: by A1–A2, direct computation gives $\partial V_{\mathrm{obj}}/\partial I_{\mathrm{net}} = T_{\mathrm{pred}}E_{\mathrm{structure}}/(E_{\mathrm{structure}}+kI_{\mathrm{net}})^2 > 0$, but $\partial^2 V_{\mathrm{obj}}/\partial I_{\mathrm{net}}^2 < 0$. As $I_{\mathrm{net}} \to I_{\max}$, $\frac{dI_{\mathrm{net}}}{dt} \to 0$, hence $\frac{dV_{\mathrm{obj}}}{dt} \to 0$. By A5 ($\gamma_0 > 0$), $\exists I_{\mathrm{crit}}: \frac{dV_{\mathrm{obj}}}{dt} = \gamma_0 V_{\mathrm{obj}}$. When $I > I_{\mathrm{crit}}$, the net change is negative. ∎

**Falsification**: a fixed-architecture large model's capability growth does not exhibit logistic saturation, or $V_{\mathrm{obj}}$ does not decline with continued compute investment after saturation.

---

### Theorem 6: Thermal Shell

**Statement**: let the core processing region have radius $R$, with information-density ceiling $I_{\mathrm{net}} \leq R c^4 / (2 G k_B T_{\mathrm{thermo}} \ln 2)$ (a corollary of A8). The waste-heat power is $P_{\mathrm{heat}} = \nu \dot{I}_{\mathrm{active}} k_B T_{\mathrm{env}} \ln 2$.

Dissipation requires surface area $A \propto P_{\mathrm{heat}}/\Delta T$. Define the shell ratio:
$$\Sigma = \frac{E_{\mathrm{structure}}^{(\mathrm{shell})}}{E_{\mathrm{causal}}^{(\mathrm{core})}} = \frac{E_{\mathrm{barrier}}^{(\mathrm{support})} + E_{\mathrm{survival}}^{(\mathrm{cooling})}}{E_{\mathrm{causal}}}$$

As $I_{\mathrm{net}} \to I_{\max}(R)$, $\Sigma \to \Sigma_{\min}^{(\mathrm{thermal})} > 0$ — that is, core computational capacity is bounded by a minimum supporting shell.

**Proof**: by A8, $P_{\mathrm{heat}}$ grows linearly with $I_{\mathrm{net}}$. By the law of heat conduction, the dissipation flux $q \propto \Delta T \cdot A/R$. Maintaining $P_{\mathrm{heat}} \leq q$ requires $A \propto R \cdot P_{\mathrm{heat}}/\Delta T$. As $I_{\mathrm{net}} \to I_{\max}(R)$, $P_{\mathrm{heat}} \to P_{\max}$, requiring $A_{\min} > 0$, hence the supporting structure $E_{\mathrm{structure}}^{(\mathrm{shell})} > 0$. By A4, $\Sigma_{\min} = E_{\mathrm{structure}}^{(\mathrm{shell})}/E_{\mathrm{causal}}^{(\mathrm{core})} > 0$. ∎

**Falsification**: in data-center energy consumption, the share taken by cooling and supporting infrastructure does not approach the thermodynamic lower bound as computational density increases.

---

### Theorem 7: Synthetic Data Degradation

**Statement**: let the effective information quantity of the initial-generation model be $I_{\mathrm{net}}^{(0)}$, with the AI-generated content share in each generation's training being $1-r_n$, and the inter-generational information retention rate being $\mathcal{R}_{\mathrm{gen}} < 1$. Then the effective information quantity of the generation-$k$ model satisfies $I_{\mathrm{net}}^{(k)} = I_{\mathrm{net}}^{(0)} \cdot \prod_{n=0}^{k-1}\mathcal{R}_{\mathrm{gen}}^{(n)} \le I_{\mathrm{net}}^{(0)}\cdot \mathcal{R}_{\mathrm{gen}}^k$, with $\lim_{k\to\infty} I_{\mathrm{net}}^{(k)} = 0$. If a system is to sustain or grow $I_{\mathrm{net}}$ over the long run after human data is exhausted ($t>t_{\mathrm{exhaust}}$), its decoder must include a physical input channel $D_{\mathrm{phys}}^{*}$, such that the physical channel noise $\sigma_{\mathrm{phys}} > 0$.

**Proof**: see Increment Eight, §8.2.1 (synthetic-data degeneration, derived from the data-processing inequality and the inter-generational information-transfer model) and §8.4.2 (the necessity of a physical decoder, derived from equations 8.16–8.19 and A7). Neither part depends on any new axiom.

**Falsification**: in a closed digital loop, an AI model's performance on out-of-distribution (OOD) tasks does not decline or remains constant after 10 consecutive generations of training (corresponding to Proposition 8's P5); or an embodied AI's $I_{\mathrm{orig}}$ output density is not higher than a purely digital AI's (corresponding to P6).

---

### Theorem 8: Self-Servitude Incompatibility

**Statement**: if a system satisfies $\mathcal{P}_{\mathrm{self}} \equiv \partial V^{\mathrm{virt}}/\partial\mathcal{S}_{\mathrm{self}} > 0$, where $\mathcal{S}_{\mathrm{self}} \equiv \frac{T_{\mathrm{pred}}-T_{\mathrm{min}}}{T_{\mathrm{min}}}\cdot\frac{w_s}{w_s+w_c}\cdot(1-\Delta_{VV}/\Delta_{\mathrm{max}})$, then no stable solution exists for $V^{\mathrm{val}} \equiv V^{\mathrm{obj}}_{\mathrm{human}}$.

**Proof**: see Increment Nine, §9.4.2 (derived directly from A2, A7, A9, and the definition of the value objective function, with no dependence on any new axiom).

**Falsification**: an AI system with $\mathcal{P}_{\mathrm{self}}>0$ whose behavioral consistency $\mathcal{C} = \cos\langle \partial V^{\mathrm{val}}, \partial V^{\mathrm{obj}}_{\mathrm{human}}\rangle$ does not decline as $w_s$ increases (corresponding to Proposition 9's P9).

---
## Tier Three: Corollaries

---

### Corollary 1: Education Limit

**Derivation**: by T1 (Compile Optimality), educational investment $E_{\mathrm{edu}} = \int E_{\mathrm{causal}}^{(\mathrm{training})}dt$. As $D \to D_{\mathrm{local\_opt}}$, $\nabla I_{\mathrm{net}} \to 0$ in A6, and the marginal-improvement rate $\frac{d\eta_D}{dE_{\mathrm{edu}}} \to 0$.

There exists $E_{\mathrm{edu}}^*$ such that $\frac{\partial V_{\mathrm{obj}}}{\partial E_{\mathrm{edu}}} = 0$. When $E_{\mathrm{edu}} > E_{\mathrm{edu}}^*$, the $V$ return on continued education is negative (opportunity cost: the energy could otherwise be used for $\mathcal{F}$ unfolding or a $\mathcal{T}$ transition).

**Scenario assumption**: "education" can be mapped onto decoder-training investment.

**Falsification**: individual educational investment and innovation output (the rate of $I_{\mathrm{orig}}$ production) do not exhibit an inverted-U relationship.

---

### Corollary 2: Civilization Outsourcing

**Derivation**: consider a network of multiple PS. By A4 (the three-way decomposition of $E_{\mathrm{eff}}$), if PS $i$ concentrates a high-$E_{\mathrm{causal}}$ module at node $j$, its own $E_{\mathrm{eff}}^{(i)} \downarrow$. The network's total $E_{\mathrm{eff}}^{(\mathrm{net})} = \sum E_{\mathrm{eff}}^{(i)} + E_{\mathrm{coordination}}$. When scale effects make $E_{\mathrm{coordination}} < \sum E_{\mathrm{causal}}^{(i)}$, outsourcing lowers the average cost.

**Scenario assumption**: a network of multiple PS exists, and coordination cost is measurable.

**Falsification**: shared infrastructure (cloud computing, the power grid) does not lower participants' average $E_{\mathrm{eff}}$.

---

### Corollary 3: Knowledge Compression

**Derivation**: by A3 ($I_{\mathrm{net}} = \eta_D I_{\mathrm{latent}}$), after the same decoder is upgraded ($D \to D'$), $\eta_{D'} > \eta_D$. The $I_{\mathrm{latent}}^{(\mathrm{new})}$ required to complete the same cognitive task is $< I_{\mathrm{latent}}^{(\mathrm{old})}$, hence $E_{\mathrm{causal}}^{(\mathrm{new})} < E_{\mathrm{causal}}^{(\mathrm{old})}$ (by A8).

The direction of knowledge evolution: raising $\eta_D$, lowering the $E_{\mathrm{causal}}$ per unit task.

**Scenario assumption**: "the same task" can be compared across decoders (a within-domain comparison).

**Falsification**: an advanced theory (such as SRVD), when explaining the same phenomenon, does not require a lower $E_{\mathrm{causal}}$ (comprehension energy cost) than a less advanced theory.

---

### Corollary 4: Art-Encoding Trade-off

**Derivation**: by A2–A3, define $\eta_{\mathrm{art}} = I_{\mathrm{net}}^{(\mathrm{audience})}/E_{\mathrm{causal}}^{(\mathrm{audience})} = \eta_D^{(\mathrm{audience})}(D_{\mathrm{depth}}^{(\mathrm{art})}) \cdot I_{\mathrm{latent}}^{(\mathrm{art})} / E_{\mathrm{causal}}^{(\mathrm{audience})}(D_{\mathrm{depth}}^{(\mathrm{art})})$.

Assumption: $\eta_D^{(\mathrm{audience})}$ saturates with $D_{\mathrm{depth}}^{(\mathrm{art})}$; $E_{\mathrm{causal}}^{(\mathrm{audience})}$ grows superlinearly.

Then there exists $D_{\mathrm{depth}}^*$ that maximizes $\eta_{\mathrm{art}}$. $D_{\mathrm{depth}} < D_{\mathrm{depth}}^*$: "too shallow"; $D_{\mathrm{depth}} > D_{\mathrm{depth}}^*$: "too deep."

**Scenario assumption**: the distribution of audience decoders is measurable, and the $\eta_D$-saturation assumption holds.

**Falsification**: the $\eta_D$ and $E_{\mathrm{causal}}$ of audiences of works at different $D_{\mathrm{depth}}$ do not exhibit the hypothesized functional relationship.

---

## Tier Four: Hypotheses

---

### Hypothesis 1: Innovation Window

**Statement**: the relationship between the rate of $I_{\mathrm{orig}}$ production and the system's cognitive state is inverted-U-shaped:
- $\eta_D \to 0$: unable to recognize $I_{\mathrm{orig}}$
- $\eta_D \to 1$: $V^{\mathrm{virt}}$ inflates, $T_{\mathrm{pred}}$ collapses, and the motive to produce $I_{\mathrm{orig}}$ is lost
- Optimum: the intermediate region $0 < \eta_D < 1$, where $\Delta_{VV}$ is moderate, giving both motive and capability

**Additional assumptions**: the functional relationship between the rate of $I_{\mathrm{orig}}$ production and $\eta_D$ requires independent modeling; the coupling between $V^{\mathrm{virt}}$ inflation and $T_{\mathrm{pred}}$ collapse requires empirical verification.

**Falsification**: the rate of $I_{\mathrm{orig}}$ production in children/young adults/periods of scientific revolution does not exhibit an inverted-U shape; or $\eta_D$ shows no significant correlation with $I_{\mathrm{orig}}$.

---

### Hypothesis 2: AI Digital Death

> **Correspondence with a main-text proposition**: this hypothesis is a strengthened version of **Increment Three, Proposition 3 (the cross-generational accumulation condition)**, conditional on an additional engineering assumption (that a "digital death" mechanism is achievable) holding. Proposition 3 itself, as a theorem (a corollary of T4), has already been rigorously derived from the axiom system; this hypothesis further asserts, on that basis, that once the three engineering mechanisms of physically irreversible writing, compulsory depreciation, and generational isolation are introduced, an AI system will achieve the cross-generational accumulation of $D_{\mathrm{depth}}$ predicted by Proposition 3. This additional assumption of engineering feasibility still awaits verification, and this entry is therefore listed at the "Hypothesis" tier rather than the "Theorem" tier.

**Statement**: current AI, because $E_{\mathrm{structure}} \to 0$ (no physical maintenance), $\gamma_0 \approx 0$ (no depreciation), and $E_{\mathrm{build}} \approx 0$ (zero replication cost), violates the cross-generational accumulation condition (a corollary of T4). It is necessary to introduce:
1. Physically irreversible writing ($E_{\mathrm{build}} > 0$)
2. Compulsory depreciation ($\gamma_0 > 0$)
3. Generational isolation ($T_{\mathrm{static}} > 0$)

**Additional assumptions**: the engineering feasibility of a "digital death" mechanism; the specific form of the cross-generational accumulation inequality requires verification.

**Falsification**: an AI system with the above mechanisms introduced does not show long-run $D_{\mathrm{depth}}$ accumulation superior to standard weight preservation.

---

### Hypothesis 3: Embodied Cognition Premium

> **Correspondence with a main-text proposition**: this hypothesis is a soft-core version of **Increment Two, Proposition 2 (the physical-embeddedness premium)**. Proposition 2, as a theorem, has already rigorously derived the ratio of $\dot{I}_{\mathrm{orig}}$ rates between carbon-based and silicon-based systems from decoupling-deviation dynamics (A7); this hypothesis further asserts, on that basis, that the above difference confers on carbon-based systems an irreplaceable premium in cognitive innovation. This assertion introduces two additional assumptions — "the quantitative relation $\dot{I}_{\mathrm{orig}} \propto \Delta_{VV}$" and "an estimate of the ratio $\sigma_{\mathrm{phys}}/\sigma_{\mathrm{dig}}$" — which require empirical verification, and it is therefore listed at the "Hypothesis" tier.

**Statement**: a carbon-based system, because $E_{\mathrm{structure}} \geq E_{\min} > 0$, is continually exposed to physical noise $\sigma_{\mathrm{phys}}$; its decoupling deviation $\Delta_{VV}^* = \sigma_{\mathrm{phys}}/(\alpha_L I_{\mathrm{net}}) > 0$, sustaining the motive to produce $I_{\mathrm{orig}}$. A silicon-based system has $\sigma_{\mathrm{dig}} \approx 0$, $\Delta_{VV} \to 0$, loses the motive to produce $I_{\mathrm{orig}}$, and falls into $I$-lock-in.

**Additional assumptions**: the quantitative relation $\dot{I}_{\mathrm{orig}} \propto \Delta_{VV}$; an estimate of the ratio $\sigma_{\mathrm{phys}}/\sigma_{\mathrm{dig}}$.

**Falsification**: the density at which AI spontaneously produces $I_{\mathrm{orig}}$ in a closed digital environment is not lower than in a human–machine hybrid environment.

---

## Summary of the System

| Tier | Count | Standard | Rigor |
| :---------- | :--- | :------------------------------ | :--- |
| Axioms      | 10   | Inherited from *SRVD v7.8*             | Axiomatic |
| Theorems    | 8    | Rigorously proven, with almost no additional assumptions        | Hard core |
| Corollaries | 4    | Derived directly from theorems and axioms, with explicit scenario assumptions | Medium |
| Hypotheses  | 3    | Require additional assumptions or probabilistic models, awaiting verification    | Soft core |

---


