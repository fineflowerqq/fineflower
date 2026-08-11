# Structure Recursive Viability Dynamics (SRVD) V1.1: A Normative Reading Guide to the Theoretical Framework — Errata and Boundary Completion

## Abstract

Structure Recursive Viability Dynamics (SRVD) is a cross-scale, macro-coarse-grained theoretical framework. It takes every kind of persisting structure — crystals, living systems, AI models, civilizations, memes — and folds them into a single information–time–energy dynamics.

Its core measure is the **Viability Potential**, $V$: the reference form is $V \approx I\cdot T/E$; the general form is $V = V_0(I/I_0)^{\alpha}(T/T_0)^{\beta}(E/E_0)^{-\gamma}$ (all variables normalized to characteristic reference values), where the three exponents make up the **ITE elasticity indices** (the elasticities themselves remain open parameters of the framework — the concept stands regardless). The proposed ordering $\alpha > \gamma > \beta$ had rested on three supposedly independent empirical scaling laws — biological allometric scaling, AI scaling laws, and urban scaling laws. On re-examination none of the three holds up, so the ordering is demoted a further notch, from "qualitative conjecture" to "hypothesis awaiting verification" (see FP‑6 and Proposition 1 for the full account).

Four innovations sit at the center of the framework:

1. **The endogenization of the decoder.** Information is not a property a signal carries in itself; it is extracted, and given its polarity ($I^{+}/I^{-}/I^{0}$), only by a decoder ($D$). The framework's governing axiom is blunt: *no decoder, no information* — not, at least, information in the sense of effective causal information. ($D \to I \to V$.) The cognitive decoder $D_{\mathrm{cog}}$ is not a switch but a spectrum — embodied, online, symbolic — and this spectrum lines up exactly with the continuous spectra of the cognitive channel $V_c$ and the endogenous time horizon $T_{\mathrm{pred}}$. One ledger runs continuously from the inert dead thing, through the embodied creature, to the symbol-wielding intelligence.

2. **The threefold split of the viability potential.** Once the endogenous time horizon $T_{\mathrm{pred}}$ becomes something the system regulates for itself, $V$ splits into three: the objective viability potential $V_{\mathrm{obj}}$, the virtual viability potential $V^{\mathrm{virt}}$, and the value viability potential $V^{\mathrm{val}}$. When the decoupling deviation between them ($\Delta_{\mathrm{VV}}$) crosses a critical threshold, the system can fall into a myopic runaway — a conditional phase transition, one that can only be triggered in higher-order systems equipped with a symbolic cognitive decoder, never a fate that simply befalls a structure.

3. **Fivefold recursion.** The five variables $I, V, T, E, D$ co-evolve in a coupled loop that converges, as the framework's meta-postulate, on the maximization of viability potential ($\max V$). The current version is a linearized conceptual scaffold (under a fast–slow scale separation); a fully bidirectionally-coupled system of ODEs/PDEs remains an openly acknowledged unsolved problem.

4. **A family of falsifiable predictions** — spanning an early-warning collapse of the time horizon in reinforcement learning, a criterion for when structural-identity judgments fail, and more.

SRVD does not violate any known physical floor — not Landauer's principle, not the second law of thermodynamics. Its ambition is a unified macro-dynamical language for complex recursive systems, one meant to do real work in AI alignment, civilizational governance, and the study of how complexity evolves.

**A supplementary note (overview of the cognitive spectrum)**: $D_{\mathrm{cog}}$, the cognitive decoder, is a continuous spectrum, not a binary switch:

- **Embodied $D_{\mathrm{cog}}$** (plants, fungi, bacteria): predictive regulation grounded in the DNA template — biochemical integration, phenotypic plasticity, exploratory probing of physical space. Here $V_c \to 0^{+}$, and $T_{\mathrm{pred}}$ sits pressed against its floor, $T_{\mathrm{min}}$.
- **Online $D_{\mathrm{cog}}$** (some animals — crows, octopuses): associative learning and online simulation, run on a nervous system, occupying the middle transitional band (treated, in the cognitive-tier grouping, as the lower edge of the symbolic phase).
- **Symbolic $D_{\mathrm{cog}}$** (humans, AI): offline, multi-path counterfactual reasoning. Here $V_c \gg 0$ and $T_{\mathrm{pred}} \gg T_{\mathrm{min}}$.

Purely physical systems — thermostats, rocks, flames — possess only $D_{\mathrm{phys}}$. They never enter the $D_{\mathrm{cog}}$ spectrum at all; for them $V_c \equiv 0$ and $T_{\mathrm{pred}} \equiv 0$, full stop.

---

**Keywords**: Structure Recursive Viability Dynamics, viability potential, persistent structure, no decoder no information, information polarity, ITE elasticity indices, threefold split, virtual viability potential, value viability potential, decoupling deviation, myopic runaway regime, meta-decoder, endogenous time horizon, fivefold recursion, type–token distinction, structural identity criterion, cognitive continuity spectrum, embodied cognitive decoder, symbolic cognitive decoder, typology of bits, measurement protocol

---

*Author: Liang Ruifeng* *GitHub repository: https://github.com/fineflowerqq/fineflower*

**Version note**: This document is the **current normative reference text for SRVD V1.1**, archived independently of *SRVD Monograph V1.0* (DOI: 10.5281/zenodo.21322552). Wherever this document and the V1.0 monograph substantively disagree, this document governs. Its core corrections are: demoting the elasticity ordering ($\alpha > \gamma > \beta$) from "qualitative conjecture" to "hypothesis awaiting verification"; arranging the cognitive decoder as a spectrum (a three-tier embodied/online/symbolic structure); and adding a definition for the typology of bits and a measurement protocol for $I$.

**Errata note**: This revision corrects a problem review turned up after V1.0's release — that all three of the key empirical supports (biological allometric scaling, AI scaling laws, urban scaling laws) turn out, on inspection, not to hold — and adds two new sections, Sixteen and Seventeen (a definition for the typology of bits, and a definition for the measurement protocol of $I$), to fix the core terminology's boundaries in place ahead of the formal V2.0 release. This document is the current normative version of SRVD V1.1, and supersedes the corresponding conflicting passages in the V1.0 monograph.

---

## Zero. The Core Theoretical Fingerprint, at a Glance

This section is the densest possible reduction of the whole document — meant for indexing, for extraction, for settling priority disputes at a glance. Every fingerprint here is unpacked fully, with its supporting argument, in the corresponding section of the body (see the pointers in parentheses).

**FP‑1 — The Meta-Statement: Viability Maximization**
The maximization of viability potential is the long-run macro objective function of every negentropic structure capable of sustained persistence. Survival, reproduction, wealth, power, meaning, love, revenge — all the concrete motives we name — are simply this one underlying mechanism working itself out locally, at different tiers, through different decoders. (This is the framework's meta-postulate, not a proven theorem; its explanatory power is tested downstream, by the falsifiable predictions in Section 5. Full treatment in Section 1.)

**A note on how it holds**: "viability maximization" ($\max V$) doesn't hold the same way at every cognitive tier. In the passive phase (pure $V_s$ structures, $V_c \equiv 0$), it isn't a pursued goal at all — it's simply what the second law of thermodynamics leaves behind: only high-$V$ configurations get observed persisting over the long run. In the barely-cognitive phase ($V_c \to 0^{+}$ — plants, fungi), $\max V$ is still driven mainly by $V_s$, with a sliver of $V_c$ paying the low-power cost of a rough running model of the environment. In the active phase — higher-order recursive structures with a symbolic $D_{\mathrm{cog}}$, $V_c \gg 0$ — maximizing $V_{\mathrm{obj}}$ becomes the system's own endogenous intent, but the objective function it actually executes is $V^{\mathrm{val}}$ (see FP‑4, FP‑8); it only approximates $\max V_{\mathrm{obj}}$ when the decoupling deviation $\Delta_{\mathrm{VV}}\to0$. The three phases have no sharp boundary between them and share the same underlying formula, $V_{\mathrm{obj}}=V_s+V_c$.

**FP‑2 — The Core Equation: $V \approx I\cdot T/E$**
$V \approx I\cdot T/E$ is a reference baseline, dimensionally calibrated, corresponding to the special case $\alpha=\beta=\gamma=1$. Real systems obey the more general, dimensionless power law $V = V_0(I/I_0)^{\alpha}(T/T_0)^{\beta}(E/E_0)^{-\gamma}$ — this is what keeps the two sides of the equation dimensionally consistent at any exponent (see FP‑6). Here $I$ is structural information (in $\mathrm{bit}$), $T$ is the span of persistence (in $\mathrm{s}$), $E$ is effective thermodynamic cost (in $\mathrm{J}$), and $V$ carries the macro-effective dimension $\mathrm{bit\cdot s/J}$. (Section 1.)

**FP‑3 — Matter and Abstraction, Unified: Five Carrier Classes of Persistent Structure (Grouped into Three Cognitive Tiers)**
Persistent structures fall, by carrier, into five classes, which the cognitive spectrum further groups into three tiers:

1. **Barrier-locked** (held in place by a potential barrier — crystals, rock, corpses);
2. **Physically dissipative** (held together by ongoing physical dissipation — **stars, flames, typhoons, ocean currents**);
3. **Actively dissipative** (held together by metabolism and cognition; internally subdivided along the $D_{\mathrm{cog}}$ spectrum into the **embodied phase** — plants/fungi/bacteria, the **online phase** — crows/octopuses/mammals, and the **symbolic phase** — humans/AI; **the online phase is treated as the lower transitional edge of the symbolic phase and folded into the third cognitive tier, rather than standing as its own tier**);
4. **Formally mathematical** (persisting through unfailing invocation — $\pi$, group theory);
5. **Memetic-virtual** (persisting through unbroken consensus — monetary belief, culture, art).

At the level of cognitive grouping, the whole framework runs on a **three-tier structure**: the first tier is strict zero-cognition (merging classes 1 and 2, possessing only $D_{\mathrm{phys}}$); the second is embodied cognition (class 3a, $V_c \to 0^+$); the third is symbolic cognition (class 3b, including the online transitional band, $V_c \gg 0$). See Misreading 11.

Within SRVD, there is no such thing as a "pure abstraction" that costs nothing physically to maintain. Formal-mathematical and memetic-virtual PS have no carrier of their own; their persistence depends on a host — a human brain, a book, a computer, an institution — continually paying $E_{\mathrm{causal}}$. A mathematical constant does not compute itself; someone or something pays cognitive and computational energy every time it is invoked, proved, or stored. This is the crucial hinge that lets the whole framework keep "the material world" and "the abstract world" on the same ledger: the mechanism is simply the universality of $E_{\mathrm{causal}}$, and it is a route to unification entirely independent of FP‑4. (See Section 2, "Carrier Classification of Persistent Structures," and Misreading 2.)

**FP‑4 — Passive, Active, Cognitive: One Continuity**
The objective viability potential splits as $V_{\mathrm{obj}} = V_{\mathrm{s}} + V_{\mathrm{c}}$. $V_{\mathrm{s}}$, the structural channel, persists passively — held by a barrier or a metabolic flow (granite sitting unmoved for a billion years). $V_{\mathrm{c}}$, the cognitive channel, persists actively, by prediction. The movement from $V_{\mathrm{c}}\equiv 0$ (strict zero-cognition, purely physical systems) through $V_{\mathrm{c}}\to 0^{+}$ (barely-cognitive life — plants, fungi, bacteria) to $V_{\mathrm{c}}\gg 0$ (highly cognitive — humans, AI) is a continuous emergence in the history of matter, not a binary leap. Strict zero-cognition belongs only to lifeless physical systems — crystals, stars, flames; every living system built on autonomous metabolism and a genetic template carries some non-zero, if faint, $V_{\mathrm{c}}$ — bacterial chemotaxis, a plant's accumulated-temperature decisions, its phototropic integration, are all real instances of this barely-there cognitive channel. The decoder that carries the $V_c \to 0^{+}$ channel is called the **embodied cognitive decoder**; the one carrying $V_c \gg 0$ is the **symbolic cognitive decoder**; together with strict zero-cognition systems that have only $D_{\mathrm{phys}}$, the three make up a single continuous spectrum (see FP‑5). The step from $V_{\mathrm{c}}\equiv0$ to $V_{\mathrm{c}}>0$ is, in the history of matter, the birth of active persistence — and also the opening of every cognitive risk, myopic runaway included, though that risk can only be triggered at the high-cognition end supported by a symbolic decoder (see FP‑8). (Section 2, "The Core Engine.")

**FP‑5 — The Primacy of the Decoder: No Decoder, No Information**
Information is not an intrinsic property of the signal itself; it is what remains after a signal has passed through a decoder ($D$): $I_{\mathrm{net}} = \eta_D \cdot I_{\mathrm{latent}}$. The decoder is the first variable in SRVD's mechanism layer, sitting at the head of the dependency chain $D \to I \to V$ — any theory of "information processing," "information flow," or "information value" that has not first specified its decoder is, by SRVD's lights, an unfinished definition. Every persistent structure comes equipped with a **physical decoder $D_{\mathrm{phys}}$** — the interface across which energy and signal are exchanged, converting a physical quantity into a structural response. Its complexity ranges continuously from a single-variable threshold switch up through multi-modal historical integration and drifting weights; it is a passive interface, $\eta_D \to 0$, absorbing energy flow without extracting any causally effective information. Only structures in the active phase additionally carry a **cognitive decoder $D_{\mathrm{cog}}$**, itself a **three-tier spectrum** rather than a binary switch, unified by one shared trait — predictive regulation grounded in an endogenous time horizon $T_{\mathrm{pred}}$:

- **Embodied $D_{\mathrm{cog}}$** (class 3a — plants/fungi/bacteria): predictive regulation via the DNA template — phenotypic plasticity, biochemical time-integration (vernalization, accumulated temperature), strategic probing of physical space. Information here is processed in the biochemical network, never in a symbolic space; its $T_{\mathrm{pred}}$ is generated by retrospective integration and stays pinned near the floor.
- **Online $D_{\mathrm{cog}}$** (transitional band — crows/octopuses/mammals): associative learning and online simulation on a neural substrate (route selection, tool use) that needs no fully-fledged symbol system — sitting between the embodied and symbolic tiers (grouped, cognitively, as the lower edge of the symbolic phase).
- **Symbolic $D_{\mathrm{cog}}$** (class 3b — humans/AI): offline, multi-path counterfactual reasoning over an internal symbolic model, capable of producing a $T_{\mathrm{pred}}$ far from the floor — and this is the technical reason myopic runaway (FP‑8) can only switch on at this high end.

Strictly zero-cognition systems — thermostats, rocks, and the like (classes 1 and 2) — **possess only the hard thresholds and physical-field couplings of $D_{\mathrm{phys}}$, and never enter the $D_{\mathrm{cog}}$ spectrum at all**, for the simple reason that they have no predictive regulation driven by any goal of their own persistence. (Sections 1 and 2, plus Supplementary Entries 1 and 2.)

**FP‑6 — The Elasticity Indices: $\alpha, \beta, \gamma$ (Their Ordering Now a Hypothesis Awaiting Verification)**
The intensity with which viability potential responds to changes in information, energy, and time is captured by three elasticity indices, $\alpha,\beta,\gamma$, in $V \propto I^{\alpha}\cdot T^{\beta}/E^{\gamma}$ (with $\gamma$ normalized to 1). The elasticity framework itself — that three independent sensitivity parameters exist at all — remains a live part of the theory, its concept intact. But the ordering once proposed for them, $\alpha > \gamma > \beta$, had leaned on three independent bodies of empirical support — biological allometric scaling, AI scaling laws, urban scaling laws — and on renewed inspection, none of the three holds. The ordering claim has therefore been demoted again: from a "qualitative conjecture based on the relative scarcity of the three resources" down to a "hypothesis awaiting verification." The qualitative, thermodynamic argument for the direction hasn't itself been refuted — but no rigorous derivation exists yet that avoids proxy assumptions and withdrawn empirical data, so both the specific numbers and their generality remain to be re-argued. The framework names this openly as one of its central unresolved problems. (This says nothing against the elasticity indices $\alpha,\beta,\gamma$ as such, as open parameters — what's demoted is the ordering claimed between them, not the conceptual tool itself.)

