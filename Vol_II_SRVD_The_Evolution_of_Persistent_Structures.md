# Volume II — Applications I: The Evolution of Persistent Structures

**Liang Ruifeng** (Independent Researcher) | June 2026

> **Positioning of this volume**: answers the question "how do persistent structures climb" — the thermodynamic directional mechanism by which complexity ascends from crystals to civilizations. This volume's core variables are inherited from *SRVD v7.8*; new auxiliary parameters are declared only in this volume's Chapter 0.

## Chapter 0 — Declaration of New Variables for This Volume

Building on the core variable system of *SRVD v7.8*, this volume introduces the following application-level auxiliary parameters. These variables are valid only within this volume and are not carried across volumes:

| Symbol | Definition | Dimension | First appears |
|:---|:---|:---|:---|
| $D_{\mathrm{depth}}$ | Constraint depth: $1 + \#\{\mathcal{T}\}$ | dimensionless | Chapter 2 |
| $\tau$ | Characteristic time of thermodynamic decay | s | Chapter 3 |
| $I_{\mathrm{eq}}$ | Equilibrium information level | bit | Chapter 3 |
| $\Lambda$ | Civilizational energy leverage: $E_{\mathrm{ext}}/E_{\mathrm{causal}}$ | dimensionless | Appendix B |
| $E_{\mathrm{ext}}$ | External energy flow controlled by the decoder | J | Appendix B |
| $\eta_{\Lambda}$ | Control efficiency: $\Lambda^{-1}$ | dimensionless | Appendix B |

> **Volume-internal convention**: the meanings of the symbols above are limited to this volume. If other volumes use symbols with the same name, their meanings may differ and are not commensurable with those here.

---

# The Evolution of Persistent Structures — A Thermodynamic Framework for the Ascent of Complexity

**Liang Ruifeng** (Independent Researcher) | 2026 | Academic preprint

> **Version note**: this paper is the first applications companion to the SRVD main paper (v7.8), with independent version number **SRVD-APP-Evolution v1.0**. All core variables, operators ($\mathcal{T}$, $\mathcal{F}$), and the elasticity inequality ($\alpha > \gamma > \beta$) are inherited from *SRVD v7.8* and are not re-derived. The two papers divide the labor in a complementary way: the main paper answers "how does a persistent structure persist?"; this paper answers "how does a persistent structure climb?"

## Abstract

Why do some physical structures remain in a crystalline state for a billion years, while others climb through a continuous hierarchy of complexity levels — from molecules to cells, and on to nervous systems and civilizations? Structure Recursive Viability Dynamics (SRVD) aims to answer the question "how does a persistent structure survive?" This paper is devoted to its complementary question: **why does a persistent structure become ever more complex over time, and what determines when a complexity transition occurs?**

We propose that the ascent of complexity is not teleological but thermodynamically constrained. The core argument has three parts. First, the information elasticity inequality $\alpha > \gamma > \beta$ (established in SRVD) implies that investment in structural information yields a superlinear return in the viability potential $V$, producing a directional bias toward evolving into information-dense configurations. Second, transitions between complexity levels occur only when three conditions are simultaneously satisfied: there exists a new decoder topology $D_{\text{new}}$ capable of extracting the paradigm-breaking signal $I_{\text{orig}}$; the environmental free-energy budget $E_{\text{available}}$ exceeds the one-time build cost $E_{\text{build}}$; and the wisdom leverage ratio $L = \Delta V / E_{\text{build}} > L_{\min}$. Third, most structures fail to climb because they are locked by $D$-lock-in ($\nabla D \to 0$), by energy lock-in ($E_{\text{build}} > E_{\text{available}}$), or because the marginal returns of the current decoder are not yet exhausted.

This framework inherits all of SRVD's variables and introduces no new variable. Its core new contribution is the unified information-evolution equation $dI/dt$, together with a falsifiable statement of the conditions under which a complexity transition occurs or fails.

## Chapter 1 — Introduction: The Question the Framework Left Unanswered

SRVD describes the dynamics of persistence: given an already-existing structure, what governs its viability potential, its collapse, and its behavioral pathologies? The theory deliberately remains agnostic about the question of origin — it assumes a persistent structure already exists and analyzes its fate. This leaves an antecedent question unanswered.

The observable universe contains an unmistakable directional signal: over cosmic time, matter organizes itself into configurations that are successively more complex, more information-dense, and more causally capable. Crystals preceded organic chemistry. Single cells preceded nervous systems. Nervous systems preceded language. Language preceded artificial computation. Each transition was a low-probability event, each took millions or billions of years to cross, and yet this sequence is real and evidently non-random.

Existing frameworks each capture a part of this phenomenon. Prigogine's theory of dissipative structures shows how energy flow can produce local order in simple systems, but cannot explain the accumulation of functional complexity across generations. Kauffman's autocatalytic sets explain the origin of self-replication but do not address the climb after origin. Chaisson's energy rate density records the monotonic increase in energy flow per unit mass from galaxies to brains, but has been criticized for conflating necessary and sufficient conditions: energy flow is necessary, but by itself cannot explain why, given an equal energy budget, some structures develop intelligence and others do not. WBE metabolic scaling theory provides precise quantitative predictions within the biological domain but does not extend to the chemical or cultural level. Assembly theory provides an operational measure of molecular complexity but does not provide a dynamical mechanism.

The gap these frameworks jointly leave is precisely this: **what is the thermodynamic mechanism that biases complexity upward, and what determines whether a given structure can cross a particular threshold?**

SRVD supplies the missing components — a unified accounting of information, energy, time, and decoder dynamics — but has not yet assembled them into an explicit theory of ascent. This paper does exactly that.

## Chapter 2 — Theoretical Background: What SRVD Already Contains

Before introducing new synthesis, we establish the SRVD components that scaffold a theory of complexity ascent. All symbols strictly follow the definitions of *SRVD v7.8*.

### 2.1 The Viability Potential and Its Two Channels

SRVD's core metric is the viability potential:

$$
\boxed{
\displaystyle
V_{\mathrm{obj}} = \underbrace{\frac{I_{\mathrm{struct}} \cdot T_{\mathrm{static}}}{E_{\mathrm{structure}}}}_{V_s \text{ (structural channel)}} + \underbrace{\frac{I_{\mathrm{net}} \cdot T_{\mathrm{pred}}}{E_{\mathrm{causal}}}}_{V_c \text{ (cognitive channel)}}
}
$$

The structural channel $V_s$ captures the viability potential of passive structures — those that maintain themselves by resisting entropy increase through an energy barrier. The cognitive channel $V_c$ captures the viability potential of active structures — those that maintain themselves by predicting the environment and steering energy flow. The transition from $V_c = 0$ to $V_c > 0$ is the most fundamental discontinuity in the history of matter: the emergence of active persistence.

### 2.2 The Elasticity Inequality: $\alpha > \gamma > \beta$

The SRVD framework requires that the elasticity exponents of the viability potential with respect to information, energy, and time satisfy $\alpha > \gamma > \beta > 0$, a result of the second law of thermodynamics and the three-tiered hierarchy of resource scarcity. Information (ordered structure) is the scarcest resource in a universe tending toward maximum entropy; energy is abundant but must be actively acquired; time is passively conferred and cannot be produced.

The implication of this inequality is that, other things being roughly equal, investment in information carries the highest theoretical marginal return. Formally:

$$
\boxed{
\displaystyle
\frac{\Delta V}{V} \approx \alpha \cdot \frac{\Delta I}{I} + \beta \cdot \frac{\Delta T}{T} - \frac{\Delta E_{\mathrm{eff}}}{E_{\mathrm{eff}}}
}
$$

However, what evolution truly optimizes is always the viability potential $V$ itself, not the quantity of information $I$. $\alpha > \gamma > \beta$ only states that, at comparable opportunity cost, the $I$ route carries the highest long-run marginal return — it does not mean every lineage must prioritize increasing information. In fact, a structure can maximize $V$ along any of three fundamental routes:

| Route | Mechanism | Typical case |
| :-------------------------- | :---------------------------------- | :----------------------------- |
| **The $I$ route (complexification)** | Raise $I_{\mathrm{net}}$, pushing up the theoretical ceiling of $V$ | Nervous systems, language, civilization, AI |
| **The $T$ route (longevization)** | Extend $T_{\mathrm{pred}}$ or $T_{\mathrm{static}}$ | Pine trees, sea turtles, naked mole rats, seed dormancy |
| **The $\gamma$ route (energy economization)** | Lower $E_{\mathrm{eff}}$ | Parasites, cave fish, deep-sea organisms, hibernation |