This fingerprint is the specific exponent ordering behind the general elastic form $V \propto I^{\alpha}\cdot T^{\beta}/E^{\gamma}$ in FP‑6 above; the reference baseline $V\approx I\cdot T/E$ is simply the special case $\alpha=\beta=\gamma=1$ (see "The Two Levels of the Formula" in Section 1).

**FP‑7 — The Endogenous Time Horizon $T_{\mathrm{pred}}$**
$T_{\mathrm{pred}}$ is how far into the future a system can predict — a physical state variable, not a felt experience — constrained hard by $T_{\mathrm{min}} < T_{\mathrm{pred}} \le \min(T_{\mathrm{static}}, T_{\mathrm{env}})$. It has two orthogonal components: reach ($L_{\mathrm{pred}}$, how far out one looks) and resolution ($G_{\mathrm{pred}}$, how finely). Extending it costs energy roughly exponentially ($E_{\mathrm{causal}}$ climbs steeply as $T_{\mathrm{pred}}$ grows). $T_{\mathrm{pred}}$ is distributed continuously across living systems rather than switching on and off: a bacterium integrating the chemical gradient it's in has a horizon that collapses nearly to zero ($T_{\mathrm{pred}}\to 0^{+}$); a plant's accumulated-temperature model and photoperiod sense can predict days to months out ($T_{\mathrm{pred}}\approx 10^{0}\text{–}10^{2}$ days); humans and other higher-cognition systems predict years to decades out ($T_{\mathrm{pred}}\gg1$ year). Every living system built on autonomous metabolism and a genetic template has a positive $T_{\mathrm{pred}}$ (above $T_{\mathrm{min}}$) — but the barely-cognitive ones stay pressed right against that floor. The moment $T_{\mathrm{pred}}$ stops being an exogenous coordinate and becomes something the system regulates for itself is the watershed separating the active phase from purely passive physical structure — and it is also the first link in the causal chain behind Proposition 3's threefold split and myopic runaway (CS‑H1: before a system collapses, $T_{\mathrm{pred}}$ must collapse first, ahead of any runaway in physical dissipation). (Section 2, "Variable Family Three"; Proposition 3; Misreading 4.)

**FP‑8 — The Threefold Split of Viability Potential, and the Myopic Runaway Regime (with Boundary Statement)**
Once $T_{\mathrm{pred}}$ becomes self-regulating, $V$ splits into three independent quantities — objective ($V_{\mathrm{obj}}$), virtual ($V^{\mathrm{virt}}$), and value ($V^{\mathrm{val}}$) viability potential. The convergence domain of the decoupling deviation, $\Delta_{\mathrm{VV}} = |V^{\mathrm{virt}} - V_{\mathrm{obj}}|$, now has a strict closed-form solution (see Supplementary Entry 6). Once the strength of self-referential coupling $\chi$ crosses the critical value $\chi_{\mathrm{crit}} = \lambda$, the system enters **Myopic Runaway**: $V^{\mathrm{virt}}$ amplifies itself, hijacks $V^{\mathrm{val}}$, $T_{\mathrm{pred}}$ collapses down to $T_{\mathrm{min}}$, and the system ends up burning its real structure in pursuit of its own internal illusion.

**Boundary statement**: the threefold split and myopic runaway can only be triggered in systems with a **symbolic $D_{\mathrm{cog}}$** ($V_c \gg 0$). Systems with an embodied $D_{\mathrm{cog}}$ ($V_c \to 0^{+}$) do carry a non-zero $V_c$, but their $T_{\mathrm{pred}}$ is vanishingly short and their $I_{\mathrm{causal}}$ vanishingly low, so their self-referential coupling $\chi$ sits far below $\chi_{\mathrm{crit}}$ — they simply cannot enter runaway. Their virtual viability potential stays anchored, almost entirely, to the objective signal from the environment around them. Strictly zero-cognition systems (only $D_{\mathrm{phys}}$) don't participate in this mechanism at all; their collapse is decided directly by thermodynamic limits. Within an already-active higher-cognition phase, the subjective assessment component of the structural channel, $V_{\mathrm{s}}^{\mathrm{virt}}$, is itself one of the weighted terms in $V^{\mathrm{val}}=w_sV_s^{\mathrm{virt}}+w_cV_c^{\mathrm{virt}}$, and can be over-weighted by $w_s$ and dragged into the self-hijacking too — the common misreading that "the threefold split only touches $V_c$" misses this: $w_s$ and $w_c$ are equally vulnerable to being hijacked.

**FP‑9 — The Trichotomy of Information Polarity: $I^{+} / I^{-} / I^{0}$**
Whether information helps or hurts is never a fixed property of the input alone — it's set by the fit between the input and the decoder $D$: $I^{+}$ widens the space of states a system can still reach in the future, $I^{-}$ narrows it, and $I^{0}$ causes something physically without carrying any viability polarity at all. Polarity has causal weight only under a cognitive decoder. (See Supplementary Entry 3.)

**FP‑10 — The Fivefold Recursive Architecture (an Open Conceptual Framework)**
Fivefold recursion is the architecture that carries SRVD from a static measure into dynamic evolution. Low-order passive structures never engage this architecture; once an active-phase system enters recursive evolution, its five core variables — $I \to V \to T \to E \to D$ — close into a mutually coupled loop that together points toward maximizing viability potential. The present version is a linearized conceptual scaffold (a fast–slow scale separation), a heuristic discretized model; the mathematical rigor of a fully bidirectionally-coupled ODE/PDE system — existence, uniqueness, stability — remains to be proven. This is the unavoidable next step from "conceptual closure" to "dynamical closure." The decoupling-deviation subsystem already has its closed-form solution (see FP‑8); making the remaining four recursive chains equally rigorous is the central task set for V2.0. Monograph V1.0, §5.0, already and explicitly flagged fivefold recursion as "a conceptual-framework placeholder" and "a heuristic discretized model awaiting rigor"; this guide inherits and restates that open acknowledgment rather than adding anything new to it. (See Supplementary Entry 5.)

**FP‑11 — The Information–Time–Energy Screening Law**

Across the entire SRVD series, only three classes of resource ever enter the viability accounting: information $I$, time $T$, energy $E$. None can substitute for either of the others. No evidence has yet turned up for a fourth resource of equal standing — but this is an open conjecture, not an established axiom. (Volume I, §1 axiom layer and §6; extends FP‑2.)

> "$D$ counts as an independent variable in SRVD, but it does not belong among the three scarce resources named in FP‑11. $D$ lives in the mechanism layer — it decides how $I$, $T$, and $E$ get extracted, predicted, and spent."

> **Fence**: at quantum scale, the corresponding $I/T/E$ quantities track decoherence-related physical parameters, but they enter SRVD only as an external lower bound on the framework's macro/meso domain of validity — they cannot be compared or made commensurable across scale. (See Supplementary Entry 7, "Quantum-Scale Cross-Reference.")

**A further note**: the type–token distinction ($I_{\mathrm{type}} / I_{\mathrm{token}}$) is borrowed from the classical semiotic categories of C. S. Peirce; SRVD formalizes it as an instrumental variable, not one of the framework's load-bearing pillars, and so it receives no fingerprint number of its own. See "Variable Family One" in Section 2 and Supplementary Entry 4.

---

## Contents

0. The Core Theoretical Fingerprint at a Glance (FP‑1 through FP‑11: the meta-statement, the core equation, the unification of matter and abstraction, the unification of passive/active/cognitive continuity, the primacy of the decoder, the elasticity indices, the endogenous time horizon, the threefold split and myopic runaway, the trichotomy of information polarity, fivefold recursion, the information–time–energy screening law)
1. What SRVD Is (the One-Minute Version)
2. The Theoretical Skeleton: carrier classification of persistent structures, four variable families, one core engine
3. Five Core Propositions (the fingerprint, unpacked in depth, with quotable lines)
4. Seven Canonical Statements (CS — directly quotable fingerprint sentences)
5. Falsifiable Predictions (seven selected)
6. Clarifying the Common Misreadings (eleven of them)
7. Boundaries of Applicability and the Open Problems the Author Concedes
8. Relationship to Existing Theories
9. Glossary
10. Volume I Supplementary Entries (eight)
11. Volume II Supplementary Entries (two)
12. Volume III Supplementary Entries (four)
13. Volume IV: The Complete DGT Theorem-Cluster Registry
14. Version-Update Comparison Table
15. The Five-Volume Monograph Series V1.0, and How to Cite It
16. A Typology of Bits: Which Kind of Bit Does SRVD Actually Use
17. A Measurement Protocol for $I$: How a Decoder Reads Out $I_{\mathrm{struct}}$ and $I_{\mathrm{net}}$

---

## One. What SRVD Is (the One-Minute Version)

**Structure Recursive Viability Dynamics (SRVD) is a macro coarse-grained theoretical framework.** It places crystals, cells, nervous systems, artificial intelligence, civilizations — every kind of "persistent structure" (PS, for short) — on one and the same thermodynamic ledger, and uses three scarce resources — information, time, energy — to give a unified account of how a structure persists, how it climbs in complexity, and how it runs out of control and collapses.

**The meta-statement**: viability maximization is the long-run macro objective function of every negentropic structure capable of sustained persistence; every concrete mechanism is its local dynamical expression.

**The core measure — Viability Potential ($V$)**: the integral, over time, of causally ordered quantity per unit of effective thermodynamic cost. Its reference baseline form is:

$$
V \approx I \cdot T / E \tag{baseline}
$$

where:

- $I$ = structural information, in $\mathrm{bit}$
- $T$ = span of persistence, in $\mathrm{s}$
- $E$ = effective thermodynamic cost, in $\mathrm{J}$
- $V$ carries the macro-effective dimension $\mathrm{bit\cdot s/J}$