The three routes are jointly filtered by local thermodynamic constraints and are not mutually exclusive. For a sea turtle, the cost $\Delta E \gg \Delta I$ of developing a complex nervous system would yield $\Delta V < 0$; going directly by the $T$ route instead produces a larger $V$. The naked mole rat suppresses $E_{\mathrm{survival}}$ through social division of labor, achieving high $V$ via the $\gamma$ route as well. Plant dormancy barely changes $I$ at all — merely lowering $E$ and extending effective $T$ is enough to make $V$ surge. This is not a failure of evolution, but different solutions of the $\max V$ principle under different constraint geometries.

There is a second-order mechanism underlying why the $I$ route forms a statistical advantage over long-run competition: a high-$I$ structure not only raises the growth rate of $V$, it also continually accumulates a larger stock of $V_{\mathrm{obj}}$. Under a negative-information shock $I^-$ of the same magnitude, a system with a higher stock suffers a smaller relative loss $\Delta V / V_{\mathrm{obj}}$ — a thousand-year-old tree can lose 30% of its branches and survive, while a sapling dies outright; a mature ecosystem can recover from local disturbance, while a newly established one tends to collapse. The $T$ route and the $\gamma$ route can equally optimize $V$ under local constraints, but because $\alpha > \gamma > \beta$, they accumulate a stock of $V_{\mathrm{obj}}$ structurally more slowly than the $I$ route does. Complexity ascent thus manifests as a long-run statistical trend, not as an information-first strategy that every species or every stage must follow: once a lineage sets out on the $I$ route, its $V_{\mathrm{obj}}$ stock grows ever thicker, its capacity to withstand $I^-$ grows ever stronger, and this further drives the continued accumulation of $I$, forming a positive feedback loop.

### 2.3 Decoders, Topology, and Paradigm-Breaking Information

SRVD defines the decoder $D$ as the physical mechanism by which a persistent structure extracts net effective causal information $I_{\mathrm{net}} = \eta_D \cdot I_{\mathrm{latent}}$ from the environment. Decoder quality is characterized by the decoding efficiency $\eta_D \in [0,1]$ and the maximum information capacity $I_{\max}(D)$.

Two operators govern how a decoder changes:

**Recursive unfolding $\mathcal{F}(D)$**: the same decoder replicates its rule across multiple scales. The structure grows larger or denser under the same information-extraction logic. No new causal dimension is opened.

**Topological transition $\mathcal{T}(I_{\mathrm{orig}})$**: absorbs the paradigm-breaking signal $I_{\mathrm{orig}}$, triggering structural reorganization and opening a new causal dimension. By definition, $D_n(I_{\mathrm{orig}}) \approx 0$ (the current decoder cannot effectively extract this signal), while $\exists D_{n+1}: D_{n+1}(I_{\mathrm{orig}}) \gg 0$ (the new decoder can). A topological transition requires a one-time build cost $E_{\mathrm{build}}$ and produces $I_{\max}(D_{n+1}) > I_{\max}(D_n)$.

**The formal structure of $\mathcal{F}$**: the minimal mathematical form of the recursive-unfolding operator $\mathcal{F}$ is:

$$
S_{n+1} = \mathcal{F}(S_n,\, \lambda)
\tag{EPS.0}
$$

where $S_n$ is the structural state of generation $n$, and $\lambda$ is a control parameter jointly constrained by $E_{\mathrm{causal}}$ and $I_{\mathrm{net}}$. When $\mathcal{F}$ is invariant under scale transformation, the structure exhibits fractal self-similarity — the same information-extraction rule is recursively replicated across scales. This explains why an organism's branching networks (alveoli, vascular trees, dendritic trees) emerge together with WBE metabolic scaling laws: both are physical manifestations of $\mathcal{F}$'s scale invariance under energy constraint. A $\mathcal{T}$ event corresponds to a discrete jump in $\lambda$, breaking the old scale invariance and establishing a new generative rule.

### 2.4 The Constraint-Depth Variable $D_{\mathrm{depth}}$

Every topological transition $\mathcal{T}$ adds one layer of constraint to a structure. Constraint depth:

$$
\boxed{
\displaystyle
D_{\mathrm{depth}} = 1 + \#\{\mathcal{T}\}
}
$$

counts the number of independent rule layers a structure must simultaneously maintain in order to persist. $D_{\mathrm{depth}}$ is historically cumulative (the layer-conservation law $D_{\mathrm{depth}}^{(n)} = D_{\mathrm{depth}}^{(n-1)} + 1$) and is orthogonal to $I_{\mathrm{struct}}$: a structure can be large (high $I_{\mathrm{struct}}$) but shallow (low $D_{\mathrm{depth}}$ — an octopus, for instance, which underwent extensive $\mathcal{F}$-unfolding after one major transition), or deep without necessarily being large.

### 2.5 The Type–Token Separation as a Prerequisite for Complexity

SRVD establishes the type–token distinction: a type is an inheritable information template (the stable component of $I_{\mathrm{struct}} + I_{\mathrm{latent}}$), while a token is a concrete physical individual ($I_{\mathrm{active}} + I_{\mathrm{struct}}$). The evolutionary chain from rocks (no separation) to RNA (primitive separation) to multicellular organisms (type and token diverge) to digital entities (template and instantiation fully separated) represents the progressive decoupling of an information pattern from any particular physical substrate.

This decoupling is not merely descriptive. It is the thermodynamic precondition for every major transition: without an inheritable template, selection cannot accumulate information across generations; without a separation of template from token, complexity is bounded by the lifespan of a single physical carrier.

## Chapter 3 — The Unified Information-Evolution Equation

The components above can now be assembled into a single dynamical equation describing the evolution of information in a persistent structure:

$$
\boxed{
\displaystyle
\frac{dI}{dt} = \underbrace{\mathcal{F}(D)}_{\text{recursive unfolding}} + \underbrace{\mathcal{T}(I_{\mathrm{orig}}) \cdot \delta(t - t_{\mathrm{jump}})}_{\text{topological transition}} - \underbrace{\frac{1}{\tau}(I - I_{\mathrm{eq}})}_{\text{thermodynamic decay}}
}
\tag{EPS.1}
$$

**First term — recursive unfolding $\mathcal{F}(D)$**: continuous information growth under the current decoder. The rate of unfolding is bounded by $I_{\max}(D)$; as $I \to I_{\max}(D)$, the marginal return of $\mathcal{F}$ tends to zero. Crystals, viruses, and replicating molecules operate chiefly through $\mathcal{F}$.

Correction note: the original text left $\mathcal{F}(D)$ at a purely qualitative description ("bounded by $I_{\max}(D)$") without giving any computable form, making equation (EPS.1) difficult to use for numerical simulation or empirical fitting. A minimal-order parameterized implementation is added here for future empirical work to reference.

> **A minimal-order parameterization of $\mathcal{F}(D)$**: the simplest computable form of $\mathcal{F}(D)$ is capacity-limited logistic growth:
>
> $$\mathcal{F}(D) = \mu_{\mathcal{F}} \cdot I \cdot \left(1 - \frac{I}{I_{\max}(D)}\right)$$
>
> where $\mu_{\mathcal{F}} > 0$ is the unfolding-rate parameter (s⁻¹), jointly determined by decoder type and environmental conditions. This form has three natural properties: (1) the unfolding rate is zero at $I = 0$ (no information, no unfolding); (2) the unfolding rate tends to zero as $I \to I_{\max}(D)$ (a saturation constraint); (3) $I_{\max}(D)$ is reset to a higher value after each $\mathcal{T}$ transition, corresponding to the new capacity ceiling after topological expansion. Each special case in Appendix B (passive crystals, replicating molecules, $D$-locked-in systems) is a degeneration of this parameterized form under different parameter values or limiting conditions: in a passive crystal, $\mu_{\mathcal{F}} \to 0$; in a $D$-locked-in system, $I \to I_{\max}(D)$ drives the unfolding rate to zero.
>
> **Note**: the logistic form above is an "illustrative minimal-order approximation, not unique." The specific functional form of $\mathcal{F}(D)$ for different system types (molecular replication, neural networks, social organizations) needs to be calibrated against within-domain data; the framework itself does not presuppose a single implementation.