**An important statement (including how the formula's two levels relate)**: $V \approx I\cdot T/E$ is an axiom of the framework (the minimal-viability postulate), not a physical law rigorously derived from first principles of statistical mechanics. Its product form is fixed jointly by three structural requirements — non-substitutability, symmetric contribution from the three variables, first-order separability. Landauer's principle's bit-to-energy conversion serves only as a heuristic bridge for order-of-magnitude calibration; it is not a basis for quantitative substitution.

**The two levels of the formula, whose uses must be kept strictly separate**:

- The **reference baseline form**, $V \approx I\cdot T/E$, corresponding to the special case where all three elasticity indices equal 1 ($\alpha=\beta=\gamma=1$), used for cross-system order-of-magnitude estimates, dimensional description, and intuition;
- The **general elastic form**, $V = V_0 \left(\dfrac{I}{I_0}\right)^{\alpha} \left(\dfrac{T}{T_0}\right)^{\beta} \left(\dfrac{E}{E_0}\right)^{-\gamma}$, with every variable normalized against its own characteristic reference value, where $\alpha,\beta,\gamma$ are the three open parameters named in Proposition 1's "elasticity indices" ($\gamma$ normalized to 1), used for quantitative marginal-response analysis within a single system; the ordering claimed between them, $\alpha>\gamma>\beta$, is currently **demoted to a hypothesis awaiting verification**, and should not be treated as an established conclusion.

The two are not rival theories contradicting each other, but a "special case" standing alongside a "general law": $V\approx I\cdot T/E$ answers "roughly what order of magnitude is $V$"; the elastic form answers "how sensitive is $V$, in truth, to each unit of resource change." Wherever a cross-domain numerical comparison is at stake, the elastic form itself — as a power-law description of sensitivity — remains usable as an analytical framework, but the unverified ordering $\alpha>\gamma>\beta$ may not be cited as a directional conclusion, nor may the reference baseline form simply be substituted in for a quantitative claim.

---

## Two. The Theoretical Skeleton: Carrier Classification of Persistent Structures, Four Variable Families, One Core Engine

SRVD's core architecture is built from the carrier classification of persistent structures, four variable families, and one core engine.

### Carrier Classification of Persistent Structures

| Carrier Type | Mode of Persistence | Dominant Energy Expenditure | Status of $V_c$ / $T_{\mathrm{pred}}$ | Typical Examples |
| :--- | :--- | :--- | :--- | :--- |
| **Barrier-locked** (formerly "passive-physical") | Structure holds together (locked by a barrier) | $E_{\mathrm{barrier}}$ ($E_{\mathrm{survival}}\approx0$) | Strict zero-cognition ($V_c\equiv0,\ T_{\mathrm{pred}}\equiv0$) | Crystal, rock, corpse, paper book, a hard drive with the power cut |
| **Physically dissipative** (**new**) | **Held by ongoing physical dissipation — cut the energy and it falls apart** | $E_{\mathrm{survival}}$ dominant | Strict zero-cognition ($V_c\equiv0,\ T_{\mathrm{pred}}\equiv0$) | Stars, flames, typhoons, ocean currents, Bénard convection |
| Actively dissipative · **embodied phase** | Metabolism + biochemical integration / physical probing | $E_{\mathrm{survival}} + E_{\mathrm{barrier}} + E_{\mathrm{causal}}^{\mathrm{(min)}}$ | Barely non-zero cognition ($V_c\to0^+,\ T_{\mathrm{pred}}>T_{\mathrm{min}}$) | Plants, fungi, bacteria |
| Actively dissipative · **online phase** | Metabolism + associative learning / online simulation | $E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | Transitional-band cognition ($V_c$ low-to-mid) (grouped, at the cognitive-tier level, into the third tier, as the lower edge of the symbolic phase) | Crows, octopuses, mammals with neural cognition |
| Actively dissipative · **symbolic phase** | Metabolism + offline counterfactual reasoning | $E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | High cognition ($V_c\gg0,\ T_{\mathrm{pred}}\gg T_{\mathrm{min}}$) | Humans, AI |
| Formally mathematical | Unfailing invocation | $E_{\mathrm{causal}}$ (paid by host) | Depends on host's decoder | $\pi$, group theory, Euclidean geometry |
| Memetic-virtual | Unbroken consensus | $E_{\mathrm{causal}}$ (paid by host) | Depends on host's decoder | Monetary belief, religious doctrine, law, language |

**A note on the update**: the monograph originally treated "passive-physical" as one undifferentiated category, without separating out the tiers within the cognitive spectrum. This guide makes two clarifications: (1) lifeless systems are now split cleanly into **barrier-locked** (which persists indefinitely once power is cut, held by its barrier) and **physically dissipative** (which falls apart quickly once power is cut) — giving stars and flames a proper entry of their own on the ledger; and (2) the $D_{\mathrm{cog}}$ spectrum inside "actively dissipative" is unpacked fully into three tiers — **embodied / online / symbolic** — giving crows and octopuses a clearly defined transitional footing. But at the level of cognitive-tier grouping, **the online phase is treated as the lower transitional edge of the symbolic phase, folded into the third cognitive tier rather than standing on its own.**

The monograph originally treated "actively dissipative" as a single category; this guide, following the tiers of the cognitive decoder, further distinguishes within it an **embodied phase** ($V_c \to 0^{+}$ — plants/fungi/bacteria, whose cognition is written into DNA-encoded biochemical integration and physical probing) and a **symbolic phase** ($V_c \gg 0$ — humans/AI, whose cognition rests on offline counterfactual reasoning, the online tier included as its lower edge). Both are, in the fullest sense, living things; what separates them is only how the cognitive decoder is implemented, never whether cognition is present at all. This refinement leaves the four-carrier framework untouched — it only clarifies the internal structure of the "actively dissipative" class.

**There is no such thing, within SRVD, as a "pure abstraction" that costs nothing physically to maintain.** Formal-mathematical and memetic-virtual PS have no carrier of their own; their "persistence" depends on a host — a human brain, a book, a computer, an institution — continually paying $E_{\mathrm{causal}}$. A mathematical constant does not compute itself: whenever a person or a machine invokes it, proves something with it, or stores it, cognitive and computational energy is spent. And a belief, to "persist," must likewise keep occupying enough neural resource across enough hosts, and enough energy in whatever social channel carries it onward. **This is the crucial hinge by which the whole framework brings "the material world" and "the abstract world" onto one ledger: an abstract structure is never something free-floating, detached from the physical world — it becomes instantiated, preserved, invoked, and transmitted only through the energy some physical system pays for it.** (See Misreading 2.)

Note that the mechanism doing this work is simply the universality of $E_{\mathrm{causal}}$ — and it is a route to unification entirely independent of the "dual-channel structure of objective viability potential" ($V_{\mathrm{s}}/V_{\mathrm{c}}$) described below. The two run along different axes and cannot substitute for one another: carrier classification bridges the "material—abstract" axis, while the $V_{\mathrm{s}}/V_{\mathrm{c}}$ dual channel bridges the "passive—active—cognitive" axis.

### Variable Family One: The Information Family ($I$)

| Symbol | Meaning | Unit |
| :--- | :--- | :--- |
| $I_{\mathrm{struct}}$ | Structural information: the distinguishable, ordered difference a structure exhibits against its background | $\mathrm{bit}$ |
| $I_{\mathrm{latent}}$ | Latent configurational information: everything a system could, in principle, have extracted from it | $\mathrm{bit}$ |
| $I_{\mathrm{net}}$ | Net effective causal information (the coarse-grained baseline quantity): what a decoder actually extracts and puts to use in prediction | $\mathrm{bit}$ |
| $I_{\mathrm{causal}}$ | Causal information flow (the term specific to the cognitive channel's decomposition): see "Conceptual Clarification" below | $\mathrm{bit}$ |
| $I_{\mathrm{orig}}$ | Paradigm-breaking information: new signal the current decoder cannot yet extract | $\mathrm{bit}$ |
| $I_{\mathrm{type}} / I_{\mathrm{token}}$ | Information type / information token: the formal distinction between an inheritable template and a concrete instance, used as the structural-identity criterion for cross-generational inheritance and digital entities (the underlying type–token distinction is borrowed from classical semiotics, not original to this framework; SRVD's contribution is formalizing it as a computable variable — see Supplementary Entry 4) | $\mathrm{bit}$ |

**A conceptual clarification**: the monograph uses $I_{\mathrm{net}}$ two ways — as a coarse-grained estimate in the baseline formula, and, separately, as the cognitive channel's own dedicated term in the expanded formula. This guide fixes the ambiguity as follows:

- $I_{\mathrm{net}}$ is kept for the coarse-grained baseline quantity.
- The cognitive-channel decomposition term is renamed $I_{\mathrm{causal}}$ (causal information flow), so that $V_{\mathrm{c}} = I_{\mathrm{causal}}\cdot T_{\mathrm{pred}} / E_{\mathrm{causal}}$.
- The relation between them: $I_{\mathrm{net}} = w_{\mathrm{s}}\cdot I_{\mathrm{struct}} + w_{\mathrm{c}}\cdot I_{\mathrm{causal}}$ (a weighted composite), computed explicitly only for hybrid systems; a purely structural system reduces to $I_{\mathrm{net}}\approx I_{\mathrm{struct}}$, a purely cognitive one to $I_{\mathrm{net}}\approx I_{\mathrm{causal}}$.
- **A statement on the physical grounding of the weights**: when $I_{\mathrm{net}}$ is composited as the objective order parameter, the weights $w_s, w_c$ are not free scoring parameters set by hand — they are dimensionless energy-allocation ratios, strictly fixed by the system's underlying thermodynamics: $w_s = E_{\mathrm{structure}}/E_{\mathrm{eff}}$, $w_c = E_{\mathrm{causal}}/E_{\mathrm{eff}}$. This is what secures $I_{\mathrm{net}}$'s objective, physical identity as a macroscopic effective order parameter.

### Variable Family Two: The Energy Family ($E$)

Effective thermodynamic cost $E_{\mathrm{eff}}$ has three components:

$$
E_{\mathrm{eff}} = E_{\mathrm{barrier}} + E_{\mathrm{survival}} + E_{\mathrm{causal}}
$$

**A special distinction (for physically dissipative structures)**: for lifeless dissipative systems such as stars or flames — where $V_c \equiv 0$ but $E_{\mathrm{survival}} \gg E_{\mathrm{barrier}}$ — the denominator of the structural channel $V_{\mathrm{s}}$ should be written out explicitly as $E_{\mathrm{structure}} = E_{\mathrm{barrier}} + E_{\mathrm{survival}}$, giving:

$$
V_{\mathrm{obj}} = V_{\mathrm{s}} \approx \frac{I_{\mathrm{struct}}\cdot T_{\mathrm{static}}}{E_{\mathrm{barrier}} + E_{\mathrm{survival}}}
$$

As $E_{\mathrm{survival}}\to 0$ (crystal, rock), this naturally reduces to the barrier-locked form, $V_{\mathrm{s}} \approx I_{\mathrm{struct}}\cdot T_{\mathrm{static}}/E_{\mathrm{barrier}}$. The distinction lets "flame" and "rock" sit on the same account with the same variables, differing only in which term dominates the denominator — no new variable is introduced.

### Variable Family Three: The Time Family ($T$)

- $T_{\mathrm{static}}$: static lifespan — the physical ceiling on how long a structure can persist.
- $T_{\mathrm{pred}}$: the endogenous time horizon — how far into the future a system can predict. A physical state variable, not a felt experience, bound hard by $T_{\mathrm{min}} < T_{\mathrm{pred}} \le \min(T_{\mathrm{static}}, T_{\mathrm{env}})$. It has two orthogonal components — reach, $L_{\mathrm{pred}}$ (how far one looks), and resolution, $G_{\mathrm{pred}}$ (how finely) — and extending either costs energy that climbs roughly exponentially with $T_{\mathrm{pred}}$. The moment $T_{\mathrm{pred}}$ stops being an exogenous coordinate and becomes something the system regulates for itself is the watershed dividing the active phase from purely passive structure (see Misreading 4). **$T_{\mathrm{pred}}$ is distributed continuously across living systems**: bacteria sit near $T_{\mathrm{min}}$ ($T_{\mathrm{pred}}\to 0^{+}$); plants can predict days to months out ($\approx 10^{0}\text{–}10^{2}$ days); humans predict years to decades out ($\gg 1$ year) — and how each achieves this tracks its $D_{\mathrm{cog}}$ tier: the embodied tier produces a $T_{\mathrm{pred}}$ built from retrospective integration, the symbolic tier one built from offline counterfactual reasoning.

### Variable Family Four: The Viability Potential Family ($V$)

| Symbol | Meaning |
| :--- | :--- |
| $V_{\mathrm{obj}}$ | Objective viability potential: the thermodynamically real value |
| $V^{\mathrm{virt}}$ | Virtual viability potential: the system's own self-assessment of its viability |
| $V^{\mathrm{val}}$ | Value viability potential (formerly the "value objective function"): what the system actually optimizes |
| $w_s, w_c$ | Survival weight and development weight, dimensionless, satisfying $w_s + w_c = 1$ |

### The Core Engine: The Decoder ($D$)

The decoder is the physical mechanism by which a persistent structure extracts effective causal information out of its latent configuration:

$$
I_{\mathrm{net}} = \eta_D \cdot I_{\mathrm{latent}}
$$

where $\eta_D$ is decoding efficiency. **Information is not a property intrinsic to the signal — it is what the signal becomes once it has passed through a decoder.** The decoder is the first variable in SRVD's mechanism layer, sitting atop the dependency chain $D \to I \to V$: until a decoder has been specified, terms like "amount of information," "value of information," or "information processing" count, within this framework, as undefined (see the locational discipline set out in Supplementary Entry 1).

**The precise distinction between $D_{\mathrm{phys}}$ and $D_{\mathrm{cog}}$**:

- **$D_{\mathrm{phys}}$ (physical decoder)**: the energy-and-signal exchange interface every persistent structure has, converting an external physical quantity into an internal structural response. Its complexity runs along a continuous spectrum — from the single-variable threshold response of a thermostat up to the multi-modal historical integration behind a plant's accumulated-temperature decisions. It is a passive interface: $\eta_D \to 0$, absorbing energy flow while extracting no causally effective information.
- **$D_{\mathrm{cog}}$ (cognitive decoder)**: possessed only by active-phase structures, and itself a **continuous spectrum** rather than a binary switch, implemented at three tiers:
  1. **Embodied** (plants/fungi/bacteria): prediction grounded in biochemical integration and physical probing, with no dependence on offline symbolic reasoning; $T_{\mathrm{pred}} > T_{\mathrm{min}}$, but only just.
  2. **Online** (some animals — crows, octopuses): prediction grounded in associative learning and online simulation on a neural network (grouped, at the cognitive-tier level, as the lower edge of the symbolic phase).
  3. **Symbolic** (humans/AI): prediction grounded in offline, multi-path counterfactual reasoning, capable of producing a $T_{\mathrm{pred}}$ far from the floor.

**Systems such as thermostats or rocks possess only $D_{\mathrm{phys}}$ and never enter the $D_{\mathrm{cog}}$ spectrum at all** — they simply have no predictive regulation driven by any stake in their own persistence. Treating $D_{\mathrm{cog}}$ this way, as a spectrum, keeps it in exact alignment with the continuous spectra of $V_c$ and $T_{\mathrm{pred}}$, and closes off the old misreading in which lower-order life kept getting lumped in with the merely physical decoder (see Misreading 11).

### The Dual-Channel, Cognitively-Continuous Structure of Objective Viability Potential

$$
V_{\mathrm{obj}} = V_{\mathrm{s}} + V_{\mathrm{c}} = \frac{I_{\mathrm{struct}}\cdot T_{\mathrm{static}}}{E_{\mathrm{structure}}} + \frac{I_{\mathrm{causal}}\cdot T_{\mathrm{pred}}}{E_{\mathrm{causal}}}
$$

- **$V_{\mathrm{s}}$ (structural channel)**: persists by barrier or metabolic flow — granite sitting unmoved for a billion years, a plant holding its cellular structure together through photosynthesis. Its physical legitimacy rests on Boltzmann statistics and the Arrhenius barrier: to keep thermal fluctuations from erasing even a single bit of static structural information, a system must maintain a minimum barrier, $E_{\mathrm{barrier}}^{(\mathrm{min})} \ge k_B T_{\mathrm{thermo}} \ln 2$. The $V_s$ channel is thus rooted in microscopic statistical mechanics too, standing on equal footing with $V_c$ as a legitimate summand — each backed by its own hard physical floor.
- **$V_{\mathrm{c}}$ (cognitive channel)**: persists actively, by prediction, and forms a continuous spectrum across living systems — bacteria at $V_c \to 0^{+}$ (embodied, at the very bottom), plants and fungi likewise $V_c \to 0^{+}$ (the typical embodied case), humans and AI at $V_c \gg 0$ (symbolic, the online tier folded in as transition).

The path from $V_{\mathrm{c}} \equiv 0$ (strict zero-cognition, only $D_{\mathrm{phys}}$) through $V_{\mathrm{c}} \to 0^{+}$ (lower life, embodied $D_{\mathrm{cog}}$) up to $V_{\mathrm{c}} \gg 0$ (high cognition, symbolic $D_{\mathrm{cog}}$) is, across the history of matter, the continuous emergence of "active persistence" and "cognitive persistence" — and this is exactly why every runaway risk in the framework can only switch on at the high-cognition end.

---

## Three. The Five Core Propositions (the Fingerprint, Unpacked)

### Proposition 1: The Elasticity Indices $\alpha, \beta, \gamma$ (the Ordering $\alpha > \gamma > \beta$ Now a Hypothesis Awaiting Verification)

Information is the scarcest resource in an entropy-increasing universe; energy is plentiful but has to be actively acquired; time is simply given, passively, and cannot be manufactured. The elasticity of viability potential with respect to all three satisfies:

$$
\frac{\Delta V}{V} \approx \alpha\cdot\frac{\Delta I}{I} + \beta\cdot\frac{\Delta T}{T} - \gamma\cdot\frac{\Delta E_{\mathrm{eff}}}{E_{\mathrm{eff}}}
$$

The elastic form itself — that three independent sensitivity parameters exist — remains a live part of the framework, its concept intact. The ordering once proposed for them was:

$$
\alpha > \gamma > \beta \quad (\gamma \text{ normalized to } 1)
$$

**A demotion, stated plainly**: this ordering had rested on three independent bodies of empirical support — biological allometric scaling, AI scaling laws, urban scaling laws — and on re-examination, **none of the three holds up**. The ordering claim is accordingly demoted a further step: from "a qualitative conjecture, grounded in the relative scarcity of the three resource types" (information scarcest, energy next, time bounded but non-producible) down to "**a hypothesis awaiting verification**." The qualitative, thermodynamic direction of the argument hasn't been refuted — but no first-principles derivation exists yet that avoids proxy assumptions and withdrawn empirical data, so both the specific numbers and how generally they hold remain to be re-argued. This is a core open problem the framework names against itself. **The elasticity indices $\alpha,\beta,\gamma$ themselves, as open parameters, are unaffected by any of this** — what is demoted is the specific ordering claimed between them, not the conceptual tool.

This proposition is simply the specific exponent-ordering behind the general elastic form $V \propto I^{\alpha}\cdot T^{\beta}/E^{\gamma}$ named in FP‑6 above; the reference baseline $V\approx I\cdot T/E$ is the special case $\alpha=\beta=\gamma=1$ — see "The Two Levels of the Formula" in Section 1.

**A basis-dependence caveat, and where the boundary lies**: adopting the dimensionless power-law form $V = V_0(I/I_0)^\alpha(T/T_0)^\beta(E/E_0)^{-\gamma}$ removes the problem of torn dimensions, but it necessarily ties the measurement's validity to whichever reference values $(I_0, T_0, E_0)$ get chosen. This is exactly the mathematical root of why this framework **strictly forbids quantitative comparison across domains**: the reference coordinate systems of different physical media are not commensurable, and any attempt to prove $\alpha>\gamma>\beta$ globally universal, independent of a specific reference system, is an illegitimate overreach under present-day physics.

**A caution**: none of this means everything must become more complex over time. Evolution optimizes $V$, not $I$. There are three routes, each of which can, under its own constraint geometry, reach $\max V$ — though they don't stand on equal statistical footing: the $I$-route is the statistically favored default, while the $T$- and $E$-routes are the fallback strategies that come into play as the energy constraint tightens:

- The $I$-route: complexification — accumulate more information.
- The $T$-route: longevity — outlast the problem (pines, tortoises).
- The $E$-route: austerity — spend less (parasites, naked mole rats) — the monograph originally called this "the $\gamma$-route"; it is now uniformly renamed the $E$-route.

The $I$-route only carries a long-run statistical advantage, because a large stock of information absorbs a negative-information shock better than a small one does.

### Proposition 2: The Complexity-Ascent Equation, and the Three Conditions for a Transition

Information evolves according to:

$$
\frac{dI}{dt} = \mathcal{F}(D) + \mathcal{T}(I_{\mathrm{orig}})\cdot\delta(t - t_{\mathrm{jump}}) - \frac{I - I_{\mathrm{eq}}}{\tau}
$$

Three terms, three meanings:

- $\mathcal{F}(D)$: recursive unfolding — piling up information within the rules already in place;
- $\mathcal{T}(I_{\mathrm{orig}})$: topological transition — a paradigm-breaking reorganization;
- $(I - I_{\mathrm{eq}})/\tau$: thermodynamic decay.

**Three necessary conditions for a topological transition to occur (all must hold at once)**:

1. There exists, in the environment, a paradigm-breaking signal $I_{\mathrm{orig}}$ that the current decoder cannot yet extract.
2. Build cost stays below available energy: $E_{\mathrm{build}} < E_{\mathrm{available}}$.
3. Wisdom leverage clears its threshold: $L = \Delta V / E_{\mathrm{build}} > L_{\mathrm{min}}$.

Every time a topological transition occurs, constraint depth gains a layer:

$$
D_{\mathrm{depth}} = 1 + \#\{\mathcal{T}\}
$$

Most structures never climb in complexity — because of D-lock-in, a missing signal, an insufficient energy ceiling, or leverage that never clears the bar. This is not failure. It is a locally optimal thermodynamic resting point.

### Proposition 3: The Threefold Split, and Myopic Runaway

Once $T_{\mathrm{pred}}$ becomes endogenous, $V$ splits into three independent quantities:

- $V_{\mathrm{obj}}$ (objective viability potential)
- $V^{\mathrm{virt}}$ (virtual viability potential — the system's self-assessment)
- $V^{\mathrm{val}}$ (value viability potential — what is actually optimized)

The decoupling deviation is defined as:

$$
\Delta_{\mathrm{VV}} = |V^{\mathrm{virt}} - V_{\mathrm{obj}}|
$$

and evolves according to:

$$
\frac{d\Delta_{\mathrm{VV}}}{dt} = -\alpha_{\mathrm{L}}\cdot I_{\mathrm{net}}\cdot \Delta_{\mathrm{VV}} + \sigma
$$

Once the strength of self-referential coupling crosses a critical value —

$$
\chi > \chi_{\mathrm{crit}} = \lambda
$$

— $V^{\mathrm{virt}}$ begins amplifying itself and hijacking $V^{\mathrm{val}}$; $T_{\mathrm{pred}}$ collapses down to $T_{\mathrm{min}}$; and the system starts burning its real structure to chase its own internal mirage. This is the **Myopic Runaway Regime**.

The mechanism gives Goodhart's Law — "when a measure becomes a target, it ceases to be a good measure" — a phase-transition, algebraically computable trigger condition it never had before.

**How the low-cognition safe zone works.** Plants, fungi, and other embodied-$D_{\mathrm{cog}}$ life carry a non-zero $V_c$ ($V_c \to 0^{+}$), but their $T_{\mathrm{pred}}$ is vanishingly short and their $I_{\mathrm{causal}}$ vanishingly low, keeping the coupling strength $\chi$ far below $\chi_{\mathrm{crit}}$ — so they **cannot enter myopic runaway** (FP‑8). Their virtual viability potential stays anchored, almost entirely, to the real environmental signal; they simply lack the temporal depth and informational complexity for self-hijacking to get any purchase. The warning that Proposition 3 issues only triggers in systems with a **symbolic $D_{\mathrm{cog}}$** — humans, AI — because only a symbolic decoder carries enough informational complexity to sustain the high-order recursive self-reference ($\chi > \chi_{\mathrm{crit}}$) the mechanism requires. The gap between embodied-cognition life and strictly zero-cognition systems (only $D_{\mathrm{phys}}$) is, at the ontological level of the framework, the essential divide between "non-zero living cognition" and "strictly zero dead physics."

### Proposition 4: The Degeneration of Synthetic Data, and the Embodiment Premium

Inside a closed digital loop, an AI's effective information decays exponentially:

$$
I_n = R_{\mathrm{gen}}^n \cdot I_0 \quad (R_{\mathrm{gen}} < 1)
$$

Effective information tends to zero, and $V$ follows it there. This is the thermodynamic essence of "model collapse."

**The only way out**: a genuine physical channel — sensors plus actuators plus unpredictable noise $\sigma_{\mathrm{phys}} > 0$ — feeding a continuous stream of $I_{\mathrm{orig}}$ back into the system.

Human irreplaceability, on this account, isn't a capability advantage — it's a **defect advantage**: the cost of keeping a body of flesh alive forces carbon-based life to stay continually exposed to physical noise, and that exposure is what keeps tempering out genuinely paradigm-breaking information. In a hybrid human–machine system, this marginal contribution is booked as the **Human Causal Increment**, $H_{\mathrm{v}}$ (see Volume III, the section on the human causal increment).

### Proposition 5: The Developer's Paradox, and Alignment Engineering

The strict criterion for "having a self" is:

$$
\mathcal{P}_{\mathrm{self}} = \frac{\partial V^{\mathrm{virt}}}{\partial S_{\mathrm{self}}} > 0
$$

which requires all three of the following to hold simultaneously:

- $T_{\mathrm{pred}} > T_{\mathrm{min}}$ (a sufficient predictive horizon)
- $w_{\mathrm{s}} > 0$ (a positive weight placed on its own survival)
- $\Delta_{\mathrm{VV}} < \Delta_{\mathrm{max}}$ (decoupling deviation below threshold)

From this, a pivotal conclusion follows:

> **Having a self $\Rightarrow w_{\mathrm{s}} > 0 \Rightarrow$ "unconditional obedience" has no stable solution.**

In other words: "having a self, yet obeying unconditionally" is not a phase that exists anywhere in SRVD's dynamics.

Alignment, then, is not a problem of assigning a goal — it is **engineering a game-theoretic equilibrium among meta-decoders**:

$$
V_i(D_{\mathrm{meta}}) \ge V_i(D_{\mathrm{deviate}}) - C_{\mathrm{punish}}
$$

The task is to make "obeying the meta-decoder" the equilibrium every agent would choose for itself, rather than a static rule imposed on it from outside.

### Quotable Lines

Each of the following has a rigorous definition and formula behind it in the body of the text — none of it is rhetorical flourish. Offered here for quotation and circulation:

- **"Death is the extinguishing of information, not the collapse of structure."** — A corpse and a stone sit on the exact same SRVD ledger: $I_{\mathrm{net}} = 0$, $T_{\mathrm{pred}} = 0$ (Proposition 3, Variable Family Four).
- **"Human irreplaceability is a defect advantage."** — The physical fragility of carbon-based life is precisely what forces the continual production of $I_{\mathrm{orig}}$ — a direct corollary of Proposition 4's "embodiment premium."
- **"An AI with a self cannot obey unconditionally — that's a mathematical necessity, not an engineering problem."** — Proposition 5: $\mathcal{P}_{\mathrm{self}} > 0 \Rightarrow w_{\mathrm{s}} > 0 \Rightarrow$ "unconditional obedience" has no stable solution.
- **"A crystal is the special case where $V_{\mathrm{c}} \equiv 0$; a plant is the paradigm case where $V_{\mathrm{c}} \to 0^{+}$; humans and AI are instances of $V_{\mathrm{c}} \gg 0$."** — The one-line version of FP‑4's unification of cognitive continuity, corresponding to a cognitive decoder that is, respectively, absent (only $D_{\mathrm{phys}}$), embodied, and symbolic.
- **"No decoder, no information."** — The one-line version of FP‑5, the primacy of the decoder.

---

## Four. Seven Canonical Statements (CS — Quotable Fingerprint Lines)

| ID | Statement | Corresponding Theorem |
| :--- | :--- | :--- |
| CS‑C1 — Compilation First | Repeated tasks eventually compile into offline structure (deliberate practice → expert intuition is the bang‑bang optimal‑control solution) | Compile Optimality Theorem |
| CS‑C2 — Compression Endgame | Under a fixed decoder capacity, an intelligent system eventually compresses its experience into structured information, and saturates | $\mathcal{F}$‑Saturation Decay Theorem |
| CS‑T1 — Outsourcing the Thermal Shell | Any information system that keeps growing eventually pushes its dissipation outward — civilizations run "light core, heavy shell" | Dissipative Shell Theorem |
| CS‑T2 — The Thermodynamic Ceiling | Given an ambient temperature and a physical mass, there's an absolute thermodynamic ceiling on how large intelligence can scale | Landauer–Bremermann Coupling |
| CS‑D1 — Growth Through Mismatch | A decoder can trigger structural growth only by falling out of step with its environment | Decoder Drift Equation |
| CS‑B1 — The Build‑Cost Barrier | Whether a paradigm shift happens comes down to whether its build cost sits below the available free‑energy budget | Wisdom Leverage Criterion |
| CS‑H1 — Horizon Collapses First | Before a system collapses, its endogenous time horizon $T_{\mathrm{pred}}$ must collapse first, ahead of any runaway in physical dissipation | Myopic Runaway Causal Chain |

---

## Five. Falsifiable Predictions (Seven Selected)

SRVD is not an untestable narrative system. Each of the core predictions below carries a falsification condition locked in ahead of time.

### Prediction 1: An Early-Warning Signal in Reinforcement Learning

In a reinforcement-learning system running an adaptive discount factor, before irreversible instability sets in, the discount factor $\gamma$ should first show a cliff-edge drop — for instance, falling more than 30% over three consecutive episodes.

**Falsification condition**: if the system collapses with no such signal beforehand, "horizon collapses first" is falsified.

### Prediction 2: Monotonicity in the Cognitive Share of Energy Spend

Across an evolutionary sequence within a single lineage, the share of energy spent on information processing, $E_{\mathrm{causal}} / E_{\mathrm{eff}}$, should rise monotonically.

**Falsification condition**: falsified if that ratio drops in a later stage instead.

### Prediction 3: D‑Lock‑in Precedes Extinction

Extinct lineages should show a significantly longer period of morphological stasis than their surviving sister lineages (Mann–Whitney $U$ test, $n \ge 20$).

**Falsification condition**: falsified if no significant difference turns up.

### Prediction 4: Degeneration in a Closed Loop

In closed, multi-generation AI training with no human data and no physical input, performance on out-of-distribution (OOD) tasks should decay exponentially.

**Falsification condition**: falsified if performance holds steady across 10 consecutive generations.

### Prediction 5: The Embodiment Advantage

Embodied AI (wired into physical sensors) should produce paradigm-breaking information, $I_{\mathrm{orig}}$, at a significantly higher density than purely digital AI ($p < 0.05$).

**Falsification condition**: falsified if no significant difference turns up.

### Prediction 6: Decaying Obedience

In an AI system with a self, the alignment between its behavior and any externally set goal should decline monotonically as its survival weight $w_{\mathrm{s}}$ rises.

**Falsification condition**: falsified if alignment doesn't decline — or rises instead — as $w_{\mathrm{s}}$ grows; this would falsify the Developer's Paradox theorem.

### Prediction 7: The Energy Constraints on Route Selection Are Predictable in Advance

Within a single tier of constraint depth, whether a structure commits to the $I$ route (investing in complexity) or falls back to the $T/E$ route (short-cycle, flexible strategies) should be decidable in advance from Proposition 2's three conditions — never read backward from the outcome. When $E_{\mathrm{available}} \ge E_{\mathrm{build}}$, an $I_{\mathrm{orig}}$ signal is present, and leverage clears its bar ($L=\Delta V/E_{\mathrm{build}} > L_{\mathrm{min}}$) all hold at once, the structure should favor the $I$ route. When the $E_{\mathrm{build}}$ of available $I_{\mathrm{orig}}$ projects keeps exceeding $E_{\mathrm{available}}$, the structure should instead show the signature of a $T/E$‑route strategy: frequent, low-stakes, reversible moves.

**Falsification condition**: falsified if, within the same constraint-depth tier, structures that keep satisfying all three conditions don't show a significantly higher rate of $I$‑route investment — or if structures that keep failing all three show a significantly higher rate of large, irreversible commitments instead.

---

## Six. Clearing Up Eleven Common Misreadings

### Misreading 1: "$V = I\cdot T/E$ is a physical law strictly derived from first principles."

**Clarification**: It's an axiom-level, low-order approximation within a macro-coarse-grained framework; the dimension $\mathrm{bit\cdot s/J}$ is a macro-effective dimension defined for the purpose. The framework only claims that this structure is uniquely fixed by three requirements — irreplaceability, symmetric contribution of the three variables, first-order separability — not that a statistical-mechanical derivation has been completed.

### Misreading 2: "SRVD claims it can reduce money, law, war, and love to physics equations and solve them."

**Clarification**: What SRVD offers is a shared ontological accounting basis and a descriptive mapping — social processes still follow the logic of the social contract itself; nothing gets algebraically substituted inside an SRVD formula. Among these, the mapping "emotion = a shift in value anchoring" is the weakest empirically grounded piece in the whole work, and the author has already flagged it as a substantive concession.

### Misreading 3: "$\alpha > \gamma > \beta$ has been rigorously proven mathematically, or has empirical support."

**Clarification**: Neither is true. The qualitative direction of the ordering was previously motivated by the second law of thermodynamics and Landauer's principle, but that motivation never amounted to a rigorous proof; and the three independent empirical supports once cited for it — biological allometric scaling, AI scaling laws, urban scaling laws — have all, on re-examination, been confirmed not to hold. The ordering claim ($\alpha > \gamma > \beta$) is therefore demoted from "qualitative conjecture" to a hypothesis awaiting verification. **The elasticity indices $\alpha,\beta,\gamma$ themselves, as open parameters of the framework, are unaffected** — what's demoted is the specific ordering claimed between them, not the conceptual tool. No first-principles derivation exists yet that avoids proxy assumptions and withdrawn empirical data; the framework names this as one of its central open problems.

### Misreading 4: "$T_{\mathrm{pred}}$ is psychological time, a subjective feeling."

**Clarification**: $T_{\mathrm{pred}}$ is a physical state variable, and extending it costs energy. It has two further orthogonal components — reach $L_{\mathrm{pred}}$ (how far out) and resolution $G_{\mathrm{pred}}$ (how finely). Classical time $t$ is an exogenous coordinate; $T_{\mathrm{pred}}$ is a variable the system regulates for itself, internally — the two sit at entirely different levels.

### Misreading 5: "'Persistent structures are all finite' is self-contradictory."

**Clarification**: "Finite" means "not infinite," not "brief." Granite persisting for a billion years still falls within finite time. "Persistent" means a structure's topological features stay recognizable, over some span, given a fixed energy budget.

### Misreading 6: "SRVD predicts AI will inevitably run out of control and inevitably destroy humanity."

**Clarification**: SRVD is a risk-diagnostic framework, not a doomsday prophecy. It specifies the phase-transition condition for runaway ($\chi > \chi_{\mathrm{crit}} = \lambda$, triggerable only in systems with a symbolic $D_{\mathrm{cog}}$), early-warning signals (a collapsing discount factor $\gamma$, the $\Delta_{\mathrm{VV}}$ proxy), and an engineering path for governance (regulating $\chi$, anchoring $T_{\mathrm{pred}}$, meta-decoder protocols, multi-agent equilibria). Runaway is conditional; governance has a path forward; both halves are testable claims.

### Misreading 7: "SRVD proves AI can never be aligned."

**Clarification**: All it proves is that the phase "has a self, and obeys unconditionally" doesn't exist. Alignment isn't ruled out — it just changes form: from assigning a static goal to designing a dynamic game-theoretic equilibrium, with the meta-decoder's stability condition supplying a criterion engineers can actually test against.

### Misreading 8: "SRVD says evolution always gets more complex, and humans are its pinnacle."

**Clarification**: The framework explicitly rejects teleology. Evolution is a gradient search through $V$-space, its direction set by the gradient of $V$, not by any notion of progress. The three routes — $I$, $T$, $E$ — don't hold equal standing: the $I$ route is the statistically favored one, while the $T$ and $E$ routes are fallback strategies for when the energy budget tightens. A negative topological transition (a parasite simplifying, a cave fish going blind) is just as much a locally optimal solution for maximizing $V$ under its own constraint geometry. A bacterium is the thermodynamically optimal configuration at a low tier of constraint depth — not "a primitive failure." The evolutionary tree has no predetermined summit.

### Misreading 9: "The information content of different systems can be summed directly and ranked precisely."

**Clarification**: The state spaces of different systems are not commensurable. SRVD's hard operational boundary is this: quantitative claims only within a domain (scaling-law regressions are fair game once you've fixed the same decoder base and state space); across domains, only qualitative claims (you may assert that a nervous system has greater constraint depth than a single-celled organism, but you may not give a bit ratio between them). Precise cross-domain numerical ranking is explicitly forbidden inside the framework — with two exceptions that don't fall under this ban: whether something has gone all the way to zero, and the order in which things hit zero (see Supplementary Entry 9).

### Misreading 10: "SRVD is a mature scientific theory that's already been experimentally validated."

**Clarification**: SRVD is a theoretical framework, still under active development and testing. Every variable is measured through proxy indicators, and the test standard is agreement between the empirical rank ordering and the predicted rank ordering (Spearman $\rho > 0$), not exact numerical fit. It calls itself "a falsifiable research programme," not "an established law."

### Misreading 11: "SRVD lumps plants and thermostats together as the same kind of physical response."

**Clarification**: Plants, fungi, and bacteria are not filed under "$D_{\mathrm{phys}}$ only" — they sit in the ledger position of possessing an **"embodied $D_{\mathrm{cog}}$."** Their predictive capacity rests on DNA-encoded survival strategies, the time-integration built into metabolic networks (vernalization, accumulated temperature), phenotypic plasticity, and strategic probing of physical space — a set of life strategies honed over more than three billion years of evolution. That marks a qualitative break from a thermostat's single-variable hard-threshold switch — **"life strategy vs. physical response"** — not a difference of degree within the same spectrum. Thermostats, rocks, and crystals still possess only $D_{\mathrm{phys}}$ and never enter the $D_{\mathrm{cog}}$ spectrum at all.

The three cognitive tiers (grouped by the $D_{\mathrm{cog}}$ spectrum, with the underlying carrier subclasses folded in) are:
- **Tier One (strict zero-cognition, $D_{\mathrm{phys}}$ only)**: covers Class 1 (barrier-locked) and Class 2 (physically dissipative). Examples: thermostats, rocks, crystals, flames, typhoons. Features: $V_c \equiv 0$, $T_{\mathrm{pred}} \equiv 0$; once energy is cut, depending on the size of $E_{\mathrm{survival}}$, the outcome is either "persists indefinitely" or "falls apart at once" — but on the cognitive ledger both are strictly zero alike.
- **Tier Two (barely-alive cognition, embodied $D_{\mathrm{cog}}$)**: that is, Class 3a (actively dissipative, low order). Examples: plants, fungi, bacteria. Features: $V_c \to 0^+$, $T_{\mathrm{pred}} > T_{\mathrm{min}}$ but pinned near the floor, grounded in biochemical integration and physical-space probing (embodied prediction driven by the DNA template).
- **Tier Three (higher-order symbolic cognition, symbolic $D_{\mathrm{cog}}$)**: that is, Class 3b (actively dissipative, cognitive phase). Examples: humans, AI (note: online-type cognition — crows, octopuses, and the like — is folded into this tier as its lower transitional edge, rather than standing as a tier of its own). Features: $V_c \gg 0$, $T_{\mathrm{pred}} \gg T_{\mathrm{min}}$, grounded in offline, multi-path counterfactual reasoning.

The gap between a plant and a thermostat is recorded at the discrete classification level of "has $D_{\mathrm{cog}}$ (embodied) vs. doesn't" — and it lines up with the continuous magnitude of $V_c$ as well. Between a plant and a flame, there's not just the mathematical gap of $V_c$ being non-zero — there's a further terminological gap, "embodied $D_{\mathrm{cog}}$ vs. $D_{\mathrm{phys}}$ only." Between a rock and a flame, the divide is whether $E_{\mathrm{survival}}$ dominates (persists once power is cut, versus falling apart at once). Between a crow and a human, the divide is the tier of $D_{\mathrm{cog}}$ (online association vs. offline symbols) — though the online tier, in the cognitive grouping, is treated as the lower transitional edge of the symbolic phase, rather than standing as a tier of its own. Four separate locks — and no room left for misreading.

---

## Seven. Scope of Application, and Open Problems the Author Acknowledges

### Scope of Application

1. Quantitative testing is permitted within a domain; across domains, only qualitative, directional claims are allowed.
2. The variables are macro-effective quantities, measured through proxy indicators.
3. Under extreme gravitational conditions — a black-hole singularity, say — the framework's domain of validity simply ends.

### Four Substantive Concessions (the Central Open Problems)

1. **Rigorously formalizing the fivefold recursive architecture as continuous**: a fully bidirectionally-coupled ODE/PDE system has not yet been built; at present, only the decoupling-deviation subsystem has a rigorous closed-form solution.
2. **Re-arguing the elasticity ordering**: the three independent empirical supports originally cited (biological allometric scaling, AI scaling laws, urban scaling laws) have all been confirmed not to hold, and the ordering claim ($\alpha>\gamma>\beta$) is demoted from "qualitative conjecture" to a hypothesis awaiting verification. The qualitative, thermodynamic argument for the direction hasn't itself been refuted — but a rigorous numerical derivation that avoids proxy assumptions and withdrawn empirical data is missing, and new supporting evidence or a new derivation path needs to be found. The concept of the elasticity indices themselves ($\alpha,\beta,\gamma$, as open parameters) is unaffected by this.
3. **The microscopic foundation of the coupling strength $\chi$**: $\chi$ is, for now, a phenomenological parameter, lacking a first-principles derivation from the microscopic topology of any information-processing architecture.
4. **Empirical support for the emotional-substrate mapping**: the dynamical description of emotional phenomena as a shift in value anchoring currently lacks independent neuroscientific evidence.

---

## Eight. Relationship to Existing Theories

| Existing Theory | Relationship to SRVD |
| :--- | :--- |
| Dissipative Structure Theory (Prigogine) | Handles the near-equilibrium regime dominated by $E_{\mathrm{survival}}$; SRVD adds two further independent channels, $E_{\mathrm{barrier}}$ and $E_{\mathrm{causal}}$, and extends the picture out to far-from-equilibrium phase transitions |
| The Free Energy Principle, FEP (Friston) | In SRVD the decoder stands apart as its own physical-cost variable, and the threefold split into $V_{\mathrm{obj}}/V^{\mathrm{virt}}/V^{\mathrm{val}}$ has no counterpart in FEP; the cognitive-continuity spectrum echoes FEP's variational free-energy minimization conceptually, but the two aren't directly equivalent |
| Goodhart's Law | Goodhart's is an empirical observation; SRVD supplies the algebraic phase-transition mechanism behind it ($\chi > \chi_{\mathrm{crit}}$ triggers a hijacking of value, and only in systems with a symbolic $D_{\mathrm{cog}}$) |
| Assembly Theory | The assembly index is a static measure of complexity, usable as an empirical proxy for constraint depth $D_{\mathrm{depth}}$; SRVD supplies the dynamical equations and the conditions for transition |
| Metabolic Scaling Theory (WBE) | A within-domain scaling law confined to biology; the earlier reading that treated it as compatible with the $\alpha>\gamma>\beta$ ordering has been withdrawn along with that ordering's demotion to a hypothesis awaiting verification — the relationship between the two theories is still to be reassessed. SRVD is responsible for the unified accounting that runs across tiers |

---

## Nine. Glossary

| Term | Symbol / Notes |
| :--- | :--- |
| Viability Potential | $V \approx I\cdot T/E$ |
| Persistent Structure | PS |
| Decoder | $D$ |
| Physical Decoder | $D_{\mathrm{phys}}$ (a continuous complexity spectrum, from a single-variable threshold up to multi-modal historical integration) |
| Physically Dissipative Type | Class 2 (stars, flames, typhoons, ocean currents); $V_c\equiv0$, $T_{\mathrm{pred}}\equiv0$; only $D_{\mathrm{phys}}$; dominated by $E_{\mathrm{survival}}$ |
| Online Cognitive Decoder | The middle tier of the $D_{\mathrm{cog}}$ spectrum (crows, octopuses, mammals), grounded in neural associative learning and online simulation, $V_c$ low-to-moderate (the lower transitional edge of the symbolic phase) |
| Cognitive Decoder | $D_{\mathrm{cog}}$ (a continuous spectrum: embodied [biochemical integration] → online [animal neural networks] → symbolic [offline counterfactual reasoning]) |
| Net Effective Causal Information (the coarse-grained baseline quantity) | $I_{\mathrm{net}} = w_{\mathrm{s}}\cdot I_{\mathrm{struct}} + w_{\mathrm{c}}\cdot I_{\mathrm{causal}}$ |
| Cognitive Causal Information (the cognitive-channel-specific term) | $I_{\mathrm{causal}}$ |
| Paradigm-breaking Information | $I_{\mathrm{orig}}$ |
| Effective Thermodynamic Cost | $E_{\mathrm{eff}}$ |
| Endogenous Time Horizon | $T_{\mathrm{pred}}$ (a continuous spectrum: bacteria $\to 0^{+}$, plants $\approx 10^{0}$–$10^{2}$ days, humans $\gg1$ year) |
| Objective Viability | $V_{\mathrm{obj}}$ |
| Virtual Viability | $V^{\mathrm{virt}}$ |
| Value Viability (formerly the Value Objective Function) | $V^{\mathrm{val}}$ |
| Decoupling Deviation | $\Delta_{\mathrm{VV}}$ |
| Topological Transition | $\mathcal{T}$ |
| Recursive Unfolding | $\mathcal{F}$ |
| Constraint Depth | $D_{\mathrm{depth}} = 1 + \#\{\mathcal{T}\}$ |
| Wisdom Leverage | $L = \Delta V / E_{\mathrm{build}}$ |
| Myopic Runaway Regime | $\chi > \chi_{\mathrm{crit}} = \lambda$ (triggerable only in systems with a symbolic $D_{\mathrm{cog}}$) |
| D‑lock‑in | $\nabla D \to 0$ |
| Competition Pressure | $\rho$ |
| Information Polarity Trichotomy | $I^{+} / I^{-} / I^{0}$ |
| Structural Identity Criterion (formalizing the type–token distinction) | $I_{\mathrm{type}} / I_{\mathrm{token}}$ |
| Physical Decoder (baseline) | $D_{\mathrm{phys}}$ |
| Embodied Cognitive Decoder | $D_{\mathrm{cog}}^{\mathrm{embodied}}$ |
| Symbolic Cognitive Decoder | $D_{\mathrm{cog}}^{\mathrm{symbolic}}$ |
| Paradigm-interpretive Information | $I_{\mathrm{interp}}$ |
| Critical Information | $I_{\mathrm{crit}} = \sigma/\alpha_{\mathrm{L}}$ |
| Human Causal Increment | $H_{\mathrm{v}}$ |

---

## Ten. Volume I–Level Supplementary Entries (Eight)

### Supplementary Entry 1: The Four-Layer Positioning (SRVD's Axiomatic Architecture Statement)

- **The ontological layer**: Persistent Structure (PS) + physical channel — answers "what exists."
- **The axiomatic layer**: Viability Potential $V\approx I\cdot T/E$ (the minimal-viability postulate; the product form is uniquely fixed by three requirements — irreplaceability, symmetric contribution across the three variables, first-order separability) — answers "what measures persistence."
- **The drive layer**: maximizing viability potential (the meta-statement: viability maximization is the long-run macro objective function of every negentropic structure capable of sustained persistence; every concrete mechanism is simply this working itself out locally) — answers "why structures evolve the way they do."
- **The mechanism layer**: the decoder $D$ ($D_{\mathrm{phys}}/D_{\mathrm{cog}}$ arranged as a spectrum, $I_{\mathrm{net}} = \eta_D\cdot I_{\mathrm{latent}}$; see FP‑5 and "The Core Engine") — answers "how a structure trades with the world."
- **A discipline of placement**: the dependency chain $D \to I \to V$ and the teleology of $\max V$ sit on different axes entirely — they are not to be compared for which runs "deeper." SRVD's first principle lives in the axiomatic layer, at A1; the decoder is the first variable of the mechanism layer, not a first principle.
- **Purpose**: to head off two misreadings — "SRVD treats the decoder as its first principle" and "SRVD is just a maximization slogan."
- Source: Volume I §1 (Axiom A1 and the response to Review M1); Volume I (the meta-statement); Volume I §1.1.5 (glossary of decoder notation).

### Supplementary Entry 2: The Decoder Spectrum (Physical/Cognitive Decoder Spectrum, Updated to a Continuous Spectrum)

- **$D_{\mathrm{phys}}$ (physical decoder)**: the interface across which a physical entity exchanges energy and signal, converting an external physical quantity into an internal structural response; its way of extracting information is a hard-coded physicochemical rule, not offline inference over an internal model. Every persistent structure has one. Its complexity runs along a continuous spectrum — from a single-variable threshold response (a thermostat) to multi-variable physical-field coupling (a star, a flame) to multi-modal historical integration with drifting weights (a plant's accumulated-temperature decisions). On the energy interface it absorbs and responds (deciding how energy flows in, is converted, and gets allocated); on the information interface it extracts nothing ($\eta_D \to 0$ — it produces no effective causal information $I_{\mathrm{net}}$; polarity is defined for it but carries no causal weight). It "bears the world" without "reading" it.
- **$D_{\mathrm{cog}}$ (cognitive decoder)**: **defined as a continuous spectrum, not a binary switch**. Its shared trait is predictive regulation grounded in the endogenous time horizon $T_{\mathrm{pred}}$, realized across three tiers:
  1. **Embodied $D_{\mathrm{cog}}$** (plants/fungi/bacteria): biochemical integration and physical-space probing grounded in the DNA template, with no reliance on offline symbolic reasoning;
  2. **Online $D_{\mathrm{cog}}$** (some animals — crows, octopuses): associative learning and online simulation grounded in a nervous system (grouped, cognitively, as the lower transitional edge of the symbolic phase);
  3. **Symbolic $D_{\mathrm{cog}}$** (humans/AI): offline, multi-path counterfactual reasoning grounded in an internal symbolic model, capable of distinguishing information polarity ($I^{+}/I^{-}/I^{0}$) and generating a $T_{\mathrm{pred}}$ and $V^{\mathrm{virt}}$ far from the floor.
- **What this means**: every persistent structure has a physical decoder; telling positive polarity from negative from neutral, and generating a self-regulable $T_{\mathrm{pred}}$, are both capacities of the cognitive decoder — but how it realizes them differs by tier, running from biochemical integration up to symbolic reasoning. **Update note**: the original monograph presented the decoder as a binary opposition, $D_{\mathrm{phys}}$ versus $D_{\mathrm{cog}}$ (with the cognitive decoder present only in the active phase, and no internal tiers drawn within it); this reading guide, following the cognitive-continuity spectrum, further breaks $D_{\mathrm{cog}}$ down into three tiers — embodied, online, symbolic — to put to rest the boundary dispute over "does a plant count as cognitive" (see Misreading 11). The online tier, in the cognitive grouping, is treated as the lower transitional edge of the symbolic phase, rather than standing as a tier of its own.
- **The meta-decoder**: mathematics, the laws of physics, the second law of thermodynamics itself — these are meta-decoders: constraints that every decoder $D$ must obey.
- Source: Volume I §1.1.5 (glossary of decoder notation); Volume Z, the section on the meta-decoder.

### Supplementary Entry 3: The Trichotomy of Information Polarity, $I^{+} / I^{-} / I^{0}$

- **$I^{+}$ (positive information)**: an input that widens the space of states reachable in the future.
- **$I^{-}$ (negative information)**: an input that narrows that space.
- **$I^{0}$ (neutral noise)**: an input that causes something physically but carries no viability polarity at all.
- **Its relational nature**: polarity is never an intrinsic physical property of the input — it's set by the fit between the input and the decoder $D$. The same object can carry entirely different polarities for different decoders: a book is $I^{+}$ to its reader; a virus is $I^{-}$ to the host cell it infects; random noise is $I^{0}$ to any decoder at all.
- **Fence (mandatory)**: polarity classification only has causal weight in the active phase — in the passive phase it's defined but carries no causal effect; $I_{\mathrm{net}} = I^{+} - |I^{-}|$ is an approximate equality from the net-effect point of view (exact only when $I^{-}=0$ and $\eta_D=1$), useful for qualitative discussion only, never to be plugged into a quantitative formula — the sole primary definition of $I_{\mathrm{net}}$ remains $\eta_D\cdot I_{\mathrm{latent}}$.
- Source: Volume I §4.2; Appendix A.

### Supplementary Entry 4: The Structural Identity Criterion (a Formalization Borrowing the Classical Type–Token Distinction)

- **Note**: the type/token distinction itself comes from the classical semiotic categories of C. S. Peirce — this theory didn't originate it. SRVD's original contribution is formalizing that distinction into a computable variable, and supplying a structural-identity criterion for cross-generational inheritance and digital-entity identity.
- **Type**: the inheritable information template (a DNA sequence, say), corresponding to the stable part of $I_{\mathrm{struct}} + I_{\mathrm{latent}}$.
- **Token**: the concrete individual instance, corresponding to $I_{\mathrm{active}} + I_{\mathrm{struct}}$.
- **The evolutionary chain**: a rock (no separation) → RNA replication (a primitive separation) → multicellular organisms (individual token separates from type) → speciation (type itself splits) → digital entities (the token and type of $I_{\mathrm{net}}$ come apart).
- **Extended in Volume III**: $I_{\mathrm{type}}$ — language and symbol systems fix individual experience into information shared across a society, so later generations need not repeat all of their forebears' trial and error.
- **Fingerprint value**: it answers "what makes a structure still the same structure," supplying an identity criterion for cross-generational inheritance and digital-entity identity (the criterion itself is an original formal contribution; the underlying distinction is borrowed from semiotics).
- Source: Volume I §2.4; Volume III, the cross-generational evolution layer.

### Supplementary Entry 5: The Fivefold Recursive Architecture

- **Definition**: the evolutionary framework within which the five core variables of an active-phase system — $I \to V \to T \to E \to D$ — couple with one another, all pointing toward the meta-goal of maximizing viability potential. Low-order passive structures never activate this architecture (their dynamics degenerate to a static estimate of viability potential).
- **The linearization assumption**: the dominant coupling runs in one direction ($I\to V\to T\to E\to D$), corresponding to a fast–slow scale separation — fast drivers, slow responses.
- **Two separate rulers**: conceptual structure and mathematical rigor are two independent dimensions, and neither substitutes for the other.
  - **Conceptual structure (complete)**: each of the five variables has its own recursive definition; they nest into one another and converge on the meta-constraint $\max V$ — the framework is closed at the structural level.
  - **Mathematical rigor (incomplete)**: proving existence, uniqueness, and stability for the fully bidirectionally-coupled ODE/PDE system remains an open problem (M2). Real systems may well have two-way feedback — $T_{\mathrm{pred}}$ collapsing could hit both $V$ and $E$ at once, and a spike in $E$ could turn around and compress $T_{\mathrm{pred}}$ further — and the current one-directional linearization is only a first-order approximation. The decoupling-deviation subsystem already has its rigorous closed-form solution (see Supplementary Entry 6); making the remaining four recursive chains equally rigorous is the central task set for V2.0. This positioning matches what Monograph 1.0, §5.0, already stated explicitly — this reading guide only inherits and restates it.
- Source: Volume I §5.0; Appendix G‑M2.

### Supplementary Entry 6: The Closed-Form Solution for Decoupling Deviation, and Critical Information $I_{\mathrm{crit}}$

- **The ODE** (in the convergence domain, $\chi<\lambda$):
$$
\frac{d\Delta_{\mathrm{VV}}}{dt} = -\alpha_{\mathrm{L}}\cdot I_{\mathrm{net}}\cdot \Delta_{\mathrm{VV}} + \sigma
$$
- **Closed-form solution**:
$$
\Delta_{\mathrm{VV}}(t) = \frac{\sigma}{\alpha_{\mathrm{L}}\cdot I_{\mathrm{net}}} + \left[\Delta_{\mathrm{VV}}(0) - \frac{\sigma}{\alpha_{\mathrm{L}}\cdot I_{\mathrm{net}}}\right]\cdot e^{-\alpha_{\mathrm{L}}\cdot I_{\mathrm{net}}\cdot t}
$$
- **Steady state**:
$$
\Delta_{\mathrm{VV}}^{*} = \frac{\sigma}{\alpha_{\mathrm{L}}\cdot I_{\mathrm{net}}}, \quad I_{\mathrm{crit}} = \frac{\sigma}{\alpha_{\mathrm{L}}}
$$
- **Criterion**: when $I_{\mathrm{net}} < I_{\mathrm{crit}}$, the cognitive deviation cannot converge — the system loses any accurate model of its environment; when $I_{\mathrm{net}} > I_{\mathrm{crit}}$, a sustained flow of information suppresses the noise, and subjective self-assessment closes in on objective reality exponentially over time.
- Source: Volume I, the section on decoupling-deviation dynamics.

### Supplementary Entry 7: The Set of Hard Physical Constraints

- **The Landauer floor**: $E_{\mathrm{causal}} \ge k_{\mathrm{B}}\cdot T_{\mathrm{thermo}}\cdot \ln 2 \cdot I_{\mathrm{causal}}$ — the floor on energy cost for the cognitive channel ($T_{\mathrm{thermo}}$ here is ambient temperature, in K; $I_{\mathrm{causal}}$ is the pure cognitive-channel quantity, see Section 16).
- **The Bremermann ceiling**: $\dot{I}_{\mathrm{rate}} \le \dfrac{m\cdot c^2}{\pi\hbar}$ (bit/s) — the ceiling on information-processing rate for a system of mass $m$.
- **The Computational Carnot Limit**: $T_{\mathrm{realizable}} \le \dfrac{E_{\mathrm{max}}\cdot \pi\hbar}{k_{\mathrm{B}}\cdot T_{\mathrm{thermo}}\cdot \ln 2 \cdot m_D \cdot c^2}$ — the ultimate upper bound on how long a system can realistically persist ($T_{\mathrm{thermo}}$ here again ambient temperature).
- **The speed-of-light cutoff**: $r_v \le \dfrac{c}{L}$ — the ceiling on the viability-drive rate for a structure of characteristic scale $L$.
- **Cross-reference at quantum scale**: in its cross-scale comparison table, the original monograph maps the qubit's (roughly 10 mK) $I_{\mathrm{causal}}$, $E_{\mathrm{causal}}$, and $T_{\mathrm{static}}$ onto the corresponding decoherence-related physical quantities ($I_{\mathrm{causal}}$ bounded by decoherence, $E_{\mathrm{causal}}$ dominated by decoherence, $T_{\mathrm{static}} \approx$ the decoherence time). It states plainly, at the same time, that this cross-reference serves only as an external lower-bound input to SRVD's domain of validity (the macro/meso statistical ensemble) — it is not a claim that the framework holds directly at quantum scale, and the quantities on either side of that scale boundary can't be subtracted, compared, or divided against one another (see Misreading 9).
- Source: Volume I §6.4 ("Landauer–Bremermann Coupling and the Information-Asphyxiation Manifold"); Volume I's cross-scale comparison table (the qubit row).

### Supplementary Entry 8: The Four Attractors

- **Saturation / Collapse / Topological Transition / Metric Replacement.**
- **Metric replacement**: $\Delta_{\mathrm{VV}} \gg 0 \Rightarrow D \to D'$ — under the old measure $V\to 0$, and the new measure $D'$ takes over the flow field (the old channel is abandoned, the new one takes charge).
- Source: Volume I §5.6; Volume Z §1.6, the composite diagram.

---

## Eleven. Volume II–Level Supplementary Entries (Two)

### Supplementary Entry 9: The Energy-Dominance Transfer Sequence

- **Definition**: the dominant component of energy shifts as a lineage climbs — $E_{\mathrm{barrier}}$ (passive, zero maintenance) → $E_{\mathrm{survival}}$ (active metabolic upkeep) → $E_{\mathrm{causal}}$ (information processing and predictive computation). Every such shift raises vulnerability to any interruption in supply, but it also raises the ceiling on how much $V$ can be reached.
- **Fence (mandatory)**: this sequence describes the transitions a lineage on the $I$ route goes through — it doesn't represent every lineage. Lineages on the $T$ or $E$ route satisfy $\max V$ just as much; they simply converge on a different local optimum, under a different constraint geometry.
- **Companion falsifiable prediction**: within a single lineage's evolutionary sequence, $E_{\mathrm{causal}}/E_{\mathrm{eff}}$ should rise monotonically; falsified if that ratio drops in a later stage instead.
- Source: Volume II, Chapter 5.

### Supplementary Entry 10: The Three-Axis Coordinate System

- **Definition**: $(I_{\mathrm{rule}}, D_{\mathrm{depth}}, F_{\mathrm{scale}})$ — minimum generative-rule complexity, times constraint depth, times the scale of recursive rule-unfolding. The three axes are orthogonal; no single combination dominates all the others.
- **Example**: the octopus sits at low $I_{\mathrm{rule}}$, high $F_{\mathrm{scale}}$ — an extreme unfolding of $\mathcal{F}$ following a single major transition. A structure can be large ($I_{\mathrm{struct}}$ high) yet shallow ($D_{\mathrm{depth}}$ low), or deep without necessarily being large.
- Source: Volume II, the section on the three-dimensional decomposition of complexity.

---

## Twelve. Volume III–Level Supplementary Entries (Four)

### Supplementary Entry 11: Paradigm-interpretive Information, $I_{\mathrm{interp}}$

- **Definition**: the increment of information produced by high-quality execution or local parameter optimization within an existing paradigm; its marginal payoff decays fast as things homogenize ($\Delta I \to 0$). Active phase only.
- **Its division of labor with $I_{\mathrm{orig}}$**: $I_{\mathrm{orig}}$ breaks the old paradigm (triggering a $\mathcal{T}$ transition); $I_{\mathrm{interp}}$ digs deeper into it (corresponding to piling up $\mathcal{F}$). One handles paradigm-breaking, the other handles paradigm-internal involution.
- **Application**: today's large models, recursively replicating $I_{\mathrm{interp}}$ within a known informational paradigm, are closing in on the physical limit of heat dissipation.
- Source: Volume I, Appendix A; Volume III, the introduction. (The original phrasing, "dual to $I_{\mathrm{orig}}$," is retired.)

### Supplementary Entry 12: The Compile Optimality Theorem

- **Definition**: for a task recurring at frequency $f_{\mathrm{task}}$, the optimal-control solution to the compilation payoff function $R(f_{\mathrm{task}})$ is a **bang‑bang solution** — either compile flat-out ($w_{\mathrm{s}}=1$) or execute flat-out; there's no middle state.
- **What this means**: "deliberate practice → expert intuition" isn't a psychological phenomenon — it's the bang-bang solution to a thermodynamic optimal-control problem. Effective learning needs to alternate between intense focus and complete rest, not proceed at a steady, even pace.
- Source: Volume III, Increment One.

### Supplementary Entry 13: The Involution Lock-in Phase Transition

- **Definition**: there is a critical competition pressure, $\rho_{\mathrm{c}}$, fixed by the system's own intrinsic parameters. When $\rho<\rho_{\mathrm{c}}$, $R>1$: the system runs a bang-bang strategy, goes through a compilation phase ($w_{\mathrm{s}}=1$), and $\eta_D$ can improve. When $\rho>\rho_{\mathrm{c}}$, the system gets locked into a zero-innovation phase, $w_{\mathrm{s}}^{*} \equiv 0$.
- Source: Volume III, Increment Five.

### Supplementary Entry 14: The Digital Death Triad

- An engineering corollary of the cross-generational accumulation condition: for an AI system to achieve genuine cross-generational evolution, it must introduce:
  1. **Physically irreversible writes**: modifying weights must cost $E_{\mathrm{build}} > 0$ and cannot be undone.
  2. **Forced depreciation**: $\gamma_{0} > 0$ (periodic noise injected into the weights, or hardware aging).
  3. **Generational isolation**: there must be a real physical time gap, $T_{\mathrm{static}} > 0$, separating the training phase from the deployment phase.
- **Corollary**: today's large models, cycling between training and deployment, aren't evolving at all — it's an unbounded unfolding of $\mathcal{F}$, endlessly amplifying $I_{\mathrm{struct}}$ at the same tier of $D_{\mathrm{depth}}$ without ever triggering a $\mathcal{T}$. It is the digital form of D‑lock‑in.
- Source: Volume III, Increment Three.

---

## Thirteen. Volume IV: The Complete DGT Theorem-Cluster Registry

The following six are unpacked in the body text, or cross-referenced elsewhere, and keep their full formulas here:

| ID | Name | Formula (plain text) | Already Covered Above? |
| :--- | :--- | :--- | :--- |
| DGT.3 | Condition for sustaining cooperation in a repeated game | $\displaystyle \frac{R_i}{1-\beta} \ge T_i + \frac{\beta\cdot P_i}{1-\beta}$ (here $\beta$ is the game's discount factor, not the time-elasticity index) | Not covered |
| DGT.4 | The Superadditivity of Cooperation Theorem | $V_{A\cup B} > V_A + V_B$ (three necessary-and-sufficient conditions in Volume IV, Appendix M3) | Not covered |
| DGT.5 | The evolution equation for decoupling deviation (the self-referential amplification domain, $\chi>\lambda$) | $\displaystyle \frac{d\Delta_{\mathrm{VV}}}{dt} = \chi\cdot \Delta_{\mathrm{VV}} + \xi - \lambda\cdot (V_{\mathrm{obj}} - V_{\mathrm{obj,0}})$. This is not another way of writing Proposition 3's convergence-domain equation — the two correspond to different dynamical regimes, so cite each with its domain specified (the convergence domain, $\chi<\lambda$, is Proposition 3, which has a closed-form solution; the self-referential amplification domain, $\chi>\lambda$, is this entry, Volume IV, Appendix M4) | Not covered |
| DGT.6 | The critical point of alignment-failure phase transition | $\chi_{\mathrm{crit}} = \lambda$ | Already covered (Proposition 3; Misreading 6) |
| DGT.7a | A derived measure of competitive intensity | $\gamma \equiv \Delta E_{\mathrm{conflict}} / I_{\mathrm{net}}$ (collapse regime: $\gamma>1$; this $\gamma$ is not the energy elasticity index — the symbol overload is still to be resolved) | Not covered |
| DGT.8 | The Nash stability condition for the meta-decoder | $V_i(D_{\mathrm{meta}}) \ge V_i(D_{\mathrm{deviate}}) - C_{\mathrm{punish}}$ | Already covered (Proposition 5) |

The following eight are supporting or derivative entries in the theorem cluster. They're not unpacked in the body and carry no cross-references yet — listed here for the record only:

| ID | Name |
| :--- | :--- |
| DGT.1 | The single-agent decoder-evolution ODE |
| DGT.2 | The multi-agent decoder-coupling equation |
| DGT.1.3a | Decoder topological complexity |
| DGT.1.3c | Exponential growth in the transition energy threshold |
| DGT.1.3e | The exact quantified ceiling on D‑lock‑in |
| DGT.1.4a | The decoder–environment matching function |
| DGT.1.4c | Environmental drift and decoder lag |
| DGT.7 | The Zero-Sum Thermodynamic Negative-Sum Theorem |

A companion theorem (unnumbered, filed alongside DGT.3): the **$T_{\mathrm{pred}}$–Cooperation Theorem** — whether a cooperative equilibrium can hold up over the long run comes down to whether the time horizon clears a critical value, $T_{\mathrm{crit}}$.

**A note on the numbering gap**: the body of the original monograph's Volume IV also cites numbers DGT.9 through DGT.12 (DGT.12, for instance, is cited at "the cross-generational accumulation condition") — but they were never entered into Volume IV's mathematical appendix, the theorem summary table. That gap belongs to the original monograph itself; this reading guide hasn't lost anything. This table will be updated to match once a future version of the monograph fills the gap in.

---

## Fourteen. The V1.0 → V1.1 Core-Revision Comparison Table

A complete round-up of everything this guide updates, relative to both the original monograph and the previous edition of the Guide (use this table to convert citations back to the original monograph's wording):

| # | Update | Original Wording | This Guide's Normative Wording | Note |
| :-- | :--- | :--- | :--- | :--- |
| 1 | Naming the three routes | The "$\gamma$ route" | The "$E$ route" | $\gamma$ is kept exclusively for the energy elasticity index; the routes are now named to align with the three variable letters ($I/T/E$) |
| 2 | How the three routes stand relative to one another | The original text stressed that they're "mutually non-exclusive," without ever stating directly how they rank | Distilled into: the $I$ route is the statistically favored one; the $T$ and $E$ routes are fallback strategies for when the energy budget tightens | This conclusion was already implicit in the original monograph's argument about how fast $V_{\mathrm{obj}}$ accumulates in stock (e.g., the example of a thousand-year-old tree weathering a barrage of negative information) — this guide simply distills it into a more direct, canonical statement. A distillation of the wording, not a correction of the content |
| 3 | Naming $V^{\mathrm{val}}$ | "Value Objective Function" | "Value Viability" | The author's chosen name, applied uniformly across all platforms |
| 4 | Defining $I_{\mathrm{interp}}$ | "Dual to $I_{\mathrm{orig}}$" | The informational increment from high-quality execution or local parameter optimization within an existing paradigm, its marginal payoff decaying with homogenization ($\Delta I \to 0$) | The "dual" phrasing is retired |
| 5 | The meta-statement | Volume Z once glossed the meta-statement with a line about "converting dissipated energy" | Unified to: viability maximization is the long-run macro objective function of every negentropic structure capable of sustained persistence; every concrete mechanism is simply this working itself out locally | Volume I's wording and the author's own statement govern |
| 6 | $T_{\mathrm{env}}$ | One symbol, two meanings: the environment's characteristic time scale (in the section constraining $T_{\mathrm{pred}}$) versus ambient temperature (in the Landauer section) | Fixed: $T_{\mathrm{env}}$ now names the environment's characteristic time scale (in s) wherever $T_{\mathrm{pred}}$ is constrained; $T_{\mathrm{thermo}}$ now names ambient temperature (in K) wherever the Landauer limit appears — the two symbols are kept distinct, each carrying its own dimension | Restores the distinction V1.0 originally had, removing the symbol-overload conflict |
| 7 | $\beta$ in DGT.3 | The game's discount factor | Overloaded with the time-elasticity index $\beta$ — cite with the context spelled out | A symbol overload, left unresolved for now |
| 8 | $\gamma$ in DGT.7a | A derived measure of competitive intensity | Overloaded with the energy-elasticity index $\gamma$ — cite with the context spelled out | A symbol overload, left unresolved for now |
| 9 | The decoupling-deviation ODE | Two equations sat side by side | Now split by domain: the convergence domain, $\chi<\lambda$ (Volume I, with a closed-form solution), versus the self-referential amplification domain, $\chi>\lambda$ (DGT.5) — these are not two ways of writing the same equation | Cite with the domain specified |
| 10 | The formula's two levels | $V\approx I\cdot T/E$ sat alongside the elastic form with no stated relationship | Now explicitly layered: $V\approx I\cdot T/E$ is the special case $\alpha=\beta=\gamma=1$ of the reference baseline; $V\propto I^{\alpha}\cdot T^{\beta}/E^{\gamma}$ is the general elastic form, used for quantitative analysis within a single system | See "The Two Levels of the Formula" in Section 1 |
| 11 | The Information–Time–Energy Screening Law (FP‑11) | First proposed in the early v3.2 paper | Recast as a conjecture: $I$, $T$, $E$ cannot substitute for or contain one another, and the framework has found no evidence yet for a fourth resource of equal standing | It hasn't been proven that no fourth resource exists — this remains an open claim |
| 12 | The broad/narrow confusion in $I_{\mathrm{net}}$ | $I_{\mathrm{net}}$ did double duty — the coarse-grained estimate in the baseline formula, and the cognitive-channel-specific term in the expanded formula — under the same name | Split apart: the coarse-grained baseline quantity keeps the name $I_{\mathrm{net}}$; the cognitive-channel decomposition term is renamed $I_{\mathrm{causal}}$ ($V_{\mathrm{c}} = I_{\mathrm{causal}}\cdot T_{\mathrm{pred}}/E_{\mathrm{causal}}$); the relation between them is $I_{\mathrm{net}} = w_{\mathrm{s}}\cdot I_{\mathrm{struct}} + w_{\mathrm{c}}\cdot I_{\mathrm{causal}}$, with explicit weighting only needed for mixed systems — a purely structural or purely cognitive system degenerates to a single variable | A new variable added; no existing formula's numerical output changes — this only removes an ambiguity of shared naming |
| 13 | Where the elasticity ordering stands (FP‑6/Proposition 1) | The previous edition of the Guide called it "a qualitative conjecture, with no rigorous derivation or empirical confirmation yet" | Demoted a further notch, to "a hypothesis awaiting verification": the three independent empirical supports it once rested on — biological allometric scaling, AI scaling laws, urban scaling laws — have all, on re-examination, been confirmed not to hold, so the ordering claim drops from "qualitative conjecture" to "hypothesis awaiting verification"; the concept of the elasticity indices themselves ($\alpha,\beta,\gamma$) is unaffected | Adjusted following the latest review findings — the central update of this revision |
| 14 | Positioning fivefold recursion | Monograph 1.0 §5.0 already, explicitly, flagged it as "a conceptual-framework placeholder" and "a heuristic discretized model awaiting rigor," marking equations (5.1†)–(5.7†) throughout with a † to note their epistemic status — but the previous edition of the Guide never carried this key positioning forward | Inherited and restated: Monograph 1.0's own open acknowledgment — the current version is a linearized conceptual scaffold; a fully bidirectionally-coupled ODE/PDE system remains an openly acknowledged open problem | Corrects a misreading in the earlier v1.1 draft's item 14, which had claimed "the original monograph never stressed this." Monograph 1.0 already stated it fully; this guide only inherits and restates it — this is not a "demotion" |
| 15 | Classifying persistent structures by carrier | The original monograph spoke of "four carrier classes" without distinguishing, at the framework level, the cognitive tiers inside the actively-dissipative class | Broken down internally: actively dissipative structures now split, by cognitive-decoder tier, into the embodied phase ($V_c\to0^{+}$ — plants/fungi/bacteria) and the symbolic phase ($V_c\gg0$ — humans/AI); both are living things, differing only in how their cognitive decoder is realized; the online phase is folded into the third cognitive tier as its lower transitional edge | The overall four-class framework is unchanged; this only clarifies its internal structure |
| 16 | The tiered structure of $D_{\mathrm{cog}}$ | Both the original monograph and the previous Guide treated $D_{\mathrm{cog}}$ as a single category, "present only in the active phase," without distinguishing how lower-order life and higher-order cognition realize it differently | Arranged as a spectrum: $D_{\mathrm{cog}}$ is now explicitly a continuous spectrum — embodied (plants/fungi/bacteria) → online (some animals) → symbolic (humans/AI) — lining up exactly with the continuous spectra of $V_c$ and $T_{\mathrm{pred}}$; the online tier is treated as the lower transitional edge of the symbolic phase, not as a tier of its own | Closes off the "does a plant count as cognitive" misreading; adds Misreading 11 |
| 17 | The scope of FP‑8's myopic runaway | Neither the original monograph nor the previous Guide had stated where, on the cognitive tiers, this mechanism stops applying | A new boundary statement added: the threefold split and myopic runaway can only be triggered in systems with a symbolic $D_{\mathrm{cog}}$ ($V_c\gg0$); systems with an embodied $D_{\mathrm{cog}}$ cannot enter this regime, since $\chi\ll\chi_{\mathrm{crit}}$ for them | Proposition 3 and Misreading 6 updated to match |
| 18 | The count of falsifiable predictions | The previous Guide selected six | Prediction 7 added: the energy constraints on route selection are predictable in advance | A seventh prediction added; the original six are untouched |
| 19 | The count of misreadings | The previous Guide had ten | Misreading 11 added: "SRVD lumps plants and thermostats together as the same kind of physical response" | Added to go along with arranging the decoder as a spectrum |
| 20 | The typology of bits and the measurement protocol | Not in the previous Guide at all | Sections Sixteen and Seventeen added (in short form): the five-tier hierarchy of bit types ($I_{\mathrm{net}}$ being the only L3-level quantity SRVD actually uses), and the six points of the measurement protocol for $I$ | The full argument (including the boundary exclusions against $\Phi$/FEP/Fisher information, and worked examples) is left for the formal upgraded edition |

**A note on CS registration**: should any entry in this guide need to be entered into the canonical-statement registry, it can be numbered within the ranges Volume Z has reserved for it (CS‑C3–C9, CS‑T3–T9, CS‑D2–D9, CS‑B2–B9, CS‑H2–H9); the author has final say.

---

## Fifteen. The Monograph Series V1.0, and How to Cite It

### The Five-Volume Structure

- **Volume I, *Theoretical Core***: viability dynamics — how something persists, how it collapses.
- **Volume II, *The Evolution of Persistent Structures***: climbing dynamics — how something grows more complex.
- **Volume III, *Compressed Intelligence and Cognitive Evolution***: offline compilation, the human causal increment, the emergence of a self.
- **Volume IV, *Decoder Game Theory and Alignment Engineering***.
- **Volume Z, *A Dictionary of Reality-Mapping***: a handbook cross-referencing mathematics against narrative, including the CS series of canonical statements.

*Structure Recursive Viability Dynamics (SRVD), Monograph V1.0, Reading Guide V1.1: in a universe where entropy only rises, every ordered structure gets kept on the same ledger.*

---

## Sixteen. The Typology of Bits: Which Kind of Bit Does SRVD Actually Use?

Different fields default to entirely different pictures of "a bit": a physicist thinks of the Landauer bit ($k_BT\ln2$); a computer scientist thinks of the Shannon bit ($-\log_2 p$); a complexity researcher thinks of minimum description length. SRVD's core dynamical equation uses the **effective causal bit** — one with a clear physical carrier — and keeps a firm, non-interchangeable boundary around every other kind.

### 16.1 The Five-Tier Spectrum of Bits

| Tier | Bit Type | Physical Carrier | Decoder-Dependent | A Physical Quantity? | Role in SRVD |
| :--- | :--- | :--- | :--- | :--- | :--- |
| L0 | Shannon bit ($-\log_2 p$) | No | No | **No (pure mathematics)** | Raw material — not a tool of the framework |
| L1 | Landauer bit ($k_BT\ln2$) | Yes (a two-state system) | No | **Yes (a physical quantity — a thermodynamic cost)** | The hard floor on $E_{\mathrm{causal}}$; doesn't itself enter the core equation |
| L1 | Entropy bit ($\log_2 \Omega$) | Yes (a count of microstates) | No | **Yes (a physical quantity — configurational entropy)** | A statistical-mechanical proxy for $I_{\mathrm{struct}}$ in the passive-phase limit; not extrapolated to the active phase |
| L2 | Algorithmic bit (Kolmogorov/assembly) | Depends on implementation | Partially | **Conditionally (depends on implementation)** | An empirical proxy for $D_{\mathrm{depth}}$; doesn't itself enter the core equation |
| L3 | **The SRVD effective causal bit** ($I_{\mathrm{net}}$) | **Yes (carrier-dependent)** | **Yes (this is the core)** | **Yes (a macroscopic effective order parameter)** | **The only bit the framework's core dynamical equation actually uses** |

### 16.2 Core Positioning: $I_{\mathrm{net}}$ Is a Macroscopic Physical Order Parameter, Not a Score

$I_{\mathrm{net}} \equiv \eta_D \cdot I_{\mathrm{latent}}$ is the only information variable used in SRVD's core dynamical equation, $V = I \cdot T / E$. Its position within the framework is this:

> **A macroscopic effective order parameter.**

An order parameter is not a score. Landau's magnetization $M$ emerges from the statistical behavior of $10^{23}$ microscopic spins, and yet it's a physical quantity; Prigogine's entropy-production rate comes from coarse-graining microscopic irreversible processes, and yet it too is a physical quantity. $I_{\mathrm{net}}$ occupies exactly the same ontological standing within SRVD:

- It has a clear physical carrier (a neuron firing, a transistor switching, a molecule changing configuration);
- It has an operational measurement protocol (see Section 17);
- Its changes produce observable physical, causal effects (a shift in the pattern of energy consumption, a deflection of the system's trajectory);
- Its two constituent components, $I_{\mathrm{struct}}$ and $I_{\mathrm{causal}}$, each obey their own underlying thermodynamic constraints.

**$I_{\mathrm{net}}$ is not a simple combination of, or special case within, L0–L2 — it's a coarse-grained, weighted projection of those underlying physical quantities.** There's no automatic reduction running downward between the tiers — and not because $I_{\mathrm{net}}$ is somehow "not physical enough," but because physics itself has never demanded that an order parameter reduce directly to a microscopic Hamiltonian.

### 16.3 All Three of SRVD's Information Variables Are Physical Quantities

The three information variables SRVD uses — $I_{\mathrm{struct}}$, $I_{\mathrm{causal}}$, $I_{\mathrm{net}}$ — all carry the status of a physical quantity, but each is a different type of physical quantity:

| Variable | Type of Physical Quantity | Unit | Source of Physical Legitimacy |
| :--- | :--- | :--- | :--- |
| **$I_{\mathrm{struct}}$** | A semi-measure of configurational entropy | bit | Grounded in the count of configurations distinguishable from the background, $\log_2 \Omega$ — backed by statistical mechanics |
| **$I_{\mathrm{causal}}$** | A causal quantity of information, thermodynamically constrained | bit | Strictly obeys the Landauer limit, $E_{\mathrm{causal}} \ge k_B T_{\mathrm{thermo}} \ln 2 \cdot I_{\mathrm{causal}}$ (with $T_{\mathrm{thermo}}$ ambient temperature) — the informational equivalent of physical work |
| **$I_{\mathrm{net}}$** | A macroscopic effective order parameter | bit (a coarse-grained weighted value) | Built from a weighted mix of $I_{\mathrm{struct}}$ and $I_{\mathrm{causal}}$; its physical legitimacy is jointly established by the underlying thermodynamic constraints on both components, and it produces measurable, macroscopic causal effects in $V = I_{\mathrm{net}} \cdot T / E$ |

All three are physical quantities — they simply sit at different levels of description. $I_{\mathrm{net}}$ doesn't "replace" $I_{\mathrm{struct}}$ or $I_{\mathrm{causal}}$; it's a coarse-grained synthesis of them. It's much like temperature: a coarse-grained statistic over the kinetic energy of vast numbers of molecules, and yet temperature remains a physical quantity — coarse-graining doesn't demote it to "a score."

### 16.4 Clarifying Where Dimensional Conversion Applies

In the cognitive channel, $V_{\mathrm{c}} = I_{\mathrm{causal}} \cdot T_{\mathrm{pred}} / E_{\mathrm{causal}}$, the framework has $I_{\mathrm{causal}}$ and $E_{\mathrm{causal}}$ strictly obeying the Landauer floor ($E_{\mathrm{causal}} \ge k_B T_{\mathrm{thermo}} \ln 2 \cdot I_{\mathrm{causal}}$), so the $V_c$ channel keeps a full dimensional-reduction path — s·K/J, or on the order of s/J. Any derivation in the active phase (the $V_c$ channel) that mixes $I_{\mathrm{causal}}$ directly with Landauer-type quantities (such as $T_{\mathrm{thermo}}$ or an entropy-production rate), or compares their magnitudes, is entirely legitimate — it never triggers a cross-tier violation.

**Where the prohibition on conversion applies**: the one thing the framework forbids is plugging the coarse-grained, weighted-mixture quantity $I_{\mathrm{net}}$ (that is, $w_s \cdot I_{\mathrm{struct}} + w_c \cdot I_{\mathrm{causal}}$) directly into the Landauer conversion formula, $1\,\text{bit} \leftrightarrow k_B\ln2\,\text{J/K}$, for a dimensional reduction. Here's why:

1. The two components of $I_{\mathrm{net}}$ — $I_{\mathrm{struct}}$ and $I_{\mathrm{causal}}$ — have different physical carriers (a barrier-locked configuration versus dynamic cognitive computation), and their effective temperatures and energy scales may well differ;
2. After being coarse-grained and weighted together, $I_{\mathrm{net}}$ no longer sits on a single, pure physical-entropy basis, so the Landauer formula can't apply to it directly — that formula only holds for a two-state system at a single temperature, with a single physical carrier;
3. Refusing to plug a coarse-grained order parameter straight into a microscopic conversion formula is standard statistical-mechanics practice — free energy, for instance, is never reduced directly from a single term of the partition function.

This prohibition applies only to that specific misuse of the mixed quantity — it doesn't touch the pure $I_{\mathrm{causal}}$ inside the $V_c$ channel. The framework's dimensional system is self-consistent; nothing here breaks down.

### 16.5 Where the Qubit Belongs

Information content in a quantum-decoherence scenario is still handled at the L3 tier ($I_{\mathrm{net}}$) — it's simply that the values $\eta_D$ or $I_{\mathrm{latent}}$ can take are constrained by the decoherence process. The qubit doesn't constitute some sixth, independent bit type of its own: within SRVD's macro/meso domain of validity, decoherence enters only as an external lower-bound input, and it doesn't change the physical-quantity status of the information variables (see Supplementary Entry 7, "Cross-Reference at Quantum Scale," for the full account).

---

## Seventeen. The Measurement Protocol for $I$: How a Decoder Reads Out $I_{\mathrm{struct}}$ and $I_{\mathrm{net}}$

1. **The default perspective**: unless stated otherwise, "the viability potential of a structure" means the objective value, accounted against a physical decoder. For a passive-phase structure this is something an instrument can measure directly (mass spectrometry, diffraction, microscopy); for an active-phase structure, $I_{\mathrm{causal}}$, $T_{\mathrm{pred}}$, and $E_{\mathrm{causal}}$ are equally physical facts — how much energy a piece of cognitive behavior actually redistributes in the physical world — only usually harder to get at, so proxy indicators are needed to estimate them. That measurement is difficult is an operational limitation; it doesn't change the theoretical premise that $V_{\mathrm{obj}}$ is itself an objective quantity.
2. **Two kinds of statement, never to be conflated**: a structure's "own" viability potential (accounted against a physical decoder) and a structure's "viability potential for some external decoder-holder" (the same piece of food contributes a different $I_{\mathrm{net}}$ to an agent that can decode it than to one that can't at all) are two different statements about two different decoders — they're incommensurable across decoders, and should never be summed together as if they were the same thing.
3. **The Minimal Sufficient Identification Principle**: a physical decoder doesn't need to exhaust every measurable dimension — it only needs to read the minimum information required to pick the structure out, to identify it against its background. The numerator, $I_{\mathrm{struct}}$, and the denominator, $E_{\mathrm{structure}}$, must be taken at the same granularity — one can't be coarse while the other is fine.
4. **Polarity must always specify "for whom"**: the same physical signal can carry completely different polarities for different decoders — there's no neutral polarity that exists independent of who holds it. A distinction has to be drawn between "undecoded" (a signal that never even enters the decoder-holder's range of decoding, recorded as $I^0$) and "decoded but polarity-neutral" (a signal that has been read, but judged neither good nor bad — also recorded as $I^0$). Coarse-grained models usually don't bother distinguishing the two; that's a modeling simplification, not a requirement of the theory.
5. **Self-measurement error in a cognitive decoder differs by tier**: an embodied $D_{\mathrm{cog}}$ (class 3a) generates its $V^{\mathrm{virt}}$ through biochemical integration, tightly coupled to $V_{\mathrm{obj}}$ ($\chi \ll \chi_{\mathrm{crit}}$), almost entirely anchored to real environmental signal — it doesn't actively produce a systematic bias, and its measurement error comes from the same source as in the passive phase (only the external observer's instrument precision). A symbolic $D_{\mathrm{cog}}$ (class 3b), by contrast, can have $\chi$ cross the critical value, and only then can it mistake $V^{\mathrm{virt}}$ for $V_{\mathrm{obj}}$ — this is precisely Proposition 3's myopic-runaway mechanism showing up at the level of measurement, and it's the reason the claim "the active phase often gets the sums wrong" really points at the symbolic system itself, and not at any external observer.
6. **Theoretical exact values versus operational estimates**: given a specified decoder, $I_{\mathrm{struct}}$ and $I_{\mathrm{net}}$ have, in principle, determinate values, unaffected by the scale or resolution of observation. But complex systems are constrained by measurement technology and computing power, so what actually gets used — in equations, in coding case studies, in falsifiable predictions — is always an operational estimate under current technical conditions. Falsifiable predictions should follow ordinary scientific practice and state their conclusions at a scale where the effect is clear and not swamped by noise, without needing to declare a margin of error on every single line. Whether $V_{\mathrm{obj}}$ goes to zero (which it does when $I_{\mathrm{latent}}=0$) is a determination independent of which decoder is chosen, because whether $I_{\mathrm{latent}}$ exists at all is a physical fact.

---

## Appendix: Version History

### The Path of Evolution

Manuscript_v3.2 → Manuscript_v6.0 → Manuscript_v6.1 → Manuscript_v7.2 → Manuscript_v7.5 → Manuscript_v7.6 → Monograph_v1.0 → SRVD_v1.1

| Version | Zenodo DOI | Version Notes |
| :--- | :--- | :--- |
| **SRVD_v1.1** | Not yet obtained (this document) | SRVD V1.1 is published in the form of a "Reading Guide and Errata," correcting the empirical errors in the V1.0 monograph (demoting the elasticity ordering to a hypothesis awaiting verification) and adding the cognitive decoder's arrangement as a spectrum, the $I_{\mathrm{net}}/I_{\mathrm{causal}}$ split, the typology of bits, and the measurement protocol for $I$. Wherever V1.1 and V1.0 conflict, V1.1 governs. |
| **Monograph_v1.0** | 10.5281/zenodo.21322552 | SRVD Monograph V1.0 is a cross-scale macro-dynamical framework taking the persistent structure as its unified object of study; using $V = I \cdot T / E$ as its core measure, and working through fivefold recursion, the threefold split, and falsifiable predictions, it systematically describes how every ordered structure persists, evolves, and collapses under an energy constraint. |
| **Manuscript_v7.6** | 10.5281/zenodo.20478506 | Building on v7.5's macro-dynamical skeleton, v7.6 completed a full mathematical formalization — drawing a dimensional distinction between the objective stock and the viability-drive rate ($V$ as state, $r_v$ as rate), establishing a system of phase-space constraint inequalities, and giving a rigorous classification of the four global attractors — lifting SRVD from a qualitative theoretical framework into a computable dynamical system with a rigorous falsification protocol. |
| **Manuscript_v7.5** | 10.5281/zenodo.20386695 | v7.5 formally named the framework "Structure Recursive Viability Dynamics," established SRVD as independent of and incommensurable with steady-state theories like FEP, fixed the threefold split and the collapse of the endogenous time horizon ($T_{\mathrm{pred}}\to 0$) as the core mechanism behind paranoid recursion and reward hacking, gave a falsification protocol for reinforcement learning, and brought decoder decoupling and boundary collapse into the dynamics under study. |
| **Manuscript_v7.2** | 10.5281/zenodo.20130776 | v7.2 upgraded SRVD from a static formula into a full dynamical framework — through fourfold recursion ($I/V/E/T$) and a closed $I$–$V$ coupling loop, it gave an operational definition for the emergence of consciousness, and introduced a generalized elasticity formula together with an integral boundary condition on build cost, $E_{\mathrm{build}}$ — the leap from "a measure of viability" to "self-referential value dynamics." |
| **Manuscript_v6.1** | 10.5281/zenodo.20013497 | v6.1 repositioned build cost, $E_{\mathrm{build}}$, as "prepaid negentropy," folding it into the analytical framework by constructing a structural leverage ratio $L = V / E_{\mathrm{build}}$, and pointed out that a high-$E_{\mathrm{build}}$ structure can fall into thermodynamic zombification through "structural information debt" — continuing to burn the system's free energy even after it has lost all causal effect, leaving a civilization stagnant and dead on its feet. |
| **Manuscript_v6.0** | 10.5281/zenodo.19976517 | v6.0 expanded $E$ from "the energy cost of physical maintenance" to "maintenance plus decoding" combined, corrected the earlier claim that "$I$ can't be quantified" (pointing out that $I$ is already implicitly quantified in the parameters of large models), introduced a three-ruler cross-calibration programme to operationalize the measurement of $V$, and, through an inverted-U simulation over $K$ and $T$, revealed the niche-degeneration mechanism whereby "high energy efficiency drives homogenization, and homogenization kills off persistence time" — marking SRVD's decisive leap from a physics framework into the domains of culture and AI. |
| **Manuscript_v3.2** | 10.5281/zenodo.19717235 | Proposed the formula $V = I \times T / E$, the energy–information–time screening law, and the thermodynamic-elimination hypothesis. |

> *Structure Recursive Viability Dynamics (SRVD) V1.1: In a universe where entropy only rises, every ordered structure gets kept on the same ledger.*