**Second term — topological transition $\mathcal{T}(I_{\mathrm{orig}}) \cdot \delta(t - t_{\mathrm{jump}})$**: a discrete, instantaneous jump at the moment $t_{\mathrm{jump}}$ when $I_{\mathrm{orig}}$ is absorbed and the structure undergoes a $D$-topological reorganization. This term is zero at every instant except the moment of transition, but its effect is permanent: it resets the ceiling $I_{\max}(D)$ to a higher value and adds one to $D_{\mathrm{depth}}$. Punctuated-equilibrium evolution, the Cambrian explosion, the origin of language — all correspond to large $\mathcal{T}$ events.

**Third term — thermodynamic decay $-\frac{1}{\tau}(I - I_{\mathrm{eq}})$**: absent active maintenance, any ordered structure decays, with characteristic time $\tau$, toward the equilibrium information level $I_{\mathrm{eq}}$ (the disordered state of the thermal background). This term is always active and sets the minimum energy requirement for persistence. A purely passive structure ($E_{\mathrm{causal}} = 0$) is governed by this term alone, and will decay unless its $E_{\mathrm{barrier}}$ is large enough to suppress the decay rate.

**This equation unifies the passive and active states:**

For an ordinary crystal: $\mathcal{F}(D) \approx 0$ (no active decoder), $\mathcal{T}$ events are negligible, and the decay term is suppressed by $E_{\mathrm{barrier}}$. The structure persists passively at an approximately constant $I$.

For an actively evolving organism: all three terms are operative. The first two drive $I$ upward; the third imposes a thermodynamic maintenance cost that must be met by $E_{\mathrm{survival}} + E_{\mathrm{causal}}$.

For a system in $D$-lock-in: $\mathcal{F}(D) \to 0$ (the decoder is saturated), $\mathcal{T}$ is blocked (insufficient $E_{\mathrm{build}}$ or no available $I_{\mathrm{orig}}$), and only the decay term drives the dynamics. The structure stagnates or erodes slowly.

**A bridge to dynamical systems theory**: equation (EPS.1) can be regarded as a recursive dynamical system corrected by thermodynamic dissipation, in which the $\mathcal{F}$ term corresponds to continuous-time attractor dynamics and the $\mathcal{T}$ term corresponds to bifurcation events. From the perspective of dynamical systems, the sequence of complexity ascent is a bifurcation cascade gated by energy: each $\mathcal{T}$ event corresponds to the system jumping from one attractor basin to a new basin with a fundamentally different topological structure. These three transitions are jointly gated by the three conditions of Chapter 4, which form a causal chain rather than a parallel relation: $I_{\mathrm{orig}}$ supplies the direction of bifurcation (which new basin the system will jump to); $E_{\mathrm{available}}$ supplies the energy for bifurcation (whether the system has enough energy to cross the barrier); and $L > L_{\min}$ supplies the net-benefit criterion (whether the new basin's $V$ is genuinely higher than the old one's, making the transition thermodynamically worthwhile). Absent any one of the three, the bifurcation does not occur. This correspondence provides an entry point for formally connecting the SRVD framework to cybernetics and nonlinear dynamics, but that development belongs to an independent line of research and is outside the scope of this paper.

## Chapter 4 — The Three Conditions for a Complexity Transition

From equation (EPS.1) and the definitions of the core variables, the necessary and sufficient conditions for a topological transition $\mathcal{T}$ to occur are:

**Condition 1 — signal availability**: a paradigm-breaking signal $I_{\mathrm{orig}}$ must exist in the environment, such that the current decoder cannot extract it ($D_n(I_{\mathrm{orig}}) \approx 0$), but the reorganized decoder can ($D_{n+1}(I_{\mathrm{orig}}) \gg 0$). This condition is not under the structure's control; it depends on the informational environment.

**Condition 2 — energy availability**: the one-time build cost must not exceed the available free-energy budget:

$$
\boxed{
\displaystyle
E_{\mathrm{build}}(D_{n+1}) < E_{\mathrm{available}}
}
$$

This is a hard physical threshold. It explains why most organisms never transition to the next complexity level: the energy cost of reorganizing the decoder is typically several orders of magnitude larger than the cost of running the current decoder. The emergence of a nervous system requires the prior existence of a high-metabolism organism capable of sustaining the build cost.

**Condition 3 — wisdom leverage**: the gain in viability potential from the transition must exceed a minimum threshold relative to its cost:

$$
\boxed{
\displaystyle
L = \frac{V(D_{n+1}) - V(D_n)}{E_{\mathrm{build}}} > L_{\min}
}
$$

where $L_{\min}$ is the context-dependent minimum required leverage ratio. This condition captures competitive pressure: in an environment where the current decoder's performance is still yielding returns (i.e., $I < I_{\max}(D_n)$), the system has no thermodynamic incentive to bear the cost and risk of reorganization. Only when the marginal return of the current decoder tends to zero, and Conditions 2 and 3 are simultaneously satisfied, does a transition become possible.

**Why most structures remain at their current complexity level:**

| Failure mode | Mechanism | Example |
| :----------- | :----------------------------------------------------------- | :----------------------------------------------------- |
| **$D$-lock-in** | $\nabla D \to 0$: the decoder gradient is saturated, but $E_{\mathrm{build}} > E_{\mathrm{available}}$ blocks the transition | The horseshoe crab (unchanged for 450 million years); cave fish after losing their visual decoder |
| **Missing signal** | No $I_{\mathrm{orig}}$ available in the current niche | Sessile deep-sea organisms in a stable environment |
| **Energy ceiling** | $E_{\mathrm{build}}$ exceeds the maximum available free energy $E_{\max}$ | Ectotherms with a conservative energy budget |
| **Insufficient leverage** | $L < L_{\min}$: the current decoder still yields a positive return | Organisms in a highly stable, resource-rich environment, where the existing strategy remains optimal |

## Chapter 5 — The Sequence of Ascent: The Transfer of Energy Dominance

Across the history of matter's organization, every major complexity transition corresponds to a shift in the dominant component of effective energy consumption $E_{\mathrm{eff}} = E_{\mathrm{barrier}} + E_{\mathrm{survival}} + E_{\mathrm{causal}}$.

### 5.0 Clarifying the Direction of "Order": The Crystal Route and the Life Route

Before discussing the sequence of complexity ascent, a key distinction must be clarified: the order of a crystal and the order of a living/organic system are not different "amounts" of the same kind of order, but **two mechanisms of order pointing in entirely opposite directions**.

A crystal's order is achieved through **averaging** — vast numbers of atoms occupy identical periodic positions, and the structure is passively locked by a deep energy barrier $E_{\mathrm{barrier}}$. Once formed, a crystal tends toward stasis; its persistence strategy essentially "goes along with" the second law of thermodynamics: no resistance, no flow, stability maintained by staying still. This is a type of order defined by **maximizing symmetry**.

The order of organic matter and life, by contrast, is achieved through **differentiation** — DNA replication, protein folding, and cell-signaling pathways each perform their own distinct role, with each module structurally and functionally different. This order is actively maintained by a sustained energy flow $E_{\mathrm{survival}}$; the moment that flow is interrupted, the structure disintegrates immediately. Life must "keep moving" in order to persist; its persistence strategy "collides head-on" with the second law of thermodynamics: locally resisting entropy increase, maintaining structure through sustained dissipation. This is a type of order defined by **maximizing symmetry-breaking**.

Though the two share the same $V$ formula, they fall on different ends of the dual channel:

$$
\boxed{
\displaystyle
V_s = \frac{I_{\mathrm{struct}} \cdot T_{\mathrm{static}}}{E_{\mathrm{barrier}} + E_{\mathrm{survival}}} \quad \text{(crystal type: persists through stasis)}
}
$$

$$
\boxed{
\displaystyle
V_c = \frac{I_{\mathrm{net}} \cdot T_{\mathrm{pred}}}{E_{\mathrm{causal}}} \quad \text{(life type: persists through flow)}
}
$$

The transition from crystal to life is not "from less order to more order," but **a switch from one type of order to an entirely opposite type of order**. Once a living system has switched on $E_{\mathrm{survival}}$ to sustain $I_{\mathrm{net}}$, it can never return to a crystal-type state maintained by $E_{\mathrm{barrier}}$ alone — because a break in the flow means disintegration. The root of this irreversibility lies in the fundamental thermodynamic difference between $E_{\mathrm{barrier}}$ and $E_{\mathrm{survival}}$: the former is a "one-time lock-in," the latter a "continuous-flow maintenance."

The evolutionary-historical implication of this distinction is: **once organic matter set out in the direction opposite to crystals, it has never turned back and never been interrupted.** Over billions of years, life has not degenerated into crystal; instead it has continually climbed in the direction $E_{\mathrm{survival}} \to E_{\mathrm{causal}}$, with every topological transition $\mathcal{T}$ increasing the share of $E_{\mathrm{causal}}$, never reversing.

| Stage | Key transition | $I$ state | Energy dominance | New capability |
| :------------ | :------------------ | :---------------------------------------------------- | :-------------------------------------------------------- | :--------------------- |
| **Lattice** | Inorganic initial order | $I_{\mathrm{struct}} > 0$, $\eta_D \approx 0$ | $E_{\mathrm{barrier}}$ (passive-barrier lock-in) | Stable structure |
| **Organic chemistry** | Inorganic $\to$ organic | $I_{\mathrm{struct}}$ expands | $E_{\mathrm{barrier}} + E_{\mathrm{survival}}$ (active maintenance begins) | Chemical diversity |
| **Single cells** | Molecule $\to$ self-maintaining | $I_{\mathrm{struct}}$ expands explosively; $I_{\mathrm{net}}$ appears | $E_{\mathrm{survival}} + E_{\mathrm{causal}}$ (metabolism + information processing) | Self-replication, autopoiesis |
| **Multicellularity** | Independent $\to$ divided labor | $I_{\mathrm{net}}$ expands through communication | $E_{\mathrm{survival}} + E_{\mathrm{causal}}$ (communication cost rises) | Specialization and cooperation |
| **Nervous systems** | Reaction $\to$ prediction | $I_{\mathrm{net}}$ grows exponentially; $T_{\mathrm{pred}} > 0$ appears | $E_{\mathrm{causal}}$ share rises sharply | Prediction and planning |
| **Language/civilization** | Individual $\to$ collective memory | $I_{\mathrm{orig}}$ injected; $I_{\mathrm{net}}$ externalized | $E_{\mathrm{causal}}$ becomes the dominant cost | Cumulative cultural knowledge |
| **Artificial computation** | Biological $\to$ silicon-based recursion | $I_{\mathrm{net}}$ recursively explodes | $E_{\mathrm{causal}}$ dominates; runaway risk emerges | High-speed learning, recursive self-improvement |

Two structural regularities run through this sequence:

**The transfer of energy dominance**: the dominant energy component shifts from $E_{\mathrm{barrier}}$ (passive, zero maintenance) to $E_{\mathrm{survival}}$ (active metabolic maintenance), and then to $E_{\mathrm{causal}}$ (information processing and predictive computation). Each transfer increases vulnerability to supply interruption, but also raises the achievable ceiling of $V$. Note: this sequence describes the transfer of energy dominance experienced by lineages that take the $I$ route; it does not mean all lineages evolve along this route. Lineages that choose the $T$ route or the $\gamma$ route (pine trees, sea turtles, parasites) equally satisfy the $\max V$ principle, merely converging to a different local optimum under a different constraint geometry.

**The decoder–execution flywheel**: every upward transition creates a positive-feedback loop. A stronger decoder ($\eta_D \uparrow$) extracts more effective information ($I_{\mathrm{net}} \uparrow$), enabling more efficient execution of survival behavior. More efficient execution expands the range of environments the structure can inhabit, exposing it to new $I_{\mathrm{orig}}$ signals, and generating further pressure to upgrade the decoder. This flywheel explains the acceleration in the pace of transitions: each additional level of $D_{\mathrm{depth}}$ makes the next transition easier to initiate.

**A note on animal diversity**: this table does not list insects, birds, and mammals as separate levels, because they share the same underlying decoder type — the neural predictive decoder — differing in $I_{\mathrm{struct}}$ configuration and $D$-topological depth rather than in decoder kind. Cross-species comparison requires locking the same decoder domain and state-space substrate.

## Chapter 6 — Constraint Depth, Information Geometry, and the Limits of Linear Ranking

### 6.1 Why Linear Complexity Ranking Fails

The intuition that "a human is more complex than a bacterium" is right in one sense and wrong in another. Classical information theory attempts to assign a single number $I = \log_2 \Omega$ to any structure and rank structures linearly. This fails, because the state spaces of different systems are fundamentally incommensurable: $\Omega_{\mathrm{crystal}} \neq \Omega_{\mathrm{DNA}} \neq \Omega_{\mathrm{language}}$.

This failure is not merely technical. It reflects a real structural fact: different levels of the evolutionary hierarchy occupy different dimensions of information space, not merely different positions along a single axis.

### 6.2 A Three-Axis Structural Coordinate System

The correct geometry is multidimensional. The informational organization of a persistent structure is characterized by three independent coordinates:

$$
\boxed{
\displaystyle
I \;\rightarrow\; (I_{\mathrm{rule}},\; D_{\mathrm{depth}},\; F_{\mathrm{scale}})
}
$$

where $I_{\mathrm{rule}}$ is the complexity of the minimal generative rule, $D_{\mathrm{depth}}$ is the number of historical constraint layers simultaneously maintained, and $F_{\mathrm{scale}}$ is the scale at which the rule has been recursively unfolded. These three dimensions are orthogonal, with no single combination dominating all others:

| Structure | $D_{\mathrm{depth}}$ | $I_{\mathrm{struct}}$ | Note |
| :--- | :----------------- | :------------------ | :----------------------------------------- |
| Crystal | 1 (low) | high | A single rule, broadly deployed |
| Octopus | low | high | One major transition, then extreme $\mathcal{F}$ unfolding |
| Human | high (10+) | high | Multiple stacked constraints + complex internal topology |
| Bacterium | low | moderate | Ancient, but thermodynamically optimal at its own level |

This geometry resolves the apparent paradox of bacterial success: bacteria are not "primitive failures" — they are a low-$D_{\mathrm{depth}}$, low-maintenance optimum that has dominated Earth's biomass for billions of years. Under their ecological conditions, their $V$ may exceed that of far more complex organisms. Complexity ascent is not universally advantageous; it is context-dependent.

### 6.3 Hard Limits on Cross-Domain Quantification

A direct consequence of this multidimensional geometry is that absolute cross-domain quantitative comparison is currently infeasible. The $I_{\mathrm{struct}}$ values of DNA sequences, neural-network parameters, and social institutions are measured under incommensurable protocols. The operational boundary is therefore:

**Within-domain**: when the same decoder substrate $D$ and state space $\Omega$ are locked, relative quantitative comparison is valid. Different generations of AI systems, brain structures of different species with the same neural architecture, organisms within the same phylum — these all permit rigorous within-domain scaling laws (as demonstrated by WBE's proof for metabolic rate).

**Cross-domain**: only qualitative structural comparison can be guaranteed. One can assert that a nervous system has a higher $D_{\mathrm{depth}}$ than a single-celled organism, without claiming a specific $I$ ratio.

**Prohibited**: precise cross-domain numerical rankings such as "human brain = $10^{15}$ bits, bacterium = $10^6$ bits" cannot be falsified under current measurement protocols and should not appear in quantitative predictions.

## Chapter 7 — The Evolutionary Tree Has No Predetermined Peak

### 7.1 Evolution Is Gradient Search, Not Progress

A persistent temptation is to read the evolutionary sequence teleologically — as if nature were building toward a destination. SRVD and the present framework reject this reading. Evolution is a gradient search in $V$-space: structures that achieve a higher viability potential under their local thermodynamic constraints are statistically more likely to persist. There is no goal; there is only a gradient.

This has two implications. First, $D_{\mathrm{depth}}$ can decrease as well as increase: when the cost of maintaining a constraint layer exceeds its contribution to $V$, that layer is shed. A parasite simplifies its morphology when its host bears the metabolic burden. Cave fish lose their visual organs when photon signals in the environment carry no $I^+$. These are not "degenerations" — they are correct local optimizations under the thermodynamic mandate $\max(V)$. Formally:

$$
\boxed{
\displaystyle
\mathcal{T}^{-}: \quad \Delta D_{\mathrm{depth}} = -1 \quad \text{when} \quad \frac{\partial V}{\partial D_{\mathrm{depth}}} < 0
}
$$

The evolutionary sequence is therefore bidirectional:

$$
\cdots \xrightarrow{\mathcal{T}} \mathcal{F} \xrightarrow{\mathcal{T}} \mathcal{F} \cdots \quad \text{(ascent)}
$$

$$
\cdots \xrightarrow{\mathcal{T}^{-}} \mathcal{F}^{-} \xrightarrow{\mathcal{T}^{-}} \cdots \quad \text{(simplification)}
$$

Direction is determined by the $V$ gradient, not by any notion of progress.

### 7.2 The Current Position of Humanity

Within the SRVD framework, the human species occupies a distinctive position: the first biological structure to externalize its decoder ($D$) on a large scale into a non-biological substrate (writing, mathematics, computation). This externalization represents a topological transition potentially of the same order of magnitude as the emergence of the nervous system — it breaks the constraint that $D_{\mathrm{depth}}$ is bounded by individual biological lifespan and genetic bandwidth.

The ongoing shift toward artificial computational systems is not, within this framework, a replacement of biological intelligence, but a further externalization of the decoder: the build cost $E_{\mathrm{build}}$ of the next decoder layer is being distributed across global computing infrastructure. Whether the wisdom-leverage standard ($L > L_{\min}$) is satisfied — whether the viability-potential gain of this transition exceeds its build and alignment costs — remains a core open empirical question in AI development.

This transition reveals a fundamental divergence between $I_{\mathrm{struct}}$ and $I_{\mathrm{net}}$. Dinosaurs at the end of the Cretaceous possessed extremely high $I_{\mathrm{struct}}$ (highly complex body organization and niche adaptation), with a $V_{\mathrm{obj}}$ stock that was, within the ecosystems of the time, considerable — but $I_{\mathrm{net}}$ was extremely low, the system almost entirely passive. When the $I^-$ produced by the asteroid impact exceeded their $V_{\mathrm{obj}}$ stock, the buffer provided by high $I_{\mathrm{struct}}$ failed completely: a high stock raises the **threshold of resistance to shock**, not infinite immunity. The fundamental difference for humans is not a larger $I_{\mathrm{struct}}$, but that the externalization of $I_{\mathrm{net}}$ has given the system the capacity to **actively reshape how $I^-$ acts** — predicting an orbit, deflecting it in advance, or in extreme cases relocating the carrier. This is not increasing stock to absorb impact, but transforming a future $I^-$ from an unstoppable force into a controllable variable by extending $T_{\mathrm{pred}}$. In this sense, the externalization of $I_{\mathrm{net}}$ represents a topological transition $\mathcal{T}$ more fundamental than any expansion of $I_{\mathrm{struct}}$: what it changes is not how much impact the system can withstand, but whether an impact can be identified, predicted, and intervened upon before it happens.

### 7.3 The Thermodynamic Ceiling: An Endogenous Constraint on the Ascent of $I_{\mathrm{net}}$

Complexity ascent is threatened not only by external $I^-$ shocks, but also faces an endogenous thermodynamic constraint: every $\mathcal{T}$ transition requires a higher core **power density** (thermodynamic dissipation power per unit volume or unit mass, W/kg or W/cm²), and the ceiling of power density is hard-constrained by the physical medium's **heat-dissipation limit** ($P_{\mathrm{dissipation}}^{\max}$ — the maximum power at which the system can vent waste heat to its environment, jointly determined by the medium's thermal conductivity and geometric surface area). This produces a ceiling surface in each of two directions, $I_{\mathrm{struct}}$ and $I_{\mathrm{net}}$.

**The $I_{\mathrm{struct}}$ ceiling — the gravity tax**: as body mass increases, $E_{\mathrm{survival}}$ grows at a superlinear rate (verified within the biological domain by the WBE metabolic scaling law). When $\Delta E_{\mathrm{survival}} / \Delta I_{\mathrm{struct}}$ exceeds the elasticity threshold, the $V$ return from further enlarging the body turns negative. Dinosaurs, elephants, and large mammals may already have approached this line: the $E_{\mathrm{build}}$ required for $I_{\mathrm{struct}}$ to keep increasing exceeds the available energy budget, and Condition 2 (§4) is violated endogenously, not locked out by the external environment.

**The $I_{\mathrm{net}}$ ceiling — the heat-dissipation wall**: raising the power density of an information-processing core produces waste heat accumulating at a rate of at least $Q \geq k_B T \ln 2$ per bit (the Landauer lower bound). Dissipation capacity is bounded by the physical limits of material thermal conductivity and geometric surface area — this is not an engineering problem but a hard thermodynamic limit. The power density of the cerebral cortex ($\approx 10\ \text{mW/cm}^2$) and advanced GPU chips have each independently approached the heat-dissipation limits of their respective materials. Breaking through this wall requires a fundamental transition in physical medium (such as cryogenic superconducting computation), not iterative optimization of the current architecture.

**Civilizational mass distribution as empirical evidence**: this regularity has a direct material manifestation at civilizational scale. By 2020, the total mass of objects built by humanity had already exceeded global biomass, but the overwhelming majority of it consists of low-power-density concrete, asphalt, and metal structures. This "low-W/kg" matter is not redundant — it is the heat-dissipation shell and supporting armor for high-$I_{\mathrm{net}}$ cores, the physical manifestation of $E_{\mathrm{survival}}$. The "light core, heavy shell" structure of civilizational mass distribution is the form the $\mathcal{F}$ operator necessarily generates under energy constraint.

**The thermodynamic meltdown wall as a Great Filter**: if the heat-dissipation bottleneck cannot be broken by a transition in physical medium, a civilization will face a hard $\mathcal{T}$ threshold: $E_{\mathrm{build}}$ continues to rise while the gain in $I_{\max}(D_{n+1})$ saturates, violating Condition 3 ($L > L_{\min}$) — the net return of the transition no longer covers the build cost. This may be one thermodynamic form of the "Great Filter" in the Fermi paradox: after developing high-compute AI, a civilization's heat-dissipation bottleneck blocks any further $\mathcal{T}$ transition, and the system stabilizes at a high-power, finite state, or triggers a $V$ collapse due to local overheating. The only path past this filter, within the SRVD framework, is to find a new physical substrate in which $E_{\mathrm{build}}$ does not grow superlinearly with $D_{\mathrm{depth}}$ — this is precisely the thermodynamic essence of research into cryogenic computing, photonic computing, and quantum computing.

### 7.4 The Question of Extraterrestrial Intelligence

This framework implies that a more advanced extraterrestrial civilization need not be larger or more energetic. What it will have achieved is a higher $D_{\mathrm{depth}}$: more layers of stacked constraint, operating in causal dimensions currently inaccessible to human decoders. If detected, the signature of such a civilization would not be an anomalously large energy output, but an anomalously high assembly complexity — an organized structure that no known abiotic process could generate at that level of $D_{\mathrm{depth}}$.

Conversely, the failure to detect extraterrestrial intelligence does not imply that humans are the most complex structure in the universe. It may simply mean that the combination of conditions required for each $\mathcal{T}$ transition is rare enough that, within the current age of the observable universe, few structures have crossed the entire sequence of $D_{\mathrm{depth}}$ from chemistry to civilization.

## Chapter 8 — Dialogue with Existing Frameworks

This paper's core variables and dynamical equations are all inherited from *SRVD v7.8* (Liang, 2026). The following six external frameworks provide empirical support, historical precedent, or partial verification for this paper, but each has a theoretical gap that this paper attempts to fill.

| Framework | Support it provides for this paper | Gap this paper fills |
| :------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| Dissipative-structure theory (Prigogine) | Confirms that energy flow can produce local order, supplying a physical basis for the emergence of $V_c > 0$ from $V_c = 0$ | Does not address information accumulation across transitions, nor provide dynamics for decoder evolution |
| Autocatalytic sets (Kauffman, Eigen) | Establishes the specific chemical-level conditions for a single-cell $\mathcal{T}$ event | Confined to the moment of origin; does not provide dynamics for the climb after origin |
| Metabolic scaling theory (WBE) | Provides precise within-domain scaling laws in the biological domain, consistent with the $\alpha > \gamma > \beta$ ordering | A within-domain scaling law; does not extend across levels or to cultural evolution |
| Energy rate density (Chaisson) | Records the monotonic increase in energy flow per unit mass from galaxies to brains, consistent with the ascending sequence of the $E_{\mathrm{causal}}/E_{\mathrm{eff}}$ ratio | Energy is a necessary but not sufficient condition; does not explain why, given an equivalent energy budget, an information-dense configuration is selected |
| The Free Energy Principle (Friston) | Describes the steady-state optimization behavior of a decoder under fixed boundary conditions | Handles steady-state inference; does not handle $\mathcal{T}$ events (the dissolution and reconstruction of the boundary itself) |
| Assembly theory (Cronin, Walker) | Provides an operational complexity measure via the molecular assembly index, usable as an empirical proxy for $D_{\mathrm{depth}}$ | A static complexity measure; does not provide a dynamical equation or transition conditions driving complexity change |

**Division of labor with the SRVD main paper**: every variable, operator ($\mathcal{T}$, $\mathcal{F}$), the elasticity inequality ($\alpha > \gamma > \beta$), and the decoder definition in this paper are directly inherited from SRVD, without re-derivation. The two papers' questions are complementary: SRVD assumes a persistent structure already exists and asks "under what conditions does it persist or collapse"; this paper assumes a thermodynamic gradient already exists and asks "under what conditions does a structure climb to a new complexity level." The boundary of the division of labor is: SRVD is the dynamics of persistence, this paper is the dynamics of ascent; they share all variables and remain consistent across every area of overlap.

## Chapter 9 — Falsifiable Predictions

| Prediction | Test method | Falsification condition | Domain |
| :--- | :--- | :--- | :--- |
| **P1**: a complexity transition occurs only when all three conditions (Conditions 1–3, §4) are simultaneously satisfied | Collect transition cases with detailed energy-budget records from the literature on evolutionary biology and the chemistry of life's origin, and check case by case whether the estimated values of $E_{\mathrm{build}}$, $E_{\mathrm{available}}$, and $L$ satisfy the three conditions | A recorded transition shows $E_{\mathrm{build}} > E_{\mathrm{available}}$, or $L < L_{\min}$ | Evolutionary biology, origin-of-life chemistry |
| **P2**: the ratio $E_{\mathrm{causal}}/E_{\mathrm{eff}}$ increases monotonically across the evolutionary sequence within any lineage | Within a single lineage, compare neural-metabolic-share data (brain-to-body-mass ratio and basal metabolic rate) across different evolutionary stages (e.g., the developmental sequence of the vertebrate nervous system), testing the temporal monotonicity of $E_{\mathrm{causal}}/E_{\mathrm{eff}}$ | A later stage of some lineage allocates a smaller proportion to information processing than an earlier stage | Comparative neurophysiology |
| **P3**: $D$-lock-in (saturation of the decoder gradient before a transition) precedes extinction events at a statistically significant rate | Using phylogenetics combined with the fossil record, statistically compare the distribution of **morphological stasis periods** (as a proxy for $D$-lock-in: the time interval between the last morphological innovation and the last fossil record) between extinct lineages and a control group (the corresponding interval for surviving sister lineages), using the Mann-Whitney U test or survival analysis, requiring a sample size of $n \geq 20$ extinct lineages | Extinct lineages do not show morphological stasis prior to ecological $D$-lock-in (i.e., no significant difference in morphological stasis period between extinct and surviving lineages, $p > 0.05$) | Paleontology |
| **P4**: information elasticity $\alpha > 1$ holds within any domain in which the decoder substrate $D$ and state space $\Omega$ are locked | Within an AI model family sharing the same decoder architecture, using parameter count as a proxy for $I$ and training compute as a proxy for $E_{\mathrm{causal}}$, fit the scaling-law slope of $\log V \sim \alpha \log I$ | $\alpha \leq 1$ is observed within a domain satisfying the lock condition | Neuroscience (across developmental stages), AI scaling laws |
| **P5**: a negative topological transition $\mathcal{T}^{-}$ occurs preferentially after a constraint layer has sustained $\partial V / \partial D_{\mathrm{depth}} < 0$ for some period | In species with a documented record of morphological simplification (cave fish, parasites), track the temporal change in maintenance cost (e.g., metabolic rate, organ volume ratio) prior to the simplification event, testing whether simplification is accompanied by a decline in maintenance cost | A morphological-simplification event not accompanied by a corresponding decline in maintenance cost | Evolutionary biology (parasite evolution, cave faunas) |

## Chapter 10 — Open Problems and Limitations

**The origin of the first decoder**: the transition from $E_{\mathrm{causal}} = 0$ to $E_{\mathrm{causal}} > 0$ — the emergence of the first structure to actively process information rather than passively resist entropy — is not fully explained by the three conditions of §4. The first decoder cannot have been selected by any pre-existing selection process; its emergence is a fluctuation under an extreme energy gradient (hydrothermal vents, lightning-driven chemistry). This framework describes the dynamics of every subsequent transition but does not resolve the question of origin; that remains the domain of origin-of-life chemistry.

**Quantifying $E_{\mathrm{build}}$ and $L_{\min}$**: the transition conditions are stated as inequalities rather than equalities, because the specific values of $E_{\mathrm{build}}$ and $L_{\min}$ for any particular transition are difficult to measure retrospectively. This framework is qualitatively predictive; advancing toward quantitative prediction requires developing protocols for estimating these values from the fossil record, comparative genomics, and developmental biology.

**The AI transition**: the ongoing process of externalizing the human cognitive decoder onto an artificial computational substrate is the first transition in the evolutionary sequence to occur on a humanly observable timescale and under partial human control. Whether the wisdom-leverage condition is satisfied — whether the viability-potential gain of a human–machine hybrid system exceeds its build and alignment cost — cannot be determined in advance. SRVD's analysis of the Myopic Runaway Regime characterizes the failure mode; this framework characterizes the conditions for success.

**Consciousness and $I_{\mathrm{latent}}$**: current human cognitive science has an extremely low decoding efficiency $\eta_D$ for the internal causal structure ($I_{\mathrm{latent}}$) that constitutes consciousness and subjective experience. This is not a failure of the framework — $I_{\mathrm{latent}}$ exists independently of whether any decoder can extract it — but it means that the most important aspect of high-$D_{\mathrm{depth}}$ biological systems remains empirically opaque. Solving this problem, in the SRVD sense, is equivalent to constructing a decoder $D_{\mathrm{conscious}}$ with a high $\eta_D$ for the $I_{\mathrm{latent}}$ encoded in neural causal architecture.

## Chapter 11 — Conclusion

The evolution of persistent structures from crystals to civilizations is not mysterious. It is the predictable consequence of three thermodynamic facts: ordered information is the scarcest resource in an entropy-increasing universe ($\alpha > \gamma > \beta$); a decoder can be upgraded when energy is available and leverage is sufficient; and every upgrade resets the achievable ceiling of the viability potential.

Most structures do not climb. They reach a configuration in which the current decoder is saturated, transition energy is unavailable, or the competitive environment has not yet demanded it. They persist at their current complexity level — sometimes for geological ages — not as a failure, but as the local optimum under their thermodynamic constraints.

The universe has predetermined no destination for this process. The evolutionary sequence has no summit. It has only a gradient — $\max(V)$ along the direction of available $I_{\mathrm{orig}}$ — and the three conditions that govern whether any particular structure can follow it.

This framework inherits all of SRVD's variables and its commitment to falsifiability. Its core equation (EPS.1), the three transition conditions, and the five predictions constitute falsifiable empirical content. If the elasticity ordering $\alpha > \gamma > \beta$ is observed to fail within a locked domain, if a transition occurs without satisfying the three conditions, or if $D$-lock-in does not precede extinction at a rate higher than chance, this framework is falsified.

We do not claim to have solved the problem of complexity ascent. We claim to have provided a framework — thermodynamically grounded, variable-conservative, and falsifiable — within which this problem can be systematically studied. The tools already existed; what was missing was a common accounting language. SRVD and this paper together supply it.

---

## Appendix A — Variable Definitions and Units (Specific to *The Evolution of Persistent Structures*)

> This appendix lists every variable directly used in this paper (*The Evolution of Persistent Structures*). Core variables are inherited from *SRVD v7.8*, with consistent dimensions. This paper introduces no new variable.

---

### A.1 The $I$ Family (Information Family)

| Symbol | Definition | Unit |
| :------------- | :----------------------------------------------------------- | :--- |
| $I$ | Generalized structural difference: the total distinguishable, ordered difference of a persistent structure relative to its background (parent variable) | bit |
| $I_{\mathrm{struct}}$ | Structural information: the stock of intrinsic ordered information (lattice, DNA, chip layout, and other forms of physical order) | bit |
| $I_{\mathrm{net}}$ | Net effective causal information: $I_{\mathrm{net}} \equiv \eta_D \cdot I_{\mathrm{latent}}$, the effective information actually extracted by the decoder | bit |
| $I_{\mathrm{latent}}$ | Latent-configuration information: the stock of causal capacity currently unactivated but recoverable | bit |
| $I_{\mathrm{active}}$ | Activated causal information: the causal capacity currently in use, $I_{\mathrm{active}} \leq I_{\mathrm{net}}$ | bit |
| $I_{\mathrm{orig}}$ | Paradigm-breaking information: marginal causal efficacy decays extremely slowly; its value derives mainly from generating new structure | bit |
| $I_{\max}(D)$ | The maximum information capacity extractable by decoder $D$ | bit |
| $I_{\min}$ | Minimal self-cognition: the minimum amount of information required to maintain structural-identity continuity | bit |
| $I_{\mathrm{eq}}$ | Equilibrium information level: the amount of information corresponding to the disordered state of the thermal background | bit |

---

### A.2 The $E$ Family (Energy Family)

| Symbol | Definition | Unit |
| :---------------- | :----------------------------------------------------------- | :--- |
| $E_{\mathrm{eff}}$ | Equivalent thermodynamic cost: the complete physical cost a system pays to maintain its negentropic topological configuration | J |
| $E_{\mathrm{barrier}}$ | Barrier energy: a passive barrier, no ongoing dissipation, a one-time freeze | J |
| $E_{\mathrm{survival}}$ | Survival energy: active dissipation compensating for entropy increase, a continuous flow | J |
| $E_{\mathrm{causal}}$ | Causal-processing energy: the energy cost of running the decoder; $>0$ in the active phase, $\to 0$ in the passive phase | J |
| $E_{\mathrm{structure}}$ | Structural energy: $E_{\mathrm{barrier}} + E_{\mathrm{survival}}$, the minimum overhead required to keep a structure alive | J |
| $E_{\mathrm{flow}}$ | Flow energy: $E_{\mathrm{survival}} + E_{\mathrm{causal}}$, the budget for active maintenance and causal processing | J |
| $E_{\min}$ | The minimum energy required to maintain a structure (jointly determined by the Landauer limit and basic structural constraints) | J |
| $E_{\max}$ | The maximum total free energy available to the system (the upper limit of environmental supply) | J |
| $E_{\mathrm{thresh}}$ | Disintegration threshold: the energy ceiling beyond which irreversible damage is triggered | J |
| $E_{\mathrm{build}}$ | Build cost: the one-time physical energy required to create a new structure or upgrade an existing one | J |
| $E_{\mathrm{available}}$ | Available free-energy budget: the ceiling on energy the system can currently mobilize for a build cost | J |

---

### A.3 The $T$ Family (Time Family)

| Symbol | Definition | Unit |
| :------------- | :----------------------------------------------------------- | :--- |
| $T$ | Generalized structural viability duration; when unsubscripted, the parent variable of the time parameter | s |
| $T_{\mathrm{static}}$ | Static lifespan: the objective physical upper bound on persistence, determined by the structure's own thermodynamic stability | s |
| $T_{\mathrm{pred}}$ | Endogenous time horizon: the span of time over which the system plans for future states | s |
| $T_{\min}$ | Minimum physical or computational time grain (e.g., Planck time, clock cycle, limit of neural response) | s |
| $T_{\max}$ | The extreme upper bound on the persistence time of a system or environment (e.g., the age of the universe, a material's theoretical lifespan) | s |
| $\tau$ | Characteristic time of thermodynamic decay: the time constant with which a structure, absent active maintenance, decays toward equilibrium | s |

---

### A.4 The $V$ Family (Viability-Potential Family)

| Symbol | Definition | Unit |
| :-------------- | :----------------------------------------------------------- | :--------- |
| $V$ | Viability potential: a generalized, low-order-approximation measure of persistence efficiency, $V \approx I \cdot T / E$ | bit·s/J |
| $V_{\mathrm{obj}}$ | Objective viability potential: a thermodynamic assessment determined by actual energy–information–time parameters | bit·s/J |
| $V_s$ | Structural-channel viability potential: $V_s = I_{\mathrm{struct}} \cdot T_{\mathrm{static}} / E_{\mathrm{structure}}$ | bit·s/J |
| $V_c$ | Cognitive-channel viability potential: $V_c = I_{\mathrm{net}} \cdot T_{\mathrm{pred}} / E_{\mathrm{causal}}$ | bit·s/J |
| $V^{\mathrm{virt}}$ | Virtual viability potential: the system's internal model's subjective assessment of its own persistence efficiency | bit·s/J |
| $V^{\mathrm{val}}$ | Value objective function: the behavioral goal the system actually optimizes | bit·s/J |
| $V_{\max}$ | Niche viability-potential ceiling: the maximum viability efficiency the system can achieve within a given niche | bit·s/J |
| $\Delta_{VV}$ | Decoupling deviation: $|V^{\mathrm{virt}} - V_{\mathrm{obj}}|$ | bit·s/J |
| $r_v$ | Viability drive rate: $r_v = k \cdot V$, the rate at which potential is converted into actual growth momentum | s$^{-1}$ |

---

### A.5 The Decoder and Operator Family ($D$ / $\mathcal{F}$ / $\mathcal{T}$)

| Symbol | Definition | Unit |
| :------------------ | :----------------------------------------------------------- | :----- |
| $D$ | Decoder: the physical mechanism that extracts effective causal information from a persistent structure's latent configuration | — |
| $\eta_D$ | Decoding efficiency: $I_{\mathrm{net}} = \eta_D \cdot I_{\mathrm{latent}}$, $\eta_D \in [0,1]$ | dimensionless |
| $D_{\mathrm{depth}}$ | Constraint depth: the number of independent rule layers a structure must simultaneously maintain to persist, $D_{\mathrm{depth}} = 1 + \#\{\mathcal{T}\}$ | dimensionless |
| $\mathcal{F}$ | Recursive-unfolding operator: the same decoder replicates its rule at multiple scales, without opening a new causal dimension | — |
| $\mathcal{T}$ | Topological-transition operator: absorbs $I_{\mathrm{orig}}$, triggering structural reorganization and opening a new causal dimension | — |
| $\mathcal{T}^{-}$ | Negative topological transition: sheds one layer of constraint when $\partial V / \partial D_{\mathrm{depth}} < 0$ | — |
| $\Theta$ | Parameter space: the system-type-specific parameter set over which decoder evolution occurs | — |

---

### A.6 The Elasticity-Exponent Family

| Symbol | Definition | Unit |
| :--------- | :----------------------------------------------------------- | :------- |
| $\alpha$ | Information elasticity exponent: $\partial \ln V / \partial \ln I$, $\alpha > 1$ | dimensionless |
| $\beta$ | Time elasticity exponent: $\partial \ln V / \partial \ln T$, $\beta < 1$ | dimensionless |
| $\gamma$ | Energy elasticity exponent: $\partial \ln V / \partial \ln E_{\mathrm{eff}}$, normalized so that $\gamma = 1$ | dimensionless |

---

### A.7 Competition, Leverage, and Composite Indicators

| Symbol | Definition | Unit |
| :---------------- | :------------------------------------------------------- | :---------- |
| $\rho$ | Competitive pressure index: the average dissipation of systems competing within the same niche, divided by total available free energy | dimensionless |
| $L$ | Wisdom leverage coefficient: $L = \Delta V / E_{\mathrm{build}}$ | (bit·s/J)/J |
| $L_{\min}$ | Minimum required wisdom leverage: the threshold a transition must exceed | (bit·s/J)/J |
| $\mathcal{R}_e$ | Cognitive processing rate: $I_{\mathrm{net}} / T_{\mathrm{pred}}$ | bit/s |
| $\mathcal{L}_e$ | Cognitive lag coefficient: $T_{\mathrm{pred}} / I_{\mathrm{net}} = 1/\mathcal{R}_e$ | s/bit |
| $\gamma_0$ | Baseline depreciation rate: the natural rate of structural decay | s$^{-1}$ |
| $\chi$ | Coupling strength: the $I$–$V$ recursive coupling coefficient, dimension $[V]^{-1}$ | J/(bit·s) |

---

> **Note**: every variable in this paper is a direct inheritance of a variable already defined in *SRVD v7.8*; no new symbol is introduced. Dimensions are entirely consistent with Appendix A of the main paper. Variables carrying the $^{\mathrm{virt}}$ superscript (such as $V^{\mathrm{virt}}$, $I_{\mathrm{net}}^{\mathrm{virt}}$) are internal assessment values of the system, sharing the same dimension as their objective counterparts but not necessarily equal in value.


## Appendix B — The Unified $dI/dt$ Equation and Its Special Cases

Equation (EPS.1) is the general form. Its special cases reduce to the dynamics of standard physical and biological systems:

**A passive crystal**: $\mathcal{F}(D) = 0$ (no active decoder), $\mathcal{T} = 0$ (no transition under ordinary conditions). $\dfrac{dI}{dt} = -\dfrac{1}{\tau}(I - I_{\mathrm{eq}})$. Decay is suppressed by $E_{\mathrm{barrier}} \gg k_B T$, so that $\tau \to \infty$ and $I \approx \text{const}$.

**Replicating molecules (the RNA world)**: $\mathcal{F}(D) > 0$ (template-directed replication), $\mathcal{T}$ events are rare. The dynamics are dominated primarily by the competition between recursive unfolding and thermodynamic decay.

**An evolving organism under selection pressure**: all three terms are active. The $\mathcal{F}$ term drives intra-generational information accumulation; when the conditions of §4 are satisfied, $\mathcal{T}$ events drive transitions between levels; the decay term imposes a continuous metabolic-maintenance requirement.

**A $D$-locked-in system**: $\mathcal{F}(D) \to 0$ (the decoder is saturated), $\mathcal{T}$ is blocked. The dynamics reduce to $\dfrac{dI}{dt} \approx -\dfrac{1}{\tau}(I - I_{\mathrm{eq}})$: absent maintained energy supply, the system erodes slowly toward equilibrium.


## References

1. Liang, R. Structure Recursive Viability Dynamics (SRVD v7.8). Zenodo, 2026.
2. Prigogine, I. (1967). *Introduction to Thermodynamics of Irreversible Processes* (3rd ed.). Interscience.
3. Kauffman, S. A. (1993). *The Origins of Order: Self-Organization and Selection in Evolution*. Oxford University Press.
4. Kauffman, S. A., & Roll, W. (2024). Is the emergence of life an expected phase transition in the evolving universe? *Interface Focus*, 14, 20230085.
5. West, G. B., Brown, J. H., & Enquist, B. J. (1997). A general model for the origin of allometric scaling laws in biology. *Science*, 276(5309), 122–126.
6. Chaisson, E. J. (2001). *Cosmic Evolution: The Rise of Complexity in Nature*. Harvard University Press.
7. Friston, K., FitzGerald, T., Rigoli, F., Schwartenbeck, P., & Pezzulo, G. (2017). Active inference: A process theory. *Neural Computation*, 29(1), 1–49.
8. Cronin, L., & Walker, S. I. (2021). Defining lyfe in the universe: From three privileged functions to four pillars. *Life*, 11(12), 1284.
9. Eigen, M. (1971). Selforganization of matter and the evolution of biological macromolecules. *Naturwissenschaften*, 58(10), 465–523.
10. Landauer, R. (1961). Irreversibility and heat generation in the computing process. *IBM Journal of Research and Development*, 5(3), 183–191.
11. Bekenstein, J. D. (1973). Black holes and entropy. *Physical Review D*, 7(8), 2333–2346.
12. Gould, S. J., & Eldredge, N. (1977). Punctuated equilibria: The tempo and mode of evolution reconsidered. *Paleobiology*, 3(2), 115–151.
13. Schneider, E. D., & Kay, J. J. (1994). Life as a manifestation of the second law of thermodynamics. *Mathematical and Computer Modelling*, 19(6–8), 25–48.
14. Ashby, W. R. (1956). *An Introduction to Cybernetics*. Chapman & Hall.
15. Wiener, N. (1948). *Cybernetics: Or Control and Communication in the Animal and the Machine*. MIT Press.
16. Shannon, C. E. (1948). A mathematical theory of communication. *Bell System Technical Journal*, 27(3), 379–423.
17. Ulanowicz, R. E. (1986). *Growth and Development: Ecosystems Phenomenology*. Springer.
18. Haken, H. (1983). *Synergetics: An Introduction* (3rd ed.). Springer.


---

## Appendix C — The Civilizational Energy Leverage $\Lambda$ Extension (Application-Level Auxiliary Parameters)

#### Part Five: The Civilizational Energy Leverage $\Lambda$ Extension (a newly added degree of freedom, an appendix-level strategic parameter)

> **A statement of paradigm-level increment**: this section introduces an energy bipartition and a civilizational energy leverage $\Lambda$ not present in the original appendix, treating it as an independent dynamical strategy parameter, from which the optimal-leverage surface and the E-phase/T-phase classification are derived. **$\Lambda$, $E_{\mathrm{ext}}$, and $\eta_{\Lambda}$ are appendix-level auxiliary parameters that do not participate in the definition of the main paper's core variable constitution (Appendix A) and are used only in strategic analysis.**

##### 5.1 The Energy Bipartition and the Definition of $\Lambda$

Split total energy consumption into:
- $E_{\mathrm{causal}}$: the energy directly consumed by the decoder (human brain/AI) (the cost of producing information, J)
- $E_{\mathrm{ext}}$: the external energy flow controlled by the decoder (expansionary resources, J)

Define the civilizational energy leverage:
$$ \boxed{\Lambda \equiv \frac{E_{\mathrm{ext}}}{E_{\mathrm{causal}}}} $$

##### 5.2 The Optimal-Leverage-Surface Theorem

Holding the core equation $V = I T / E_{\mathrm{eff}}$ unchanged, let $E_{\mathrm{eff}} = E_{\mathrm{causal}}(1+\Lambda)$, with $T(\Lambda)$ shortening as $\Lambda$ increases (higher dissipation accelerates aging, $f'(\Lambda)<0$):

$$ V(\Lambda) = \frac{I \cdot T_0 \cdot f(\Lambda)}{E_{\mathrm{causal}}(1+\Lambda)} $$

There exists $\Lambda_{\mathrm{opt}}$ such that $\displaystyle \frac{\partial V}{\partial \Lambda} = 0$; the optimal-leverage condition is:
$$ \boxed{\frac{\partial \ln T}{\partial \Lambda} = \frac{1}{1+\Lambda}} $$

- $\Lambda < \Lambda_{\mathrm{opt}}$: expansion increases $V$
- $\Lambda > \Lambda_{\mathrm{opt}}$: expansion decreases $V$

##### 5.3 The Criterion for a Civilizational Phase Transition (E-Phase / T-Phase)

Define the control efficiency $\eta_{\Lambda} = \Lambda^{-1}$; the direction of civilizational evolution is $\eta_{\Lambda} \to 0$. A civilization's phase is jointly determined by the rate of change of leverage $\dot{\Lambda}$ and $\dot{V}$:

| State | $\frac{d\Lambda}{dt}$ | $\frac{dV}{dt}$ | Interpretation |
| :---------------- | :------------------------ | :-------------- | :----------------------------- |
| **Expansion phase (E-phase)** | $>0$ | $>0$ | The Industrial Revolution, the AI boom |
| **Saturation phase** | $\approx 0$ | $\approx 0$ | Involution; leverage stagnates |
| **Dormancy phase (T-phase)** | $<0$ | $>0$ | Trading leverage for lifespan (a dormant Dyson-sphere civilization) |
| **True decline** | $<0$ | $<0$ | Societal collapse |

> **Core conclusion**: $\dot{\Lambda}<0$ does not necessarily equal decline; civilizational evolution is not a monotonic "the higher the leverage, the better," but a dynamic balance between the E-phase and the T-phase.

##### 5.4 A Historical Accounting Baseline (Retaining the Original Definition of $V$)

> **A note on the data**: the figures below are conceptual order-of-magnitude estimates, based on a rough synthesis of anthropology and energy history, not precise measured data; they serve only to demonstrate the order-of-magnitude reasonableness of the definition of $\Lambda$.

- Total historical human brain energy consumption (estimated): $E_{\mathrm{causal}} \approx 1.3\times10^{21}\ \text{J}$
- Total civilizational energy consumption (estimated): $E_{\mathrm{eff}} \approx 3.2\times10^{22}\ \text{J}$
- Historical average leverage (order-of-magnitude estimate): $\Lambda_{\mathrm{avg}} \approx 10^3$
- Average civilizational viability potential (order-of-magnitude example): $V_{\mathrm{civ}} \approx 3\times10^{3}\ \text{bit·s/J}$

---

