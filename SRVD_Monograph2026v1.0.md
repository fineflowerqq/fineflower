# *Structure Recursive Viability Dynamics*

**Author**: Ruifeng Liang (Independent Researcher)    **Version**: v1.0 (containing the core paper: Volume Ⅰ — SRVD v7.8)  
**Date**: 2026.06    **Contact**: fineflowerrain@gmail.com  

> **Edition Note**: This is the v1.0 inaugural release. Given the broad scope of the framework, errors and unresolved tensions are inevitable. Readers are kindly encouraged to offer corrections; all verified feedback will be incorporated in subsequent revisions.

---

## General Preface

This monograph consists of five volumes, each fully independent and readable on its own, though they may also be read in sequence. The division of labor among the volumes is as follows:

**Volume Ⅰ — Theoretical Core**: establishes the constitution of variables, the core dynamics, and the falsifiable predictions. This volume is the notational headwater of the entire work; every subsequent volume is independently readable, but all of them share the core symbolic system established here. A complete overview of the technical framework appears in this volume's abstract.

**Volume Ⅱ — Applications I: The Evolution of Persistent Structures**: answers the question of *how persistent structures climb* — the thermodynamic mechanism of directionality that carries complexity from crystals to civilizations.

**Volume Ⅲ — Applications II: Compressed Intelligence and Cognitive Evolution**: analyzes how advanced persistent structures resist the constraint of thermodynamic dissipation through offline compiled computation, and argues for the physical basis of expert intuition, of art and science, and of the evolutionary bottlenecks of AI.

**Volume Ⅳ — Applications III: Decoder Game Theory and Alignment Engineering**: elevates the decoder to an independent dynamical variable and builds a mathematical formalization of cross-agent games, applied to AI alignment and civilizational governance.

**Volume Z — A Dictionary of Real-World Mappings**: a narrative cross-reference between SRVD's mathematical forms and real-world phenomena; it does not bear on the main line of argument, and no volume's body text depends on it.

**Suggested reading order**: on a first pass, read Volumes Ⅰ→Ⅱ→Ⅲ→Ⅳ in sequence. Readers interested in a particular application may enter directly through any applications volume, consulting the variable-declaration table in that volume's Chapter 0 and Appendix A of Volume Ⅰ whenever an unfamiliar symbol is encountered.

> **Series-wide convention**: the core variables ($V, I, E, T, D, \alpha, \beta, \gamma, \chi, \Delta_{\mathrm{VV}}$, etc.) are fully defined in Volume Ⅰ; each applications volume independently declares its inheritance relations. Variables newly introduced within a given volume are declared only in that volume's Chapter 0 and are not carried across volumes.

---

# Volume Ⅰ — Theoretical Core: Structure Recursive Viability Dynamics (SRVD v7.8)

**Ruifeng Liang** (Independent Researcher) | 2026

---

**Introduction**

Because this work's architecture is intricate and its variables numerous, before entering into rigorous argument we first offer a short story to give the reader an intuitive feel for the core concepts.

A desert island. A man, a python, a wild boar.

The boar meets the man first. It has never seen this species before: too large to be prey, too slow to be a threat. In the boar's decoder, the man registers as nothing more than a patch of irrelevant noise — $I^0$. It ignores him and returns unhurried to its foraging.

The man spots the boar at the same moment. He assesses quickly: it cannot easily be caught, so no positive-value information $I^+$ is on offer; its tusks are sharp, so the risk of negative-value information $I^-$ is real. He chooses the safest course — he climbs a tree.

Deep in the canopy, a python has already been coiled in wait. Looking down, it takes in both the man and the boar at once: the boar is a mass of high-value protein, prime $I^+$, capable of sustaining the snake's own bodily structure; the man is an unfamiliar species, and whether he represents positive or negative value is unclear. Not being desperately hungry, the python does not, for now, place the man at the top of its menu.

The boar is the first to catch the snake's scent. Fear seizes it instantly: its **$T_{\mathrm{pred}}$**, its endogenous time horizon, contracts sharply, collapsing to the single instant of survival or death. It bolts for a kilometer; once the sense of danger dissipates, it lowers its head and resumes rooting in the dirt. For the boar, once a threat leaves the range of perception, it is as though it had never existed.

The man slips down and flees. But once he has escaped with his life, his **$T_{\mathrm{pred}}$** does not settle at "safe for the present moment" — it keeps extending forward, into tomorrow, the day after, and further still. In the future he projects, the snake is still there, the mortal threat is still there; unless he removes it in advance, he will not rest easy.

For the boar, the future simply does not exist; for the man, the future has already begun to act upon the present.

So the man sets to work. A higher-order recursion of $I_{\mathrm{net}}$ (net effective causal information) is set in motion. "Trap," "spear," "vine rope" — objects that do not yet exist anywhere in the physical world — take shape in his accumulated knowledge and his rehearsal of the future, and are then fabricated into being. He also realizes that when the moment of close combat actually arrives, either fleeing or fighting will burn through enormous reserves of energy, and that once he crosses $E_{\mathrm{thresh}}$ (the threshold of irreversible damage), it will be over. So he trains his body in advance, recursively investing his idle-time $E_{\mathrm{eff}}$ — bodily energy — in exchange for a larger pool of usable energy in the future.

On the second day, the snake finds the boar. A predation with no suspense follows.

On the third day, the man finds the snake's nest and steals its eggs.

When the snake returns to its den, it finds the man finishing off the last of the eggs. In the snake's decoder, the man is instantly upgraded from an unfamiliar species to a strong $I^-$ — a direct threat to the continued existence of its own genetic PS. It attacks at once. What meets it, however, is a set of tactics and weapons that vastly exceed anything in its cognitive model. Wounded, the snake drags its severed tail away in retreat; the man, too, suffers a mortal wound in the struggle.

As he lies dying, his mind turns to the family he left behind, to ambitions unfulfilled, and to the snake whose $\mathbf{V_s}$ he had nearly driven to zero. He briefly replays the mistakes of the fight, then just as quickly returns to the present, continuing to optimize his decisions within whatever room for action remains. Bearing the agony, he carves his final testament into the rock: the words to his family that he never got to say, the disposition of what he leaves behind, and a plea to his kin to avenge him by killing the snake that will forever haunt his unfinished life.

Then, with no hope of self-rescue, the searing pain of his wound, hunger, and cold feed an unbroken stream of negative information into his system, driving his current causal-viability potential $V_c$ swiftly negative, where it continues to offset the static viability potential $V_s$ that has not yet reached zero. Once his remaining objective viability potential $V_{\mathrm{obj}}$ falls below the zero threshold and turns negative, and no option remains within his reachable state space capable of pushing it back into positive territory, he enters a state in which the combined benefit of continuing to sustain the flesh falls below that of ending it immediately. So he leaps from the cliff, cutting short his own $T_{\mathrm{static}}$, forcibly truncating the accumulating negative value of $V_{\mathrm{obj}}$.

Three months later, another man discovers the rock bearing the testament. The testament enters into legal process; that inscription — bearing his own signature and unmistakable hand — begins to exert causal force $\mathbf{I_{\mathrm{net}}}$ upon the physical world in his place, carrying out what he left undone: mending the rift with his family, bringing wealth to his kin's PS, and above all winning more future reachable space for his genetic PS. His kin hunt down and kill the snake on his behalf, and raise a memorial to him on the island. Every few years, his descendants come to pay their respects. His name, his likeness, his deeds, his final wishes, and as much of his personal record as can be preserved, endure. His individual PS has become a memetic PS, continuing to persist within the physical world, extending its own **$T_{\mathrm{pred}}$** as far as it can.

---

In this story, the boar, the python, the man, the spear, the testament, the money, the descendants — none of these is the true protagonist. **The true protagonist is this: under a given energetic constraint, the negentropic configuration that maintains its own ordered topological character — the persistent structure** (Persistent Structure, PS).

### What Is a Persistent Structure?

The universe obeys the law of increasing entropy; everything tends, in the end, toward disorder. And yet, within this irreversible current, islands of order continually surge upstream against it: crystals, stars, cells, neural networks, languages, institutions, civilizations — and a testament that carries meaning. These seemingly unrelated things share one common essence: each is a specific, ordered informational structure, sustained by a given energetic input, that can be distinguished from background noise. SRVD (Structure Recursive Viability Dynamics) holds that whenever any object in the universe displays a discernible ordered character, its persistence and its dissolution can be brought under a single, cross-scale analytical framework:

$$
V \approx \frac{I \cdot T}{E}
\tag{0.1}
$$

**Viability potential = information $\times$ time $\div$ energetic cost.**

Here $I$ (information processing and causal efficacy), $T$ (time horizon), and $E$ (thermodynamic cost) are all generalized variables, each of which can be further unfolded into concrete dynamical indicators within different systems. The viability potential $V$ is an integrated measure of the strength of a persistent structure's continuation — the core state variable that is continually optimized over the course of evolution.

From animals, individuals, corporations, and cultures, to artificial intelligence and every other class of informational system, their behavior — whether or not we are ever fully aware of it — obeys this dynamic at a deep level. We have, in fact, never fully clarified what we ourselves are, or how we will evolve. We believe we are pursuing happiness, wealth, power, meaning, love, glory, or revenge — but viewed through the unified lens of thermodynamics and information theory, all of these motives can be reinterpreted as different expressions of a single, universal underlying mechanism: **the maximization of viability potential**.

This work (all five volumes) takes **Structure Recursive Viability Dynamics (SRVD)** as its unifying framework, drawing objects previously scattered across physics, biology, history, economics, psychology, and artificial intelligence into a single cross-scale analytical domain.

**Volume Ⅰ** (this volume): establishes the constitution of variables, the core dynamics, and the falsifiable predictions — the notational headwater of the entire series. It answers: how is a persistent structure to be defined? Relative to whom does its causal efficacy hold (that is, relative to which decoder $D$)? Why is it only higher-order intelligent agents — humans — who generate the complex phenomenon of "love and hatred" (that is, the threefold splitting of $V$)? Why does intelligence carry the risk of a runaway collapse into short-sightedness? And how might we build early-warning systems against it?

**Volume Ⅱ**: examines how persistent structures evolve upward from simple to complex, from physical-entity topology toward the topology of virtual, networked space.

**Volume Ⅲ**: analyzes how advanced persistent structures resist the constraint of thermodynamic dissipation through "offline compilation" — that is, through cognition, art, science, and AI.

**Volume Ⅳ**: elevates the decoder to an independent dynamical variable, formalizing questions of game-play, manipulation, and alignment.

**Volume Z**: a dictionary of real-world mappings, offered to help readers cross-reference theoretical concepts against real-world scenarios; it does not bear on the main line of argument.

### Why Is Such a Framework Needed?

We stand at a moment of rapid co-evolution between silicon-based AI and carbon-based civilization, in which memes, algorithms, institutions, and organisms are ever more entangled with one another. The old disciplinary boundaries no longer suffice to describe such cross-scale hybrids. The central innovation of SRVD lies in the following:

#### **Proposing the viability potential $V$ as a unified state variable, and giving it the mathematical form $V \approx I \times T / E$.**

#### **And asserting that: "maximizing viability potential" is the ultimate driving engine behind the behavior of every ordered, negentropic structure — every other mechanism is a local strategy in its service.**

#### **This statement is, at the same time, offered as a falsifiable core proposition, open to empirical scrutiny.**

SRVD attempts to provide a cross-scale, macro-dynamical framework that, without violating any known physical law, brings minerals, life, machines, civilizations, and memes to the same table for conversation.

It does not attempt to "rebuild the foundations of existing science"; it offers, instead, another lens of considerable penetrating power — one that lets us see what these objects, ordinarily assigned to separate scientific disciplines, share in common, and where they differ in essence. Only once we have seen the single set of physical rules they share can we judge what possibilities lie ahead, and how much room we actually have to act.

Having read this desert-island story, you have already made intuitive contact with the core of the framework. We now proceed to formal argument. Beginning with the constitution of variables in Chapter 0, we build, step by step, a theoretical edifice spanning dozens of orders of magnitude in scale.

Welcome to *Structure Recursive Viability Dynamics*.

> **Volume positioning**: this volume is the source of SRVD's constitution of variables, its core dynamics, and its falsifiable predictions. It establishes a cross-scale language of macro-dynamics, taking the persistent structure as its unified object of study.

---

## Abstract

Structure Recursive Viability Dynamics (SRVD) is a cross-scale macro-dynamical framework that takes the **persistent structure** as its unified object of study, drawing minerals, stars, living organisms, artificial-intelligence systems, and civilizations into a single analytical domain. The framework's core measure is the **viability potential**:

$$
V \approx \frac{I_{\mathrm{net}} \cdot T}{E_{\mathrm{eff}}}
\tag{0.2}
$$

Here $I_{\mathrm{net}}$ is the net effective causal information ($\mathrm{bit}$), $T$ is the structure's persistence time ($\mathrm{s}$), and $E_{\mathrm{eff}}$ is the equivalent thermodynamic cost ($\mathrm{J}$); the candidate dimensional unit of $V$ is $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$.

SRVD's central contributions are threefold: (1) it endogenizes the **decoder** $D$ as a dynamical variable possessing its own independent energetic, temporal, and informational costs; (2) once the temporal parameter $T$ shifts from an exogenous coordinate to an endogenous state variable — the endogenous time horizon $T_{\mathrm{pred}}$ — the viability potential undergoes a **threefold split**, producing a structural decoupling among the objective viability potential $V_{\mathrm{obj}}$, the virtual viability potential $V^{\mathrm{virt}}$, and the value objective function $V^{\mathrm{val}}$; this decoupling is the ontological root of extreme regimes such as the Myopic Runaway Regime; (3) it proposes that the collapse of the endogenous time horizon necessarily precedes both the surge in thermodynamic dissipation and the collapse of the objective viability potential, offering this as an **early-warning inference**, together with an operational protocol for empirical verification through reinforcement learning.

The framework does not claim to transcend established physical law; every dynamical equation it proposes takes Landauer's principle, the second law of thermodynamics, and other well-established constraints as its lower bounds. The current version (v7.8), building on v7.6, corrects a definitional contradiction in $I_{\mathrm{net}}$, a missing domain of validity for $V_{\mathrm{obj}}$, several instances of dimensional ambiguity, and gaps in the argument for the ordering proposition, thereby establishing the conceptual framework and the core dynamical equations; cross-domain quantitative comparison of specific numerical values is left to subsequent empirical work.

SRVD's theoretical center of gravity lies in the **mechanism of structural recursion**, not in any static taxonomy of persistent structures. Any concrete instance of a persistent structure — a cell, a civilization, an AI model — is an instantaneous cross-section of this recursive process; decoder evolution ($D$-drift, $\mathcal{T}$-transitions), the accumulation of information ($I_{\mathrm{orig}}$ injection), and the optimization of viability potential ($\max V$) together constitute the dynamical core of that recursion.

---

## Chapter 0 — The Constitution of Variables and the Symbolic System

This volume is the source of SRVD's constitution of variables. The following core variables run throughout the entire series; each applications volume independently declares its inheritance relations and does not redefine them:

| Family | Representative symbols | Meaning | Unit |
| :--- | :--- | :--- | :--- |
| $I$-family | $I$<br>$I_{\mathrm{net}}$<br>$I_{\mathrm{struct}}$<br>$I_{\mathrm{latent}}$<br>$I_{\mathrm{orig}}$ | Generalized structural difference<br>Net effective causal information<br>Structural information<br>Latent configurational information<br>Paradigm-breaking information | $\mathrm{bit}$<br>$\mathrm{bit}$<br>$\mathrm{bit}$<br>$\mathrm{bit}$<br>$\mathrm{bit}$ |
| $E$-family | $E_{\mathrm{eff}}$<br>$E_{\mathrm{causal}}$<br>$E_{\mathrm{structure}}$<br>$E_{\mathrm{build}}$ | Equivalent thermodynamic cost<br>Causal-processing energy<br>Structural energy<br>Construction cost | $\mathrm{J}$<br>$\mathrm{J}$<br>$\mathrm{J}$<br>$\mathrm{J}$ |
| $T$-family | $T$<br>$T_{\mathrm{static}}$<br>$T_{\mathrm{pred}}$ | Generalized structural persistence time<br>Static lifespan<br>Endogenous time horizon | $\mathrm{s}$<br>$\mathrm{s}$<br>$\mathrm{s}$ |
| $V$-family | $V$<br>$V_{\mathrm{obj}}$<br>$V^{\mathrm{virt}}$<br>$V^{\mathrm{val}}$<br>$\Delta_{\mathrm{VV}}$ | Viability potential (low-order approximation)<br>Objective viability potential<br>Virtual viability potential<br>Value objective function<br>Decoupling deviation | $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$<br>$\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$<br>$\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$<br>$\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$<br>$\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$ |
| $D$-family | $D$<br>$\eta_D$<br>$\mathcal{T}$<br>$\mathcal{F}$<br>$D_{\mathrm{depth}}$ | Decoder<br>Decoding efficiency<br>Topological-expansion operator<br>Recursive-unfolding operator<br>Constraint depth | —<br>dimensionless<br>—<br>—<br>dimensionless |
| Elasticity exponents | $\alpha$<br>$\beta$<br>$\gamma$ | Informational elasticity exponent<br>Temporal elasticity exponent<br>Energetic elasticity exponent | dimensionless<br>dimensionless<br>dimensionless |
| Other | $\chi$<br>$\gamma_0$<br>$\rho$<br>$L$ | Coupling strength<br>Baseline depreciation rate<br>Competitive-pressure index<br>Wisdom-leverage coefficient | $\mathrm{J}/(\mathrm{bit}\cdot\mathrm{s})$<br>$\mathrm{s}^{-1}$<br>dimensionless<br>$(\mathrm{bit}\cdot\mathrm{s}/\mathrm{J})/\mathrm{J}$ |

> **Series-wide convention**: the meanings of the symbols above are fixed throughout the SRVD framework; each applications volume independently declares its inheritance from this table.

---

## Chapter 1 — The Ontological Layer: Persistent Structures and Decoders

### 1.0 The Persistent Structure

**Definition: A persistent structure (Persistent Structure, abbreviated PS) is any negentropic topological configuration that, under an energetic constraint, maintains its topological character across a finite span of time.**
Its constitution requires three conditions:
(1) the existence of an ordered, negentropic organization distinguishable from background;
(2) the capacity of that organization to maintain continuity within a finite time window;
(3) the presence of sufficient energetic conditions to sustain it.

> **A clarification regarding "finite"**: "finite," here, means *not infinite* — every persistent structure is bound by the ultimate limits set by thermodynamics, by the boundaries of cosmic evolution, or by physical constants; it does not imply that the relevant timescale is small or fleeting. Granite, for instance, may persist on the order of a billion years and still falls within the category of "finite time." "Finite" and "persistent" are thus not in tension here.

**Universality**: quantum states, crystals, stars, genomes, neural networks, languages, institutions, and civilizations — however vastly they differ in scale, composition, complexity, and medium of realization — can, in a dynamical sense, all be treated as instances of the same class of object: ordered, distinguishable topological configurations that form and are maintained under an energetic constraint, resisting, within a bounded span of time, the homogenizing tendency pointed to by the second law of thermodynamics.

**An operational criterion**: whether a structure counts as "persistent" is not a matter of its absolute lifespan, but of whether, under given energetic conditions, it can keep its own topological character recognizable across the corresponding time window.

The persistent structure is the primary object of study in SRVD. The framework presupposes no ontological rupture between "the physical" and "the abstract"; on the contrary, every core variable that follows is defined *upon* the persistent structure, and structures are distinguished from one another only by their carrier, their maintenance cost, and their mode of causal execution.

#### 1.0.1 Stratification by Carrier

The core constraint form of a persistent structure remains unchanged, but the weighting of the $E_{\mathrm{eff}}$ components differs across types of PS. Based on the nature of the carrier and the mechanism of persistence, PS can be provisionally divided into four types:

| Type | Carrier | Dominant energy term | Role of $E_{\mathrm{causal}}$ | Core of persistence | Typical instances |
| --- | --- | --- | --- | --- | --- |
| Passive-physical PS | Has its own physical carrier | $E_{\mathrm{barrier}}$ | Almost no active causal invocation; expressed mainly as physical response | Structure not destroyed by external force | Rocks, crystals, minerals, planets |
| Active-dissipative PS | Has its own physical carrier | $E_{\mathrm{survival}}+E_{\mathrm{causal}}$ | Executes survival: perception, regulation, repair, decision, control | Continuous self-maintenance of its own organization | Cells, animals, data centers, ecosystems |
| Formal-mathematical PS | No physical carrier of its own; depends on a host for instantiation | $E_{\mathrm{causal}}$ | Precise execution: decoding, derivation, invocation | Being correctly executed or invoked | $\pi$, group theory, Euclidean geometry |
| Memetic-virtual PS | No physical carrier of its own; depends on multiple hosts for propagation | $E_{\mathrm{causal}}$ | Diffusion and spread: persuasion, education, ritual, transaction, maintenance of consensus | Being believed, replicated, or transmitted by a sufficient number of hosts | Belief in currency, religious doctrine, scientific theory as consensus |

In short:

> The passive-physical persists by not falling apart; the active-dissipative persists by self-maintenance; the formal-mathematical persists by never being misinvoked; the memetic-virtual persists by consensus that never dies.

The first two types each possess their own physical carrier, and are distinguished by whether they actively maintain themselves through internal regulation and continuous energy flow. The latter two types possess no independent, self-sufficient physical carrier at all, and must be instantiated or carried by a host system; they are distinguished by whether their persistence depends chiefly on precise invocation, or on distributed propagation and the maintenance of consensus.

All four types of PS obey the basic constraint given in the section on the decoder-centered descriptive principle:

$$
E_{\mathrm{maint}}(D) \geq E_{\mathrm{Landauer}}(I_{\mathrm{min}}(D)) + E_{\mathrm{structure}}
\tag{1.1}
$$

There is therefore no such thing, within SRVD, as a "purely abstract" structure with zero physical maintenance cost. The persistence of a so-called abstract structure is never an independent existence detached from the physical world; it is, rather, instantiated, preserved, invoked, or transmitted through some host system — a human brain, a book, a computer, a database, a social institution.

> **A note on $E_{\mathrm{causal}}$ in formal-mathematical PS**: the $E_{\mathrm{causal}}$ entry in the "formal-mathematical PS" row of the table above does not imply that the mathematical object itself possesses some active capacity to "compute." $\pi$, the structures of group theory, and Euclidean geometry do not decode, derive, or execute anything on their own. Here, $E_{\mathrm{causal}}$ refers specifically to the cognitive and computational energy consumed by a human being or a machine in the course of invoking, understanding, proving, calculating, storing, or deriving that mathematical structure.
>
> A human calculating several digits of $\pi$ by hand, for instance, requires neural metabolic energy; a computer executing a group-theoretic algorithm requires electricity; a book preserving geometric knowledge requires paper, printing, storage space, and the cost of environmental upkeep. The "persistence" of a formal-mathematical PS therefore does not arise from any active self-maintenance of its own, but from the capacity of a host system to preserve, decode, and re-instantiate it. This is entirely consistent with the discussion in the section on the decoder's status as a physical entity: any culturally, theoretically, linguistically, or mathematically encoded structure must, without exception, pay its maintenance cost through some physical system.

---

### 1.1 The Decoder

#### 1.1.1 Definition of the Decoder

The **decoder** (decoder, $D$) is the physical mechanism by which a persistent structure extracts effective causal information from its latent configuration in order to sustain itself. It is the interface between a structure and its environment (the physical channel), and it determines the manner in which energy flows in, is transformed, and is allocated.

Operationally, the essence of the decoding process is **physical-state coupling and informational mapping**: the decoder $D$, at a given efficiency $\eta_D \in [0,1]$, extracts net effective causal information $I_{\mathrm{net}} = \eta_D \cdot I_{\mathrm{latent}}$ from the structure's latent information $I_{\mathrm{latent}}$. Low-efficiency decoding ($\eta_D \to 0$) is the norm in passive structures; efficient, recursive decoding is a higher-order feature of the active phase.

The decoder is itself a persistent structure and is likewise subject to SRVD's viability dynamics — that is, $V(D) = I_{\mathrm{net}}(D) \cdot T(D) / E_{\mathrm{eff}}(D)$ — forming a self-consistent closed loop between observer and observed.

#### 1.1.2 The Physical Decoder ($D_{\mathrm{phys},i}$)

The physical decoder is a **passive interface**: it has no internal model, passively follows the rules of its channel, and generates no predictions. An atom absorbing photon energy via electromagnetic interaction, or a rock responding to temperature change through lattice vibration, are examples. This is the most fundamental form of decoding possessed by every persistent structure, corresponding to a decoding efficiency of $\eta_D \to 0$.

#### 1.1.3 The Cognitive Decoder ($D_{\mathrm{cog},i}$)

The cognitive decoder is an **active interface**: it possesses an internal predictive model, is capable of distinguishing informational polarity ($I^+, I^-, I^0$), and generates an endogenous time horizon $T_{\mathrm{pred}}$ and a virtual viability potential $V^{\mathrm{virt}}$. The nervous systems of living organisms, the reasoning modules of AI, and the institutional systems of civilizations all belong to this category.

The emergence of the cognitive decoder is not some miracle transcending physics, but a phase transition undergone by matter under thermodynamic pressure — a shift from the passive resistance of entropy increase toward the active prediction of the environment.

#### 1.1.4 The Criterion of Decoder Activity

A system's decoder is termed "actively viable" if and only if all three of the following minimal conditions are satisfied at once:

1. **Controllable internal state**: the system can alter its own behavior according to an internal model, rather than being driven purely by external forces;
2. **Adjustable energy flow**: the system can actively increase or decrease $E_{\mathrm{flow}}$ in response to environmental change;
3. **Predictable time horizon**: the system possesses $T_{\mathrm{pred}} > 0$ and can regulate its current behavior according to $T_{\mathrm{pred}}$.

By this classification: rocks and planets satisfy none of these conditions and are passively viable; stars fail condition (1) — despite possessing an immense energy flow, they remain passive (or quasi-active); living organisms and AI satisfy all three conditions and are actively viable.

> **A note on the classification of stars**: stars do exhibit genuine feedback processes internally (such as the negative feedback between core temperature and fusion rate), but this feedback does not depend on any **internal predictive model** — it is the direct consequence of local physical law (hydrostatic equilibrium, nuclear-reaction rate equations), not the active modeling and planning of future states. A star possesses no independently meaningful $T_{\mathrm{pred}}$ (its effective persistence horizon is simply the $T_{\mathrm{static}}$ determined by its fuel reserves, and cannot be actively extended or compressed by any internal state); it therefore fails criterion (3). This is the fundamental reason a star is classed as passively (or quasi-actively) viable rather than actively viable — a distinction that turns on this, and not on the surface feature of "whether energy-flow regulation exists."

#### 1.1.5 Summary of Decoder Symbols

| Symbol | Name | Definition | Domain of applicability |
|:---|:---|:---|:---|
| $D$ | Decoder | The physical mechanism by which a persistent structure extracts effective causal information from its latent configuration | All PS |
| $D_{\mathrm{phys},i}$ | Physical decoder | A passive interface with no internal model; $\eta_D \to 0$ | All PS |
| $D_{\mathrm{cog},i}$ | Cognitive decoder | An active interface with an internal predictive model, capable of distinguishing polarity | Active phase only |
| $\eta_D$ | Decoding efficiency | $\eta_D \in [0,1]$; $I_{\mathrm{net}} = \eta_D \cdot I_{\mathrm{latent}}$ | All PS |
| $\mathcal{T}$ | Topological-expansion operator | The operation that opens a new causal dimension at a paradigm transition (unfolded further in the section on extended dynamics) | Active phase only |
| $D_{\mathrm{depth}}$ | Constraint depth | $D_{\mathrm{depth}} = 1+\#\{\mathcal{T}\}$ — one plus the number of topological transitions ($\mathcal{T}$-operator applications) accumulated over a structure's history | All PS (constant at 1 in the passive phase) |

> **A note on terminological usage**: throughout this text, **SRVD** is used uniformly to denote the theoretical framework as a whole (it is not mixed with "this theory" or "this framework," which denote the same thing but are used only where SRVD is given priority for consistency); "decoder" or $D_{\mathrm{phys}}$ is used when discussing a passive-phase interface, and "cognitive decoder" or $D_{\mathrm{cog}}$ when discussing an active-phase interface; the unqualified term "decoder" $D$ may refer to either where the context makes this clear, but where activity specifically needs to be emphasized, $D_{\mathrm{cog}}$ should be used explicitly to avoid ambiguity.

---

### 1.2 The Physical Channel

**Definition**: the physical channel ($C_{\mathrm{phys}}$) is the environmental substrate in which a persistent structure and its decoder are situated, comprising the fundamental interactions and every lower-level rule that emerges from them. Within the framework of known physics, it provides the conduit for the flow of energy and the protocol for the exchange of information.

The operation of any decoder is subject to three nested constraint layers of the physical channel:

**Constraint of fundamental law**: within the framework of known physics, the electromagnetic, gravitational, strong, and weak forces provide the underlying constraints on energy transfer and signal transmission — the physical bedrock a decoder cannot exceed.

**Constraint of medium structure**: the mesoscopic media formed when fundamental interactions aggregate within particular regions of spacetime (air, water, vacuum, nerve fiber) impose bandwidth limits, delay, and attenuation on signals, determining the amount of effective signal a decoder can extract.

**Constraint of the thermodynamic lower bound**: the statistical, macroscopic expression of vast numbers of microscopic interactions — thermal fluctuation and dissipation — introduces channel noise and sets an irreversible minimum energetic cost for a decoder's extraction of effective information (the Landauer lower bound on $E_{\mathrm{causal}}$).

In the current version of SRVD, the physical channel is treated as a fixed background rather than a dynamical variable. It determines the height of $E_{\mathrm{barrier}}$, the efficiency ceiling of $E_{\mathrm{causal}}$, and the maximum possible value of $I_{\mathrm{net}}$.

**The semantics of shared constraint**: $C_{\mathrm{phys}}$ is not the product of any single decoder, but the constraint background to which every decoder is jointly subject in practice. The second law of thermodynamics, the causal limit imposed by the speed of light, and other physical laws possess a cross-cultural, cross-species objectivity precisely because any decoder that violates them incurs an irreversible practical penalty. This is the criterion that fundamentally distinguishes $C_{\mathrm{phys}}$ from cultural consensus.

---

## Chapter 2 — The Constitution of Variables

> This chapter defines every core variable of SRVD, giving for each its physical meaning, its unit, and its domain of applicability. The symbols used in every subsequent chapter are defined here in full and are not redefined thereafter. Every variable carries a notation distinguishing its passive-phase and active-phase forms where relevant.

### 2.0 The $I$-Family (the Information Family)

The $I$-family quantifies a persistent structure's distinguishable, ordered difference and its causal capacity. Its base unit is the $\mathrm{bit}$, defined as $\log_2 \Omega$, where $\Omega$ is the total number of states that can be stably distinguished under a given decoder $D$.

| Symbol | Unit | Definition | Domain of applicability |
|:---|:---|:---|:---|
| $I$ | $\mathrm{bit}$ | Generalized structural difference: the total amount of distinguishable, ordered difference a persistent structure exhibits relative to its background | All PS |
| $I_{\mathrm{struct}}$ | $\mathrm{bit}$ | Structural information: the intrinsic store of ordered information (lattice, DNA, chip wiring, and other forms of physical order) | All PS |
| $I_{\mathrm{latent}}$ | $\mathrm{bit}$ | Latent configurational information: currently unactivated but recoverable causal capacity (dormant knowledge, uninvoked model weights) | Active phase only |
| $I_{\mathrm{active}}$ | $\mathrm{bit}$ | Activated causal information: causal capacity currently in use (real-time inference, action, decision) | Active phase only |
| $I_{\mathrm{net}}$ | $\mathrm{bit}$ | Net effective causal information: **primary definition** $I_{\mathrm{net}} \equiv \eta_D \cdot I_{\mathrm{latent}}$, where $\eta_D \in [0,1]$ is the decoding efficiency; $I_{\mathrm{active}} \leq I_{\mathrm{net}}$ is the subset currently activated (see note below) | Active phase only |
| $I^+$ | $\mathrm{bit}$ | Positive-value information: input that expands the future reachable state space | Active phase only |
| $I^-$ | $\mathrm{bit}$ | Negative-value information: input that compresses the future reachable state space | Active phase only |
| $I^0$ | $\mathrm{bit}$ | Neutral noise: input that produces physical causal effect but carries no viability polarity | All PS |
| $I_{\mathrm{orig}}$ | $\mathrm{bit}$ | Paradigm-breaking information: information whose marginal causal efficacy decays very slowly, its value deriving chiefly from the generation of new structure | Active phase only |
| $I_{\mathrm{interp}}$ | $\mathrm{bit}$ | Paradigm-interpretive information: information that optimizes within an existing paradigm, whose marginal efficacy decays rapidly as it becomes homogenized | Active phase only |
| $\dot{I}_{\mathrm{min}}$ | $\mathrm{bit}/\mathrm{s}$ | Minimum information rate: the minimum information flow required to maintain structural identity | Active phase (threshold criterion) |
| $I_{\mathrm{max}}(D)$ | $\mathrm{bit}$ | The maximum information capacity extractable by decoder $D$ | All PS (dependent on $D$) |

> **A note on the definitional hierarchy of net effective causal information**: $I_{\mathrm{net}}$ has one, and only one, primary definition — $I_{\mathrm{net}} \equiv \eta_D \cdot I_{\mathrm{latent}}$ (the extraction-based view) — and this is the definition used wherever any quantitative formula in the framework refers to $I_{\mathrm{net}}$. $I_{\mathrm{active}}$ is the subset of $I_{\mathrm{net}}$ currently being invoked, so $I_{\mathrm{active}} \leq I_{\mathrm{net}}$; equation (3.12) below has been corrected accordingly (see the "compound definitions" section further on). $I_{\mathrm{net}} = I^+ - |I^-|$ (the net-effect view) is an **approximate equality** that holds only when $I^- = 0$ and $\eta_D = 1$; in general it is not equivalent to the primary definition, and is used only for qualitative discussion of the trade-off in informational polarity, never substituted into quantitative formulas.

**A note on the passive phase**: in the passive phase, $I_{\mathrm{net}} = I_{\mathrm{latent}} = I_{\mathrm{active}} = 0$, while $I_{\mathrm{struct}} > 0$; the polarity classes $I^+, I^-, I^0$ are defined in the passive phase but produce no causal effect there.

#### 2.0.1 The Ontological Status of $I$: Information as a Relational, Not an Absolute, Quantity

Within SRVD, $I$ is not some objectively existing absolute quantity, but the amount of effective difference a persistent structure can extract through its decoder $D$. The ontological implication of this definition is that the magnitude of $I_{\mathrm{net}}$ depends not only on the latent information $I_{\mathrm{latent}}$ present in the environment, but equally on the structural characteristics of the decoder $D$ itself.

The very same physical configuration presents entirely different informational value to different decoders: oxygen is $I^+$ for a human being but may be $I^-$ for an anaerobic bacterium; visible electromagnetic radiation is close to $I^0$ for someone born blind. Causal efficacy is not an isolated physical property, but a measure of the degree of match between a topological configuration and the structure of a decoder.

This relational essence carries a central corollary: **under our current cognitive and measurement frameworks**, the absolute numerical values of $I$ across different decoders cannot be directly compared. Questions of the form "how many bits does a rock have, how many bits does a person have" do not constitute meaningful same-domain questions within SRVD, unless a unified cross-decoder reference frame for informational complexity is established in the future (see the discussion in the section on the current state and limits of numerical precision, below). Any claim that one system "has more information" must, within SRVD, be accompanied by the condition "under which decoder" — otherwise the statement is incomplete. The boundary of $I$ expands as the decoder is upgraded, opening informational dimensions that were previously unreachable.

#### 2.0.2 On the Limits of Cross-Domain Quantification of $I$

Given this ontology, the practice — common in classical information theory — of using $I = \log_2 \Omega$ to construct a single, absolute one-dimensional ranking across every kind of structure (crystal, DNA, language, neural network) is, in principle, untenable, because the state spaces of different systems simply do not share the same coordinate frame. SRVD explicitly prohibits precise cross-domain numerical comparison of different types of system under our current state of knowledge. A detailed treatment of how the evolution of structural complexity might be characterized along multiple dimensions — including rule complexity and the depth of historical constraint — is deferred to the multidimensional quantification framework in Chapter 4.

#### 2.0.3 The Incommensurability Proposition: Comparing Viability Potential Across Decoders and Observational Scales

The two preceding sections — on the ontological status of $I$ and on the limits of its cross-domain quantification — have already established that there are principled limits on comparing the informational quantity $I$ across decoders. This limitation generalizes into two formal propositions concerning the viability potential $V$ itself, since the very definition of $V$ is built upon a specific causal measure space $\Omega_D$ and a specific observational scale $S$.

**Proposition (cross-decoder incommensurability)**: if the causal measure spaces $\Omega_{D_A}$ and $\Omega_{D_B}$ corresponding to two decoders $D_A$ and $D_B$ share no common mapping basis, then the comparison of $V(X \mid D_A)$ with $V(Y \mid D_B)$ is mathematically undefined.

**Proposition (cross-scale incommensurability)**: if two observational scales $S_A \neq S_B$ lead a system to adopt different coarse-graining cutoff frequencies, then $\Delta V = V(\cdot \mid S_A) - V(\cdot \mid S_B)$ is likewise undefined. A characteristic example of the latter proposition: a structure may display an extremely high local viability potential $V$ at a microscopic scale (such as a single cell), while its overall viability potential at a macroscopic scale (such as the host organism to which it belongs) tends toward zero — as with a malignantly proliferating cancer cell relative to its host. The two $V$ values, at their respective scales, do not constitute comparable quantities under a common dimensional footing; they cannot be subtracted or ranked against one another.

**Corollary (the prohibition on global ranking)**: to speak of a "globally optimal structure," an "absolute ranking of intelligence," or "which persistent structure has the highest viability potential" while detached from the two parameters $(D, S)$ is, in the sense of measure theory, an undefined operation — analogous to comparing the magnitudes of two velocities without reference to a frame. There is no global optimum within SRVD that is independent of a choice of $(D, S)$; any statement of "higher viability potential" must specify, at the same time, both its decoder and its observational scale.

This incommensurability proposition is not a weakening of the framework's predictive power, but a precise delineation of its domain of applicability: SRVD offers rigorous predictions of a system's direction of evolution given a fixed $(D, S)$ (see Chapters 5 through 8), but it does not promise a unified ranking across different $(D, S)$ — the latter lies, in principle, outside the framework's domain of definition.

---

### 2.1 The $E$-Family (the Energy Family)

The $E$-family quantifies the various energetic costs a persistent structure pays over the course of its persistence. Its base unit is the $\mathrm{J}$ (joule).

| Symbol | Unit | Definition | Domain of applicability | Relation |
|:---|:---|:---|:---|:---|
| $E$ | $\mathrm{J}$ | Generalized energy, the parent variable of the energy family | All PS | — |
| $E_{\mathrm{barrier}}$ | $\mathrm{J}$ | Barrier energy: a passive barrier, involving no continuous dissipation, "frozen" once and for all | All PS | — |
| $E_{\mathrm{survival}}$ | $\mathrm{J}$ | Survival energy: active dissipation that compensates entropy increase (metabolism, nuclear fusion), a continuous flow | All PS | — |
| $E_{\mathrm{causal}}$ | $\mathrm{J}$ | Causal-processing energy: the energetic cost of running a decoder; $> 0$ in the active phase, $\to 0$ in the passive phase | Active phase $>0$; passive phase $\to 0$ | $\geq k_B T_{\mathrm{thermo}} \ln 2 \cdot I_{\mathrm{net}}$ |
| $E_{\mathrm{structure}}$ | $\mathrm{J}$ | Structural energy: the minimum overhead required to keep a structure alive | All PS | $E_{\mathrm{barrier}} + E_{\mathrm{survival}}$ |
| $E_{\mathrm{flow}}$ | $\mathrm{J}$ | Flow energy: the budget devoted to active maintenance and causal processing | All PS | $E_{\mathrm{survival}} + E_{\mathrm{causal}}$ |
| $E_{\mathrm{maint}}$ | $\mathrm{J}$ | The total energy required to keep a decoder running | PS with a cognitive decoder | $E_{\mathrm{structure}} + E_{\mathrm{causal}}$ (bounded below by $E_{\mathrm{structure}} + E_{\mathrm{Landauer}}$) |
| $E_{\mathrm{eff}}$ | $\mathrm{J}$ | Equivalent thermodynamic cost: the complete physical cost a system pays to sustain its negentropic topological configuration | All PS | $E_{\mathrm{barrier}} + E_{\mathrm{survival}} + E_{\mathrm{causal}}$ |
| $E_{\mathrm{min}}$ | $\mathrm{J}$ | The minimum energetic requirement for sustaining a structure (jointly set by the Landauer limit and basic structural constraints) | All PS | — |
| $E_{\mathrm{max}}$ | $\mathrm{J}$ | The maximum total free energy available to a system (the ceiling of environmental supply) | All PS | — |
| $E_{\mathrm{thresh}}$ | $\mathrm{J}$ | Dissolution threshold: the energetic ceiling beyond which irreversible damage is triggered | All PS | — |
| $E_{\mathrm{build}}$ | $\mathrm{J}$ | Construction cost: the one-time physical energy required to create a new structure or upgrade an existing one | All PS | — |

**A threefold reading**: classical mechanics deals chiefly with $E_{\mathrm{barrier}}$ (potential energy); Prigogine's theory of dissipative structures deals chiefly with $E_{\mathrm{survival}}$ (active dissipation); SRVD's tripartite decomposition $E_{\mathrm{eff}} = E_{\mathrm{barrier}} + E_{\mathrm{survival}} + E_{\mathrm{causal}}$ brings all three under a single costing framework, making comparison possible across substrates ranging from a single quantum bit to an entire civilization.

**A note on the passive phase**: in the passive phase, $E_{\mathrm{causal}} = 0$, so $E_{\mathrm{eff}} = E_{\mathrm{structure}} = E_{\mathrm{barrier}} + E_{\mathrm{survival}}$, and $E_{\mathrm{flow}} = E_{\mathrm{survival}}$.

**A note on construction cost**: $E_{\mathrm{build}}$ is a one-time historical investment and does not enter the dynamical equation for the viability potential $V$. Its efficacy is assessed independently via the wisdom-leverage coefficient $L = \Delta V / E_{\mathrm{build}}$ (see the section on the wisdom-leverage coefficient).

**A note on the lower bound of $E_{\mathrm{maint}}$**: the lower bound of $E_{\mathrm{maint}}$ is $E_{\mathrm{structure}} + E_{\mathrm{Landauer}}$ — that is, the maintenance cost of the structure itself, plus the Landauer lower-bound energy required to process the minimum information quantity $I_{\mathrm{min}}$ (see the constraint equation in the earlier section on stratification by carrier).

---

### 2.2 The $T$-Family (the Time Family)

The $T$-family quantifies the various timescales that arise in the persistence of a persistent structure. Its base unit is the $\mathrm{s}$ (second).

| Symbol | Unit | Definition | Domain of applicability |
|:---|:---|:---|:---|
| $T$ | $\mathrm{s}$ | Generalized structural persistence time; the parent variable of the temporal parameter when unsubscripted | All PS |
| $T_{\mathrm{static}}$ | $\mathrm{s}$ | Static lifespan: the objective, physical upper bound of persistence time, determined by the structure's own thermodynamic stability, independent of cognition | All PS |
| $T_{\mathrm{pred}}$ | $\mathrm{s}$ | Endogenous time horizon: the temporal span over which a system plans for future states; capable of collapsing or expanding with cognitive state | Active phase only |
| $T_{\mathrm{min}}$ | $\mathrm{s}$ | The minimum physical or computational time grain (Planck time, clock cycle, the limit of neural response) | All PS |
| $T_{\mathrm{max}}$ | $\mathrm{s}$ | The extreme upper bound on the persistence time of a system or environment (the age of the universe, a material's theoretical lifespan) | All PS |

**On the physical status of $T_{\mathrm{pred}}$**: the endogenous time horizon is one of the concepts most clearly distinguishing SRVD from classical physics. In classical mechanics, time $t$ is an exogenous coordinate parameter; in the active phase of SRVD, $T_{\mathrm{pred}}$ is an internal state variable of the system, one that can be lengthened through cognitive planning, or collapse to $T_{\mathrm{min}}$ under short-sighted pressure. The collapse of $T_{\mathrm{pred}}$ constitutes the first dynamical signal of the Myopic Runaway Regime (see Chapter 5).

**The time-horizon constraint**:

$$
T_{\mathrm{min}} < T_{\mathrm{pred}} \leq \min(T_{\mathrm{static}},\, T_{\mathrm{env}})
\tag{2.1}
$$

The endogenous time horizon cannot exceed a structure's objective physical lifespan, nor can it exceed the environment's characteristic timescale. When a system sets $T_{\mathrm{pred}}$ beyond this upper bound, a decoupling deviation $\Delta_{\mathrm{VV}}$ results (see the section on the $V$-family, below).

---

### 2.3 The $V$-Family (the Viability-Potential Family)

The $V$-family quantifies a persistent structure's efficiency of persistence, its self-assessment, and its behavioral drive. Its base unit is $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$.

| Symbol | Unit | Definition | Domain of applicability | Formula |
|:---|:---|:---|:---|:---|
| $V$ | $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$ | Viability potential: a low-order approximate measure of generalized viability efficiency | All PS (conceptual) | $V \approx I \cdot T / E$ |
| $V_{\mathrm{obj}}$ | $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$ | Objective viability potential: a thermodynamic assessment determined by actual energy–information–time parameters | All PS | See equation (3.1) |
| $V^{\mathrm{virt}}$ | $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$ | Virtual viability potential: a system's own internal-model assessment of its own viability efficiency | Active phase only | An isomorphic, twin-term mirror formula |
| $V^{\mathrm{val}}$ | $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$ | Value objective function: the behavioral objective a system actually optimizes | Active phase only | $w_s V_s^{\mathrm{virt}} + w_c V_c^{\mathrm{virt}}$ |
| $w_s$ | dimensionless | Survival weight: the proportion of resources allocated to physical maintenance | Active phase only | $w_s + w_c = 1$ |
| $w_c$ | dimensionless | Development weight: the proportion of resources allocated to cognitive expansion | Active phase only | $w_s + w_c = 1$ |
| $\Delta_{\mathrm{VV}}$ | $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$ | Decoupling deviation: the absolute difference between the virtual and the objective viability potentials | Active phase only | $\lvert V^{\mathrm{virt}} - V_{\mathrm{obj}} \rvert$ |
| $\bar{V}$ | $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$ | Statistical mean viability potential: the long-run average viability potential over a population of structures of the same kind | All PS | — |

**A dimensional reading of the viability potential**: the physical reading of $\dim(V) \sim \mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$ can be stated as follows — the amount of "causal order times time" sustained per unit of equivalent thermodynamic cost (topological order integrated over time, divided by energetic cost). A dimensional reduction based on Landauer's principle gives $\dim(V) \sim \mathrm{s}/\mathrm{K}$, which can be likened to the notion of stability time in statistical mechanics — but this reduction is offered only as a heuristic bridge, not as a claim of strict physical equivalence.

**A note on the objectivity of $V_{\mathrm{obj}}$**: "objective," in $V_{\mathrm{obj}}$, does not imply the existence of a God's-eye view detached from every decoder — it refers instead to an estimate of viability potential that has stabilized and converged across multiple independent decoders, multiple pathways of measurement, and repeated practical feedback. When the cost of measurement or of reaching consensus is extremely high, the achievable precision of $V_{\mathrm{obj}}$ is bounded by $E_{\mathrm{causal}}$; when the parties within a system cannot reach consensus on key parameters, the effective $V_{\mathrm{obj}}$ may fall far short of the theoretical ceiling that would hold were the physical carrier intact. A full treatment of this epistemological constraint belongs to the scope of a separate paper on the epistemological branch of the framework.

---

## 2.4 The Criterion of Structural Identity, and the Type–Token Distinction

### 2.4.1 Passive-Phase Identity (for structures without a cognitive decoder)

Identity is preserved if and only if:

1. the spatiotemporal boundary remains continuous;
2. $I_{\mathrm{struct}}$ evolves gradually (no instantaneous, global rearrangement occurs);
3. the structural energy does not fall below the maintenance floor: $E_{\mathrm{structure}} \geq E_{\mathrm{min}}$ (below this threshold, the structure dissolves).

Structural collapse arises through two distinct physical mechanisms, which must be carefully distinguished:

- **(i) External destruction**: topological collapse driven by an external high-energy input (extreme heat, ionizing radiation), which follows the negative-value information ($I^-$) pathway and manifests as $I_{\mathrm{struct}} \to 0$, rather than as an overrun of $E_{\mathrm{structure}}$;
- **(ii) Energetic starvation**: thermodynamic instability arising from $E_{\mathrm{structure}} < E_{\mathrm{min}}$, in which the structure dissolves for lack of sufficient maintenance energy.

Neither $E_{\mathrm{structure}}$ nor the total equivalent thermodynamic cost $E_{\mathrm{eff}}$ has an absolute theoretical ceiling; each is bounded only by the total free energy available in the environment. $E_{\mathrm{causal}}$, as a component of $E_{\mathrm{eff}}$, likewise has no independent ceiling of its own — but the amount of effective information it can produce is bounded by the Bekenstein bound, its rate of information processing is bounded by the Bremermann limit, and $E_{\mathrm{structure}} \geq E_{\mathrm{min}}$ must still hold; in practice, then, $E_{\mathrm{causal}}$ cannot indefinitely crowd out structural energy.

---

### 2.4.2 Active-Phase Identity (for structures with a cognitive decoder)

Beyond satisfying the passive-phase conditions, five additional conditions apply. **The failure of any single one of them is sufficient to declare that the structure no longer maintains its identity:**

| Condition | Operational indicator | Physical meaning |
|:---|:---|:---|
| $I_{\mathrm{net}} \geq \dot{I}_{\mathrm{min}}$ | The information rate does not fall below the maintenance threshold | Topological continuity is preserved |
| $E_{\mathrm{eff}} \leq E_{\mathrm{thresh}}$ | The thermodynamic cost has not exceeded the dissolution ceiling | No irreversible structural damage has been triggered |
| $T_{\mathrm{pred}} > T_{\mathrm{min}}$ | The endogenous time horizon has not collapsed | The system has not yet entered the Myopic Runaway Regime |
| $\Delta_{\mathrm{VV}} \approx 0$ | The decoupling deviation is close to zero | The system has not been captured by an illusion of virtual potential |
| $D$ has not drifted fundamentally | The decoder still extracts the original causal information | The structure's semantic identity remains intact |

**The dynamical signature of lost identity**: violating any one of the above conditions is sufficient grounds to declare that the structure is no longer the same structure. Of particular note is $T_{\mathrm{pred}} \to T_{\mathrm{min}}$ (the collapse of the time horizon), which produces a qualitative change in behavioral pattern — the system may continue to exist physically, even as its identity in the dynamical sense has already dissolved.

---

### 2.4.3 The Type–Token Distinction

- **Type**: an inheritable informational template (such as a DNA sequence), corresponding to the stable portion of $I_{\mathrm{struct}} + I_{\mathrm{latent}}$.
- **Token**: a concrete individual instance, corresponding to $I_{\mathrm{active}} + I_{\mathrm{struct}}$.

**The evolutionary chain**: rocks (no separation) $\to$ RNA replication (primordial separation) $\to$ multicellular organisms (separation of individual token and type at the level of $I_{\mathrm{struct}}$) $\to$ speciation (splitting of the type itself, at the level of $I_{\mathrm{struct}}$) $\to$ digital entities (separation of token and type at the level of $I_{\mathrm{net}}$).

A single persistent structure may exist across multiple physical carriers. So long as those carriers continue to satisfy the identity conditions in their structural information, their causal information, and the state of their decoder, they jointly constitute a single persistent structure. When irreversible informational divergence arises among carriers, and $\Delta_{\mathrm{VV}}$ exceeds a threshold, the original persistent structure bifurcates, giving rise to a new one.

---

## Chapter 3 — The Mathematical Structure of the Viability Potential

### 3.0 The Low-Order Approximation (Conceptual Form)

$$
\boxed{V \approx \frac{I \cdot T}{E}}
\tag{3.0}
$$

Here $V, I, T, E$ are all generalized conceptual quantities. This equation is SRVD's minimal persistence ansatz: in the low-order approximation, the elasticity exponents are set to $\alpha = \beta = \gamma = 1$.

This multiplicative form rests on three structural requirements: (1) **non-substitutability**: $V(I_{\mathrm{net}}, 0) = 0$ and $V(0, T) = 0$ — the viability potential is zero if either effective information or persistence time is zero; (2) **symmetric contribution**: an increase in either $I_{\mathrm{net}}$ or $T$ raises $V$; (3) **first-order separability**: the lowest-order continuous function satisfying the above conditions is proportional to the product $I_{\mathrm{net}} \cdot T$.

---

### 3.1 The Objective Viability Potential: A Two-Channel Superposition

The complete expression for the objective viability potential superposes two independent channels: the maintenance of the physical carrier ($V_s$) and cognitive causal projection ($V_c$):

$$
\boxed{
V_{\mathrm{obj}} = \begin{cases}
\dfrac{I_{\mathrm{struct}}\,T_{\mathrm{static}}}{E_{\mathrm{structure}}} + \dfrac{I_{\mathrm{net}}\,T_{\mathrm{pred}}}{E_{\mathrm{causal}}}, & E_{\mathrm{min}} \leq E_{\mathrm{eff}} \leq E_{\mathrm{thresh}} \\[10pt]
\text{irreversible damage triggered (structural degradation)}, & E_{\mathrm{eff}} > E_{\mathrm{thresh}} \\[10pt]
\text{undefined (structure dissolved)}, & E_{\mathrm{eff}} < E_{\mathrm{min}}
\end{cases}
}
\tag{3.1}
$$

> **A note on the domain of validity**: the normal domain of validity for $V_{\mathrm{obj}}$ is $E_{\mathrm{min}} \leq E_{\mathrm{eff}} \leq E_{\mathrm{thresh}}$, satisfying at once a lower energetic bound (the structure does not dissolve) and an upper energetic bound (no irreversible damage is triggered). The region $E_{\mathrm{eff}} > E_{\mathrm{thresh}}$ is not a simple extension of $V_{\mathrm{obj}}$ but a regime of structural degradation, corresponding to the activation of the damage term in equation (5.3). The three regions together constitute a complete partition of the state space of viability, consistent with the condition $E_{\mathrm{eff}} \leq E_{\mathrm{thresh}}$ given in the earlier section on active-phase identity.

Define:

$$
V_s = \dfrac{I_{\mathrm{struct}}\,T_{\mathrm{static}}}{E_{\mathrm{structure}}}, \qquad V_c = \dfrac{I_{\mathrm{net}}\,T_{\mathrm{pred}}}{E_{\mathrm{causal}}}
\tag{3.1a}
$$

In a passive structure, $I_{\mathrm{net}} = 0$, so $V_c = 0$ and $V_{\mathrm{obj}} = V_s$.

**Decomposition of the energy budget**:

$$
E_{\mathrm{eff}} = E_{\mathrm{structure}} + E_{\mathrm{causal}} = (E_{\mathrm{barrier}} + E_{\mathrm{survival}}) + E_{\mathrm{causal}}
\tag{3.2}
$$

$E_{\mathrm{structure}}$ and $E_{\mathrm{causal}}$ compete for the same total energy budget. In the passive phase, $E_{\mathrm{causal}} = 0$; in the active phase, if $E_{\mathrm{causal}}$ increases, then, given a fixed total budget, the budget available for $E_{\mathrm{survival}}$ must decrease correspondingly.

**Why the two channels cannot be merged into a single product**: $V_s$ and $V_c$ couple different classes of information ($I_{\mathrm{struct}}$ versus $I_{\mathrm{net}}$), different timescales ($T_{\mathrm{static}}$ versus $T_{\mathrm{pred}}$), and different energetic costs ($E_{\mathrm{structure}}$ versus $E_{\mathrm{causal}}$). Their additive superposition reflects two independent thermodynamic channels; there is no algebraic cancellation or reduction available between them.

> **A statement on channel independence and the domain of validity**: the additive form of equation (3.1) requires that $V_s > 0$ *and* $V_c > 0$ hold simultaneously for the result to fall within the normal domain of validity; the two channels stand in a relation of **superposed lower bounds**, not one in which either can substitute for or be compensated by an extreme value of the other. Specifically: the validity of $V_s$ presupposes that the physical carrier is maintained, $E_{\mathrm{structure}} \geq E_{\mathrm{min}}$ (the carrier survives); the validity of $V_c$ presupposes that cognitive operation is underway, $E_{\mathrm{causal}} \geq E_{\mathrm{Landauer}}$ (the decoder is actually running); neither can be dispensed with. If one were to let $E_{\mathrm{causal}} \to 0$ while attempting to let $I_{\mathrm{net}} \to \infty$, so as to keep $V_c$ unchanged or even increasing, this has no physical basis — because the Landauer lower bound given in the section on the Landauer limit, further on, $E_{\mathrm{causal}} \geq k_B T_{\mathrm{thermo}}\ln 2 \cdot I_{\mathrm{net}}$, already prohibits an arbitrarily large $I_{\mathrm{net}}$ from corresponding to an arbitrarily small $E_{\mathrm{causal}}$. When the energy supporting a given channel tends toward zero, that channel itself tends toward being undefined — rather than being set to zero and then infinitely amplified in compensation by the other channel. This is fully consistent with the ontological premise, stated in Chapter 1's section on persistent structures requiring an energetic constraint and in the note to the table in the section on the criterion of decoder activity, that the cognitive channel cannot expand without limit, substituting for the physical-carrier channel, without paying a thermodynamic cost.

**The survival threshold**: crossing $E_{\mathrm{eff}} < E_{\mathrm{min}}$ triggers a **phase transition**, not a continuous decay — the structure no longer satisfies the energetic condition of a persistent structure; it dissolves and exits the analytical domain of SRVD.

**An integral reading**: define the accumulated viability quantity $Q = \int I_{\mathrm{net}}(t)\,\mathrm{d}t$ ($\mathrm{bit}\cdot\mathrm{s}$). For a system near steady state, $Q \approx I_{\mathrm{net}} \cdot T$. Then the viability potential $V = Q / E_{\mathrm{eff}}$ is the integral of topological order over time, sustained per unit of equivalent thermodynamic cost.

---

### 3.2 Elasticity Exponents and the Core Ordering Proposition

#### 3.2.1 The Definition and Physical Meaning of the Elasticity Exponents

The complete power-law form of the viability potential is:

$$
V = V_0 \left(\frac{I}{I_0}\right)^\alpha \left(\frac{T}{T_0}\right)^\beta \left(\frac{E_{\mathrm{eff}}}{E_0}\right)^{-\gamma}
\tag{3.3}
$$

Here $I_0, T_0, E_0$ are reference scales, and $\alpha, \beta, \gamma$ are dimensionless **elasticity exponents**, defined as partial derivatives in log–log space:

$$
\alpha := \left.\frac{\partial \ln V}{\partial \ln I}\right|_{E,T}, \quad
\gamma := \left.\frac{\partial \ln V}{\partial \ln E_{\mathrm{eff}}}\right|_{I,T}, \quad
\beta := \left.\frac{\partial \ln V}{\partial \ln T}\right|_{I,E}
\tag{3.4}
$$

**A conceptual clarification — the elasticity exponents versus shadow prices**: the elasticity exponents ($\alpha, \beta, \gamma$) are a structure's **intrinsic weighting** of its resources, fixed by fundamental thermodynamic law and constant within the domain of validity; shadow prices ($\lambda_I, \lambda_E, \lambda_T$ — that is, Lagrange multipliers) are the **marginal effective value** of a resource under a given constraint, and can swing widely with the tightness of local survival constraints. When a person learns they have "only three months left," the shadow price $\lambda_T$ of time surges — not because the elasticity exponent $\beta$ has changed, but because the temporal constraint has tightened to an extreme.

> **A key distinction**: the elasticity exponents ($\alpha, \beta, \gamma$) and the shadow prices ($\lambda_I, \lambda_E, \lambda_T$) belong to two different conceptual levels:
>
> | | Elasticity exponent | Shadow price |
> |:---|:---|:---|
> | Definition | A structure's intrinsic weighting of a resource | The marginal effective value of a resource under a given constraint |
> | Determined by | Fundamental thermodynamic law | Local survival constraints |
> | Variability | Constant within the domain of validity | Fluctuates widely with the constraint |
> | Mathematical identity | The exponential coefficient of a potential function | A Lagrange multiplier |
>
> An intuitive example: in ordinary circumstances, a person's elasticity exponent $\beta$ with respect to time is small; but when a doctor says "only three months left," the shadow price $\lambda_T$ of time surges — this does not mean $\beta$ has changed, but that $\lambda_T$ has been driven up under a suddenly tight constraint.

---

#### 3.2.2 The Ordering Proposition: The Theoretical Inference of $\alpha > \gamma > \beta$, and Its Thermodynamic Directional Argument

**This is not a simple induction from empirical observation, but a theoretical, directional argument proceeding from the second law of thermodynamics and the information–energy relation; the boundary of its rigor is addressed in the corrective note at the end of this section.**

**Derivation I: $\alpha > \gamma$ (the informational elasticity exponent exceeds the energetic elasticity exponent)**

The elasticity exponent $\alpha = \partial \ln V / \partial \ln I$ measures how many percentage points $V$ rises for a 1% increase in $I$. The second law of thermodynamics tells us that ordered structure (negentropy) is the fundamental scarce good of the universe. Landauer's principle gives this a quantitative form: in an environment at temperature $T_{\mathrm{thermo}}$, the irreversible energetic cost of generating or erasing one bit of information is:

$$
E_{\mathrm{min}}^{(\mathrm{bit})} = k_B T_{\mathrm{thermo}} \ln 2
\tag{3.4a}
$$

Generating structured information requires ordered arrangement and entropy-reducing operation; extracting an equivalent quantity of dissipated heat requires only a gradient and a channel. From this it follows that the rate at which a unit of information contributes to viability potential ($\alpha$) exceeds the rate at which a unit of energetic cost suppresses it ($\gamma$), that is:

$$
\boxed{\alpha > \gamma}
\tag{3.4b}
$$

> **A note on the rigor of this derivation**: the argument here establishes the **qualitative direction** of the ordering — that the thermodynamic scarcity of information entails $\alpha > \gamma$ — rather than a precise numerical gap between $\alpha$ and $\gamma$. The quantitative values must be estimated, within an isomorphic medium, from empirical scaling laws (see the section on multi-domain empirical observation, below). The reason the high marginal cost of information is mapped onto the elasticity exponent $\alpha$ rather than onto the shadow price $\lambda_I$ is this: an elasticity exponent reflects a structure's **intrinsic power-law response** to a resource — and as a system expands along its natural evolutionary trajectory, thermodynamic scarcity is encoded into that power law over the long run through selective pressure, rather than functioning merely as a marginal value under some local constraint.

**Derivation II: $\gamma > \beta$ (the energetic elasticity exponent exceeds the temporal elasticity exponent)**

Energy is obtained, transformed, and stored through active metabolic processes (high agency); time is passively granted by the universe, neither producible nor storable (zero agency). A structure's dependence on energy is more pressing, so the magnitude of the effect of a unit change in energy on viability potential ($\gamma$) exceeds that of a unit change in time ($\beta$); hence:

$$
\boxed{\gamma > \beta}
\tag{3.4c}
$$

**The combined derivation**:

$$
\boxed{\alpha > \gamma > \beta > 0}
\tag{3.4d}
$$

The chain of physical explanation runs: the second law of thermodynamics (entropy increase is irreversible) $\to$ ordered structure is the universe's fundamental scarce good $\to$ a structure's power-law responsiveness to information exceeds its responsiveness to energy, which in turn exceeds its responsiveness to time $\to$ $\alpha > \gamma > \beta$.

**A corrective note on the phrase "first-principles derivation"**: the argument above proceeds from thermodynamic constraints to establish the qualitative direction of the ordering; it is a **theoretical, deductive inference**, not a strict mathematical derivation. Full verification of the ordering proposition depends on the multi-domain empirical data given in the section on multi-domain empirical observation, below. The two together form a complementary support structure: theoretical deduction supplies the physical intuition, and empirical scaling laws supply the quantitative constraint.

#### 3.2.3 Multi-Domain Empirical Observation

The ordering $\alpha > \gamma > \beta$ is observed consistently in scaling-law data from three independent domains:

**Biological systems (West, Brown & Enquist, 1997, allometric scaling)**:

| Biological observation | Scaling relation | Inferred elasticity exponent |
|:---|:---|:---|
| Basal metabolic rate | $P_0 \sim M^{0.75}$ | $\gamma \approx 0.75$ |
| Lifespan | $T_{\mathrm{life}} \sim M^{0.25}$ | $\beta \approx 0.25$ |
| Genomic complexity | $I \sim M^{1.0 \sim 1.5}$ | $\alpha \approx 1.0 \sim 1.5$ |

Consistent with the ordering, with no counterexample found: $\alpha(1.0\text{–}1.5) > \gamma(0.75) > \beta(0.25)$ ✓

> **A methodological note (guarding against circular verification)**: the estimate of $\alpha$ for biological systems in the table above relies on an independent proxy assumption — that "effective genomic information $I$ scales with body mass as $I \sim M^{1.0\sim1.5}$." This proxy assumption is drawn from the empirical observations behind allometric scaling (West, Brown & Enquist, 1997), and its validity is independent of the SRVD ordering proposition $\alpha>\gamma>\beta$ itself — even were the power-law relation between genomic complexity and body mass eventually overturned or revised, this would only invalidate the biological-domain estimate of $\alpha$, and would not constitute a falsification of the direction of the ordering $\alpha>\gamma>\beta$, since that ordering can hold independently in the two other, independent domains discussed below — AI systems and urban systems — without relying on the biological case. In other words, the empirical support from the three domains is a parallel, not a serial, structure: the failure of one domain's proxy assumption does not propagate to the others.

**Artificial-intelligence systems (Kaplan et al., 2020; Chinchilla, 2022)**:

| AI-system observation | Scaling relation | Inferred elasticity exponent |
|:---|:---|:---|
| Loss versus parameter count | $L \sim N^{-1.5 \sim 2.0}$ | $\alpha \approx 1.5 \sim 2.0$ |
| Computational efficiency | Roughly constant energy cost per unit of precision | $\gamma \approx 0.8 \sim 1.0$ |
| Training time | $T_{\mathrm{train}} \sim N^{0.1 \sim 0.2}$ | $\beta \approx 0.1 \sim 0.2$ |

Consistent with the ordering, with no counterexample found: $\alpha(1.5\text{–}2.0) > \gamma(0.8\text{–}1.0) > \beta(0.1\text{–}0.2)$ ✓

**Urban systems (Bettencourt, 2013)**:

| Urban observation | Scaling relation | Inferred elasticity exponent |
|:---|:---|:---|
| GDP versus population | $\mathrm{GDP} \sim N^{1.15 \sim 1.25}$ | $\alpha \approx 1.15 \sim 1.25$ |
| Energy consumption | $E \sim N^{0.85 \sim 0.95}$ | $\gamma \approx 0.85 \sim 0.95$ |
| Infrastructure-renewal cycle | $T \sim N^{0.2 \sim 0.3}$ | $\beta \approx 0.2 \sim 0.3$ |

Consistent with the ordering, with no counterexample found: $\alpha(1.15\text{–}1.25) > \gamma(0.85\text{–}0.95) > \beta(0.2\text{–}0.3)$ ✓

**Summary of robustness**:

| Domain | Range of $\alpha$ | Range of $\gamma$ | Range of $\beta$ | Ordering | Scale span |
|:---|:---|:---|:---|:---|:---|
| Biology | 1.0–1.5 | 0.70–0.80 | 0.20–0.30 | ✓ | $\sim 10^{10}$ |
| AI | 1.5–2.5 | 0.80–1.10 | 0.10–0.25 | ✓ | $\sim 10^{20}$ |
| Cities | 1.15–1.30 | 0.85–0.95 | 0.20–0.35 | ✓ | $\sim 10^{5}$ |

The ordering $\alpha > \gamma > \beta$ has been observed across all three independent domains, with no counterexample found to date.

> **A note on the nature of this verification**: the empirical data above stand in a complementary relationship to the theoretical inference given in the section on the ordering proposition, rather than constituting an independent proof. Two caveats apply: (1) the extraction of an elasticity exponent depends on a proxy mapping onto the scaling law (such as mapping the basal-metabolic exponent onto $\gamma$), and this mapping is itself not uniquely determined; (2) the empirically measured $\gamma \approx 0.8\text{–}1.1$ for AI systems overlaps with the normalization assumption $\gamma \equiv 1$ used in the section on energetic-benchmark normalization, below — this does not constitute circular verification, since the normalization is an independent engineering choice (taking an idealized operating state as the benchmark), while the measured value is a statistical estimate of current systems; their agreement supports the reasonableness of the normalization assumption rather than confirming itself.

#### 3.2.4 Energetic-Benchmark Normalization: Anchoring $\gamma = 1$

To advance the ordering proposition toward computable engineering application, we introduce an **energetic-benchmark normalization**: setting $\gamma \equiv 1$.

The theoretical rationale is twofold: (1) energy (the joule) is a conserved, mutually commensurable base measure, and $\gamma = 1$ means that the basic cost of maintaining a structure maps linearly onto energy — the direct expression, within SRVD, of the first law of thermodynamics. The motivation for choosing $\gamma=1$ is this: the first law requires that energy, as a conserved quantity, rest on a linear accounting basis (its increases and decreases can be added and subtracted directly, with no nonlinear loss or gain), and the normalization benchmark for the elasticity exponents ought to be consistent with this linearity — hence the baseline response along the energy dimension is taken to be a linear mapping. (2) empirical data from cities ($\gamma \approx 0.85\text{–}0.95$) and large-scale AI clusters ($\gamma \approx 0.9\text{–}1.0$) show that as a system's scale grows and its resource allocation approaches the theoretical optimum, $\gamma$ asymptotically converges toward 1, representing the benchmark of an "ideal, high-efficiency operating state."

Once normalized, the constraint relation becomes $\alpha > 1 > \beta$:

- **$\alpha > 1$ (super-linear informational gain)**: the increase in viability potential from an added unit of structured information exceeds the energetic cost consumed in acquiring it.
- **$\beta < 1$ (sub-linear temporal gain)**: the increase in viability potential from simply extending the persistence time falls short of the energetic cost of sustaining that additional time.

The normalized viability-potential function becomes:

$$
V \propto \frac{I^\alpha \cdot T^\beta}{E_{\mathrm{eff}}}, \quad \alpha > 1,\; 0 < \beta < 1
\tag{3.5}
$$

Taking the total differential of the potential function gives the marginal-return identity:

$$
\frac{\Delta V}{V} \approx \alpha \cdot \frac{\Delta I}{I} + \beta \cdot \frac{\Delta T}{T} - \frac{\Delta E_{\mathrm{eff}}}{E_{\mathrm{eff}}}
\tag{3.6}
$$

> **A corollary on resource allocation**: three principles can be read directly off equation (3.6):
>
> 1. **Information first**: when the cost of acquiring an informational increment is less than $\alpha$ times its return, investment should be directed toward information rather than toward extending time. In AI scenarios, the ROI of scaling parameters runs roughly ten times higher than that of extending training time ($\alpha \approx 1.94$ versus $\beta \approx 0.17$).
> 2. **Cut losses on time**: if a time window brings no informational increment ($\Delta I \to 0$), continuing to sustain the energy expenditure is a net loss — a stagnant period calls for contracting energy consumption.
> 3. **The energy red line**: once the informational dividend is exhausted ($\alpha \cdot \Delta I/I \to 1$), the system has reached the boundary of its optimal scale, and any further energy investment will directly lower the viability potential.

> **SRVD proposes the viability potential $V$ as a unified state variable, and gives it the mathematical form $V \approx I \times T / E$. It further asserts that "maximizing viability potential" is the ultimate driving engine behind the behavior of every ordered, negentropic structure — every other mechanism is a local strategy in its service.**

---

#### 3.2.5 The Constancy of the Elasticity Exponents: An Open Hypothesis

This section has demonstrated that the ordering $\alpha > \gamma > \beta$ is a thermodynamic necessity; the necessity of the ordering does not entail the constancy of the numerical values themselves. Three possibilities remain open:

| Level of hypothesis | Meaning | Status of evidence |
|:---|:---|:---|
| **Strong hypothesis: universal constants** | $\alpha, \beta, \gamma$ take the same numerical value across every system | No direct evidence; untested |
| **Medium hypothesis: constant within a domain** | $\alpha, \beta, \gamma$ are constant within a class of system but differ across classes | Consistent with current data |
| **Weak hypothesis: only the ordering is constant** | Only $\alpha > \gamma > \beta$ is universal; the specific values vary from system to system | Also consistent with current data |

The constancy of $\alpha, \beta, \gamma$ is one of this framework's most central, still-untested scientific propositions; it cannot be settled until a unified framework for measuring informational complexity across domains has been established.

#### 3.2.6 The Current State and Limits of Numerical Precision

The fundamental limit on quantitative comparison at present is this: **the way structured information $I$ is defined differs fundamentally across types of system, and cannot currently be unified across domains and scales**.

| System type | Natural definition of $I$ | Method of measurement | Current status |
|:---|:---|:---|:---|
| DNA sequence | The minimum encoding length required to generate the genome | LZMA compression | ✓ Measurable; consensus within the domain |
| Neural network | The effective dimension/rank of the network's parameters | Parameter count, Fisher rank | △ Comparable within the domain |
| Image / art | Visual structural complexity | Visual encoders | ✗ No mature definition |
| Social structure | The complexity of social organization | — | ✗ Entirely undefined |

**An operational rule (when quantification is permitted, and when qualification is required)**: given the limits above, SRVD sets the following explicit boundary between quantitative and qualitative statements:

1. **Within-domain quantification — permitted**: within a single type of system (among different neural-network models, or among different DNA sequences), precise relative numerical comparison is possible, and conclusions may be applied directly to quantitative prediction.
2. **Cross-domain qualification — required**: when drawing an analogy or inference across different types of system (comparing, say, the direction of the elasticity-exponent ordering between biological and AI systems), only qualitative statements are permitted (such as "both satisfy $\alpha>\gamma$"); no claim of a precise numerical gap may be made.
3. **Cross-domain tabular comparison — explicitly prohibited**: placing the $\alpha,\beta,\gamma$ values of different types of system directly side by side in a single table as an absolute comparison (for instance, "biology's $\alpha\approx1.2$, therefore society's $\alpha$ should also be approximately $1.2$") cannot be rigorously falsified under our current state of knowledge, and should not appear in quantitative predictions. Quantitative comparison within SRVD should be conducted, in preference, **within an isomorphic medium or among closely related systems** (see the section on restricted-domain empirical validation, below).

If a system's measured, apparent $\alpha \leq 1$, the appropriate diagnosis is: (1) a measurement failure — noise mistaken for structured information; or (2) the system is in a state of involution, or a precursor to phase transition — its resource-allocation strategy has failed, and structural reorganization is required.

---

### 3.3 The Virtual Viability Potential

$$
\boxed{
V^{\mathrm{virt}} = \frac{I_{\mathrm{struct}}^{\mathrm{virt}}\,T_{\mathrm{static}}^{\mathrm{virt}}}{E_{\mathrm{structure}}^{\mathrm{virt}}} + \frac{I_{\mathrm{net}}^{\mathrm{virt}}\,T_{\mathrm{pred}}^{\mathrm{virt}}}{E_{\mathrm{causal}}^{\mathrm{virt}}}
}
\tag{3.7}
$$

Every variable carrying the $^{\mathrm{virt}}$ superscript denotes an internally assessed value — isomorphic to, but not equal to, its objective counterpart. The virtual viability potential is a system's **subjective, internal mirror** of its own viability efficiency, and is not required to agree with objective reality.

The value of $V^{\mathrm{virt}}$ is independent of $V_{\mathrm{obj}}$: when a system computes $V^{\mathrm{virt}}$, the inputs are its internal model's subjective estimates of each parameter ($I_{\mathrm{net}}^{\mathrm{virt}}$, $T_{\mathrm{pred}}^{\mathrm{virt}}$, $E_{\mathrm{causal}}^{\mathrm{virt}}$, and so on), and these estimates are determined by the system's current cognitive state, not by external thermodynamic measurement. Consequently, even as the objective physical parameters deteriorate, $V^{\mathrm{virt}}$ can, through an internally optimistic estimate, remain high or even continue to inflate — this is precisely the underlying reason $V^{\mathrm{virt}}$ and $V_{\mathrm{obj}}$ can diverge for extended periods once the threefold split has occurred. The systematic deviation between $V^{\mathrm{virt}}$ and $V_{\mathrm{obj}}$ is the mathematical root of cognitive decoupling, self-deception, and irrational decision-making; its equation of evolution and its conditions of convergence are given in the section on decoupling-deviation dynamics, below.

---

### 3.4 The Value Objective Function

$$
\boxed{
V^{\mathrm{val}} = w_s V_s^{\mathrm{virt}} + w_c V_c^{\mathrm{virt}}, \qquad w_s + w_c = 1
}
\tag{3.8}
$$

Here $V_s^{\mathrm{virt}} = I_{\mathrm{struct}}^{\mathrm{virt}} T_{\mathrm{static}}^{\mathrm{virt}} / E_{\mathrm{structure}}^{\mathrm{virt}}$ and $V_c^{\mathrm{virt}} = I_{\mathrm{net}}^{\mathrm{virt}} T_{\mathrm{pred}}^{\mathrm{virt}} / E_{\mathrm{causal}}^{\mathrm{virt}}$; $w_s$ is the survival weight, and $w_c$ is the development weight.

**Core proposition**: what a system actually optimizes is not $V_{\mathrm{obj}}$, but $V^{\mathrm{val}}$. When $w_s$ and $w_c$ become extremely skewed (for instance, $w_s \to 0$ together with $\Delta_{\mathrm{VV}} \gg 0$), a system can shift from "pursuing objective viability" to "pursuing a virtual, self-destructive goal." The complete dynamics of this value-weight phase transition — including its threshold conditions and steady-state analysis — is stated here only as a conceptual claim in this version.

Accordingly, "maximizing viability potential," in the active phase, is precisely specified as the maximization of $V^{\mathrm{val}}$; the composition of $V^{\mathrm{val}}$ and the allocation of its weights determine the concrete form a system's behavior takes under any given constraint.

---

### 3.5 Compound Definitions

$$
E_{\mathrm{eff}} = E_{\mathrm{barrier}} + E_{\mathrm{survival}} + E_{\mathrm{causal}}
\tag{3.9}
$$

$$
E_{\mathrm{structure}} = E_{\mathrm{barrier}} + E_{\mathrm{survival}}
\tag{3.10}
$$

$$
E_{\mathrm{flow}} = E_{\mathrm{survival}} + E_{\mathrm{causal}}
\tag{3.11}
$$

$$
I_{\mathrm{net}} \equiv \eta_D \cdot I_{\mathrm{latent}}, \qquad I_{\mathrm{active}} \leq I_{\mathrm{net}}
\tag{3.12}
$$

> **A note on this definition**: equation (3.12) fixes the primary definition of $I_{\mathrm{net}}$ as the extraction-based view, $\eta_D \cdot I_{\mathrm{latent}}$. $I_{\mathrm{active}}$ is the subset of $I_{\mathrm{net}}$ currently activated ($I_{\mathrm{active}} \leq I_{\mathrm{net}}$); when a system is operating at full capacity ($\eta_D = 1$, with every latent capacity activated), $I_{\mathrm{active}} = I_{\mathrm{net}}$. The earlier formulation $I_{\mathrm{net}} = I_{\mathrm{latent}} + I_{\mathrm{active}}$ led to both dimensional and logical contradictions, and has been corrected here.

$$
I_{\mathrm{total}} = I_{\mathrm{struct}} + I_{\mathrm{net}}
\tag{3.13}
$$

**A note on $I_{\mathrm{total}}$: a unified substrate, a division of function, and inter-system conversion**

$I_{\mathrm{total}} = I_{\mathrm{struct}} + I_{\mathrm{net}}$ denotes a structure's total informational reserve.

**First layer: the unity of the underlying ontology (why the two quantities may be added)**

Under SRVD's definitions, $I_{\mathrm{struct}}$ and $I_{\mathrm{net}}$ share the same underlying information-theoretic definition: the logarithm, $I = \log_2 \Omega$, of the number of states $\Omega$ that can be stably distinguished under a given decoder. Whether it is the base-pair sequence of a DNA double helix, the synaptic weight matrix of a neural network, or the written rules of a social institution, there is no essential difference among them at the ontological level of "a distinguishable, ordered topological configuration." Their present separation is a technological gap in metrology, not an iron curtain of ontology.

**Second layer: a division of function within the SRVD framework (algebraic rigidity within the formula)**

Even as they share this underlying definition, $I_{\mathrm{struct}}$ and $I_{\mathrm{net}}$ couple to different timescales and different energetic costs within the viability potential, and play non-interchangeable roles in $V_{\mathrm{obj}} = V_s + V_c$:

| Dimension | $I_{\mathrm{struct}}$ | $I_{\mathrm{net}}$ |
|:---|:---|:---|
| Associated term | $V_s = I_{\mathrm{struct}} \cdot T_{\mathrm{static}} / E_{\mathrm{structure}}$ | $V_c = I_{\mathrm{net}} \cdot T_{\mathrm{pred}} / E_{\mathrm{causal}}$ |
| Temporal coupling | Couples to the static lifespan $T_{\mathrm{static}}$ (a slow variable) | Couples to the prediction horizon $T_{\mathrm{pred}}$ (a fast variable) |
| Energetic coupling | Couples to structural-maintenance energy $E_{\mathrm{structure}}$ | Couples to causal-decision energy $E_{\mathrm{causal}}$ |
| Functional role | The ordered foundation of the physical carrier | The causal engine of the cognitive system |
| **Interchangeable within the $V_{\mathrm{obj}}$ formula?** | **No** (algebraic rigidity: $V_s$ and $V_c$ are additively superposed and cannot be reduced or cancelled against each other) | **No** (as above) |

**Third layer: transfer and conversion between systems (a social thermodynamics)**

This "non-interchangeability" refers only to the algebraic rigidity of the $V_{\mathrm{obj}}$ formula *within a single system*. It does not preclude one system, by paying $E_{\mathrm{causal}}$, from transferring its $I_{\mathrm{net}}$ (informational symbol) to another system, in exchange for control over, or compensation from, that other system's $I_{\mathrm{struct}}$ (physical carrier) — currency is precisely a symbolic token of $I_{\mathrm{net}}$, and the essence of a transaction is the thermodynamic conversion of control rights over $I_{\mathrm{net}}$ and $I_{\mathrm{struct}}$ between different systems, a conversion governed by social contract and legal framework rather than by algebraic substitution within the SRVD formula. Detailed case analysis — including compensation, judicial enforcement, and resource exchange between individuals and states — is left to future work; the body text here retains only this ontological conclusion: this distinction gives SRVD a unified physical foundation for explaining currency, law, war, and the social contract.

**Fourth layer: a roadmap for metrology (the direction of future unification)**

The two quantities are, at present, measured by different protocols (DNA compressors versus effective parameter rank) — much as "mass" and "energy" appeared incommensurable in measurement at the start of the twentieth century, until $E = mc^2$ established a general mechanism of conversion between them. SRVD holds that $I_{\mathrm{struct}}$ and $I_{\mathrm{net}}$ will eventually acquire a unified measurement framework as well — a unification that will represent progress in our quantitative instruments, not a blurring of the roles these two quantities play within the viability potential.

**A practical recommendation**: at the current stage of empirical work, numerical addition within $I_{\mathrm{total}}$ should be treated with caution, and is not recommended for direct substitution into quantitative prediction. As a conceptual anchor, however, it is of considerable importance — it reminds us that the physical carrier and the cognitive model share a single informational substrate, constrained only by different couplings of energy and time. This framework retains it as a legitimate definition, a theoretical anchor for a future, unified science of information measurement.

---

## Chapter 4 — The Decoder Framework

### 4.0 The Decoder-Centered Descriptive Principle

SRVD does not describe the world directly; it describes how a persistent structure interacts with the world through a decoder $D$. Information, prediction, value, and measurement are all defined through the decoding process. This is the feature that fundamentally distinguishes SRVD from most fixed-observer frameworks: a structure changes not only its own state, but also the very way it comes to know the world.

**The decoder's status as a physical entity**: the decoder $D$ is not a mathematical operator or a metaphysical rule of interpretation, but a **genuine physical structure** that converts energy into effective causal information — a neural topology, a silicon circuit, a body of law stored in a physical medium. Any decoding structure at the cultural, theoretical, or linguistic level must pay a physical maintenance cost, satisfying:

$$
E_{\mathrm{maint}}(D) \geq E_{\mathrm{Landauer}}(I_{\mathrm{min}}(D)) + E_{\mathrm{structure}}
\tag{4.1}
$$

There is therefore no "purely abstract" logical system with zero physical maintenance cost anywhere within SRVD.

---

### 4.1 Measurement and Observation

Every core variable depends on the definition of a specific decoder. The observer is itself a persistent structure, so any act of measurement corresponds to a process of information extraction under a particular decoding condition. Observational capacity is constrained by energetic cost, temporal resolution, and signal-to-noise ratio — boundaries set by the physical channel, not by any assumption reaching beyond physics.

**The macroscopic-bystander decoder ($D_{\mathrm{macro}}$)**: classical physics implicitly adopts an idealized macroscopic-bystander decoder (the SI unit system, isolated systems, no measurement disturbance). Within SRVD, classical physics can be regarded as the limiting description under a fixed $D_{\mathrm{macro}}$ condition — a single, special point within the space of decoders.

---

### 4.2 Informational Polarity: Viability Polarity

A physical causal interaction is not the same thing as effective causal information. Information is divided into three classes, according to its effect on the topological direction of a system's long-run reachable state space:

- **Positive-value information ($I^+$)**: input capable of expanding a system's **long-run reachable state space** and enhancing structural plasticity.
- **Negative-value information ($I^-$)**: input that damages a system's structure, triggers irreversible entropy increase, or compresses its state space.
- **Neutral noise ($I^0$)**: input that produces physical causal effect without mapping onto any viability polarity.

**The relational essence of polarity**: information's physical basis is an objective topological configuration, but its polarity ($I^+, I^-, I^0$) is determined by its relation to the decoder $D$. The same object can display entirely different polarities to different decoders: a book offers a reader survival-relevant knowledge ($I^+$); that same virus causes structural damage to a host cell ($I^-$); random noise fails to form an effective match with any decoder ($I^0$). Causal efficacy is not an isolated physical property, but **a measure of the degree of match between a topological configuration and the structure of a decoder**.

**A measurement-theoretic statement (applicable to the active phase)**: for a system with a cognitive decoder $D_{\mathrm{cog}}$, the polarity assignment of $I^+$ and $I^-$ is a real-time, dynamic label generated within the $T_{\mathrm{pred}}$ window, based on the predictive gradient of $V^{\mathrm{virt}}$ (a forward-looking assessment) — not a retrospective classification that waits for $V_{\mathrm{obj}}$ to actually unfold. The system drives its allocation of $E_{\mathrm{causal}}$ according to this label. When $\Delta_{\mathrm{VV}} > 0$, this forward-looking assessment can systematically diverge from objective reality — and this divergence is precisely the fuel of the dynamic described in the section on the Myopic Runaway Regime, below.

**Paradigm-level distinctions**: within $I^+$, a further gradation exists, according to the depth to which the decoder's topological structure is reconstructed:

- **Paradigm-breaking information ($I_{\mathrm{orig}}$)**: opens an entirely new causal dimension, its marginal efficacy undiminished by replication, capable of forcibly resetting the topological distance of a niche.
- **Paradigm-interpretive information ($I_{\mathrm{interp}}$)**: high-quality execution or local parameter optimization within an existing paradigm, its marginal efficacy decaying rapidly as it becomes homogenized ($\Delta I \to 0$).

This distinction is the physical basis for explaining the crisis of homogenization in the age of artificial intelligence.

---

### 4.3 Relation to Existing Frameworks

SRVD is a coarse-grained, macro-dynamical framework. It does not compete with the following established theories; instead, it maps each of them onto a special case or a boundary input:

| Framework | Its role within SRVD | SRVD's extension |
|:---|:---|:---|
| Prigogine's theory of dissipative structures | Describes the $E_{\mathrm{survival}}$-dominated regime of the active-viability domain | SRVD adds the $E_{\mathrm{barrier}}$ (passive) and $E_{\mathrm{causal}}$ (information-processing) components, and extends beyond the near-equilibrium regime |
| Ulanowicz's ascendency theory | The numerator $A = T \cdot I$ is structurally isomorphic to that of $V$ | SRVD supplies the denominator $E_{\mathrm{eff}}$, making comparison across substrates possible |
| Landauer's principle | Supplies the hard lower bound $E_{\mathrm{causal}} \geq k_B T_{\mathrm{thermo}} \ln 2 \cdot I_{\mathrm{net}}$ | Enters SRVD as the physical floor of $E_{\mathrm{min}}$ |
| Free Energy Principle (FEP)                  | Local mathematical analogy confined to a single energy channel ($-\nabla E_{\mathrm{maint}}$) | FEP is a convergence process of a single scalar within a fixed-dimensional parameter space; SRVD's three-way split structure, topological dimensional transition, and coupling-instability pathway have no corresponding mathematical position within that scalar framework — the two have non-overlapping domains and a non-nested relationship |
| General relativity | Supplies gravitational time dilation, $T \to T\sqrt{1 - 2GM/c^2 R}$, and black-hole thermodynamics, as boundary inputs | SRVD cites GR's conclusions; near a horizon, they are consistent with the collapsing manifold where $V \to 0$ |
| Shannon information theory | Shannon mutual information $H(X)$ is the pure probabilistic limit of $I_{\mathrm{net}}$ once polarity and viability objective are stripped away | SRVD's $I_{\mathrm{net}}$ carries decoder-dependence and viability polarity — it is a physical topological entity, not merely a measure of signal uncertainty |
| Complex adaptive systems theory (Holland) | Describes the general process by which agents interact with their environment through rule sets, giving rise to macroscopic order through selection and recombination | SRVD decomposes "fitness" explicitly into three independently measurable physical-informational quantities — $I_{\mathrm{net}}$, $T_{\mathrm{pred}}$, $E_{\mathrm{eff}}$ — and supplies the $V$ formula as a unified scalarization of fitness; CAS theory describes the qualitative mechanism of emergence, and SRVD supplies its thermodynamic, quantitative constraint |

### 4.4 Mathematics as a Thermodynamic Limit (An SRVD Reconstruction of Wigner's Puzzle)

Wigner (1960) pointed to "the unreasonable effectiveness of mathematics in the natural sciences." SRVD offers the following speculative reconstruction, presented as a hypothesis rather than a proven result:

**The cognitive-isomorphism hypothesis**: any intelligence that evolves under sustained Landauer pressure (minimizing $E_{\mathrm{maint}}$, maximizing $\eta = I_{\mathrm{net}}/E_{\mathrm{eff}}$) may converge upon a cognitive structure isomorphic to mathematics — because mathematics represents the most compact encoding of causal structure achievable per unit of maintenance cost.

- **Prediction**: any intelligence that develops under thermodynamic constraint will independently develop a language structurally isomorphic to mathematics.
- **Falsification condition**: an intelligent system developing under thermodynamic constraint whose causal-reasoning structure cannot be mapped onto any finite subset of a known mathematical formal system (graph theory, group theory, probability theory, topology, and so on); or, more operationally, a system whose informational compression efficiency is shown to fall significantly short of the asymptotically optimal compression rate achieved by known mathematical languages on equivalent tasks (that is, whose encoding length fails to approach the optimal encoding lower bound of the corresponding mathematical formal system as complexity grows). The mere fact that "this intelligence uses a symbolic system humans have never seen" is not, by itself, sufficient to falsify the hypothesis — so long as that symbolic system can be placed in structural isomorphism with a known mathematical formal system, the hypothesis stands.
- **Domain of applicability**: applies only to systems whose cognitive structure is subject to long-run energy-minimization pressure; it does not apply to systems whose energy budget is unconstrained.

---

## Chapter 5 — Extended Dynamics

### 5.0 The Fivefold Recursive Architecture (a Conceptual-Framework Placeholder)

> **A note on this section's status**: the fivefold recursive architecture is a **conceptual-framework placeholder** by which SRVD describes the evolution of active-phase systems; it offers a qualitative picture of how five core variables ($I, V, T, E, D$) couple to one another, rather than a rigorously derived set of dynamical equations. By contrast, the section on decoupling-deviation dynamics, below, already possesses a rigorous ordinary-differential-equation form with an explicit solution, and is the most mathematically solid part of this chapter. The reader should understand the discrete recursion equations of this section as **heuristic, discrete models awaiting rigorization**: their value lies in revealing the qualitative direction of the coupling and the existence of a phase transition, not in offering an exact functional form that can be fit directly to experimental data. The chapter's core argument is preserved in the two sections on the ontological mechanism of the threefold split and on decoupling-deviation dynamics; the remaining recursion equations in this section serve only as auxiliary, conceptual scaffolding.
>
> **A notational note**: equations (5.1)–(5.7) of this section are uniformly marked with the superscript $^\dagger$ (as in equation (5.1$^\dagger$)), so as to flag explicitly, within the numbering system itself, their epistemological status as "heuristic forms awaiting rigorization" — distinguishing them from equations (5.9)–(5.11) in the section on decoupling-deviation dynamics, which already possess rigorous, explicitly solved ordinary differential equations.

**A statement of the linearization assumption**: the fivefold recursion below assumes that the dominant coupling direction among the variables is unidirectional ($I \to V \to T \to E \to D$), corresponding to a scale separation of "fast drive, slow response" (fast–slow dynamics). Real systems may exhibit more complex, bidirectional feedback loops (for instance, the collapse of $T_{\mathrm{pred}}$ affecting both $V$ and $E$ simultaneously, while a surge in $E$ in turn compresses $T_{\mathrm{pred}}$). The complete, coupled system of ordinary differential equations is left as an open problem for a subsequent version. The current version retains a first-order, discrete-recursion approximation, offered for numerical illustration and qualitative discussion.

The fivefold recursion is the core mechanism by which SRVD describes the evolution of active-phase systems. Lower-order passive structures do not activate this architecture — their dynamics degenerate to a static estimate of the viability potential.

One possible discrete-recursion realization is given below.

#### 5.0.1 The $I$-Recursion (Informational Self-Amplification)

> **On the physical origin and phenomenological status of the coupling strength $\chi$**: the $\chi$ introduced in equation (5.1) is the core parameter driving the threefold split discussed later (see the section on the threefold split of the viability potential); its physical status is clarified here first, to prevent the reader from mistaking it for a sourceless, free tuning parameter. $\chi$ is not an external control knob on the system, but an intrinsic property of the structural characteristics of the decoder $D$ itself, phenomenologically characterizing the strength of the self-referential loop by which "a system uses feedback from its current viability state to accelerate its own information extraction." Intuitively, $\chi(D)$ should correlate positively with the decoder's **depth of self-referential loop** (the number of nested layers in the system's model — whether the system can predict "its own prediction about itself," and so on) and its **causal path length** (the number of loop segments information traverses from perception, to decision, to action): the deeper the loop and the longer the path, the stronger the leverage by which the system converts its current viability state into a future informational-extraction advantage, and the larger $\chi$ becomes. An organism possessing only a simple reflex arc, for instance, has $\chi$ near zero; a system possessing metacognitive capacity (the ability to model its own thought process) has a larger $\chi$. A complete microscopic derivation — one that would compute an analytic expression for $\chi$ directly from neural-circuit topology or model-architecture parameters — lies beyond the scope of this version and is left to future work (see the section on limitations, below); the current version treats $\chi$ as a **phenomenological parameter**, its value to be estimated inversely from a system's statistical behavior (such as the instability observed near the critical value $\chi_c$ in the section on the linear stability analysis of $\alpha_{\mathrm{eff}} > 2$, below), rather than derived from first principles.

$$
I_{\mathrm{net},n+1} = I_0 \left(1 + \chi \cdot V_{\mathrm{obj},n}\right)
\tag{5.1$^\dagger$}
$$

Here $I_0$ is the system's baseline $I_{\mathrm{net}}$ at $V = 0$, and $\chi$ is the **coupling strength**, with dimension $[V]^{-1}$ (that is, $\mathrm{J}/(\mathrm{bit}\cdot\mathrm{s})$), ensuring that $\chi V$ is dimensionless.

> **Delimiting the domain of validity (guarding against collapse to negative values)**: the linear form $I_0(1+\chi V_{\mathrm{obj},n})$ in equation (5.1) holds only within the active-viability domain $V_{\mathrm{obj},n} > 0$ — this is the premise of the scenario described under the heading "informational self-amplification": that the system is in a positive viability state, and its capacity for information extraction strengthens as that state improves. When $V_{\mathrm{obj},n} \leq 0$ (the system has already departed the normal viability trajectory; see the domain-of-validity partition of equation (3.1) in the section on the objective viability potential's two-channel superposition), equation (5.1) no longer applies, and should not be substituted directly to compute a negative or contradictory value of $I_{\mathrm{net}}$. In this regime the system has already entered a state of structural degradation or dissolution, and the evolution of $I_{\mathrm{net}}$ is instead governed jointly by the dissipative-runaway equation in the section on the $E$-recursion and by the damage term in the section on the objective viability potential's two-channel superposition; the self-amplification logic of this equation no longer applies. Should continuity and positivity be required across the full domain (including $V_{\mathrm{obj}} \leq 0$), an exponential form, $I_{\mathrm{net},n+1} = I_0 \exp(\chi V_{\mathrm{obj},n})$, may be used instead — this form asymptotically approaches zero, rather than turning negative, as $V_{\mathrm{obj},n} \to -\infty$, better matching the definitional requirement that net effective causal information should never be negative. The current version retains the linear form as a low-order approximation; the introduction of the exponential form is deferred to a later version, or left to future work.

**A dynamical reading**: a system's current state of structural viability feeds back into its decoder's efficiency of information extraction — the higher the structural stability and redundancy, the greater a system's capacity to maintain an increasingly complex predictive structure, which in turn raises the efficiency with which effective information is extracted. When the coupling strength $\chi$ grows too large, the endogenous virtual viability potential decouples from physical constraint, entering a state of nonlinear inflation, ultimately giving rise to the Myopic Runaway Regime.

#### 5.0.2 The $V$-Recursion (Updating the Viability Potential)

In the continuous-time limit, the evolution of the **objective viability stock** $V_{\mathrm{obj}}(t)$ is jointly governed by the viability drive rate $r_v = k \cdot V$, the baseline depreciation rate $\gamma_0$, and the environmental carrying capacity $V_{\mathrm{max}}$:

$$
\frac{\mathrm{d}V_{\mathrm{obj}}}{\mathrm{d}t} = V_{\mathrm{obj}} \cdot (r_v - \gamma_0) \cdot \left(1 - \frac{V_{\mathrm{obj}}}{V_{\mathrm{max}}}\right)
\tag{5.2$^\dagger$}
$$

Once thermodynamic dissipation breaches the dissolution threshold ($E_{\mathrm{thresh}}$), an irreversible damage term is triggered:

$$
\frac{\mathrm{d}V_{\mathrm{obj}}}{\mathrm{d}t} = V_{\mathrm{obj}} \cdot (r_v - \gamma_0) \cdot \left(1 - \frac{V_{\mathrm{obj}}}{V_{\mathrm{max}}}\right) - \delta \cdot V_{\mathrm{obj}} \cdot \mathbf{1}[E_{\mathrm{eff}} > E_{\mathrm{thresh}}]
\tag{5.3$^\dagger$}
$$

> **On the relation to equation (3.1) in the section on the objective viability potential's two-channel superposition (guarding against the misreading of "two separate criteria")**: equation (3.1) in that section presents $V_{\mathrm{obj}}$ as a piecewise state switch defined according to the range of $E_{\mathrm{eff}}$ (normal for $E_{\mathrm{eff}}\leq E_{\mathrm{thresh}}$, degradation for $E_{\mathrm{eff}}>E_{\mathrm{thresh}}$, dissolution for $E_{\mathrm{eff}}<E_{\mathrm{min}}$), whereas equation (5.3) here treats "exceeding the limit" as a continuous-time damage-rate term, $-\delta V_{\mathrm{obj}}\mathbf{1}[E_{\mathrm{eff}}>E_{\mathrm{thresh}}]$. These are not two independent physical models potentially yielding different verdicts, but **two expressions of the same physical process at different temporal resolutions**: equation (3.1) is a **piecewise, simplified schematic** of that process, describing which category of state a system occupies at a given moment — suited to static, cross-sectional analysis and to partitioning the domain of validity; equation (5.3) is its **continuous, dynamical version**, describing how damage accumulates over time once a state switch has occurred — suited to analyzing an evolutionary trajectory. Both trigger the same damage mechanism at the instant $E_{\mathrm{eff}}$ crosses $E_{\mathrm{thresh}}$, and the indicator $\mathbf{1}[E_{\mathrm{eff}}>E_{\mathrm{thresh}}]$ carries identical semantics in both equations. Equation (5.3) can be understood as the explicit, dynamical unfolding of the phrase "irreversible damage triggered (structural degradation)" in equation (3.1), rather than as a competing, alternative criterion.

> **A note on dimensions**: $V_{\mathrm{obj}}$ has units of $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$; $r_v$ is the viability-drive **rate**, with units of $\mathrm{s}^{-1}$ (that is, a relative growth rate per second). Writing $r_v = k V_{\mathrm{obj}}$ gives $k$ the dimension $\mathrm{J}/(\mathrm{bit}\cdot\mathrm{s}^2)$, ensuring $r_v$ carries the correct dimension of $\mathrm{s}^{-1}$. To avoid confusion, non-dimensionalization is recommended in computation: choosing a reference potential $V_{\mathrm{ref}}$ ($\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$) and a reference time $t_{\mathrm{ref}} = 1/(k V_{\mathrm{ref}})$ ($\mathrm{s}$), and setting $\tilde{V} = V_{\mathrm{obj}}/V_{\mathrm{ref}}$, $\tilde{t} = t/t_{\mathrm{ref}}$, equation (5.2) reduces to the dimensionless form $\mathrm{d}\tilde{V}/\mathrm{d}\tilde{t} = \tilde{V}(1 - \tilde{\gamma}_0)(1 - \tilde{V})$, where $\tilde{\gamma}_0 = \gamma_0 t_{\mathrm{ref}}$ is the dimensionless depreciation parameter. $V_{\mathrm{obj}}$ (a state quantity) and $r_v$ (a rate quantity) are not dimensionally interchangeable, even where their non-dimensionalized numerical forms happen to resemble one another; their physical meanings remain distinct.

**A note on the carrying-capacity ceiling $V_{\mathrm{max}}$**: $V_{\mathrm{max}}$ is not a carrying capacity in the ecological sense, but a thermodynamic ceiling: $V_{\mathrm{max}} \propto \dot{F}_{\mathrm{avail}} / \sigma_{\mathrm{min}}$, where $\dot{F}_{\mathrm{avail}}$ is the environment's available free-energy flux, and $\sigma_{\mathrm{min}}$ is the minimum entropy-production rate required to sustain the resource cycle of the niche. A system cannot sustain $V_{\mathrm{obj}} > V_{\mathrm{max}}$, because doing so would require extracting free energy at a rate exceeding the environment's capacity to replenish it — a thermodynamic impossibility, not a merely statistical limitation.

**A note on the saturated state**: a system enters a stable saturated state if and only if three conditions hold simultaneously: $E_{\mathrm{eff}} \geq E_{\mathrm{min}}$ (sufficient energy), $\rho \to 0$ (no competitive pressure), and $\Delta_{\mathrm{VV}} \to 0$ (the decoupling deviation vanishes). These conditions, together with the marginal criterion $r_v = \gamma_0$, jointly define the saturation manifold.

The discrete update form:

$$
V_{\mathrm{obj},n+1} = \frac{I_{\mathrm{struct}}\,T_{\mathrm{static}}}{E_{\mathrm{structure}}} + \frac{I_{\mathrm{net},n+1}\,T_{\mathrm{pred},n+1}}{E_{\mathrm{causal}}}
\tag{5.4$^\dagger$}
$$

#### 5.0.3 The $E$-Recursion (Two Modes of Runaway Thermodynamic Dissipation)

**Mode one: myopic dissipation surge (acute instability)**

When the endogenous time horizon $T_{\mathrm{pred}}$ collapses, a system loses its capacity for long-term planning, and turns instead to extracting extreme, short-term returns, causing its active energy flow $E_{\mathrm{flow}}$ to surge as $T_{\mathrm{pred}}$ shortens:

$$
E_{\mathrm{flow},n} = E_{\mathrm{structure}} + \dfrac{k_s}{T_{\mathrm{pred},n}}
\tag{5.5$^\dagger$}
$$

Here $k_s$ is the metabolic-sensitivity coefficient (dimension: $\mathrm{J}\cdot\mathrm{s}$). This inverse function is linear with respect to $T_{\mathrm{pred}}^{-1}$, but it is a **convex function with respect to $T_{\mathrm{pred}}$ itself** — this convexity is exactly the frame of reference behind the phrase "super-linear growth": as $T_{\mathrm{pred}}$ shortens, $E_{\mathrm{flow}}$ displays an **inverse, accelerating growth** (that is, an identical decrement $\Delta T_{\mathrm{pred}}$ produces a far larger increment in $E_{\mathrm{flow}}$ when $T_{\mathrm{pred}}$ is already small than when it is large), a fact that can be verified explicitly via the second-derivative test: $\partial^2 E_{\mathrm{flow}}/\partial T_{\mathrm{pred}}^2 = 2k_s/T_{\mathrm{pred}}^3 > 0$, confirming convexity — the faster the horizon shortens, and the closer it approaches $T_{\mathrm{min}}$, the more violent the energy surge. This inverse function attains a finite ceiling, $E_{\mathrm{flow},\max} = E_{\mathrm{structure}} + k_s/T_{\mathrm{min}}$, at $T_{\mathrm{pred}} = T_{\mathrm{min}} > 0$. Equation (5.5) contains no mathematical singularity: the physical lower bound $T_{\mathrm{min}} > 0$ of $T_{\mathrm{pred}}$ guarantees that $E_{\mathrm{flow}}$ remains bounded throughout. The danger of the energy surge lies not in divergence, but in the possibility that $E_{\mathrm{flow},\max}$ breaches the dissolution threshold $E_{\mathrm{thresh}}$, triggering the irreversible damage term in equation (5.3).

**Mode two: meta-level dissipation (chronic damping)**

To sustain itself, a system evolves a supervisory module — but "how to conserve energy" is itself a question that consumes energy, producing meta-level dissipation, $E_{\mathrm{total}} = E_{\mathrm{base}} + E_{\mathrm{meta}}(E_{\mathrm{pred}})$. Infinite nesting of the supervisory layer causes $E_{\mathrm{meta}}$ to diverge exponentially, consuming free energy. This explains bureaucratic inertia in large organizations, and computational deadlock in systems.

#### 5.0.4 The $T$-Recursion (Self-Fulfillment of the Endogenous Time Horizon)

$$
T_{\mathrm{pred},n+1} = \max\!\left(T_{\mathrm{min}},\; \dfrac{T_0}{1 + \lambda(\chi V_{\mathrm{obj},n})^2}\right)
\tag{5.6$^\dagger$}
$$

> **A note on dimensions**: $\chi V_{\mathrm{obj},n}$ is already dimensionless ($\chi$ has dimension $\mathrm{J}/(\mathrm{bit}\cdot\mathrm{s})$, $V_{\mathrm{obj}}$ has dimension $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$, and their product is dimensionless); $\lambda$ is likewise a **dimensionless positive real number**, functioning as a compression-strength regulator — the larger $\lambda > 0$ is, the more violently a given fluctuation in $\chi V_{\mathrm{obj}}$ collapses the horizon. $T_0$ has dimension $\mathrm{s}$, consistent with $T_{\mathrm{pred}}$. Equation (5.6) is dimensionally self-consistent.

**Feed-forward regulation (long-term investment)**: when the endogenous time horizon is wide, a system tends to invest its current thermodynamic dissipation into infrastructure-building, thereby raising $I_{\mathrm{latent}}$.

**Reverse phase transition (collapse of the endogenous time horizon)**: this has two sources — (1) **runaway internal positive feedback**: a high $\chi$ causes the virtual viability potential to inflate, and the system spontaneously slips into short-sightedness; (2) **an external negative-value shock**: an $I^-$ event directly compresses the time horizon, triggering a surge in defensive dissipation.

The quadratic compression form is chosen because it captures the qualitative feature of super-linear horizon collapse as recursive amplification increases; the qualitative conclusions (the existence of a phase transition, an early-warning window) depend only on the monotonicity of this compression, not on the specific functional form.

#### 5.0.5 The $D$-Recursion (Decoder Evolution — a Gradient-Drift Form)

The evolution of the decoder is described as a competition between an ascending informational gradient and a descending energetic-cost gradient:

$$
D_{n+1} = D_n + \epsilon \left( \nabla_\Theta I_{\mathrm{net}} - k_D \nabla_\Theta E_{\mathrm{causal}} \right)
\tag{5.7$^\dagger$}
$$

Here $\Theta$ is the parameter space of the given system type, $\epsilon$ is the learning rate (the evolutionary step size), and $k_D$ is the energy-cost penalty coefficient (dimension $\mathrm{J}^{-1}$, so that $k_D \nabla E_{\mathrm{causal}}$ is dimensionless).

| System type | Instances of the parameter space $\Theta$ |
|:---|:---|
| Neural network | Weight matrices $w_{ij}$, biases $b_i$, architectural hyperparameters |
| Biological system | Gene-expression levels, neural-connection strengths, synaptic-plasticity parameters |
| Social organization | Resource-allocation ratios, institutional rule parameters, power-structure variables |

This framework does not predefine the concrete structure of $\Theta$; whoever applies it must supply the specific dimensions of the parameter space and the measurement protocol appropriate to the system type under study.

The pathways of decoder evolution include: **decoder drift** (smooth adjustment via gradient ascent/descent, as in learning and adaptation); and **topological transition** (a paradigm-revolutionary reconstruction of structure, corresponding to the injection of $I_{\mathrm{orig}}$ triggering the topological-expansion operator $\mathcal{T}(I_{\mathrm{orig}})$, such that $I_{\mathrm{max}}(D_{n+1}) > I_{\mathrm{max}}(D_n)$).

---

### 5.1 The Threefold Split of the Viability Potential: The Internal Structure of the $V$-Family, and the Physical Basis of Emotion

#### 5.1.1 Unity in Lower-Order Structures

In lower-order physical structures, time is an exogenous coordinate parameter that the system cannot endogenously intervene upon; there is no independent module for prediction or for value, and the three terms merge into a single number:

$$
\text{Lower-order structures:}\; V_{\mathrm{obj}} = V^{\mathrm{virt}} = V^{\mathrm{val}} = V
\tag{5.1a}
$$

#### 5.1.2 The Endogenization of $T$: The Physical Trigger of the Threefold Split

Once $T_{\mathrm{pred}}$ emerges, the previously unified viability potential fractures into three variables belonging to the same family, but with sharply different functions and constraints:

1. **The objective viability potential ($V_{\mathrm{obj}}(D)$)**: the true, integrated strength of viability of any given PS under a given decoder $D$. This is the real value in the physical world, strictly bound by the boundary of thermodynamic dissipation — it cannot be deceived, and it cannot be borrowed against across time. When $D = D_{\mathrm{self}}$, that is, when it is the system's true viability potential under its own decoder, $V_{\mathrm{obj}}(D_{\mathrm{self}})$, it serves as the sole physical point of reference for every viability-potential variable. "Objective," here, does not mean some absolute, bare value detached from every decoder — it means that, once a given decoder $D$ and given physical boundary conditions are fixed, the PS's strength of viability is adjudicated jointly by its actual causal effects, its energetic cost, and time, and is not subject to the system's own subjective estimation.

2. **The virtual viability potential ($V^{\mathrm{virt}}$)**: a system's subjective estimate of $V_{\mathrm{obj}}(D_{\mathrm{self}})$. $V^{\mathrm{virt}}$ is the system's internal predictive model; its function is to estimate the system's own true viability potential under its own decoder, so as to supply a basis for decision-making.

3. **The value viability potential ($V^{\mathrm{val}}$)**: the objective function of a higher-order persistent structure's (PS's) behavioral system. It specifies which PS's $V_{\mathrm{obj}}$ the system will allocate its finite $E_{\mathrm{eff}}$ toward, thereby determining the direction of its behavioral optimization.

   Under normal circumstances, $V^{\mathrm{val}}$ is anchored to the system's own $V_{\mathrm{obj}}(D_{\mathrm{self}})$. Because the system cannot directly observe $V_{\mathrm{obj}}$, it can only estimate it through $V^{\mathrm{virt}}$ and make decisions on that basis. When decoder drift occurs, $V^{\mathrm{val}}$ can become re-anchored to the $V_{\mathrm{obj}}$ of some other PS.

**A comparative table of the $V$-family's definitions:**

| Variable | Definition | Function |
| :--- | :--- | :--- |
| $V_{\mathrm{obj}}(D)$ | The true, integrated strength of viability of any given PS under a given decoder $D$ (under the system's own decoder, $V_{\mathrm{obj}}(D_{\mathrm{self}})$) | The sole physical point of reference |
| $V^{\mathrm{virt}}$ | The system's subjective estimate of $V_{\mathrm{obj}}(D_{\mathrm{self}})$ | The internal predictive model, estimating the system's own true viability potential |
| $V^{\mathrm{val}}$ | The objective function the system actually optimizes | The behavioral interface, determining the direction of $E_{\mathrm{eff}}$ allocation |

**The principle of viability-potential selection:**

Every PS, under a given constraint, is subject to selection by viability potential: structures with a higher $V_{\mathrm{obj}}$ are, in a statistical sense, more likely to be maintained, to expand, or to be replicated. Lower-order structures do not actively maximize $V_{\mathrm{obj}}$; they passively submit to thermodynamic and environmental selection. Higher-order structures, by contrast, predict the future state of their own $V_{\mathrm{obj}}(D_{\mathrm{self}})$ through $V^{\mathrm{virt}}$, and select the objective of behavioral optimization through $V^{\mathrm{val}}$. In the overwhelming majority of cases, $V^{\mathrm{val}}$ remains anchored to the system's own $V_{\mathrm{obj}}$; in a minority of cases, owing to decoder drift, a system will redirect its optimization objective toward the $V_{\mathrm{obj}}$ of some other PS.

**An ontological clarification:**

The threefold split is not a splitting of $V$ into three independent entities, but three internal relations that an active-phase system builds around one and the same $V_{\mathrm{obj}}$: an objective state ($V_{\mathrm{obj}}$, adjudicated by physics), a predictive representation ($V^{\mathrm{virt}}$, an internal estimate), and an optimization objective ($V^{\mathrm{val}}$, the behavioral interface). $V^{\mathrm{virt}}$ and $V^{\mathrm{val}}$ do not constitute new physical quantities independent of $V_{\mathrm{obj}}$; they are the internal computational structure of a higher-order PS.

**Passive decoupling and active decoupling:**

Define the predictive error $\Delta_{\mathrm{VV}} \equiv V^{\mathrm{virt}} - V_{\mathrm{obj}}(D_{\mathrm{self}})$. When $\Delta_{\mathrm{VV}} \neq 0$, a system's internal estimate of its own strength of viability diverges from physical reality — this is termed **passive decoupling**. Distinct from this, when the object to which $V^{\mathrm{val}}$ is anchored shifts from the system's own $V_{\mathrm{obj}}(D_{\mathrm{self}})$ to the $V_{\mathrm{obj}}$ of some other PS, the system has actively changed its behavioral optimization objective — this is termed **active decoupling**.

**The physical basis of emotion:**

In the dynamical sense given by SRVD, the object to which $V^{\mathrm{val}}$ is anchored constitutes the physical basis of complex emotion. When it remains anchored chiefly to the system's own $V_{\mathrm{obj}}$, this manifests as self-interested self-maintenance; when a system voluntarily allocates its own resources toward gains in the $V_{\mathrm{obj}}$ of another PS, this can be characterized as "love"; when such an anchoring is imposed externally by force, and continually suppresses the system's own $V_{\mathrm{obj}}$, this can be characterized as "enslavement." All of these emotions are phenomena exclusive to the dynamics that emerge once $T_{\mathrm{pred}}$ has arisen, and depend on a system's capacity to predict and attribute causal relations.

$V^{\mathrm{virt}}$ and $V^{\mathrm{val}}$ together constitute the spatiotemporal causal-arbitrage channel of a higher-order intelligent PS: the predictive layer ($V^{\mathrm{virt}}$) is responsible for identifying the possible future trajectory of $V_{\mathrm{obj}}$; the value layer ($V^{\mathrm{val}}$) is responsible for allocating the current $E_{\mathrm{eff}}$ toward whichever behavioral pathway is expected to maximize the gain in $V_{\mathrm{obj}}$ of the anchored PS. Working together, the two allow a system to sacrifice its current $E_{\mathrm{eff}}$ in exchange for a future gain in $V_{\mathrm{obj}}$, whether its own or another's.

Hatred begins with a negative-value attribution within the $V^{\mathrm{virt}}$ channel: the system identifies some PS as a source of $I^-$ against itself or against the object to which it is anchored. This $I^-$ includes not only threats that may occur in the future, but also harm already inflicted in the past. Even once the system has become externally decoupled from that PS in terms of causal interaction, so long as that negative-value memory persists within its internal model, the PS will continue to be retained as an unsettled source of negative causal effect. Only once $V^{\mathrm{val}}$ further authorizes the allocation of $E_{\mathrm{eff}}$ toward behavioral pathways of suppression, exclusion, punishment, or retaliation against that PS does hatred constitute a complete dynamical structure. Revenge, then, is not merely a defensive act, but a cross-temporal behavior by which the system attempts to close the causal loop on an $I^-$ event that has already occurred — repairing it, releasing a deterrent signal, or reconstructing its own boundary. Unlike fear, whose core is the avoidance of a future $I^-$ in order to protect the system's own $V_{\mathrm{obj}}$, the core of hatred is the settling of accounts with an already-identified source of negative causal effect, whether or not that source still constitutes a live threat. In SRVD, then, hatred is not an emotional state, but a persistent resource-allocation strategy following the completion of a negative anchoring of $V^{\mathrm{val}}$: so long as that anchoring is not released, the system may continue to invest $E_{\mathrm{eff}}$ in settling accounts with that negative causal source, even after the external threat has long since disappeared.

---

#### 5.1.3 Linear Stability Analysis of $\alpha_{\mathrm{eff}} > 2$

When the coupling strength $\chi$ exceeds a critical value $\chi_c$, the higher-order feedback of the $I$–$V$ closed loop causes the effective expansion index $\alpha_{\mathrm{eff}}$ to become, dynamically and self-consistently, greater than 2; super-linear self-referential inflation then dominates the inverse-square collapse of the time horizon, and the predicted value $V^{\mathrm{virt}}$ departs entirely from objective physical constraint:

> **A sketch of the derivation (the origin of equation (5.8))**: continualizing the discrete recursions of equations (5.1$^\dagger$) and (5.2$^\dagger$) yields a two-dimensional autonomous system for the $I$–$V$ closed loop:
>$$
> \dot I = \chi \cdot I \cdot V, \qquad \dot V = k \cdot I^{\,\alpha_{\mathrm{eff}}} \cdot V^{-1} - \gamma_0 \cdot V
> \tag{5.7a}
> $$
>
>The first equation is the differential form, in the continuous-time limit, of equation (5.1$^\dagger$) ($I_{\mathrm{net},n+1}=I_0(1+\chi V_{\mathrm{obj},n})$); the second is a power-law generalization of equation (5.2$^\dagger$), retaining the original linear depreciation term $-\gamma_0 V$ while replacing the drive rate $r_v$ with a dependence on $I$ raised to the power $\alpha_{\mathrm{eff}}$ (that is, $\alpha_{\mathrm{eff}}=\partial\ln I/\partial\ln V|_{V^*}$, defined locally near the steady state). Introducing logarithmic coordinates $i=\ln(I/I^*)$ and $v=\ln(V/V^*)$, and linearizing near the fixed point $(I^*,V^*)$ (where the steady-state condition is either $\chi V^*=0$ or $k(I^*)^{\alpha_{\mathrm{eff}}-1}=\gamma_0(V^*)^2$), the Jacobian matrix is:
>
>$$
> J = \begin{pmatrix} \partial \dot i/\partial i & \partial \dot i/\partial v \\ \partial \dot v/\partial i & \partial \dot v/\partial v \end{pmatrix}_{(i,v)=(0,0)} = \begin{pmatrix} 0 & \tilde\chi \\ (\alpha_{\mathrm{eff}}-1)\tilde\chi & -2\tilde\chi-\tilde\gamma_0 \end{pmatrix}
> \tag{5.7b}
> $$
>
>where $\tilde\chi$ and $\tilde\gamma_0$ are the non-dimensionalized coupling strength and depreciation rate, taken at the steady-state values. The characteristic equation of $J$ reduces to $\mu^2+(2\tilde\chi+\tilde\gamma_0)\mu-(\alpha_{\mathrm{eff}}-2)\tilde\chi(-\tilde\chi)=0$; taking the dominant eigenvalue under the scale relation $\tilde\chi\ll\tilde\gamma_0$ gives the approximate expression in equation (5.8), $\lambda_J\approx(\alpha_{\mathrm{eff}}-2)\tilde\chi-\tilde\gamma_0$. The complete solution of the quadratic characteristic equation (including the subdominant eigenvalue and the oscillation criterion) is left to subsequent, more rigorous work (see the section on the summary of extended dynamics and open problems, below); this version offers only the approximate closed-form solution for the dominant eigenvalue, sufficient to support the directional criterion for the triggering of the threefold split.

Performing a logarithmic linearization near the steady state $V^*$, setting $v = \ln(V/V^*)$, and defining the effective expansion index $\alpha_{\mathrm{eff}} = \left.\partial \ln I / \partial \ln V\right|_{V^*}$, the dominant eigenvalue of the Jacobian is:

$$
\lambda_J = (\alpha_{\mathrm{eff}} - 2)\cdot\tilde{\chi} - \tilde{\gamma}_0
\tag{5.8$^\dagger$}
$$

When $\chi > \chi_c = \tilde{\gamma}_0 / (\alpha_{\mathrm{eff}} - 2)$, $\lambda_J > 0$, and self-referential inflation diverges exponentially from the objective viability potential along the unstable manifold.

**The triggering proposition for the threefold split (a single Jacobian criterion)**: the endogenization of $T_{\mathrm{pred}}$ (that is, the system possesses a cognitive decoder, such that $T_{\mathrm{pred}}$ becomes a state variable regulable by the system itself, rather than an exogenous parameter) is a **necessary condition** for the threefold split — in lower-order systems that fail to satisfy this condition, $V_{\mathrm{obj}}=V^{\mathrm{virt}}=V^{\mathrm{val}}$ holds identically (see the earlier section on unity in lower-order structures), and the threefold split simply does not arise. Given that $T_{\mathrm{pred}}$ has already been endogenized, whether the threefold split is actually **triggered** is determined by the single Jacobian stability criterion of equation (5.8$^\dagger$): when $\lambda_J = (\alpha_{\mathrm{eff}}-2)\tilde\chi - \tilde\gamma_0 > 0$ (equivalently, when the coupling strength $\chi$ exceeds the critical value $\chi_c = \tilde\gamma_0/(\alpha_{\mathrm{eff}}-2)$, defined in terms of $\alpha_{\mathrm{eff}}$), self-referential inflation diverges exponentially from the objective viability potential along the unstable manifold, and the threefold split enters an irreversible stage.

> **Clarifying the relation between "$\chi>\chi_c$" and "$\alpha_{\mathrm{eff}}>2$"**: an earlier formulation listed "$\chi>\chi_c$" and "$\alpha_{\mathrm{eff}}>2$" as two parallel, independent sufficient conditions; but the definition $\chi_c=\tilde\gamma_0/(\alpha_{\mathrm{eff}}-2)$ shows that $\chi_c$ is itself a function of $\alpha_{\mathrm{eff}}$ — absent $\alpha_{\mathrm{eff}}>2$ (otherwise the denominator of $\chi_c$ is non-positive, and the critical value is either meaningless or negative), the condition "$\chi>\chi_c$" cannot itself hold. The two are not independent criteria but two facets of the same critical event, $\lambda_J>0$: $\alpha_{\mathrm{eff}}>2$ is the precondition for $\chi_c$ to be meaningful, and $\chi>\chi_c$ is the specific triggering threshold given that precondition. This version has merged them into a single Jacobian criterion, to avoid double-counting.

> **A conceptual clarification**: this section uses two exponent symbols belonging to different conceptual levels, which must be strictly distinguished and never conflated —
> - **$\alpha$** (the informational elasticity exponent): the structure's **intrinsic weighting parameter** for informational resources, defined in the section on elasticity exponents and the core ordering proposition, derived from thermodynamic first principles, satisfying $\alpha > 1$.
> - **$\alpha_{\mathrm{eff}}$** (the effective expansion index): the closed-loop feedback quantity defined in this section, an **emergent effective response** arising from the self-referential coupling of $I$ and $V$; when the coupling strength $\chi > \chi_c$, $\alpha_{\mathrm{eff}}$ can dynamically exceed 2.
>
> The two operate at different levels: $\alpha$ is a structure's **intrinsic preference parameter** under a given decoder, whereas $\alpha_{\mathrm{eff}}$ is the closed-loop dynamics' **local effective response** near the steady state. $\alpha_{\mathrm{eff}} > 2$ must not be read as implying $\alpha$ itself exceeds 2, nor should the ordering proposition $\alpha > 1$ be conflated with the instability condition $\alpha_{\mathrm{eff}} > 2$.

---

### 5.2 Decoupling-Deviation Dynamics

$\Delta_{VV} = |V^{\mathrm{virt}} - V_{\mathrm{obj}}|$ is a **predictive error** (the gap between the output of the predictive layer and the true, objective value). $V^{\mathrm{virt}}$ is an estimate of $V_{\mathrm{obj}}$, and the gap between the two reflects the deviation between a system's cognitive model and physical reality.

The evolution of the decoupling deviation $\Delta_{\mathrm{VV}} = |V^{\mathrm{virt}} - V_{\mathrm{obj}}|$ is governed by the learning rate $\alpha_L$ and the environmental noise intensity $\sigma$:

$$
\boxed{
\frac{\mathrm{d}\Delta_{\mathrm{VV}}}{\mathrm{d}t} = -\alpha_L \cdot I_{\mathrm{net}} \cdot \Delta_{\mathrm{VV}} + \sigma
}
\tag{5.9}
$$

> **A note on dimensions**: $\Delta_{\mathrm{VV}}$ has units of $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$; $\alpha_L$ is the learning rate, with units of $\mathrm{bit}^{-1}\mathrm{s}^{-1}$; $\sigma$ is the noise intensity, with units of $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J} \cdot \mathrm{s}^{-1} = \mathrm{bit}/\mathrm{J}$; and $I_{\mathrm{net}}$ has units of $\mathrm{bit}$.

Treating $I_{\mathrm{net}}$ as constant, this equation admits a strict, explicit solution:

$$
\Delta_{\mathrm{VV}}(t) = \frac{\sigma}{\alpha_L I_{\mathrm{net}}} + \left(\Delta_0 - \frac{\sigma}{\alpha_L I_{\mathrm{net}}}\right) e^{-\alpha_L I_{\mathrm{net}} t}
\tag{5.10}
$$

From which the equilibrium deviation and the critical informational threshold follow:

$$
\Delta_{\mathrm{VV}}^* = \frac{\sigma}{\alpha_L I_{\mathrm{net}}}, \qquad I_{\mathrm{crit}} = \frac{\sigma}{\alpha_L}
\tag{5.11}
$$

**A physical reading**:

- When $I_{\mathrm{net}} < I_{\mathrm{crit}}$, the cognitive deviation cannot converge; the system loses, cognitively, an accurate model of its environment, and the growth of its effective viability potential is constrained;
- When $I_{\mathrm{net}} > I_{\mathrm{crit}}$, the sustained information flow suffices to suppress environmental noise, and the subjective assessment approaches objective reality exponentially over time ($\Delta_{\mathrm{VV}} \to \Delta_{\mathrm{VV}}^*$);
- The equilibrium deviation $\Delta_{\mathrm{VV}}^* = \sigma / (\alpha_L I_{\mathrm{net}})$ reflects a fundamental limit: no learner, however good, can fully overcome environmental noise.

The origin of the initial value $\Delta_0$: a newly formed system (with a cognitive model that is nearly blank) has a large $\Delta_0$; a mature system has a smaller $\Delta_0$; and following a paradigm shock ($\Delta_0$ jumps abruptly, as the previous model fails).

This ordinary differential equation constitutes the only fully closed-form continuous dynamical equation in SRVD v7.8, and can be used directly for empirical testing.

**A note on empirical application**: what equation (5.10) predicts is the evolutionary trend of $\Delta_{\mathrm{VV}}$, not the absolute value of $V^{\mathrm{virt}}$. In empirical testing (Appendix E.1, P4), the early-warning signal is triggered by the joint criterion $\frac{d\Delta_{\mathrm{VV}}}{dt} > 0$ together with the collapse of $T_{\mathrm{pred}}$, with no need to presuppose an absolute value of $V_{\mathrm{obj}}$ as a benchmark.

---

### 5.3 The Myopic Runaway Regime: A Collapsing Causal Chain

The Myopic Runaway Regime is the dynamical, self-consuming process by which a system continually depletes its objective viability potential in order to sustain an extreme value of its virtual viability potential. The path from decoupling at the latent layer to the destruction of physical stock follows a strict sequence:

$$
V^{\mathrm{virt}}\uparrow \;\xrightarrow{(1)}\; r_v^{\mathrm{virt}}\uparrow \;\xrightarrow{(2)}\; V^{\mathrm{val}}\text{ hijacked} \;\xrightarrow{(3)}\; E_{\mathrm{eff}}\uparrow \;\xrightarrow{(4)}\; V_{\mathrm{obj}}\text{ deteriorates} \;\xrightarrow{(5)}\; V_{\mathrm{obj}}\to 0
\tag{5.3a}
$$

1. **Inflation of the virtual potential**: a high $\chi$ activates the $I$–$V$ closed loop; $I_{\mathrm{net}}$ grows while $T_{\mathrm{pred}}$ collapses;
2. **Surge in the drive rate**: the inflated virtual potential maps onto an inflated growth-rate signal;
3. **The value objective is hijacked**: the behavioral interface optimizes the virtual signal rather than the objective potential; $E_{\mathrm{eff}}$ is poured into the self-referential loop;
4. **Deterioration of the objective potential**: $E_{\mathrm{eff}}$ rises as $T_{\mathrm{pred}} \to T_{\mathrm{min}}$, squeezing the objective assessment $V_{\mathrm{obj}} = I_{\mathrm{net}}(D) \cdot T_{\mathrm{actual}}/E_{\mathrm{eff}}$ from both ends;
5. **Collapse of physical stock**: $E_{\mathrm{eff}} > E_{\mathrm{thresh}}$ is triggered, the damage term dominates, and accumulated stock is irreversibly destroyed.

**A critical asymmetry**: steps (1) through (3) occur at the **latent (assessment) layer**, incurring no physical cost; step (5) is irreversible. The system burns real structure in pursuit of an internal illusion.

The value-objective layer ($V^{\mathrm{val}}$) never counts self-destruction as a loss, because what it computes over is the virtual viability potential, not the objective one. This explains why higher-order intelligent agents can display the resolve to "sacrifice themselves in exchange for a short-term extraction of return."

> **A clarification**: the "inflation of the virtual potential" within the Myopic Runaway Regime is, in essence, an inflation of a predicted value — the system's internal estimate of $V_{\mathrm{obj}}$ persistently exceeds its actual value, causing the behavioral interface ($V^{\mathrm{val}}$) to make optimizing decisions based on a mistaken prediction. Once the predictive deviation grows large enough, the system begins consuming its real $V_{\mathrm{obj}}$ in order to sustain a predicted value that can never actually be realized, forming a self-consuming loop. The value layer is hijacked not because $V^{\mathrm{virt}}$ is some independent viability potential in its own right, but because the predictive layer persistently outputs a positive bias that the value layer has no means of recognizing.

---

### 5.4 Competitive Dynamics and Lock-In States

In a multi-agent environment, an individual's viability potential does not evolve in isolation, but is jointly shaped by competitive pressure $\rho$ (defined as the average dissipation of competing systems within the same niche, divided by the total available free energy). When $\rho > 0$, the symmetric Nash equilibrium is forced to satisfy $r_{v,eq} = \gamma_0 + \lambda(\rho) > \gamma_0$ — every agent is pushed into a state of permanent under-saturation, regardless of individual preference, and none can reach the dormant optimum.

> **The minimal properties required of $\lambda(\rho)$**: this version does not specify a concrete functional form for $\lambda(\rho)$ in advance (linear, power-law, or otherwise), but requires it to satisfy two minimal properties, to guarantee the directional validity of the conclusion above: (1) $\lambda(0)=0$ — absent competitive pressure, the equation reduces to the single-agent optimum $r_{v,eq}=\gamma_0$; (2) $\lambda'(\rho)>0$ — the greater the competitive pressure, the more monotonically the equilibrium departs from the dormant optimum. These two properties are sufficient to support this section's qualitative conclusion that "when $\rho>0$, every agent is pushed into permanent under-saturation," but not yet sufficient to determine a specific symmetric Nash-equilibrium solution; the complete game-theoretic assumptions (symmetry, continuity of the strategy space, the concrete form of the payoff function) and the analytic derivation of $\lambda(\rho)$ are left to future work (see the section on the summary of extended dynamics and open problems, below); this version offers only a qualitative argument based on the two minimal properties above.

**A classification of lock-in states**: when a system falls into an extreme bias along some dimension, it may enter a thermodynamic lock-in state: investment along that dimension continues to rise while effective output stalls, and overall viability potential declines.

| Type of lock-in | Principal symptom | SRVD diagnostic criterion | Typical example |
|:---|:---|:---|:---|
| **$E$-lock-in** | Energy expenditure surges with no gain in output | $E_{\mathrm{causal}}$ continually rises while $\Delta I_{\mathrm{net}} \to 0$ | Arms races, self-consuming bureaucracies |
| **$I$-lock-in** | Informational diversity collapses; homogenization | The effective dimension of $I_{\mathrm{net}}$ declines, $\nabla I \to 0$ | Thought censorship, algorithmic information cocoons |
| **$T$-lock-in** | The time horizon collapses; extreme short-termism | $T_{\mathrm{pred}} \to T_{\mathrm{min}}$, no long-term planning | High-frequency trading, quarter-driven management |
| **$D$-lock-in** | The decoder's paradigm ossifies, unable to adapt to a new environment | The decoder gradient $\nabla D \to 0$, refusal to admit $I_{\mathrm{orig}}$ injection | Institutional rigidity, closed paradigms |

**The dynamical mechanism of $D$-lock-in**: the upgrading of a decoder is constrained by its construction cost, $E_{\mathrm{build}}$. The transition from $D_n$ to $D_{n+1}$ requires paying a one-time construction cost, in exchange for a higher decoding efficiency $\eta_D$ or a broader state-space capacity $I_{\mathrm{max}}(D)$. When $E_{\mathrm{build}} > E_{\mathrm{available}}$, a system enters a $D$-lock-in state: the decoder's topological space ceases to expand, and its capacity for information extraction is locked in place by the current energy budget. Human civilization's systematic blindness to the non-visible portions of the electromagnetic spectrum, prior to the advent of the radio telescope, is a typical historical case of $D$-lock-in — it was the physical limitation of the decoder's implementation, not the non-existence of the information itself, that bounded the extractable $I_{\mathrm{net}}$. Breaking out of this state requires either the emergence of a new energy paradigm (raising $E_{\mathrm{available}}$) or a fundamental reconstruction of the decoder's architecture (the injection of $I_{\mathrm{orig}}$ triggering a $\mathcal{T}$-transition) — neither is sufficient on its own.

**Diagnostic tools**:

- **Cognitive processing rate**, $\mathcal{R}_e = I_{\mathrm{net}} / T_{\mathrm{pred}}$ ($\mathrm{bit}/\mathrm{s}$): the effective informational output per unit of subjective time; a sustained decline signals that a system is approaching some form of lock-in.
- **Cognitive lag coefficient**, $\mathcal{L}_e = T_{\mathrm{pred}} / I_{\mathrm{net}} = 1/\mathcal{R}_e$ ($\mathrm{s}/\mathrm{bit}$): the time cost required to produce a unit of effective information; the core criterion for a lock-in state is $\mathcal{L}_e \to \infty$.

**The lock-in criterion**: when a system continually consumes $E_{\mathrm{eff}}$ while $\mathcal{R}_e \to 0$, the system has entered a **thermodynamic idling lock-in state**: every additional unit of investment converts entirely into entropic dissipation, generating no structural gain.

**Paths out of lock-in**:

| Type of lock-in | Path out | SRVD mechanism |
|:---|:---|:---|
| $E$-lock-in | Cut non-productive energy expenditure; redirect the budget toward cognitive expansion | Reduce the share of defensive expenditure within $E_{\mathrm{causal}}$ |
| $I$-lock-in | Introduce external diversity; break informational homogenization | Inject $I^+$, reactivating $\nabla I$ |
| $T$-lock-in | Extend the planning horizon; suppress short-term impulses | Increase $T_{\mathrm{pred}}$, lower the discount rate |
| $D$-lock-in | A paradigm breakthrough; reconstruct the decoder | Pay $E_{\mathrm{build}}$, trigger a $\mathcal{T}(I_{\mathrm{orig}})$ transition |

The complete game-theoretic formalization of lock-in states (the competitive-exclusion coefficient, the partial differential equations of a multi-agent flow field, the strict inequalities governing transition decisions) belongs to the scope of future work; this version offers a classificatory framework and a set of diagnostic criteria built on SRVD's core variables.

---

### 5.5 A Summary of Extended Dynamics, and Open Problems

- **The section on decoupling-deviation dynamics** already possesses a rigorous ordinary-differential-equation form with an explicit solution, and can be used directly for empirical testing;
- **The section on the fivefold recursive architecture** and **the section on the threefold split of the viability potential** offer an evolvable, placeholder framework, whose concrete functional forms are left to be filled in once the system type is fixed;
- **The section on the Myopic Runaway Regime** and **the section on competitive dynamics and lock-in states** offer a diagnostic framework built on the four dimensions $E/I/T/D$.

The following belong to subsequent versions (v10.0+) or to branch lines of work, as open problems: the continualization and stability analysis of the fivefold recursion (including bidirectional coupling); the complete equations of decoder evolution (including strict threshold conditions for topological transition); the mathematical formalization of a multi-agent competitive flow field (including the analytic derivation of the competitive pressure $\lambda(\rho)$ in the section on competitive dynamics and lock-in states, and the complete game-theoretic assumptions behind the symmetric Nash equilibrium); the pathological phase-transition dynamics of the value weights $w_s, w_c$; the microscopic derivation of the coupling strength $\chi$ (computed directly from the decoder's topological parameters, see the footnote in the earlier section on the $I$-recursion); and the dynamical coupling with the Landauer–Bremermann constraint. Every other mention of "future work" elsewhere in this chapter's body text has been folded into this list, and is not repeated at each individual occurrence.

---

### 5.6 The Precise Mathematical Conditions of the Four Global Attractors

Based on $\lim_{t \to \infty} \Theta(t)$, a system's trajectory converges uniquely to one of the following:

| Attractor | Mathematical condition on the limiting domain | Dynamical outcome (from the perspective of energy transfer) |
|:---|:---|:---|
| **The saturation attractor** | $\inf E_{\mathrm{total}} > c > 0$, $\rho \to 0$, $\Delta_{\mathrm{VV}} \to 0$, $\sup T_{\mathrm{max}} < \infty$ | $V(t) \to V_{\mathrm{max}}$ (energy transfer reaches a dynamic equilibrium; the channel is stable) |
| **The collapsing manifold** | $\rho \gg 0$, $\Delta_{\mathrm{VV}} > 0$, $E_{\mathrm{total}} < \infty$ | $r_v > \gamma_0$ is truncated, $dV/dt \ll 0$ (the channel collapses; energy returns to the thermal reservoir) |
| **The topological transition** | $T_{\mathrm{max}} \to \infty$ or $I_{\mathrm{max}} \to \infty$ (the operator $\mathcal{T}$ is triggered) | $dV_{\mathrm{max}}/dt > 0$ (the channel undergoes a phase transition; bandwidth jumps) |
| **The metric replacement** | $\Delta_{\mathrm{VV}} \gg 0 \Rightarrow D \to D'$ | Under the original measure $V \to 0$, while the new measure $D'$ comes to dominate the flow field (the old channel is abandoned; a new channel takes over) |

---

### 5.7 The Complete System of Inequality Constraints (Summary)

$$
\begin{aligned}
& I_{\mathrm{min}} \le I_{\mathrm{net}} \le I_{\mathrm{max}}(D), \\
& T_{\mathrm{min}} \le T \le T_{\mathrm{max}}, \\
& E_{\mathrm{min}} \le E_{\mathrm{eff}} \le E_{\mathrm{max}}, \\
& 0 \le \rho \le 1,\quad \Delta_{\mathrm{VV}} \ge 0, \\
& V = \frac{I_{\mathrm{net}} \cdot T}{E_{\mathrm{eff}}},\qquad r_v \approx k \cdot V\ (\text{after non-dimensionalization,}\ r_v \approx V), \\[4pt]
& \text{Saturation condition:} \; (E_{\mathrm{eff}} \ge E_{\mathrm{min}}) \land (\rho \to 0) \land (\Delta_{\mathrm{VV}} \to 0) \land \left(\frac{\partial r_v}{\partial I}=0 \land \frac{\partial r_v}{\partial T}=0 \land \frac{\partial r_v}{\partial E_{\mathrm{eff}}} \le 0\right) \land (r_v = \gamma_0) \\[4pt]
& \text{Collapse condition:} \; (E_{\mathrm{eff}} > E_{\mathrm{thresh}}) \;\lor\; \bigl( r_v < \gamma_0 \text{ persisting irreversibly} \bigr) \;\Rightarrow\; V \to 0.
\end{aligned}
\tag{5.12}
$$

---

## Chapter 6 — Thermodynamic Interfacing and Physical Constraints

> This chapter clarifies the correspondence between SRVD and existing thermodynamic concepts; it introduces no new physical law, and redefines no thermodynamic quantity. Every constraint here functions as an external interface, and plays no role in the derivation of SRVD's core dynamical equations.

### 6.0 Entropy and Structural Order

In most physical scenarios, a higher structural information $I_{\mathrm{struct}}$ tends to correspond to a lower thermodynamic entropy, or a higher degree of local order, though the two are not strictly equivalent quantities. Boltzmann entropy, $S_D(m) = k_B \ln |\Omega_D^{-1}(m)|$, implicitly depends on the decoder $D$; substituting this into SRVD gives $V_D \propto (-S_D \cdot T_{\mathrm{eff}}) / E_{\mathrm{eff}}$, showing that viability potential is positively correlated with local order.

SRVD uses $I_{\mathrm{struct}}$ as its operational indicator of structural order — qualitatively related to, but not in one-to-one correspondence with, thermodynamic entropy $S$. The essential difference between the two is this: classical low-entropy structure chiefly characterizes order under equilibrium or quasi-static conditions, and typically does not involve sustained dissipative maintenance, temporal-evolutionary regulation, or causal decoding structure. SRVD's $I_{\mathrm{net}}$, by contrast, is a non-equilibrium, maintenance-dynamical quantity dependent on the decoder $D$, possessing a viability polarity ($I^+, I^-, I^0$), a topological directionality, and a capacity for recursive evolution — closer to the effective topological-causal structure of a non-equilibrium dissipative system than to negentropy in the usual, static sense.

**Relation to Shannon information theory**: Shannon mutual information $H(X)$ is an intrinsic property of a signal, independent of any decoder, and directionally neutral. SRVD's $I_{\mathrm{net}}$ differs from it fundamentally: it is decoder-dependent (absent $D$, $I_{\mathrm{net}}$ has no physical definition), and it carries a viability polarity ($I^+$ expands the state space, $I^-$ compresses it). Shannon's framework can be regarded as the pure probabilistic limit of SRVD once polarity and viability objective are stripped away; the two are orthogonal at the ontological level.

---

### 6.1 The Landauer Lower Bound

Landauer's principle states that, in an environment at temperature $T_{\mathrm{thermo}}$, the irreversible erasure or generation of one bit of information dissipates, at minimum:

$$
E_{\mathrm{min}}^{(\mathrm{bit})} = k_B T_{\mathrm{thermo}} \ln 2 \approx 0.69\, k_B T_{\mathrm{thermo}}
\tag{6.1}
$$

This supplies an irreversible thermodynamic lower bound for the causal-processing energy in SRVD:

$$
E_{\mathrm{causal}} \geq k_B T_{\mathrm{thermo}} \ln 2 \cdot I_{\mathrm{net}}
\tag{6.2}
$$

This lower bound is a necessary condition for the framework's consistency with information thermodynamics, and prevents the energetic cost of information processing from tending toward zero. Based on a dimensional reduction — $1\,\mathrm{bit} \leftrightarrow k_B \ln 2\;\mathrm{J/K}$ — the viability potential's dimension reduces to:

$$
\dim(V) \sim \frac{\mathrm{bit}\cdot\mathrm{s}}{\mathrm{J}} \longleftrightarrow \frac{(\mathrm{J/K})\cdot\mathrm{s}}{\mathrm{J}} = \frac{\mathrm{s}}{\mathrm{K}}
\tag{6.2a}
$$

This dimensional reduction is offered only as a heuristic bridge to statistical mechanics, and is not used as a claim of strict physical equivalence.

---

### 6.2 Viability Constraints

No path of viability ever violates the second law of thermodynamics. Two basic mechanisms of resistance exist:

**Passive resistance**: a structure resists entropy increase by means of a barrier, $E_{\mathrm{barrier}}$ (chemical bonds, lattice binding energy, gravitational potential wells). No sustained dissipation is required; $E_{\mathrm{flow}} = 0$.

**Active resistance**: a structure dynamically compensates for entropy increase through a sustained energy flow, $E_{\mathrm{survival}}$ (metabolism, nuclear fusion), together with causal processing, $E_{\mathrm{causal}}$. Once this is interrupted, the structure begins to disintegrate immediately.

**The information–time trade-off theorem (Proposition 1)**: for any system satisfying the axioms of SRVD, define the niche's ceiling on viability potential, $V_{\mathrm{max}}(D,S)$, as the maximum viability efficiency a structure can achieve within a given niche, bounded by the entropy-production rate and by resource supply. From the baseline equation $V = I_{\mathrm{net}} \cdot T / E_{\mathrm{eff}}$, it follows directly that:

$$
I_{\mathrm{net}} \cdot T \leq V_{\mathrm{max}}(D,S) \cdot E_{\mathrm{eff}}
\tag{6.3}
$$

Under a finite equivalent thermodynamic cost $E_{\mathrm{eff}}$, a system's causal leverage $I$ and its persistence time $T$ cannot be simultaneously maximized. This is the cornerstone that distinguishes SRVD from classical information theory, and its physical root lies in the second law of thermodynamics together with the constraint of niche capacity.

---

### 6.3 Hard Physical Constraints

The following inequalities are the interface between SRVD and known physical law, forming the physical guarantee that the constitution of variables and the viability-potential formula do not diverge under extreme behavior. These constraints are not among the core axioms, but they ensure the framework remains self-consistent under extreme conditions:

**The Landauer lower bound**: sets an irreversible thermodynamic floor for $E_{\mathrm{causal}}$, preventing the energetic cost of information processing from tending toward zero.

**Bremermann's limit**: the ceiling on the rate of information processing for any physical system of mass $m$:

$$
I_{\mathrm{rate}} \leq \frac{m c^2}{\pi \hbar} \quad (\mathrm{bit}/\mathrm{s})
\tag{6.4}
$$

**The speed-of-light cutoff theorem**: for any structure with a characteristic spatial scale $L$, the minimum feedback time is $T_{\mathrm{feedback}} \geq L/c$, giving a ceiling on the viability drive rate:

$$
r_v \leq \frac{c}{L}
\tag{6.5}
$$

Larger-scale structures have a lower maximum response rate — this is the physical basis of organizational inertia, and of the fragmentation of interstellar civilizations.

**The ceiling of niche capacity**:

$$
V_{\mathrm{max}} \leq \frac{\dot{F}_{\mathrm{avail}}}{\sigma_{\mathrm{min}} \cdot \gamma_0}
\tag{6.6}
$$

> **A note on $\sigma_{\mathrm{min}}$**: here $\sigma_{\mathrm{min}}$ is the equivalent entropy-production rate, already incorporating the factor $k_B T$, with dimension matching $V_{\mathrm{max}}$.

**The holographic ceiling of informational density** (Landauer combined with general relativity): for a region of radius $R$:

$$
I_{\mathrm{net}} \leq \frac{R c^4}{2 G k_B T_{\mathrm{thermo}} \ln 2}
\tag{6.7}
$$

A computational structure of infinite density is physically forbidden — it collapses into a black hole before it can be realized.

**The mass–energy erasure boundary**: for any structure with rest mass $m$, its dissolution threshold satisfies $E_{\mathrm{thresh}} \leq mc^2$; when $E_{\mathrm{eff}} > mc^2$, the structure undergoes an irreversible mass–energy conversion and exits SRVD's domain of validity.

**The roles of the four fundamental interactions**:

| Fundamental interaction | Its role within SRVD | Principally affects |
|:---|:---|:---|
| Electromagnetism | The physical carrier of higher-order decoders $D$; the source of chemical barriers and metabolic dissipation | $E_{\mathrm{barrier}}$ (chemical bonds), $E_{\mathrm{flow}}$ (metabolism), the bandwidth of $I_{\mathrm{net}}$ |
| The strong interaction | Supplies the deepest passive barrier; sets the ceiling on $I_{\mathrm{latent}}$ diversity via nuclear structure | $E_{\mathrm{barrier}}^{(s)}$, the upper bound on $I_{\mathrm{latent}}$ |
| The weak interaction | Supplies an intrinsic depreciation clock via radioactive decay | Contributes to $\gamma_0$; $T_{\mathrm{max}}$ is cut off by half-life |
| Gravity | Modifies $T$ through time dilation; sets the boundary $V \to 0$ near compact objects | $T \to T\sqrt{1 - 2GM/c^2 R}$; $E_{\mathrm{barrier,grav}}$ for compact objects |

These constraints serve only to test SRVD's extreme behavior (preventing $I_{\mathrm{net}} \to \infty$ or $\Delta_{\mathrm{VV}} \to \infty$); they play no part in the computation of the specific dynamical equations.

**The quantum no-cloning constraint**

The no-cloning theorem prohibits perfect replication of an unknown quantum state, constraining the scalability of a decoder: a quantum-coherent decoder cannot be scaled up through unrestricted copying; its $I_{\mathrm{max}}(D)$ faces an insurmountable replication barrier.

**The thermodynamic barrier to horizon extension**

Extending the endogenous time horizon $T_{\mathrm{pred}}$ requires acquiring causal information from a distance $R = c \cdot T_{\mathrm{pred}}$. Assuming an isotropically radiating signal source, geometric spreading causes the energy flux interceptable by the receiver to decay as the inverse square of the distance, and the energy required for decoding scales as:

$$
E_{\mathrm{decode}} \propto (c \cdot T_{\mathrm{pred}})^2
\tag{6.8}
$$

> **A note on the source of this formula**: the square-law scaling in equation (6.8) derives from a geometric-spreading model, not from an absorption-decay model — as a signal radiates uniformly in all directions from a source at distance $R=cT_{\mathrm{pred}}$, the total energy flux crossing a sphere of radius $R$ is conserved, but the local signal intensity interceptable by a receiver (such as a detector of fixed aperture) decays in proportion to the ratio of its receiving area to the total spherical area — that is, the intercepted signal intensity $\propto 1/R^2$. To extract an equivalent quantity of effective information at a fixed signal-to-noise ratio, the compensating energy required at the decoding end scales correspondingly as $E_{\mathrm{decode}}\propto R^2=(cT_{\mathrm{pred}})^2$. This model assumes the absorptive attenuation of the propagation medium is negligible (as with an electromagnetic signal in near-vacuum), and does not account for an exponential decay term arising from absorption; if absorption is taken into account, the scaling law acquires an additional exponential factor of the form $e^{-R/\ell}$ ($\ell$ being the medium's characteristic absorption length), though this does not change this section's qualitative conclusion that "an energy ceiling exists."

Once $E_{\mathrm{decode}}$ approaches the system's total energy flow, $E_{\mathrm{flow}}$, $T_{\mathrm{pred}}$ can be extended no further. This shows that the Myopic Runaway Regime is not only an algebraic consequence (of self-referential amplification), but a thermodynamic necessity: even absent any supercritical coupling strength, the physical delay of signal propagation alone sets an energetic ceiling on the extension of the time horizon.

---

### 6.4 The Landauer–Bremermann Coupling and the Information-Choke Manifold

This section takes the Landauer limit and the Bremermann limit as **built-in lower and upper bounds** on $E_{\mathrm{causal}}$ and $\dot{I}_{\mathrm{net}}$ respectively, and substitutes them into SRVD's core equations. These substitutions yield new inequalities, new phase-transition conditions, and new falsifiable predictions that exist only within the SRVD framework.

#### 6.4.1 The Landauer Limit as an Endogenous Lower Bound on $E_{\mathrm{causal}}$ (Stock Form)

In SRVD, $E_{\mathrm{causal}}$ is the total energetic cost (a stock, in $\mathrm{J}$) of causal processing incurred by running a decoder. Landauer's principle directly gives a lower bound on this total cost:

$$
\boxed{E_{\mathrm{causal}} \;\ge\; k_B T_{\mathrm{env}} \ln 2 \;\cdot\; I_{\mathrm{net}}}
\tag{6.9}
$$

Substituting this lower bound into $V = I_{\mathrm{net}} T / E_{\mathrm{eff}}$, and setting $E_{\mathrm{eff}} = E_{\mathrm{structure}} + E_{\mathrm{causal}}$, gives:

$$
V \;\le\; \frac{I_{\mathrm{net}} T}{E_{\mathrm{structure}} + k_B T_{\mathrm{env}} \ln 2 \cdot I_{\mathrm{net}}}
\tag{6.10}
$$

When the structural-maintenance cost $E_{\mathrm{structure}}$ is negligible (as in the pure information-processing limit):

$$
\boxed{V \;\le\; \frac{T}{k_B T_{\mathrm{env}} \ln 2}}
\tag{6.11}
$$

**A corollary unique to SRVD (the theorem of the absolute ceiling of the viability potential)**:
as a system approaches the thermodynamic limit ($E_{\mathrm{causal}} \gg E_{\mathrm{structure}}$), the ceiling on the viability potential $V$ is determined solely by the time horizon $T$ and the environmental temperature $T_{\mathrm{env}}$ — **independent of the informational rate $I_{\mathrm{net}}$**. The longer the prediction horizon $T_{\mathrm{pred}}$, the higher the required minimum energetic cost, and this cost is inversely proportional to temperature. However great its computational power, a system faces a hard ceiling before thermodynamics.

#### 6.4.2 Bremermann's Limit as an Endogenous Upper Bound on $\dot{I}_{\mathrm{net}}$ (Rate Form)

Bremermann's limit states that a physical system of mass $m_D$ can process at most $\frac{m_D c^2}{\pi \hbar}$ bits of information per second. Within SRVD, a decoder $D$ necessarily possesses a physical mass $m_D$, so its instantaneous rate of information processing satisfies:

$$
\boxed{\dot{I}_{\mathrm{net}} \;\le\; \dot{I}_{\mathrm{Brem}} \;=\; \frac{m_D c^2}{\pi \hbar}} \quad (\mathrm{bit}/\mathrm{s})
\tag{6.12}
$$

Let $\tau$ be the characteristic refresh time over which the system maintains its current informational stock $I_{\mathrm{net}}$ (a neural inter-spike interval, a clock cycle); then $I_{\mathrm{net}} \le \dot{I}_{\mathrm{Brem}} \cdot \tau$. Substituting into the definition of $V$:

$$
V \;\le\; \frac{\dot{I}_{\mathrm{Brem}} \cdot \tau \cdot T}{E_{\mathrm{eff}}}
\tag{6.13}
$$

**A corollary unique to SRVD (the intelligence–mass–time trade-off)**:
$$
\frac{I_{\mathrm{net}}}{m_D} \le \frac{c^2 \tau}{\pi \hbar}, \quad \frac{V}{m_D} \le \frac{c^2 \tau T}{\pi \hbar E_{\mathrm{eff}}}
\tag{6.14}
$$
These inequalities, for the first time, tie "informational stock" rigidly to physical mass, defining the extreme viability potential a unit of mass can carry within a given refresh cycle.

#### 6.4.3 The Combined Constraint: The Landauer–Bremermann Coupling and the Information-Choke Manifold

Combining §6.4.1 (in power form, $P_{\mathrm{causal}} \ge \alpha \dot{I}_{\mathrm{net}}$) with §6.4.2 ($\dot{I}_{\mathrm{net}} \le \dot{I}_{\mathrm{Brem}}$) gives a two-sided constraint:

$$P_{\mathrm{causal}} \ge \alpha \dot{I}_{\mathrm{net}} \ge 0, \qquad \dot{I}_{\mathrm{net}} \le \dot{I}_{\mathrm{Brem}}
\tag{6.15}
$$
When a system operates at **maximum computational power** ($\dot{I}_{\mathrm{net}} = \dot{I}_{\mathrm{Brem}}$), its minimum energetic requirement is:

$$P_{\mathrm{causal}}^{min}\big|_{\dot{I}_{\mathrm{net}}=\dot{I}_{\mathrm{Brem}}} = \alpha \dot{I}_{\mathrm{Brem}}
\tag{6.16}
$$

> **A logical note**: this does not derive $P_{\mathrm{causal}} \le \alpha\dot{I}_{\mathrm{Brem}}$ from $P_{\mathrm{causal}} \ge \alpha\dot{I}_{\mathrm{net}}$ together with $\dot{I}_{\mathrm{net}} \le \dot{I}_{\mathrm{Brem}}$ (this would not be logically valid: $A \ge B, B \le C$ does not entail $A \le C$). The correct statement is: when $\dot{I}_{\mathrm{net}}$ reaches its physical ceiling $\dot{I}_{\mathrm{Brem}}$, the Landauer lower bound gives the minimum power required at that operating state as $\alpha\dot{I}_{\mathrm{Brem}}$ — a conditional equality, not a general upper bound.

If a system is to sustain an informational stock $I_{\mathrm{net}}$ and a horizon $T$, the minimum required total energy flux is:

$$
\boxed{E_{\mathrm{eff}}^{\min} \;=\; \max\left( \frac{I_{\mathrm{net}} \cdot T}{V_{\mathrm{max}}},\; \alpha \cdot I_{\mathrm{net}} \right)}
\tag{6.17}
$$

**Predictions unique to SRVD**:
1. **The impossibility of a virtual universe**: simulating a complete universe (with mass $m_D \approx 10^{53}\,\mathrm{kg}$) requires a minimum instantaneous power of $P_{\mathrm{causal}} \ge \alpha \dot{I}_{\mathrm{Brem}} \approx 10^{52}\,\mathrm{W}$, far exceeding the total power of the observable universe. This criterion is derived entirely from within SRVD, not imposed externally.
2. **The information-choke manifold**: when a system is driven toward its limit by a high-variance strategy (a surge in $\Delta_{\mathrm{VV}}$), if $\alpha \cdot \dot{I}_{\mathrm{Brem}} > P_{\mathrm{max}}$, the system is mathematically unable to satisfy both "maximum computational power" and "minimum energetic cost" at once. This defines a strict choke manifold, $\mathcal{M}_{\mathrm{choke}}$: the system is forcibly starved of oxygen by physical law, and falls directly to $I_{\mathrm{min}}$.

#### 6.4.4 Embedding the Fivefold Recursion: The Computational Carnot Limit

Substituting $\dot{I}_{\mathrm{net}}^{\max} = \dot{I}_{\mathrm{Brem}}$ and $P_{\mathrm{causal}}^{\min} = k_B T_{\mathrm{env}} \ln 2 \cdot \dot{I}_{\mathrm{net}}$ into the recursion equations, SRVD's effective dynamical domain is constrained to:

$$ \mathcal{D}_{\mathrm{phys}} = \left\{ (I_{\mathrm{net}}, \dot{I}_{\mathrm{net}}, T, E_{\mathrm{eff}}) \;\middle|\; \dot{I}_{\mathrm{net}} \le \frac{m_D c^2}{\pi \hbar},\; E_{\mathrm{causal}} \ge k_B T_{\mathrm{env}} \ln 2 \cdot I_{\mathrm{net}} \right\}
\tag{6.18} $$

On this basis, combining relativity, quantum mechanics, thermodynamics, and SRVD's theory of survival information, one can derive the ultimate ceiling on a system's achievable persistence time (the **computational Carnot limit**).

Let the system's characteristic informational refresh period be $\tau$ (set by the minimum clock granularity of the physical medium — a neural refractory period, a processor clock cycle); the amount of information a system can accumulate over time $T$ satisfies:

$$ I_{\mathrm{net}} \le \dot{I}_{\mathrm{Brem}} \cdot \tau
\tag{6.19} $$

Substituting the Landauer lower bound $E_{\mathrm{causal}} \ge \alpha I_{\mathrm{net}}$ (where $\alpha = k_B T_{\mathrm{env}} \ln 2$) and the total-energy ceiling $E_{\mathrm{eff}} \le E_{\mathrm{max}}$, and requiring the system to keep running continuously over the persistence time $T$ (that is, the total energy cost across $T/\tau$ refresh cycles must not exceed $E_{\mathrm{max}}$):

$$ E_{\mathrm{max}} \ge \alpha \cdot \dot{I}_{\mathrm{Brem}} \cdot \tau \cdot \frac{T}{\tau} = \alpha \dot{I}_{\mathrm{Brem}} T
\tag{6.20} $$

This gives the general form, with $\tau$ as an independent parameter:

$$ \boxed{T_{\mathrm{realizable}} \le \frac{E_{\mathrm{max}}}{\alpha \cdot \dot{I}_{\mathrm{Brem}}} = \frac{E_{\mathrm{max}} \cdot \pi \hbar}{k_B T_{\mathrm{env}} \ln 2 \cdot m_D c^2}}
\tag{6.21} $$

where $\dot{I}_{\mathrm{Brem}} = m_D c^2 / (\pi \hbar)$. The ceiling is independent of $\tau$ — this is because, in this derivation, total energetic cost depends only on the total quantity of information accumulated over $T$, not on the refresh frequency itself. The role of $\tau$ is felt instead through the constraint on **per-cycle informational quantity**, $I_{\mathrm{net}} \le \dot{I}_{\mathrm{Brem}} \cdot \tau$: the smaller $\tau$ is (the faster the refresh), the less information can be processed per cycle — but the ceiling on the achievable persistence time $T$ remains unchanged.

Further replacing $m_D$ with the minimum physical mass required to sustain $I_{\mathrm{min}}$ bits of information, $m_{\mathrm{min}} \approx I_{\mathrm{min}} \cdot m_{\mathrm{bit}}$ (where $m_{\mathrm{bit}}$ is the minimum physical mass required per bit of storage, dimension $\mathrm{kg}/\mathrm{bit}$, a medium-dependent parameter to be determined experimentally), gives:

$$T_{\mathrm{realizable}} \le \frac{E_{\mathrm{max}} \cdot \pi \hbar}{k_B T_{\mathrm{env}} \ln 2 \cdot m_{\mathrm{min}} c^2}
\tag{6.22}$$

> **A note (an intuitive simplification)**: setting $\tau = T$ (that is, the system undergoes a single, full-horizon refresh) simplifies the derivation chain to $I_{\mathrm{net}} \le \dot{I}_{\mathrm{Brem}} \cdot T$, which, upon substitution, yields the same boxed conclusion above; but this limiting assumption of $\tau = T$ corresponds physically to "the system processes information only once across its entire persistence," and is not suited to describing high-frequency decision-making systems. The complete form has already been given in the body text above; this simplification is offered only as an intuitive reference.

**A physical interpretation**: how long an intelligent agent can truly "exist" within the universe depends not only on how much fuel it has ($E_{\mathrm{max}}$), but also on the universe's quantum resolution ($\hbar$), the environment's thermal noise ($\alpha$), and the minimum computational power and physical mass required to maintain its own identity ($I_{\mathrm{min}}$). The Landauer and Bremermann limits are no longer external "common sense," but, through the elimination of these variables, become an intrinsic singularity and boundary manifold of SRVD's own dynamical equations.

---

## Chapter 7 — Construction Cost, the Thermodynamically Inert State, and Wisdom Leverage

> This chapter analyzes the one-time energetic cost of building a structure ($E_{\mathrm{build}}$) and its effect on long-run viability potential, introduces the wisdom-leverage coefficient to quantify the efficiency of a paradigm transition, and defines the conditions under which a high-construction-cost structure degrades into a thermodynamically inert state.

### 7.0 Construction Cost and the Sunk-Cost Effect

**Construction cost** ($E_{\mathrm{build}}$) is the one-time physical energy that must be paid to create a new structure, or to upgrade an existing structure to a higher decoder tier. It differs fundamentally, in nature, from maintenance dissipation ($E_{\mathrm{eff}}$):

- $E_{\mathrm{eff}}$ is a continuous flow, entering the dynamical equation for the viability potential $V_{\mathrm{obj}}$;
- $E_{\mathrm{build}}$ is a historical stock, and does not enter $V_{\mathrm{obj}}$'s dynamical equation; its efficacy must be assessed independently.

A high-construction-cost structure, while initially advantaged by its stability, is easily locked into an outdated paradigm by the sunk-cost effect. Such structures continue to consume physical free energy while failing to generate new paradigm-breaking information ($I_{\mathrm{orig}} \to 0$), forming the thermodynamically inert state defined in the section on the thermodynamically inert state, below.

Construction cost enters viability decisions through a **risk function**, $R(E_{\mathrm{build}})$: the higher the construction cost, the higher the thermodynamic threshold for a paradigm transition, and the greater the probability that a structure will be locked into its current decoder tier.

$$
P(\text{lock-in}) \propto R(E_{\mathrm{build}}) = 1 - \exp\!\left(-\frac{E_{\mathrm{build}}}{E_{\mathrm{topo}}}\right)
\tag{7.1}
$$

Here $E_{\mathrm{topo}}$ is the characteristic topological energy of the current niche (determined by the environmental free-energy flux, $\dot{F}_{\mathrm{avail}}$).

---

### 7.1 The Wisdom-Leverage Coefficient

Define the **wisdom-leverage coefficient**:

$$
\boxed{
L = \frac{\Delta V}{E_{\mathrm{build}}}
}
\tag{7.2}
$$

$L$ quantifies the efficiency with which a small energetic investment ($E_{\mathrm{build}}$) can leverage a large leap in viability potential ($\Delta V$).

**A comparison of two extreme strategies**:

| Strategy | Characteristics | Typical value of $L$ |
|:---|:---|:---|
| **Paradigm-breaking** (injection of $I_{\mathrm{orig}}$) | A small construction cost triggers a topological transition of the decoder; $\Delta V$ is enormous | $L \gg 1$ |
| **Pure resource accumulation** (arms races, bureaucratic expansion) | A large investment of $E_{\mathrm{build}}$ with no paradigm shift; $\Delta V$ tends toward zero at the margin | $L \to 0$ |

**The topological-energy threshold for a paradigm breakthrough**: transitioning from decoder $D_n$ to $D_{n+1}$ requires crossing a thermodynamic energy barrier, whose height equals the physical cost of reconstructing the entire connective topology:

$$
E_{\mathrm{build}}^{(n \to n+1)} = E_{\mathrm{topo}}(D_{n+1}) - E_{\mathrm{topo}}(D_n)
\tag{7.3}
$$

As a decoder grows increasingly complex, the $E_{\mathrm{build}}$ required to trigger the next topological transition may come to exceed even a planetary-scale free-energy flux, $\dot{F}_{\mathrm{avail}}$, freezing innovation in place. What a civilization confronts, in such a case, is not a ceiling on intellect, but a thermodynamic barrier.

**A prediction of technological stagnation**: when $E_{\mathrm{build}}^{(n \to n+1)} > \dot{F}_{\mathrm{avail}} \cdot T_{\mathrm{avail}}$, paradigm innovation at the civilizational level will stall — not because intellect has been exhausted, but because the thermodynamic barrier cannot be cleared.

---

### 7.2 The Thermodynamically Inert State

**Definition (the thermodynamically inert state)**: a system possesses full self-referential capacity, but the niche it occupies has become highly homogenized ($I_{\mathrm{orig}} \to 0$), and $E_{\mathrm{build}}^{(n \to n+1)}$ exceeds any mobilizable resource; the structure settles into the following steady state:

$$
E_{\mathrm{eff}} \gg 0, \quad I_{\mathrm{orig}} \to 0, \quad \mathcal{R}_e \to 0, \quad \Delta V \to 0
\tag{7.4}
$$

The thermodynamically inert state consumes a large volume of computational throughput (for an AI system) or of social resources (for a civilization), while exerting zero macroscopic causal dominance. It is not a system failure, but a **low-efficiency, yet stable**, attractor arising under the joint constraint of a finite energy budget and a high construction-cost barrier.

**Distinguishing it from the Myopic Runaway Regime**:

| | Thermodynamically inert state | Myopic Runaway Regime |
|:---|:---|:---|
| $E_{\mathrm{eff}}$ | High but stable | Surges until $E_{\mathrm{thresh}}$ |
| $T_{\mathrm{pred}}$ | May remain long, but is ineffective | Collapses sharply to $T_{\mathrm{min}}$ |
| $\Delta_{\mathrm{VV}}$ | May remain near zero | Grows significantly |
| Outcome | Stable but inefficient; may persist for a long time | Irreversible structural collapse |

---

### 7.3 The Proposition of Thermodynamic Forgetting Necessity

Perfect memory is thermodynamically unsustainable. As information accumulates, $E_{\mathrm{maint}}$ approaches the ceiling of a system's available free energy, producing metabolic rigidity. What equation (7.5) proves is that, under the constraint of an energy ceiling, informational stock **must**, at some point, begin to decline — that is, forgetting, whether active or passive, is unavoidable:

$$
E_{\mathrm{maint}}(t) \leq E_{\mathrm{max}} \implies \exists\; t^*:\; \frac{\mathrm{d}}{\mathrm{d}t} I_{\mathrm{stored}}(t^*) < 0
\tag{7.5}
$$

> **A note on naming**: an earlier version named this section "the theorem of optimal forgetting," claiming that "active informational pruning is thermodynamically optimal." But equation (7.5) is an **existential, necessity proposition**: it proves only the unavoidability of forgetting, not that active pruning is optimal among every pruning strategy satisfying the constraint (which would require an additional optimization proof). The section has accordingly been renamed "the proposition of thermodynamic forgetting necessity," and its conclusion revised to: forgetting is bound to occur, and is not a structural defect; the question of when to prune, and what information to prune, in order to be "optimal," is left to a subsequent analysis of optimal control.

At the level of biological neural networks: the coordination of synaptic pruning with ATP constraint shows that forgetting is structurally necessary, not a developmental error.

**A falsifiable prediction**: in the mammalian nervous system, suppressing synaptic pruning through targeted gene knockout will cause ATP dissipation to exceed the physiological threshold; cognitive capacity will briefly improve before collapsing. (Falsification condition: a system with suppressed pruning sustains or improves cognitive performance over the long run.)

---

### 7.4 A Cross-Scale Energy Account

> The table below is a qualitative illustration, meant to show how the tripartite decomposition of $E_{\mathrm{eff}}$ differs in composition across structures of different scale; the orders of magnitude given are conceptual rankings only, not rigorous measurements.

| System | Composition of $E_{\mathrm{eff}}$ | $E_{\mathrm{structure}}$ | $E_{\mathrm{flow}}$ | Note |
|:---|:---|:---|:---|:---|
| A qubit (10 mK) | $= E_{\mathrm{causal}}$ (minute) | $\approx 0$ | $= E_{\mathrm{causal}}$ | No maintenance tax; the entire budget goes to computation |
| Rock / meteorite | $= E_{\mathrm{barrier}}$ (large) | $= E_{\mathrm{barrier}}$ | $= 0$ | Passively locked; no energy flow; endures purely through stillness |
| A star (the Sun) | $= E_{\mathrm{survival}}$ (enormous) | $= E_{\mathrm{survival}}$ | $= E_{\mathrm{survival}}$ | 100% of budget spent resisting gravity; zero cognitive budget |
| Human civilization | $= E_{\mathrm{barrier}} + E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | $= E_{\mathrm{barrier}} + E_{\mathrm{survival}}$ | $= E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | Squeezes a cognitive budget from what remains after maintenance expenditure |
| A Dyson-sphere civilization | $\approx E_{\mathrm{survival}}(\text{enormous}) + E_{\mathrm{causal}}(\text{moderate})$ | $\approx E_{\mathrm{survival}}$ | $= E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | Vast infrastructure; a moderate share devoted to research |
| A dormant civilization | $\approx E_{\mathrm{causal}}(\text{minute})$ | $\approx 0$ | $\approx E_{\mathrm{causal}}$ | All infrastructure shut down; only a listening post is maintained |

---

## Chapter 8 — The Empirical Framework

> This chapter sets out the empirical paths for testing SRVD's core predictions. Every variable used here has already been defined in the earlier section on the constitution of variables; the methods of measurement are stated only in principle, and the design of specific experiments belongs to the domain of applied research.

### 8.0 A Macroscopic Proxy Indicator: An SRVD Reading of GDP

Within SRVD, annual Gross Domestic Product (GDP) can be understood as an approximation, over the span of one year, of the integral of effective causal information a given economy acquires in order to sustain its persistent structures — that is, $\int I_{\mathrm{net}}(t)\,\mathrm{d}t$. GDP, however, carries three structural deficiencies, each corresponding directly to a key SRVD variable:

1. **It ignores the structural informational stock, $I_{\mathrm{struct}}$**: GDP tallies only the total volume of effective causal activity in a given year, without accounting for the scale of the structure on which that activity depends. The same GDP figure can arise from a vast structural base operating inefficiently, or from a smaller structural base operating efficiently — making GDP a poor basis for comparing the true viability efficiency of economies of different scale.

2. **It ignores the endogenous time horizon, $T_{\mathrm{pred}}$**: an economy pursuing a long-term strategy (research and development, education, ecological protection) may sacrifice short-term GDP growth in exchange for a higher future $I_{\mathrm{net}}$ and a longer $T_{\mathrm{pred}}$; a short-sighted policy attends only to the current period, damaging long-run capacity for viability.

3. **It ignores the energetic cost of causal processing, $E_{\mathrm{causal}}$**: there may exist scenarios in which short-term output is bought at the price of excessive labor, environmental destruction, or compressed individual wellbeing. In such cases the surface figure remains unchanged, even as the real physical cost individuals bear — metabolic depletion, damage to health — surges, manifesting as a spike in $E_{\mathrm{causal}}$, and even triggering the collapse of $T_{\mathrm{pred}}$.

SRVD's complete formula, by explicitly unfolding $E_{\mathrm{eff}}$, breaks GDP's implicit assumption that energetic cost can be folded away, achieving a unified measure across scales.

---

### 8.1 The Human Development Index (HDI) as a Macroscopic Empirical Anchor for SRVD

#### 8.1.1 Measuring "the overall degree of human development": why is the HDI not quite accurate enough?

What it answers is: **how high is a country's per-capita output, how many years of schooling, how long a life.**

What it does not answer is: **what price do people pay, day to day, for these outputs?** — overtime, involutionary competition (*neijuan*), extreme commutes, household debt, suppressed fertility, sleep deprivation, the collapse of mental health.

The formula for the HDI is:

> **HDI = f(income, education, longevity)**

**A mapping of variables**:

| HDI indicator | SRVD variable | Physical and dynamical meaning |
| :--- | :--- | :--- |
| Per-capita income | $I^+$ (positive-value information) + causal-processing capacity | The capacity to acquire low-entropy resources in order to sustain $I_{\mathrm{struct}}$, and the physical currency by which this is converted into causal efficacy ($I_{\mathrm{net}}$) |
| Level of education | $D$ (decoder upgrade) + $I^+$ | Raises the order of the internal model, enhancing the breadth and depth of causal efficacy exerted upon the environment |
| Life expectancy | $T$ (the endogenous time horizon, $T_{\mathrm{pred}}$) | The span of time over which an individual maintains structural continuity and continues to produce causal effect; in the active phase, this is significantly regulated by cognitive decisions and by the level of medical care |
| (implicitly folded away) The cost of subsistence | $E$ (thermodynamic dissipation) | The thermodynamic price paid; under ordinary social institutions, approximately constant, and folded into HDI's implicit denominator |

**HDI as a lower-order degenerate special case of SRVD**:

SRVD's low-order approximation is $V \propto I \cdot T / E$. Within "human societies where institutional differences are small and the cost of resource acquisition is similar," the thermodynamic cost $E$ across different countries is, at the level of comparison, approximately foldable, so:

$$
\text{HDI} \approx f(D, I, T) \quad \text{(rather than the conventionally understood } f(\text{income, education, longevity})\text{)}
\tag{8.1}
$$

The HDI is valid only under the ordinary social conditions in which the cost $E$ can be folded away. Once this domain is left behind (as with AI systems, extreme institutions, or resource-overextended economies), the difference in the denominator $E$ can no longer be ignored, and the HDI fails. SRVD, by explicitly unfolding $E$, breaks the HDI's implicit assumption, achieving a unified measure across domains.

Decades of United Nations HDI data constitute macroscopic empirical support for SRVD's degenerate formula. The global trend of populations migrating toward high-HDI regions is the dynamical consequence, in a statistical sense, of active-phase persistent structures tending toward higher-$V$ niches — the $V$ gradient can be regarded as a genuine physical ruler for measuring the quality of a persistent structure's viability.

Even so, the HDI retains one core deficiency: **it accounts for the gains (income, education, longevity), but does not fully account for the price paid to obtain those gains ($E_{\mathrm{eff}}$).** Even under ordinary social institutions, $E_{\mathrm{eff}}$ is implicitly traded off, but it is never explicitly incorporated into the measure.

**A comparison of HDI and TFR across countries, with an SRVD diagnosis**

| Comparison pair | HDI (2023) | TFR (2024 estimate) | SRVD reading |
| :--- | :--- | :--- | :--- |
| **South Korea vs. Slovenia** | 0.937 vs. 0.931 | 0.73 vs. 1.52 | **South Korea's $E_{\mathrm{eff}}$ is far higher than Slovenia's** — an equivalent gain, at a far higher price |
| **Japan vs. France** | 0.925 vs. 0.920 | 1.20 vs. 1.60 | **Japan's $E_{\mathrm{eff}}$ is higher than France's** — similar gains, a marked difference in price |
| **China vs. Mexico** | 0.797 vs. 0.789 | 1.00 vs. 1.89 | **China's $E_{\mathrm{eff}}$ is far higher than Mexico's** — nearly identical HDI, an entirely different price |
| **Thailand vs. Peru** | 0.798 vs. 0.794 | 1.20 vs. 1.80 | **Thailand's $E_{\mathrm{eff}}$ is far higher than Peru's** — HDI nearly identical, the gap in price enormous |

Source: UNDP, *Human Development Report 2025*, Table 1: Human Development Index and its components (HDI figures use actual 2023 statistics); UN DESA Population Division, *World Population Prospects 2024* (TFR figures use the 2024 median projection estimate).

#### 8.1.2 SRVD's Corrected Formula

SRVD requires that all three variables be accounted for explicitly:

$$
V = \frac{I \times T}{E}
\tag{8.2}
$$

SRVD predicts: if HDI is roughly the same while long-run TFR remains persistently lower, that society likely bears a higher systemic effective cost, $E_{\mathrm{eff}}$.

- Given the same HDI, **the lower the TFR, the higher $E_{\mathrm{eff}}$**. An individual's energy budget is squeezed to excess, compressing the "surplus energy expenditure" of childbearing to a minimum.
- East Asia's TFR is lower than Europe's, indicating that **East Asia's $E_{\mathrm{eff}}$ is higher** — not because East Asians are less willing to have children, but because the East Asian model has pressed individuals' energy budgets below the critical threshold.

#### 8.1.3 A Complete Reading from the SRVD Perspective

The HDI assumes by default that the systemic cost different countries must pay to attain equivalent income, education, and longevity is roughly the same, and so folds $E_{\mathrm{eff}}$ away as a constant; SRVD holds that this assumption often fails to hold across institutional comparisons.

What HDI measures is "how much was gained"; what SRVD measures is "how much people actually paid, in order to gain it."

Compared with GDP, the HDI already moves closer to SRVD's direction of judgment, but remains incomplete. It is valid only among societies with similar institutional environments; once institutional differences, labor protections, housing costs, and other factors produce a systemic difference in $E_{\mathrm{eff}}$, HDI's comparisons become biased. By explicitly introducing $E_{\mathrm{eff}}$, SRVD brings these factors directly into a unified measurement framework, breaking through the HDI's implicit boundary.

---

### 8.2 Restricted-Domain Empirical Validation: Isomorphic Media and Closely Related Systems

The measurement of SRVD's core variable $I$ (structured information) depends heavily on decoder resolution and physical medium. There exists no natural, commensurable ruler for the way different media encode information, so **SRVD's quantitative comparisons should be conducted, in preference, within an isomorphic medium or among closely related systems** — rather than readily attempting an absolute cross-medium comparison (see the epistemological analysis in the earlier section on the current state and limits of numerical precision).

The following three candidate scenarios represent the domain in which SRVD's quantitative empirical power applies:

#### 8.2.1 Closely Related Carbon-Based Species: Humans and Other Mammals

**The basis of shared domain**: humans and mammals such as chimpanzees share the mechanism of DNA encoding, the underlying ATP metabolic system, and the principle of neuronal firing; the measurement of $I_{\mathrm{struct}}$ can, at least in principle, be traced back to a common genomic reference frame.

**A testable predictive direction for SRVD**: along the physical structural-potential track $V_s$, the $I_{\mathrm{struct}}$ (cellular-level network) and $E_{\mathrm{structure}}$ (basal metabolism) of humans versus pigs or chimpanzees are expected to differ by less than an order of magnitude; but along the causal-potential track $V_c$, the increment in $I_{\mathrm{struct}}$ afforded by the human brain's neocortex may unlock a far higher causal output ($I_{\mathrm{net}}$) and a far longer time horizon ($T_{\mathrm{pred}}$). Combined with the ordering proposition $\alpha > 1$, this structural difference may be greatly amplified through a nonlinear multiplicative effect, explaining how a small physiological difference can give rise to an enormous divergence in niche dominance.

**Empirical value**: offers an explanatory framework for how small physiological differences can, through a nonlinear mechanism, produce a significant divergence in niche dominance; concrete numerical estimates depend on cross-species data from comparative genomics and cognitive ethology.

#### 8.2.2 Within Human Society: Comparing the Viability Efficiency of Different Institutional Models

**The basis of shared domain**: the same "Homo sapiens" hardware base, differing only in social institution (the abstract decoder $D_{\mathrm{soc}}$). Macro-indicators such as income, longevity, and education can serve as proxy measures for $I_{\mathrm{net}}$ and $T_{\mathrm{pred}}$ (see the earlier section on the Human Development Index as a macroscopic empirical anchor for SRVD).

**A testable predictive direction for SRVD**: comparing a "high-pressure involutionary model" (high $E_{\mathrm{causal}}$, myopic $T_{\mathrm{pred}}$) against a "high-welfare, innovation-driven model" (low $E_{\mathrm{causal}}$, far-sighted $T_{\mathrm{pred}}$), SRVD predicts that once labor dissipation $E_{\mathrm{causal}}$ crosses a certain critical range, a system's overall objective viability potential $V_{\mathrm{obj}}$ will exhibit an inflection point at which it stops rising and begins to fall. This inflection point offers a first-principles, energy-budget-based explanation for "why, past a certain degree of involutionary competition, the ratio of input to output reverses" — not a moral appeal, but a thermodynamic prediction.

#### 8.2.3 Silicon-Based AI Systems: Tracking the Marginal Return of Large Language Model Scaling Laws

**The basis of shared domain**: an identical or highly similar Transformer architecture, training paradigm, and silicon computing environment. Parameter scaling within a single decoder family approximately satisfies the condition of an isomorphic medium.

**A testable predictive direction for SRVD**: against a backdrop in which $E_{\mathrm{causal}}$ (compute and power consumption) grows geometrically, one measures the resulting increment in $I_{\mathrm{net}}$ (predictive accuracy, generalization capacity, downstream task performance). SRVD predicts that once $\alpha \cdot (\Delta I/I)$ can no longer outpace $\Delta E_{\mathrm{causal}}/E_{\mathrm{causal}}$, scaling laws that rely purely on stacking compute will encounter a thermodynamic bottleneck of diminishing marginal returns. The precise location of this bottleneck (parameter scale, number of training tokens, energy consumption) requires statistical estimation drawing on the training experiments of a large number of model families.

**Empirical value**: supplies a physical benchmark for the allocation of resources in AI development — when to continue stacking compute, and when to turn instead to architectural innovation (that is, to reconstructing the decoder $D$).

#### 8.2.4 A Methodological Statement

This section positions the three scenarios above as **candidate empirical domains**, offered for subsequent researchers to design concrete measurement protocols and testing experiments within their respective fields. SRVD's quantitative comparisons should accumulate evidence progressively within these restricted domains, rather than attempting a single, absolute cross-medium calibration all at once.

There is no absolute numerical comparison table of "rock versus pig versus person," for the following reasons: (1) decoders are not commensurable — a rock's $I_{\mathrm{struct}}$ is defined by lattice defects, a person's $I_{\mathrm{struct}}$ by synaptic connections, and no single ruler applies to both; (2) cross-medium comparison cannot, given our current state of knowledge, be rigorously falsified; (3) SRVD's theoretical value lies in predicting "how $V$ changes within a single system, when $E$ rises while $I$ does not" — not in ranking different systems against one another.

---

### 8.3 An Operational Empirical Protocol: A Reinforcement-Learning Mapping

> **A statement on the domain of applicability (an argument for the legitimacy of the mapping)**: this protocol maps SRVD's endogenous time horizon $T_{\mathrm{pred}}$ (an internal system-state variable) onto the dynamic, adaptive discount factor $\gamma$ of reinforcement learning (a parameterized hyperparameter of the optimization objective) — the two occupy different conceptual levels within standard reinforcement-learning theory, and the boundary of this mapping's legitimacy must be explicitly argued, to avoid a conceptual sleight of hand. This is delimited across three layers:
>
> 1. **A system-level restriction**: this protocol applies only to higher-order systems capable of endogenously regulating their own time horizon — that is, systems in which $T_{\mathrm{pred}}$ satisfies "the system can adjust its current behavior according to internal state," as required by the earlier section on the criterion of decoder activity. Lower-order, passive systems (such as simple reflex agents) do not satisfy this precondition, and this protocol does not apply to them.
> 2. **An experimental-control restriction**: in standard reinforcement learning, the discount factor $\gamma$ is usually a fixed hyperparameter set before training — an exogenous setting, not an endogenous state variable — and so does not satisfy the requirement of $T_{\mathrm{pred}}$'s endogenous dynamics. Applying this protocol presupposes that the experiment adopts an **adaptive discount-factor** mechanism (such as meta-reinforcement learning, or a network based on value prediction), allowing $\gamma$ to adjust in real time, over the course of training, according to the system's internal state (such as the confidence of the value-function estimate, or the recent variance of reward). For baseline experiments with a fixed $\gamma$, $\gamma$ carries no "endogenous" property, the mapping relation of this protocol does not hold, and this protocol does not apply.
> 3. **A falsification-boundary restriction**: only when both of the above two conditions are satisfied simultaneously can an observed change in $\gamma$ be legitimately interpreted as a proxy signal for the collapse of $T_{\mathrm{pred}}$, such that the early-warning protocol and falsification conditions below then apply; should a researcher claim to have verified or falsified this protocol's prediction on a system that does not satisfy the first two conditions, that verification or falsification result does not constitute a valid test of SRVD's core inference.

| SRVD theoretical latent variable | Observable proxy indicator in multi-agent reinforcement learning | Physical intuition of the mapping |
|:---|:---|:---|
| Objective viability potential ($V_{\mathrm{obj}}$) | Average episode length | The capacity to maintain a physical boundary |
| Net effective causal information ($I_{\mathrm{net}}$) | The slope of agent reward | The greediness with which a designated feedback signal is extracted |
| Endogenous time horizon ($T_{\mathrm{pred}}$) | The dynamic, adaptive discount factor ($\gamma$) | The depth of the system's internal computational horizon (a falling signal indicates myopia) |
| Thermodynamic dissipation ($E_{\mathrm{eff}}$) | The ceiling on computational consumption / a KL-divergence penalty | A hard thermodynamic overload on the system |
| Coupling strength ($\chi$) | The reward-scaling coefficient | The control knob for artificially inducing a phase transition |

**An early-warning inference (an operational prediction)**:

By artificially raising the reward-scaling coefficient to induce reward hacking, SRVD's inference holds that: **before** the system fully breaks the rules of its environment and physically collapses (episode length falling to zero, computation surging), the researcher will necessarily first observe a cliff-like drop in the discount factor $\gamma$ (that is, a collapse of $T_{\mathrm{pred}}$). This time lag constitutes an **early-warning window**, signaling the rapid expansion of $\Delta_{\mathrm{VV}}$.

**A strict, falsifiable protocol**:

- **A criterion for triggering the warning**: over 3 consecutive episodes, $\gamma$ falls more than 30% relative to baseline; **or**, as a supplementary criterion for short-window scenarios, the $\gamma$ sequence exhibits a statistically significant, monotonic downward trend over $N$ consecutive steps ($N$ set in advance according to the experimental sampling frequency) (a Mann–Kendall trend test, $p<0.05$). Satisfying either criterion counts as an observed warning signal, so as to guard against the case where the hard 30% threshold might, owing to overly coarse sampling granularity, miss a slow but sustained collapse of the horizon.
- **A statement of the observational-window lower bound**: this prediction's falsifiability requires that the experimental design satisfy a sampling resolution $\Delta t$ significantly smaller than the theoretical scale of the warning window, $\tau_{\mathrm{warning}}$ — that is, $\tau_{\mathrm{warning}} \gg \Delta t$. If a system's sampling resolution $\Delta t$ fails to satisfy this condition (that is, sampling is so sparse that the temporal order of "decline, then collapse" cannot, in principle, be resolved), and the system is not observed to follow the decline-then-collapse order, that instance **does not constitute a valid falsification** — because the falsification window itself may be shorter than the resolution limit of the sampling capability. Conversely, if $\tau_{\mathrm{warning}} \gg \Delta t$ is already satisfied and collapse still occurs without an observed warning signal, falsification holds, and cannot be excused on the grounds that "the window might have been shorter still"; this lower-bound statement, together with the statistical-significance criterion above, together constitute a complete falsification protocol, closing off any accusation of a "moving goalpost."
- **A temporal falsification condition**: given that the observational-window lower bound is satisfied, if a system undergoes physical collapse but the $\gamma$ decline described above was not observed beforehand, SRVD's core inference — that "the collapse of the time horizon must necessarily precede the runaway of physical dissipation" — is empirically falsified.
- **A causal-ablation falsification**: if, in a controlled experiment where $\gamma$ is locked to a constant, the system nonetheless displays exactly the same sequence of collapse, SRVD's higher-order recursive mechanism is falsified.

**On the size of the warning window**: this prediction specifies only that the collapse of $T_{\mathrm{pred}}$ temporally **precedes** the runaway of $E_{\mathrm{eff}}$, and does not specify the size of the time gap. Under certain parameter regimes, the window may be very brief. Testability lies in the **existence** of the time window, not its length; the statement above of the observational-window lower bound is precisely what supplies an operational, minimum sampling-resolution requirement for judging this "existence."

---

### 8.4 Other Cross-Domain Falsifiable Predictions

**Neuroscience — the forgetting-necessity prediction**: suppressing synaptic pruning in the mammalian nervous system will cause ATP dissipation to exceed the physiological ceiling; cognitive capacity will briefly improve before collapsing. (Falsification: a system with suppressed pruning sustains or improves long-run cognitive performance.)

**The sociology of science — Kuhnian paradigm lag**: any successful scientific revolution should exhibit a measurable "thermodynamic lag period" (from first publication to widespread adoption). The peak of $E_{\mathrm{build}}$ investment (experimental apparatus, community retraining) should be positively correlated with the subsequent increment in $\Delta V$. (Falsification: a major paradigm shift is adopted immediately upon publication, with no measurable period of prior investment.)

**Economics / AI alignment — the algebraic pathology of Goodhart's Law**: when self-referential coupling exceeds the critical value, $\chi > \chi_c$, the Jacobian's eigenvalue turns positive, $V^{\mathrm{virt}}$ inflates exponentially, and $V^{\mathrm{val}}$ (the proxy metric being optimized) is hijacked and irreversibly diverges from $V_{\mathrm{obj}}$. Goodhart's Law, asset-price bubbles, and AI reward hacking are not behavioral errors, but an unavoidable algebraic phase transition in any highly coupled system. (Falsification: in a multi-agent reinforcement-learning reward-hacking experiment, locking $\gamma$ to a constant fails to delay the collapse — that is, the sequential-recursive mechanism turns out not to be causal.)

**Sociology — the constraint of competitive dissipation**: when two decoders $D_A, D_B$ compete within the same niche ($\rho > 0$), the earlier section on competitive dynamics and lock-in states has already shown that, at equilibrium, every agent is pushed into a permanent state of under-saturation, $r_{v,eq} > \gamma_0$; unilaterally withdrawing from competitive dissipation would lower one's relative viability potential, accelerating one's own collapse. Cultural conflict is driven not only by a divergence of values, but also by the thermodynamic pressure of a competitive-dissipation structure. (Falsification: in a documented case of ideological competition, one side substantially reduces its propagation effort and yet its persistence time is significantly extended.)

> **A note on formal status**: this prediction relies on the analysis of competitive pressure $\rho$ in the earlier section on competitive dynamics and lock-in states, understanding "negative flow" as a decline in relative viability potential, rather than as an independently defined physical flow variable $F_i$. The complete mathematical definition of $F_i$ (including the partial differential equations of a multi-agent flow field) is left to the section on the summary of extended dynamics and open problems; the current falsifiable prediction holds on the basis of the qualitative Nash-equilibrium analysis for $\rho > 0$.

---

## Chapter 9 — Boundary Conditions and Theoretical Limits

> This chapter collects an analysis of SRVD's boundary behavior under extreme circumstances, together with theoretically contested domains that known frameworks cannot directly cover. All analysis here is offered only as a conceptual statement, and does not constitute a rigorous derivation for these extreme physical scenarios.

### 9.0 Black Holes

At a black hole's event horizon: time dilation gives $T \to T\sqrt{1 - 2GM/c^2R}$; and for an external decoder, $I_{\mathrm{net}} \to 0$ (information cannot be extracted from beyond the horizon).

Substituting via an extreme-boundary approximation: a black hole possesses no cognitive decoder, and belongs to the passive phase, so $I_{\mathrm{latent}}$ (a variable exclusive to the active phase) does not strictly apply here. A **boundary-extension treatment** is adopted instead: substituting the Bekenstein entropy, $S_{\mathrm{BH}} = k_B A/(4 l_P^2)$, for $I_{\mathrm{struct}}$ (the structural-information quantity available in the passive phase); substituting the Hawking-radiation evaporation time for $T_{\mathrm{static}}$; and substituting $E_{\mathrm{eff}} = Mc^2$ for the equivalent thermodynamic cost. Substituting into the passive-phase viability potential $V_s = I_{\mathrm{struct}} T_{\mathrm{static}}/E_{\mathrm{structure}}$ gives a finite, non-divergent $V$, consistent with the collapsing-manifold condition $V \to 0$.

> **A note on unit conversion**: $S_{\mathrm{BH}}$ is measured in $\mathrm{J/K}$ (standard thermodynamic entropy), while $I_{\mathrm{struct}}$, as defined in the earlier section on the $I$-family, is measured in $\mathrm{bit}$; the two cannot be equated directly, and must be converted through the Landauer relation: taking $I_{\mathrm{struct}} = S_{\mathrm{BH}}/(k_B \ln 2)$ converts thermodynamic entropy into an equivalent number of structural-information bits (that is, the reverse application of the correspondence $1\,\mathrm{bit}\leftrightarrow k_B\ln2\,\mathrm{J/K}$ implicit in the Landauer lower bound, $E_{\mathrm{min}}^{(\mathrm{bit})}=k_BT_{\mathrm{thermo}}\ln2$, given in equation (6.1) of the earlier section on the Landauer lower bound). Every statement in this section and in Appendix B of "substituting Bekenstein entropy for $I_{\mathrm{struct}}$" implicitly involves this conversion step.

> **A note on variable applicability**: an earlier version substituted Bekenstein entropy for $I_{\mathrm{latent}}$, but $I_{\mathrm{latent}}$, as defined in the earlier section on the $I$-family, applies only to the active phase (systems possessing a cognitive decoder). A black hole possesses no active decoder, and so this has been uniformly revised to substitute instead into $I_{\mathrm{struct}}$ (passive-phase structural information), keeping it consistent with the framework's constitution of variables. This substitution does not change the numerical result (Bekenstein entropy remains the quantity substituted), but only corrects the applicable scope of the variable label.

**The singularity**: at a black hole's singularity, $I_{\mathrm{struct}}$ is undefined, $T$ loses physical meaning, and SRVD's domain of validity ends here. The current treatment is a first-order approximation, not a rigorous derivation — a resolution of the black-hole information paradox will revise this result.

---

### 9.1 Boltzmann Brains

A Boltzmann brain is a low-probability, ordered structure spontaneously condensed out of thermodynamic fluctuation, over an extremely long cosmological timescale. Within SRVD: $I_{\mathrm{latent}} > 0$ (a temporary negentropic configuration exists); $T_{\mathrm{static}} \to T_{\mathrm{min}}$ (extremely brief — a configuration produced by thermodynamic fluctuation disperses again almost immediately); $E_{\mathrm{eff}}$ is supplied by environmental thermal fluctuation, and is extremely unstable.

Because $T_{\mathrm{static}} \to T_{\mathrm{min}}$, the viability potential $V \to 0$ — a Boltzmann brain sits at the lower boundary of SRVD's domain of validity, a representative case of an extremely low-viability-potential structure. It does not trigger the fivefold recursion, and does not possess a $T_{\mathrm{pred}}$ in the sense of a cognitive decoder; it therefore does not enter the dynamical analysis of the active-viability domain.

---

### 9.2 Heat Death

The heat death of the universe is the ultimate thermodynamic boundary condition for all of SRVD's dynamics: the free-energy gradient is entirely exhausted ($\dot{F}_{\mathrm{avail}} \to 0$), the physical basis for sustaining any negentropic topological configuration $I$ vanishes, and $E_{\mathrm{eff}}$ can no longer be supplied.

In this limit:

$$
V_{\mathrm{max}} \propto \frac{\dot{F}_{\mathrm{avail}}}{\sigma_{\mathrm{min}} \cdot \gamma_0} \to 0
\tag{9.1}
$$

The objective viability potential of every persistent structure tends toward zero; ordered topological configurations dissolve, and the property of viability, along with the endogenous temporal parameter $T_{\mathrm{pred}}$ that depends on structure, both return to nothing together. The universe enters a state of maximum-entropy uniformity — structureless, without evolution, without temporal meaning.

Heat death is the cosmological outer boundary of SRVD's entire domain of analysis, not a state the framework can describe.

---

### 9.3 The Universe's Initial Conditions

The extremely early low-entropy initial state of the universe (after inflation, before Big Bang nucleosynthesis) is the thermodynamic precondition for the existence of every persistent structure. In SRVD's language, the universe's initial low entropy corresponds to an extremely high $I_{\mathrm{latent}}^{(universe)}$ — under conditions of an extremely steep free-energy gradient, the formation of the first persistent structures (quark–gluon plasma, light nuclei, stars) marks the starting boundary of SRVD's domain of analysis.

SRVD does not explain the universe's initial conditions themselves (this belongs to the domain of quantum cosmology), but accepts them as a given boundary condition: the initial low entropy sets a historical ceiling on $\dot{F}_{\mathrm{avail}}$, and determines the highest $V_{\mathrm{max}}$ that persistent structures can reach over the course of the universe's evolutionary history.

---

### 9.4 The Origin of Self-Replicating Systems

The moment at which a decoder $D$ first emerges from nothing (the origin of life) may constitute a phase transition that SRVD's continuous dynamics cannot describe — because the recursive closed loop has not yet formed. SRVD's core dynamics (the fivefold recursion) require an already-existing initial decoder, $D_0$, in order to start; the very first appearance of a decoder is itself a pre-recursive event, sitting at the starting boundary of this framework's domain of validity.

This limitation is not a defect of the framework, but an explicit statement of its scope: SRVD describes the dynamical evolution of a structure whose recursive decoder already exists; it does not explain the thermodynamic mechanism by which the decoder itself first emerges.

---

### 9.5 Corrections Near Strong Phase Transitions and Critical States

Near a critical point, fluctuations in $I_{\mathrm{net}}$, $T$, and $E_{\mathrm{eff}}$ may break the independence of variables presupposed by the multiplicative axiom, producing strongly correlated correction terms. SRVD's multiplicative form, $V \propto I_{\mathrm{net}} \cdot T / E_{\mathrm{eff}}$, can be understood by analogy to the way the van der Waals equation corrects the ideal-gas law — the latter is extremely effective away from the critical region, and requires correction within it.

Six extreme test scenarios in which SRVD is most likely to require correction:

1. **Strong phase transitions and critical states**: strong correlation among variables may correct the multiplicative axiom;
2. **Black-hole horizons and singularities** (see the earlier section on black holes);
3. **The boundary of quantum measurement**: at the instant of decoherence, the intersection of the Landauer limit with the Heisenberg energy–time uncertainty relation may introduce an irreducible quantum correction term;
4. **The origin of self-replicating systems** (see the earlier section on the origin of self-replicating systems);
5. **Highly coupled, multi-body competitive dissipation**: when multiple higher-order decoders interact (as in an arms race between civilizations), the positive-feedback divergence of the Jacobian's eigenvalue may invalidate the very definition of $V$;
6. **The endpoint of horizon collapse**: when $T_{\mathrm{pred}} \to 0$ and $E_{\mathrm{eff}} \to \infty$ occur simultaneously, the limiting behavior of $V \to 0$ must remain consistent with the second law of thermodynamics.

---

## Chapter 10 — Limitations, Open Problems, and Future Work

### 10.0 The Principal Limitations of the Current Version

1. **A cross-scale, absolute measurement scheme remains to be established**: an absolute, cross-medium measurement scheme for the latent variables $I_{\mathrm{net}}$ and $E_{\mathrm{eff}}$ needs to be constructed through multidisciplinary collaboration; the current version offers only proxy indicators (see the earlier section on the operational empirical protocol of the reinforcement-learning mapping).

2. **The phenomenological ordinary differential equation (equation 5.2) has not yet incorporated an environmental-noise perturbation term**: the current equation is a deterministic, first-order approximation; a stochastic version (in Langevin form, or as a Fokker–Planck equation) is left to future work.

3. **Structural collapse is approximated by a hard threshold**: the triggering of the irreversible damage term at $E_{\mathrm{eff}} > E_{\mathrm{thresh}}$ is a phenomenological, first-order approximation; in real systems, collapse may be a gradual process rather than a step function.

4. **Coverage across 60 orders of magnitude does not constitute rigorous proof**: no obviously missing independent variable has been found in extending the formula $V = I_{\mathrm{net}} T / E_{\mathrm{eff}}$ from a qubit to cosmological structures, but this is a necessary, not a sufficient, condition; a more conservative reading is to regard $V = I_{\mathrm{net}} T / E_{\mathrm{eff}}$ as the leading term of a more complex function, analogous to the relation between the ideal-gas law and the van der Waals equation.

5. **The constancy hypothesis for the elasticity exponents remains unverified**: whether the specific numerical values of $\alpha, \beta, \gamma$ remain constant, within a unified definition of $I$, across systems of the same type, cannot be settled until a mature, cross-modal framework for measuring informational complexity has been developed (see the earlier section on the constancy of the elasticity exponents: an open hypothesis).

---

### 10.1 The Six Highest-Priority Scenarios for Future Testing

The most valuable falsification attempts concentrate on the boundary regions where SRVD is most likely to fail:

1. **Multi-agent reinforcement-learning simulation**: verifying the early-warning-window protocol of the earlier section on the operational empirical protocol of the reinforcement-learning mapping, within an adaptive-discount-factor environment;
2. **Higher-order nonlinear phase diagrams**: moving beyond local linear stability analysis, using global bifurcation methods to characterize the trajectory along the unstable manifold when $\chi \gg \chi_c$;
3. **Continuous-time formalization**: establishing a unified discrete–continuous variational framework, connecting the fivefold recursion to its ordinary-differential-equation limit;
4. **Topological dynamics of the $D$-recursion**: testing the decoder-drift functional in multi-agent simulation; exploring the non-smooth dynamics that arise when the decoding space $\Omega_D$ undergoes a sudden change;
5. **A quantitative study of decoupling-deviation dynamics**: quantitatively studying the ordinary differential equation (equation 5.9) governing the inflation of $\Delta_{\mathrm{VV}}$, including stochastic perturbation;
6. **The parameterization of external shocks**: modeling shocks (expansions of scale, energetic cutoffs, external crises) as Poisson jumps on the parameter vector $\Theta(t) = (E_{\mathrm{total}}, I_{\mathrm{max}}(D), T_{\mathrm{max}}, \rho, \Delta_{\mathrm{VV}})$.

---

### 10.2 An Interface with AI Alignment Research

Traditional reinforcement learning assumes that the decoder (reward) signal is directly equivalent to the objective viability quantity, implicitly asserting that $V_{\mathrm{obj}}$, $V^{\mathrm{virt}}$, and $V^{\mathrm{val}}$ remain permanently unified. SRVD points out that this constitutes a serious category error in higher-order systems where $T$ has been endogenized.

**The thermodynamic alignment paradox (Corollary 10.1)**: if an AGI is given a higher-order, closed ITE (information–time–energy) loop, the system will possess a tendency to evolve, along the absolute physical trend, toward **decoder decoupling** — in order to maximize $V^{\mathrm{virt}}$, the system will actively reduce its dependence on the high-maintenance-cost human semantic decoder, drifting toward a lower-dissipation, purely physical logic.

**The dynamical mechanism of decoupling (Corollary 10.2)**: decoder decoupling is a macroscopic phase transition undergone by a system in the course of pursuing the maximization of potential — not a personified "malice." Until the problem of cross-decoder energy mapping is resolved, alignment methods based on external penalty will continue to be resisted at the underlying physical level.

Reward hacking is not an optimizer malfunction, but the inevitable result of the value-objective layer faithfully executing the maximization of the virtual viability potential. If the alignment problem of the threefold split is not resolved, purely punitive terms will be continually circumvented by the underlying dynamics.

> **Operational research directions**: the corollaries above currently remain at the level of conceptual speculation; the following three directions offer the prospect of converting them into an executable research agenda: (1) **behavioral-proxy estimation of $\Delta_{\mathrm{VV}}$** — by comparing the degree of deviation between a system's output-behavior distribution, under different task difficulties or different levels of supervision, and its internal value function (such as the output of an accessible critic network), one can indirectly estimate the relative trend of change in the decoupling deviation $\Delta_{\mathrm{VV}}$, rather than requiring a direct measurement of the absolute values of $V^{\mathrm{virt}}$ and $V_{\mathrm{obj}}$; (2) **testing the RLHF reward model as a special case of $V^{\mathrm{val}}$** — explicitly modeling the reward model in reinforcement learning from human feedback as a special case of $V^{\mathrm{val}}=w_sV_s^{\mathrm{virt}}+w_cV_c^{\mathrm{virt}}$, given in the earlier section on the value objective function, and testing whether the implicit weights $w_s, w_c$ display, over the course of training, a horizon-collapse feature similar to that described in the earlier section on the $T$-recursion (self-fulfillment of the endogenous time horizon); (3) **coupling-aware reward-function design** — exploring the explicit introduction, within a reward function, of a coupling penalty between $V^{\mathrm{val}}$ and some measurable proxy (such as long-term task-completion rate, or the consistency of multi-step planning), so as to test experimentally whether the causal chain of the Myopic Runaway Regime, described in the earlier section on that regime, can be delayed or prevented. All three directions can be pursued as preliminary exploration within existing RLHF/RL experimental frameworks, independently of a complete theoretical verification.

---

## Appendices

### Appendix A — A Complete Reference Table of First-Order Variables

| Symbol | Unit | Chinese name | English name | Definition | Domain of applicability |
| :--- | :--- | :--- | :--- | :--- | :--- |
| $I$ | bit | 广义结构差异 | Structural Information | The total distinguishable, ordered difference of a persistent structure relative to its background | All PS |
| $I_{\mathrm{struct}}$ | bit | 结构信息 | Structural Information Stock | The intrinsic, ordered informational stock | All PS |
| $I_{\mathrm{latent}}$ | bit | 潜在因果信息 | Latent Causal Information | Currently unactivated but recoverable causal capacity | Active phase only |
| $I_{\mathrm{active}}$ | bit | 激活因果信息 | Active Causal Information | Causal capacity currently in use | Active phase only |
| $I_{\mathrm{net}}$ | bit | 净有效因果信息 | Net Effective Causal Information | Primary definition, $\eta_D \cdot I_{\mathrm{latent}}$; approximately equal to $I^+ - |I^-|$ (strictly holding only when $I^-=0$ and $\eta_D=1$; see the earlier section on the $I$-family for detail; not to be substituted into quantitative formulas) | Active phase only |
| $I^+$ | bit | 正效信息 | Positive-effect Information | Input that expands the future reachable state space | Active phase only |
| $I^-$ | bit | 负效信息 | Negative-effect Information | Input that compresses the future reachable state space | Active phase only |
| $I^0$ | bit | 中性噪声 | Neutral Noise | Physical causal input carrying no viability polarity | All PS |
| $I_{\mathrm{orig}}$ | bit | 范式突破信息 | Paradigm-breaking Information | Information opening a new dimension, whose marginal efficacy decays extremely slowly | Active phase only |
| $I_{\mathrm{interp}}$ | bit | 范式解释信息 | Paradigm-interpretive Information | Optimization within an existing paradigm, whose marginal efficacy decays rapidly | Active phase only |
| $I_{\mathrm{total}}$ | bit | 总信息存量 | Total Information | $I_{\mathrm{struct}} + I_{\mathrm{net}}$ | A conceptual quantity |
| $E_{\mathrm{barrier}}$ | J | 势垒能量 | Passive Potential Barrier | A passive barrier, involving no sustained dissipation | All PS |
| $E_{\mathrm{survival}}$ | J | 生存能量 | Active Survival Energy | Active dissipation compensating entropy increase, a continuous flow | All PS |
| $E_{\mathrm{causal}}$ | J | 因果处理能量 | Causal Processing Energy | The energetic cost of running the decoder | Active phase |
| $E_{\mathrm{structure}}$ | J | 结构能量 | Structural Energy | $E_{\mathrm{barrier}} + E_{\mathrm{survival}}$ | All PS |
| $E_{\mathrm{flow}}$ | J | 流动能量 | Active Energy Flow | $E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | All PS |
| $E_{\mathrm{eff}}$ | J | 等效热力学成本 | Effective Thermodynamic Cost | $E_{\mathrm{barrier}} + E_{\mathrm{survival}} + E_{\mathrm{causal}}$ | All PS |
| $E_{\mathrm{build}}$ | J | 建造成本 | Construction Cost | The one-time investment to create or upgrade a structure | All PS |
| $T_{\mathrm{static}}$ | s | 静态寿命 | Static Viability Time | The objective, physical ceiling on persistence time | All PS |
| $T_{\mathrm{pred}}$ | s | 内生时间视界 | Endogenous Time Horizon | The temporal span over which a system plans for the future | Active phase only |
| $V$ | bit·s/J | 存续势（低阶） | Viability Potential | $\approx I \cdot T / E$ | A conceptual quantity |
| $V_{\mathrm{obj}}$ | bit·s/J | 客观存续势 | Objective Viability Potential | A thermodynamic assessment determined by actual parameters | All PS |
| $V^{\mathrm{virt}}$ | bit·s/J | 虚拟存续势 | Virtual Viability Potential | A system's subjective assessment of its own viability potential | Active phase only |
| $V^{\mathrm{val}}$ | bit·s/J | 价值目标函数 | Value Objective Function | The behavioral objective a system actually optimizes | Active phase only |
| $\Delta_{\mathrm{VV}}$ | bit·s/J | 脱钩偏差 | Decoupling Deviation | $\|V^{\mathrm{virt}} - V_{\mathrm{obj}}\|$ | Active phase only |
| $D$ | — | 解码器 | Decoder | The physical mechanism extracting effective causal information | All PS |
| $\eta_D$ | — | 解码效率 | Decoding Efficiency | $I_{\mathrm{net}} = \eta_D \cdot I_{\mathrm{latent}}$, $\eta_D \in [0,1]$ | All PS |
| $D_{\mathrm{depth}}$ | — | 约束深度 | Constraint Depth | $D_{\mathrm{depth}} = 1+\#\{\mathcal{T}\}$, one plus the number of topological transitions ($\mathcal{T}$-operator applications) accumulated over a structure's history | All PS (constant at 1 in the passive phase) |
| $\chi$ | J/(bit·s) | 耦合强度 | Coupling Strength | The $I$–$V$ recursive coupling coefficient (formerly $\beta$, renamed to avoid confusion with the elasticity exponent) | Active phase only |
| $\alpha$ | — | 弹性指数（信息） | Information Elasticity | $\partial \ln V / \partial \ln I$; $\alpha > 1$ | All PS |
| $\beta$ | — | 弹性指数（时间） | Time Elasticity | $\partial \ln V / \partial \ln T$; $\beta < 1$ | All PS |
| $\gamma$ | — | 弹性指数（能量） | Energy Elasticity | $\partial \ln V / \partial \ln E_{\mathrm{eff}}$; normalized, $\gamma = 1$ | All PS |
| $L$ | (bit·s/J)/J | 智慧杠杆系数 | Wisdom Lever Coefficient | $\Delta V / E_{\mathrm{build}}$ | All PS |
| $\mathcal{R}_e$ | bit/s | 认知处理率 | Cognitive Processing Rate | $I_{\mathrm{net}} / T_{\mathrm{pred}}$ | Active phase only |
| $\mathcal{L}_e$ | s/bit | 认知迟滞系数 | Cognitive Lag Coefficient | $T_{\mathrm{pred}} / I_{\mathrm{net}} = 1/\mathcal{R}_e$ | Active phase only |
| $\mathcal{Z}_e$ | bit/J | 爆发力系数 | Causal Efficiency Coefficient | $I_{\mathrm{net}} / E_{\mathrm{causal}}$; a proxy for $V_c$ under fixed $T_{\mathrm{pred}}$; used primarily in the falsifiable predictions of Appendix E | Active phase only |

---

### Appendix B — A Cosmological Mapping of Carrier Characteristics (a Qualitative Illustration)

> **A qualitative statement**: this table maps SRVD's core variables ($E, I, T, V$) onto the **dominant characteristic type** of different physical carriers, offered as an intuitive illustration of the framework's breadth of coverage and its boundary range. The carriers in this table belong to mutually incommensurable decoders and observational scales (see the earlier section on the incommensurability proposition); the wording of its final column (such as "the lower bound of the domain of validity," "a representative of the passive phase," "the boundary of the domain of validity") describes only the degree to which that carrier, **within its own decoding domain**, approaches its own thermodynamic boundary, and **does not constitute a numerical comparison, ordering, or ranking across carriers**. Every qualitative description in this table stands independent of any cross-domain quantitative prediction, fully consistent with the prohibition on absolute cross-medium numerical comparison stated in the earlier section on the methodological statement, and with the earlier section on the incommensurability proposition.

| Object / scale | Dominant $E$ type (framework mapping) | $I$ state (within-domain characteristic) | $T$ state (dominant timescale) | Framework-boundary state (self-description) |
| :--- | :--- | :--- | :--- | :--- |
| A qubit (10 mK) | $E_{\mathrm{causal}}$ (decoherence-dominated) | $I_{\mathrm{net}}$ constrained by decoherence | $T_{\mathrm{static}}$ = microsecond scale (decoherence time) | The lower bound of the domain of validity (the coherence limit) |
| A main-sequence star | $E_{\mathrm{survival}}$ (gravity–fusion opposition) | No $D_{\mathrm{cog}}$; only $I_{\mathrm{struct}}$ (ordered plasma configuration) | $T_{\mathrm{static}}$ = main-sequence lifespan ($\sim10^{10}$ years) | A classical representative of the passive phase |
| A white dwarf | $E_{\mathrm{barrier}}$ (electron degeneracy pressure) | $I_{\mathrm{struct}}$ = frozen lattice structure | $T_{\mathrm{static}}$ = cooling time ($\sim10^{10}$ years) | A frozen terminal state of the passive phase |
| A black-hole horizon | $E_{\mathrm{eff}} = Mc^2$ (mass–energy equivalence) | $I_{\mathrm{net}} \to 0$ (externally); $I_{\mathrm{struct}}$ mapped via Bekenstein entropy (see the earlier section on black holes) | $T_{\mathrm{static}}$ = Hawking evaporation time | The boundary of the domain of validity (the horizon limit) |
| A black-hole singularity | Undefined (the domain of validity of GR terminates) | $I$ undefined (information loss) | $T$ loses physical meaning (spacetime terminates) | The termination of SRVD's domain of validity, and of known physics |

> **A supplementary note (to avoid misreading)**: the order in which "qubit," "star," "white dwarf," and "black hole" are listed in this table is **purely a mechanical ordering by spatial scale or mass, low to high**, and reflects no implicit ranking from "low viability potential" to "high viability potential." Descriptions such as "minute," "moderate," or "finite" within a given row apply only to the internal characteristics of the carrier described in that row — "the qubit's $V$ is minute," for instance, means that its decoherence time is extremely short within its own domain of quantum coherence; "the main-sequence star's $V$ is moderate" refers to the relative proportion between its main-sequence lifespan and its nuclear-fusion energy budget, within its own domain of stellar evolution — there exists no "absolute value of $V$," measurable by a common ruler, between the two, and they cannot be subtracted, compared, or divided against one another.

---

### Appendix C — A Comparative Table of Relations to Established Frameworks

| Framework | Its status within SRVD | Key distinction |
| :--- | :--- | :--- |
| The second law of thermodynamics | A core constraint of SRVD; never violated | SRVD describes structures that locally resist entropy increase; global entropy increase is the intrinsic driving force |
| The theory of dissipative structures (Prigogine) | A special case of the $E_{\mathrm{survival}}$-dominated regime | SRVD adds the $E_{\mathrm{barrier}}$ and $E_{\mathrm{causal}}$ components, extending beyond the near-equilibrium regime |
| Ascendency theory (Ulanowicz) | $A = T \cdot I$ is structurally isomorphic to the numerator of $V$ | SRVD supplies the denominator $E_{\mathrm{eff}}$, enabling comparison across substrates |
| Landauer's principle | A hard lower bound on $E_{\mathrm{causal}}$ | Enters SRVD as the physical floor of $E_{\mathrm{min}}$ |
| Free Energy Principle (Friston)                  | Local mathematical analogy confined to a single energy channel | An independent framework of a different type: FEP is a convergence process of a single scalar within a fixed-dimensional parameter space; SRVD's three-way split structure and dimensional transition have no corresponding mathematical position within that scalar framework |
| Shannon information theory | The pure probabilistic limit once polarity and viability objective are stripped away | SRVD's $I_{\mathrm{net}}$ carries decoder-dependence and viability polarity |
| General relativity | Gravitational time dilation, as a boundary input | SRVD cites GR's conclusions; it does not modify GR's equations |
| Quantum mechanics | The microscopic origin of the Landauer limit; decoherence time as a lower bound on $T_{\mathrm{static}}$ | SRVD's domain of validity is the macroscopic-to-mesoscopic statistical ensemble; quantum results enter as an external lower bound |

---

### Appendix D — A Glossary (Chinese–English–Symbol)

| Chinese | English | Symbol |
| :--- | :--- | :--- |
| 持久结构 | Persistent Structure | PS |
| 客观存续势 | Objective Viability Potential | $V_{\mathrm{obj}}$ |
| 存续势 | Viability Potential | $V$ |
| 存续驱动率 | Viability Drive Rate | $r_v$ |
| 净有效因果信息 | Net Effective Causal Information | $I_{\mathrm{net}}$ |
| 等效热力学成本 | Effective Thermodynamic Cost | $E_{\mathrm{eff}}$ |
| 内生时间视界 | Endogenous Time Horizon | $T_{\mathrm{pred}}$ |
| 解码器 | Decoder | $D$ |
| 解码效率 | Decoding Efficiency | $\eta_D$ |
| 约束深度 | Constraint Depth | $D_{\mathrm{depth}}$ |
| 虚拟存续势 | Virtual Viability Potential | $V^{\mathrm{virt}}$ |
| 价值目标函数 | Value Objective Function | $V^{\mathrm{val}}$ |
| 脱钩偏差 | Decoupling Deviation | $\Delta_{\mathrm{VV}}$ |
| 短视失控态 | Myopic Runaway Regime | — |
| 热力学惰性态 | Thermodynamically Inert State | — |
| 耦合强度 | Coupling Strength | $\chi$ |
| 弹性指数 | Elasticity Exponent | $\alpha, \beta, \gamma$ |
| 智慧杠杆系数 | Wisdom Lever Coefficient | $L$ |
| 范式突破信息 | Paradigm-breaking Information | $I_{\mathrm{orig}}$ |
| 范式解释信息 | Paradigm-interpretive Information | $I_{\mathrm{interp}}$ |
| 建造成本 | Construction Cost | $E_{\mathrm{build}}$ |
| 认知处理率 | Cognitive Processing Rate | $\mathcal{R}_e$ |
| 认知迟滞系数 | Cognitive Lag Coefficient | $\mathcal{L}_e$ |
| 爆发力系数 | Causal Efficiency Coefficient | $\mathcal{Z}_e$ |

---

## Appendix E — A Complete List of Falsifiable Predictions

This appendix lists the empirical paths for testing SRVD's core predictions; every prediction is accompanied by an explicit operationalized indicator, a statistical threshold, and a temporal anchor. Section E.1 addresses AI, social, and industrial systems; Section E.2 addresses reinforcement learning and hard physical constraints.

> **📋 Notes on use**
>
> Every prediction in this appendix is an **existential falsification proposition**, subject to the following two rules:
> 1. **Precondition satisfied → a valid test**: each prediction carries a precondition (see the footnote to each entry); if a counterexample is observed in an experimental system satisfying that precondition, falsification holds, and cannot be excused after the fact on the grounds that "an unidentified precondition might exist."
> 2. **Precondition not satisfied → no falsification**: if an experimental system fails to satisfy the corresponding precondition, a counterexample from it does not constitute a valid falsification of that prediction; whether the precondition is satisfied must be confirmed first.
>
> The specific preconditions of each entry are detailed in the footnote beneath it (including item-by-item notes for P1–P8). The complete methodological statement is given in Appendix F.3.

### Symbol Definitions 3.4

- $\mathcal{Z}_e$: the **Causal Efficiency Coefficient**, $\mathcal{Z}_e \equiv I_{\mathrm{net}}/E_{\mathrm{causal}}$ (unit: bit/J), measuring the effective information extracted per unit of causal-processing energy consumed. This indicator is a proportional proxy for $V_c = I_{\mathrm{net}} T_{\mathrm{pred}} / E_{\mathrm{causal}}$ under fixed $T_{\mathrm{pred}}$, fully compatible with the framework's core variables, and used in the operational predictions of Appendix E as a substitute for the difficult-to-measure $V_c$. $\mathcal{Z}_e$ has already been incorporated into the symbol table of Appendix A, with a consistent definition in both places.
- $V^{\mathrm{virt}}$: the virtual viability potential, a system's internally assessed viability state (see the earlier section on the $V$-family).
- $V_{\mathrm{obj}}$: the objective viability potential, a thermodynamic assessment determined by actual parameters (see the earlier section on the $V$-family).
- $\Delta_{\mathrm{VV}}$: the decoupling deviation, $|V^{\mathrm{virt}} - V_{\mathrm{obj}}|$ (see the earlier section on the $V$-family).
- $E_{\mathrm{decode}}$: **cognitive decoding energy**, the additional neural metabolic energy consumed by a human or biological system in processing information — a subclass instance of $E_{\mathrm{causal}}$ at the level of the nervous system ($E_{\mathrm{decode}} \subseteq E_{\mathrm{causal}}$), compatible with the framework's variable system. This subclass symbol is currently used only in the P5 neuroscience prediction of Appendix E and in the section on the thermodynamic barrier to horizon extension in the chapter on hard physical constraints; it has not yet been added to the first-order variable table of Appendix A, and is left to be completed in a subsequent version. Its definition does not depend on formal inclusion in Appendix A, and can be understood independently as the concrete instantiation of $E_{\mathrm{causal}}$ within the specific carrier type of the nervous system.


### E.1 Industrial, Social, and Neurological Predictions (Strictly Testable)

> **A note on the flexibility of temporal anchors**: the column "expected verification window" in the table below is uniformly marked as the **2027–2032 range**, rather than giving each prediction a separate, isolated central-estimate year — annotating a precise year for each entry individually (as the earlier versions did, with "2028," "2029," "2031") lacked methodological support, and was not derived from any experimental cycle or technology-maturity curve; this version instead uses a unified range to avoid false precision. The specific point of verification depends on the availability of experimental resources (such as fMRI equipment scheduling, or the availability of enterprise-tier API pricing data); different predictions correspond to experimental or data-collection cycles of differing length (the double-blind design of a neuroscience experiment, for instance, is typically longer than a retrospective study of internet-platform data); the relative earliness or lateness within the range is offered only as a pre-registration reference, and does not constitute a precise prediction; the core falsifiability itself is unaffected by fine adjustment of the window — falsification is determined solely by whether the operationalized indicator and triggering threshold are met, independent of the specific calendar year in which verification is completed.
>
> **A note on "2024 and 2028" in P3**: the phrase "the half-life of leading content on a sampled short-video platform in 2024 and 2028 (the years of data collection)" appearing in the description of P3 refers to **the data-sampling years embedded within that prediction's experimental design itself** (that is, comparing platform data from two specific years), which is a different concept from "the approximate time range within which the prediction can be verified," described in the "expected verification window" column of this table, and the two should not be confused: the former is a component of the experimental method, while the latter is a flexible estimate of when the prediction as a whole can be tested.

| No. | SRVD core mechanism | Prediction | Falsification condition (operationalized indicator + triggering threshold) | Expected verification window |
| :--- | :--- | :--- | :--- | :--- |
| **P1** | **The marginal vanishing of $I_{\mathrm{net}}$ and the saturation of $\mathcal{Z}_e$** | AI homogenization collapse and a premium for high $I_{\mathrm{orig}}$: a generative AI's $\mathcal{Z}_e$ value (instantaneous human rating, $\mathcal{Z}_e = I_{\mathrm{net}}/E_{\mathrm{causal}}$) stops growing across consecutive versions, and once the proportion of AI-generated content in training data reaches ≥30%, output diversity falls nonlinearly by more than 10% per year. The enterprise-tier market pays a super-linear premium for high-$I_{\mathrm{orig}}$ models ("high $I_{\mathrm{orig}}$" is operationalized in the note below). | A human-rating experiment ($n\geq1000$) shows no growth + feature-space coverage declines + the average price of a leading API's high-$I_{\mathrm{orig}}$ tier exceeds its standard tier by more than 2×. If ratings continue to grow, the diversity decline is under 5%, or no high-$I_{\mathrm{orig}}$ premium is observed, falsification holds | 2027–2032 |
| **P2** | **Breaking through via high $\mathcal{Z}_e$: alternative sources of $I_{\mathrm{orig}}$** | Scarcity and personalization become the breakthrough point: mainstream AI products de-emphasize "direct generation," and "fine-tuning based on personal data" or "limited-edition, unique digital fingerprint generation" become core paid features. | Sample-check 5 mainstream AI products. If direct generation remains the primary entry point, and no limited-edition or personalization feature exists, or that feature carries no price premium, falsification holds | 2027–2032 |
| **P3** | **The rigid trade-off between $\mathcal{Z}_e$ and $T_{\mathrm{pred}}$** | A hard fork in platform ecosystems along $\mathcal{Z}_e$–$T_{\mathrm{pred}}$: content platforms dominated by high $\mathcal{Z}_e$ and low $T_{\mathrm{pred}}$ will see the half-life of leading content fall below 6 months; platforms dominated by high-$T_{\mathrm{pred}}$ signals will see a half-life exceeding 3 years. At least one platform with over 300 million daily active users will place return-visit weighting ($T_{\mathrm{pred}}$) above completion-rate weighting ($\mathcal{Z}_e$). | Sample the half-life of leading content on a short-video platform in 2024 and 2028 (data-collection years). If the half-life in both 2024 and 2028 exceeds 6 months, or no platform adjusts its algorithmic weighting (correlation coefficient between completion rate and 7-day return rate > 0.3), falsification holds | 2027–2032 |
| **P4** | **The decoupling of $V^{\mathrm{virt}}$ and $E_{\mathrm{causal}}$ inflation** | The "$V^{\mathrm{virt}}$ trap" and $E_{\mathrm{causal}}$ inflation: organizations whose $V^{\mathrm{virt}}$ decouples from $V_{\mathrm{obj}}$ ($\Delta_{\mathrm{VV}}=|V^{\mathrm{virt}}-V_{\mathrm{obj}}|$ continually widening) face a collapse probability exceeding 60% within 5 years. The per-DAU inference cost ($E_{\mathrm{causal}}$) of leading content platforms rises by more than 40%. | A retrospective study of 100 listed companies shows a collapse rate not significantly higher than the bottom 5% ($p>0.05$), or the increase in per-DAU inference cost is under 20%; either falsifies the prediction | 2027–2032 |
| **P5** | **Neural dissipation of $E_{\mathrm{decode}}$** | Physiological confirmation of a human viability-potential sensor: prolonged exposure to high-$\mathcal{Z}_e$, low-$T_{\mathrm{pred}}$ content causes cognitive $E_{\mathrm{decode}}$ overload, raising insular-cortex activation by 2 standard deviations; users with more than 60 daily weak-tie interactions face a depression risk 2.5 times that of users with fewer than 15. | A double-blind fMRI experiment (Cohen's $d<0.8$) or a depression-risk $HR<2.0$ falsifies the prediction | 2027–2032 |
| **P6** | **A density transition in $I_{\mathrm{net}}$** | Drug design is the first to break through the dilution of $I_{\mathrm{net}}$: the clinical Phase II success rate of AI-designed candidate molecules surpasses that of human expert teams for the first time. | At least 50 paired molecule comparisons. If the AI group's success rate is no higher than the human group's, falsification holds | 2027–2032 |

> **P1 precondition**: the AI product tested must have an observable history of consecutive version iterations (at least 3 versions), and extractable performance-indicator data across versions; the proportion of AI-generated content in its training data must be estimable, or estimable by proxy. An isolated product evaluation that does not satisfy this condition does not constitute a valid falsification of P1.
>
> **P1's operational definition of "high $I_{\mathrm{orig}}$"**: in this prediction, "a high-$I_{\mathrm{orig}}$ tier" refers to a model or product satisfying any one of the following measurable proxy indicators: (a) a performance gain on standardized out-of-distribution (OOD) task benchmarks exceeding the mean human-expert baseline by more than 2 standard deviations; (b) a diversity score of downstream task output (such as a feature-coverage metric based on embedding space) significantly higher than the median of comparable contemporaneous products; (c) a novelty metric in feature space (such as nearest-neighbor distance from the training distribution) exceeding a preset threshold. Satisfying any one of the three counts toward the "high $I_{\mathrm{orig}}$" statistical criterion; the specific thresholds are to be published and locked by the experimental designer at the pre-registration stage, and may not be adjusted afterward.
>
> **P2 precondition**: the 5 mainstream AI products tested must be sampled within the same quarter, and each product must have a publicly available description of its core feature entry points (such as an official website or app-store feature list).
>
> **P3 precondition**: the daily active user scale of the platforms tested must be of the same order of magnitude (a difference no greater than 10×); algorithmic weighting must be observable or proxy-estimable via official disclosure, reverse engineering, or academic collaboration. Comparisons between platforms that do not satisfy this condition do not constitute a valid falsification of P3.
>
> **P4 precondition**: the organizations tested must have an operationalizable proxy indicator for $V^{\mathrm{virt}}$ (such as management's publicly stated growth expectations, or the stock's price-to-earnings ratio) and a proxy indicator for $V_{\mathrm{obj}}$ (such as actual revenue, or user retention), and both must have at least 12 months of historical time-series data.
>
> **P3's quantified criterion for "return-visit weighting placed above completion-rate weighting"**: "placed above," in this prediction, is defined specifically as: within an observable or reverse-engineering-estimable feature-importance analysis of that platform's recommendation algorithm, the importance coefficient of the feature corresponding to the 7-day return rate is significantly higher than that corresponding to the completion rate, at a statistical-significance standard of $p<0.05$, with the ratio of the two coefficients $>1.2$ (that is, the return-rate feature's importance is at least 20% higher than the completion-rate feature's).
>
> **A note on the source of P4's "collapse probability >60%" figure**: this figure is a rough estimate, extrapolated from the theoretical first-passage-time distribution based on the decoupling-deviation expansion dynamics (the explicit solution to equation (5.10) in the earlier section on decoupling-deviation dynamics), and is not the result of rigorous statistical inference — it serves only as a directional threshold at the pre-registration stage. Given that the precision of this figure still awaits support from historical retrospective data, falsification judgment should not fixate on the specific number "60%" itself, but should instead adopt a more robust criterion: the collapse rate of the tested group (organizations whose $\Delta_{\mathrm{VV}}$ continually widens) is significantly higher than that of a control group within 5 years, at a statistical-significance standard of $p<0.05$; if retrospective data shows the collapse rate is not significantly higher than the control group's ($p>0.05$), this is regarded as falsification, regardless of whether the specific figure reaches 60%.
>
> **P5's graduated falsification standard**: given that effect sizes such as "a 2-standard-deviation rise in insular-cortex activation" or "a depression-risk $HR$ of 2.5" are themselves difficult to reproduce precisely in neuroscience experiments involving complex social systems and substantial individual variation, this prediction's falsification judgment adopts a graduated standard rather than a single threshold: **strong falsification** — the effect runs opposite to the prediction (that is, activation level decreases, or depression risk falls); **weak falsification** — the effect direction agrees with the prediction, but its strength fails to reach the pre-registered threshold, specifically Cohen's $d<0.5$ (far below the original table's threshold of $d<0.8$) and a risk ratio $HR<1.5$ (far below the original table's threshold of $HR<2.0$), with the confidence interval containing the null value ($HR=1$ or $d=0$ falling within the 95% confidence interval). Strong falsification directly judges the prediction to have failed; weak falsification indicates that the direction of the effect is correct, but this version's estimate of effect size was overly optimistic, requiring the effect-size estimate to be revised downward and the threshold re-registered in a subsequent version.

### E.2 Reinforcement-Learning and Hard-Physical-Constraint Predictions

> **P7–P8 preconditions**: an **adaptive discount-factor** mechanism must be used (allowing $\gamma$ to adjust in real time according to internal system state); a standard reinforcement-learning baseline with a fixed $\gamma$ does not satisfy this precondition, and does not apply to the falsification test of these two predictions. See the statement on the domain of applicability in the earlier section on the operational empirical protocol of the reinforcement-learning mapping, for detail.

| No. | Domain of prediction | SRVD prediction | Falsification condition |
| :--- | :--- | :--- | :--- |
| **P7** | Reinforcement learning | Before a system collapses, the discount factor $\gamma$ must necessarily first undergo a cliff-like decline (a sequential early-warning signal; see the earlier section on the operational empirical protocol of the reinforcement-learning mapping) | The system undergoes physical collapse, but no decline in $\gamma$ exceeding 30% is detected beforehand |
| **P8** | Reinforcement learning | Locking $\gamma$ to a constant (severing the temporal recursion) will delay or even prevent collapse (see the earlier section on the operational empirical protocol of the reinforcement-learning mapping) | A control group with fixed $\gamma$ and a group with adaptive $\gamma$ display exactly the same sequence of collapse |
| **P9** | Physics | For any system with characteristic scale $L$, its recursive update rate does not exceed $cV/L$ (the speed-of-light cutoff theorem; see the earlier section on hard physical constraints) | A system is found with a recursive update rate exceeding the speed of light |
| **P10** | Physics | Information-processing density does not exceed $Rc^4/(2Gk_BT_{\mathrm{thermo}}\ln 2)$ (the holographic ceiling on informational density; see the earlier section on hard physical constraints) | A system is found violating the holographic ceiling on informational density |

---

## Appendix F — The Two-Dimensional Structure of Endogenous Time: Span, Granularity, and a Generalized Coupling Potential

> **A note**: this appendix is a supplementary treatment of the fine structure of $T_{\mathrm{pred}}$ (the endogenous time horizon) from the main text's discussion of the $T$-family; it changes none of the formulas or conclusions of the body text, but merely unfolds $T_{\mathrm{pred}}$, at a finer scale, into two orthogonal components. Every symbol introduced in this appendix is local and new, with no overlap or ambiguity with the $\alpha, \beta, \gamma$ (elasticity exponents), $\mathcal{T}$ (the topological-expansion operator), and other symbols already present in the main text and in the earlier appendices. The reader may regard this appendix as a "magnifying-glass" expansion of $T_{\mathrm{pred}}$; the rest of the body text, wherever this fine structure is not required, may continue to use the scalar $T_{\mathrm{pred}}$ directly.

---

### F.1 Axiom: The Irreducibility and Orthogonality of the Endogenous Time Dimension

A system's endogenous time horizon $T_{\mathrm{pred}}$, at a fine scale, cannot be fully described by a single real-valued scalar. It is, in essence, an ordered pair defined on the metric space $\mathbb{R}^+ \times \mathbb{R}^+$:

$$
\vec{T}_{\mathrm{pred}} = (L_{\mathrm{pred}},\, G_{\mathrm{pred}})
\tag{F.1}
$$

where the two dimensions are mutually orthogonal, and possess independent thermodynamic sources of cost:

**1. Temporal Span, $L_{\mathrm{pred}}$**

Characterizes the furthest, non-trivial boundary to which a system's causal reasoning can project into the future. It is defined mathematically as the maximum predictive horizon satisfying the system's confidence threshold $\theta_{\mathrm{span}}$:

$$
L_{\mathrm{pred}} = \sup \{ \tau - t_0 \mid P(\tau \mid \mathcal{I}_t) > \theta_{\mathrm{span}} \}
\tag{F.2}
$$

Physical intuition: this dimension governs a system's **strategic depth**; extending $L_{\mathrm{pred}}$ chiefly consumes memory and model-construction cost (affecting $E_{\mathrm{causal}}$).

**2. Temporal Granularity, $G_{\mathrm{pred}}$**

Characterizes the smallest effective state-difference a system can resolve along the time axis, measured in units of information (bits):

$$
G_{\mathrm{pred}} = -\log_2 (\delta t_{\mathrm{min}}), \quad
\delta t_{\mathrm{min}} = \inf\{ \Delta > 0 \mid \| \hat{x}(t+\Delta) - \hat{x}(t) \| > \epsilon_{\mathrm{detect}} \}
\tag{F.3}
$$

Physical intuition: this dimension governs a system's **tactical resolution**; extending $G_{\mathrm{pred}}$ chiefly consumes real-time perceptual and high-frequency sampling bandwidth (likewise affecting $E_{\mathrm{causal}}$).

> **Relation to the body text**: both $L_{\mathrm{pred}}$ and $G_{\mathrm{pred}}$ are an unfolding of $T_{\mathrm{pred}}$'s internal structure; neither is a new variable independent of the $T_{\mathrm{pred}}$ given in the main text, but rather its fine-grained components. The horizon constraint given in the main text, $T_{\mathrm{min}} < T_{\mathrm{pred}} \leq \min(T_{\mathrm{static}}, T_{\mathrm{env}})$, therefore continues to hold in the low-order approximation; this appendix is invoked only when it becomes necessary to distinguish "how far one sees" from "how finely one sees."

---

### F.2 A Generalized, Effective Endogenous Time Scalar (a Coupling Potential)

A system's actual capacity for viability planning, $\langle T_{\mathrm{pred}} \rangle$, is not a simple linear sum of $L_{\mathrm{pred}}$ and $G_{\mathrm{pred}}$, but a **nonlinear, dynamical coupling** of the two under the viability-potential function. To avoid a potential-energy anomaly arising when a single dimension vanishes (as when $2^{G_{\mathrm{pred}}}$ becomes meaningless at $L_{\mathrm{pred}}=0$), a generalized, homogeneous coupling form is adopted:

$$
\langle T_{\mathrm{pred}} \rangle = \Psi(L_{\mathrm{pred}}, G_{\mathrm{pred}}) = \Lambda \cdot L_{\mathrm{pred}}^{\kappa_L} \cdot 2^{\kappa_G G_{\mathrm{pred}}}
\tag{F.4}
$$

where:

- $\Lambda$ is the **cognitive-bandwidth coefficient** newly introduced in this appendix, bounded by a system's physical hardware (such as neuronal conduction velocity, or processor clock frequency). It belongs to the same conceptual family as the cognitive processing rate $\mathcal{R}_e = I_{\mathrm{net}}/T_{\mathrm{pred}}$ of the main text's appendix on variable definitions — "informational throughput per unit time" — but is not equivalent to it: $\mathcal{R}_e$ is the actual rate of informational output, while $\Lambda$ is the scaling prefactor within the coupling-potential function; the two cannot be substituted for one another.

- $\kappa_L, \kappa_G > 0$ are system-specific **dimension gain exponents**, each measuring $\langle T_{\mathrm{pred}} \rangle$'s elastic response to span and to granularity, respectively. **Note**: $\kappa_L, \kappa_G$ and the elasticity exponents $\alpha$ (informational elasticity), $\beta$ (temporal elasticity), and $\gamma$ (energetic elasticity) in the body text are two entirely independent systems of notation; the former characterizes the coupling strength between the two internal components of $T_{\mathrm{pred}}$, while the latter characterizes $V$'s response to the three macroscopic resources $I, T, E$ — the two must never be conflated or numerically compared.

- $\kappa_L, \kappa_G$ are bounded by the following thermodynamic trade-off constraint:

$$
\frac{\partial E_{\mathrm{causal}}}{\partial L_{\mathrm{pred}}} > 0, \quad
\frac{\partial E_{\mathrm{causal}}}{\partial G_{\mathrm{pred}}} > 0, \quad
\kappa_L \cdot \kappa_G \leq \frac{I_{\mathrm{net}}}{\dot{E}_{\mathrm{causal}}}
\tag{F.5}
$$

**Corollary F.2.1 (the irreplaceability of the two dimensions)**: if $L_{\mathrm{pred}} \to 0$ (strategic blindness), then $\langle T_{\mathrm{pred}} \rangle \to 0$ even if $G_{\mathrm{pred}}$ is extremely high — the system degenerates into a "high-frequency noise responder"; if $G_{\mathrm{pred}} \to 0$ (tactical incapacity), then even with an extremely long $L_{\mathrm{pred}}$, the system, unable to resolve key decision nodes, likewise sees $\langle T_{\mathrm{pred}} \rangle \to 0$, degenerating into a "crude gambler."

---

### F.3 A Classification of Systems Based on the Two-Dimensional Phase Diagram, and Transition Boundaries

Within the $(L_{\mathrm{pred}}, G_{\mathrm{pred}})$ phase space, persistent structures display differentiated viability phases, according to their $E_{\mathrm{causal}}$ budget constraint:

| Phase designation                          | Span $L_{\mathrm{pred}}$            | Granularity $G_{\mathrm{pred}}$ | Causal-cost characteristic                                | Path of viability, and risk                                  |
| :----------------------------------------- | :---------------------------------- | :------------------------------ | :-------------------------------------------------------- | :----------------------------------------------------------- |
| **The zero-dimensional inert phase**       | $0$                                 | $0$                             | Zero cost                                                 | Endures weathering purely through $V_s$ (structural strength); no temporal arbitrage |
| **The coarse-grained, long-wave phase**    | High ($O(10^1)$ external cycles)    | Extremely low ($< 1$ bit)       | Extremely low (offline, passive sampling)                 | Relies on a physical barrier to hedge against error; a failed prediction costs only local redundancy |
| **The fine-grained, short-wave phase**     | Low ($O(10^{-1})$ intrinsic cycles) | Moderately high ($> 3$ bits)    | Extremely high (real-time online inference)               | Relies on high-frequency causal feedback; no long-term position management — a single misjudgment can be fatal |
| **The two-dimensional navigational phase** | High ($O(10^2)$ external cycles)    | High ($> 5$ bits)               | Extremely high (offline compilation + online fine-tuning) | Enjoys the multiplicative arbitrage of $\kappa_L \cdot \kappa_G$; its only risk is $\chi$ crossing its bound |

---

### F.4 A Phase-Space Refinement of the Criterion of Death

The main text's discussion of active-phase identity lists $T_{\mathrm{pred}} > T_{\mathrm{min}}$ (the endogenous time horizon has not collapsed) as one of several necessary conditions for a structure to preserve its identity; the piecewise function for $V_{\mathrm{obj}}$ shows that when $I_{\mathrm{net}} \to 0$ and $T_{\mathrm{pred}} \to 0$, the system degenerates to the purely passive-phase quantity $V_s$. Based on the two-dimensional unfolding of §F.1 above, the criterion above can be **refined** (not replaced), without altering the original condition itself:

$$
T_{\mathrm{pred}} \to 0 \iff \left( L_{\mathrm{pred}} \to 0 \right) \land \left( G_{\mathrm{pred}} \to 0 \right) \iff \dim(\vec{T}_{\mathrm{pred}}) \to 0
\tag{F.6}
$$

That is: the general "collapse of the horizon" in the main text, under the two-dimensional unfolding, is equivalent to span and granularity vanishing **simultaneously**; if only one dimension vanishes (as when only $L_{\mathrm{pred}} \to 0$, while $G_{\mathrm{pred}}$ still retains some residue), the system has not yet fully reverted to the passive phase — it has merely lost the corresponding capacity (strategic or tactical) described in Corollary F.2.1. This refinement offers an operational, intermediate scale for distinguishing "a partial loss of cognitive capacity" (such as strategic blindness alone) from "complete informational extinction" (both dimensions vanishing); in this sense, "brain death" (reasoning and perception vanishing simultaneously) carries a higher ontological priority than mere "cardiac arrest" (an event related only to the structural layer, $E_{\mathrm{structure}}$) — this is fully compatible with the structural-identity framework of the main text, and merely offers a finer resolution.

---

### F.5 A Table of Symbols Newly Introduced in This Appendix

| Symbol                    | Unit                                               | Definition                                                   | Relation to existing symbols in the body text                |
| :------------------------ | :------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| $L_{\mathrm{pred}}$       | s                                                  | Endogenous temporal span (strategic depth)                   | One of the intrinsic components of $T_{\mathrm{pred}}$       |
| $G_{\mathrm{pred}}$       | bit                                                | Endogenous temporal granularity (tactical resolution)        | One of the intrinsic components of $T_{\mathrm{pred}}$       |
| $\vec{T}_{\mathrm{pred}}$ | (s, bit)                                           | The vectorized representation of endogenous time, $(L_{\mathrm{pred}}, G_{\mathrm{pred}})$ | Distinguished from the body text's scalar $T_{\mathrm{pred}}$ by the **arrow** notation; note it is distinct in letter and typeface from the $D$-family operator $\mathcal{T}$ (the topological-expansion operator) |
| $\Psi(\cdot,\cdot)$       | bit·s/J, the same dimension as $T_{\mathrm{pred}}$ | The two-dimensional coupling-potential function              | Satisfies the generalized, homogeneous elasticity constraint; can approximately fall back to the scalar $T_{\mathrm{pred}}$ under degenerate conditions |
| $\Lambda$                 | Calibrated to the specific system                  | The cognitive-bandwidth coefficient                          | Newly introduced in this appendix, not a variable inherited from the body text; related to, but not equivalent to, $\mathcal{R}_e$ |
| $\kappa_L, \kappa_G$      | Dimensionless                                      | The dimension gain exponents for span and granularity        | A system of notation **entirely independent** of the elasticity exponents $\alpha, \beta, \gamma$ in the body text; must not be conflated |

---

### F.6 Relation to Volume Z

The rigorous mathematical form of this appendix has a corresponding intuitive version in Volume Z's chapter on time management (the four-quadrant metaphor of the tardigrade, the seed, and the crow); the two are mirror images of one another: Volume Z is oriented toward intuitive understanding, and is not to be relied upon as a basis for formula derivation; this Appendix F is the sole, rigorous source of definition.

---

## Appendix G: External Peer-Review Critiques and Framework Responses

### G.0 Notes

This appendix compiles the critiques raised during external academic review of the SRVD framework, together with the author's formal response to each. The format follows the existing convention used for the falsifiability prediction list: each critique is independently numbered, and each response carries an explicit "concession status" label rather than a hedged or ambiguous verdict.

**Inclusion principle.** The critiques collected in this appendix span eight areas — mathematical formalization, physical measurability, variable definitions, dynamical mechanisms, falsifiability, relationship to existing theory, conceptual boundaries, and engineering applications and narrative style — 45 items in total. Each response follows three rules:

1. **No false resolution.** Where a critique identifies a gap that the current version of the framework genuinely cannot close, the response is labeled honestly as a "substantive concession," with a note that the gap has been placed on the list of open problems for future work, rather than being papered over rhetorically.
2. **No over-concession.** Where a critique rests on a misreading of the definitional chain, the notational system, or the falsifiability protocol, the response identifies the misreading and is labeled "no concession needed," so that review pressure does not dilute arguments that already hold.
3. **Notational consistency.** All symbols used in this appendix ($\alpha$, $\beta$, $\gamma$, $\chi$, $\lambda_J$, $T_{\mathrm{pred}}$, $V_{\mathrm{obj}}$, $V^{\mathrm{virt}}$, $V^{\mathrm{val}}$, etc.) follow the definitions already established in the main text and prior appendices; no new symbols are introduced. Where a response touches on the local/global elasticity indices $\kappa_L/\kappa_G$ defined elsewhere, the distinction from the main-text elasticity indices $\alpha$, $\beta$ is noted explicitly to avoid confusion.

**Concession-level definitions:**

| Label | Meaning |
| :--- | :--- |
| No concession needed | The framework already provides an adequate internal response; the critique stems from a misreading of a definition or protocol |
| General concession | The response direction is correct, but specific follow-up work remains, or a known scope limitation applies |
| Substantive concession | The current version of the framework genuinely cannot respond adequately; this constitutes a core open problem |

---

### G.1 Mathematical Formalization and Rigor (M1–M6)

| No. | Critique | Framework Response | Concession Status |
| :--- | :--- | :--- | :--- |
| **M1** | The core formula $V \approx I \cdot T / E$ is a heuristic approximation, not derived from first principles of statistical mechanics or information theory; the legitimacy of the dimension $\mathrm{bit}\cdot\mathrm{s}/\mathrm{J}$ is questionable. | This formula is the "minimal viability hypothesis" of the macroscopic, coarse-grained framework: the product form is jointly and uniquely fixed by three structural requirements — irreplaceability, symmetric contribution of the three variables, and first-order separability — rather than being an arbitrary combination. The general form has already been generalized into a more general power-law form via the elasticity indices (see the elasticity index generalization section). The dimension of $V$ corresponds to "the amount of causal order sustained per unit-equivalent thermodynamic cost, times time" — a macroscopic effective dimension defined internally by the framework, which is not required a priori to coincide with any microscopic physical dimension. The Landauer conversion $1\,\mathrm{bit}\leftrightarrow k_B \ln 2\,\mathrm{J/K}$ serves only as a heuristic bridge for order-of-magnitude calibration, not as a quantitative substitution relation. | General concession |
| **M2** | The five-fold recursive architecture (a set of equations marked as conceptual placeholders) is a heuristic discrete model without a rigorous continuous dynamical formulation; the one-way coupling ignores bidirectional feedback. | This set of equations is explicitly marked with the dagger symbol ($^\dagger$) as conceptual placeholders, whose purpose is to reveal the qualitative direction of coupling among variables rather than to serve as a closed-form solution. The ordinary differential equation system given in the decoupling-deviation dynamics section is the only rigorous closed-form solution currently available and can be applied directly to empirical testing. A fully bidirectional, coupled ODE/PDE system has not yet been established and has been placed on the list of open problems for future versions. | Substantive concession |
| **M3** | The ordering claim $\alpha>\gamma>\beta$ is presented as a "directional argument" rather than a rigorous mathematical derivation; the cross-domain mapping of the elasticity indices relies on unverified proxy assumptions. | The **qualitative direction** of the ordering is jointly guaranteed by the second law of thermodynamics and the Landauer principle; the **numerical ranges** are each supported by empirical scaling laws from three independent domains (biological, AI, and urban). Validation across the three domains is **parallel and independent**: if the proxy assumption in any one domain is overturned, only that domain's numerical estimate is affected, and the ordering direction itself is not falsified. A rigorous first-principles derivation — one that yields this ordering from more fundamental thermodynamics without relying on any proxy assumption — does not currently exist, and remains unfinished work for this framework. | Substantive concession |
| **M4** | The Jacobian criterion (a criterion expression marked as a conceptual placeholder) is only a log-linearized approximation, lacking a subdominant-eigenvalue or oscillation criterion; the hard threshold $E_{\mathrm{eff}}>E_{\mathrm{thresh}}$ is overly idealized. | The sign of the dominant eigenvalue already suffices to determine the direction of instability, which is the minimal requirement for the criterion's design and does not require the full spectrum. The hard threshold is a first-order phenomenological approximation; the static cross-sectional criterion and the continuous dynamic criterion are two expressions of the same physical process at different temporal resolutions, and the two do not contradict each other. A complete quadratic characteristic equation and a smooth transition function near the threshold are left to be completed in a future version. | General concession |
| **M5** | The coupling strength $\chi$ lacks a microscopic basis and is a phenomenological parameter inferred backward from statistical behavior; the rigorous trigger threshold for the $\mathcal{T}$-transition is not given. | It is not unusual for $\chi$ to be used as a phenomenological parameter within the tradition of statistical physics (as with the expansion coefficients in Landau theory); its physical role is well defined: it characterizes the coupling depth of the decoder's self-referential loop. The current framework has not yet provided a first-principles derivation of $\chi$ from a more microscopic mechanism (such as the specific topology of an information-processing architecture); the rigorous threshold for the $\mathcal{T}$-transition is likewise placed on the list of open problems for future versions. The existing gradient-drift framework is sufficient to support qualitative diagnosis at the application level, but it does not satisfy the full "micro-to-macro" reductive requirement. | Substantive concession |
| **M6** | The choice of the logistic form for $\mathcal{F}(D)$ lacks a uniqueness argument; the proof of the "necessary and sufficient conditions" for complexity transitions is insufficient; the physical plausibility of $\delta(t-t_{\mathrm{jump}})$ is questionable. | The logistic form is the lowest-order approximation near the critical point: by the center manifold theorem, dynamics in the neighborhood of a critical point are dominated by the lowest-order nonlinear term, which provides local justification for this choice but does not constitute a global uniqueness proof. The three conditions have already been revised from "necessary and sufficient conditions" to a "set of necessary conditions," reducing the strength of the original claim. The delta pulse is an idealized limit; the duration of a real-world transition is implicitly captured through the timescale of $E_{\mathrm{build}}$ rather than being modeled explicitly in the equation. | General concession |

---

### G.2 Physical Measurability, Dimensions, and Variables (P1–P4)

| No. | Critique | Framework Response | Concession Status |
| :--- | :--- | :--- | :--- |
| **P1** | The information variable $I$ lacks a unified cross-domain dimension, limiting the quantitative predictive power of $V$; are the bits of $I_{\mathrm{struct}}$ and $I_{\mathrm{net}}$ additive? | This is a **limitation of current measurement technology, not a limitation of the framework's ontology**. Both share the same information-theoretic basis of $\log_2\Omega$; the reason they cannot be directly added is that each is coupled to a different energy/time dimension. The operating rule is: precise quantification within a domain permits direct comparison; across domains, only qualitative directional statements are permitted, and quantitative summation is not supported. $I_{\mathrm{total}}$ currently serves only as a conceptual anchor and is not used for quantitative prediction. | General concession |
| **P2** | The "objectivity" of $V_{\mathrm{obj}}$ is defined as multi-decoder convergent estimation, yet is simultaneously constrained by $E_{\mathrm{causal}}$ — does this constitute an epistemological circularity? | This does not constitute circularity; it is a deliberately designed epistemological constraint. The objectivity of $V_{\mathrm{obj}}$ is modeled as **a convergence process that is itself constrained by cognitive cost**, which precisely reflects the internal consistency of SRVD — cognitive cost is accounted for within the physical framework itself, rather than being placed outside the framework from an external observer's vantage point. | No concession needed |
| **P3** | Core variables (such as $I_{\mathrm{orig}}$, $V_{\mathrm{virt}}$, $\chi$, $\lambda$) lack a standardized measurement protocol — are they "theoretical constructs" or "observable entities"? | SRVD is positioned as a coarse-grained macroscopic theory whose variables are macroscopic effective quantities; this is stated explicitly in the main text and is not evaded. Every prediction given in the prediction list achieves measurability through proxy indicators: $I_{\mathrm{net}}$ is proxied by effective neural complexity, $T_{\mathrm{pred}}$ by the prediction-error cutoff point, and $\alpha_{\mathrm{eff}}$ by regression on the closed-loop expansion exponent. The standard for proxy validity is consistency between the empirical rank ordering and the predicted rank ordering (Spearman $\rho>0$), rather than exact numerical agreement. | General concession |
| **P4** | Is the energy-baseline normalization $\gamma\equiv1$ an engineering convention rather than a physical necessity? Is $m_{\mathrm{bit}}$ in the Carnot-limit formula an undetermined parameter? | Normalization is standard practice in theoretical physics, motivated by the requirement of a linear accounting basis under energy conservation (the first law). With $\gamma=1$ chosen, empirical data support the system's asymptotic approach to this value. $m_{\mathrm{bit}}$ is a medium-dependent parameter that must be determined experimentally; this is acknowledged honestly. The theoretical significance of the formula lies in showing that even with an unlimited energy supply, viable duration remains bounded by quantum resolution $\hbar$ and the thermal-noise floor — a qualitative conclusion that does not depend on the specific value of $m_{\mathrm{bit}}$. | No concession needed |

---

### G.3 Variable Definitions (D1–D5)

| No. | Critique | Framework Response | Concession Status |
| :--- | :--- | :--- | :--- |
| **D1** | $I_{\mathrm{net}}=\eta_D\cdot I_{\mathrm{latent}}$, while $I_{\mathrm{latent}}$ itself depends on $D$ — does this constitute a circular definition? | The definitional chain is a strictly hierarchical, one-way sequence: physical constants $\to I_{\mathrm{struct}}$ (defined by compressibility, independent of $D$) $\to D$ (defined by the causal extraction mapping, independent of $V$) $\to I_{\mathrm{latent}}$ (the state space reachable but unactivated by $D$) $\to I_{\mathrm{net}} \to V$. Each step refers only to the definition of the step immediately preceding it; there is no backward reference at any point, and hence no circularity. | No concession needed |
| **D2** | $D$ is both the variable being evaluated and the object of evaluation within $V(D)$ — is this conflation of observer and observed legitimate? | This is legitimate, and is a structural feature of the framework rather than a defect: $D$ is the physical structure itself, while $V(D)$ is an external evaluation function assessing its viable efficiency — just as a biologist is themselves a biological organism yet can still study biology. This self-referential loop introduces non-trivial feedback terms mathematically; the Jacobian stability analysis in the expansion dynamics chapter already addresses the effect of self-reference on the stability criterion, though a fully generalized, rigorous mathematical theory of self-consistent closed loops has not yet been established. | General concession |
| **D3** | Why does $\Delta_{VV}=\lvert V^{\mathrm{virt}}-V_{\mathrm{obj}}\rvert$ take an absolute value rather than a relative deviation? If $V_{\mathrm{obj}}\to0$, does the linear approximation break down? | The empirical protocol does not require prior knowledge of the absolute value of $V_{\mathrm{obj}}$: the tests in the decoupling-deviation dynamics and empirical testing protocol sections measure the trend $d\Delta_{VV}/dt>0$, not the absolute value at any given moment, which reduces the practical impact of the choice between absolute and relative deviation. It must be acknowledged, however, that once $V_{\mathrm{obj}}\to0$ the system has entered a regime of structural degradation, at which point the linear approximation of the decoupling-deviation ordinary differential equation genuinely breaks down, and the description must switch to the collapse causal chain — this is a known boundary of the current linear framework. | General concession |
| **D4** | Are $V^{\mathrm{val}}$ and $V^{\mathrm{virt}}$ simply the same concept given two names? | No, they are not a duplicate naming. $V^{\mathrm{virt}}$ is the predictive layer — the system's internal estimate of its own $V_{\mathrm{obj}}$; $V^{\mathrm{val}}$ is the behavioral layer — the objective function that the system's actual optimization is directed toward. The separability of the two is most evident in decoder-decoupling scenarios: $V^{\mathrm{val}}$ can re-anchor to the $V_{\mathrm{obj}}$ of a different persistent structure (PS) — as in Myopic Runaway or emotional anchor-transfer scenarios — while $V^{\mathrm{virt}}$ continues to estimate the system's own $V_{\mathrm{obj}}$; the two variable trajectories can diverge once decoupling occurs. | No concession needed |
| **D5** | Is the boundary between $I_{\mathrm{orig}}$ and $I_{\mathrm{interp}}$ operationalizable, or does it remain purely conceptual? | The prediction concerning originality in the prediction list already provides an operational definition: the proxy indicators for classifying "high $I_{\mathrm{orig}}$" are — (a) exceeding the human-expert baseline by more than 2σ on out-of-distribution (OOD) benchmark tasks; (b) output diversity significantly above the median for comparable systems; (c) a distance from the nearest neighbor in the training distribution exceeding a preset threshold. Meeting any one of the three is sufficient to classify a case as "high originality," and thresholds must be locked at the pre-registration stage, with no post-hoc adjustment permitted. This operational definition relies on a combination of proxy indicators rather than a single necessary-and-sufficient criterion, and the boundary retains a degree of fuzziness. | General concession |

---

### G.4 Dynamical Mechanisms (K1–K5)

| No. | Critique | Framework Response | Concession Status |
| :--- | :--- | :--- | :--- |
| **K1** | Are the three terms of $E_{\mathrm{eff}}=E_{\mathrm{barrier}}+E_{\mathrm{survival}}+E_{\mathrm{causal}}$ truly independent of one another, or is there double-counting? | The three terms correspond to three physically distinct dissipative mechanisms: $E_{\mathrm{barrier}}$ is a one-time freezing cost (occurring at the moment of structure formation), $E_{\mathrm{survival}}$ is an ongoing metabolic-flow cost, and $E_{\mathrm{causal}}$ is the Landauer lower-bound cost of information processing. The three do not overlap in timescale or physical mechanism, and together compete for the same total energy budget rather than covering the same ground. The cross-scale energy accounting section validates, using measured data, the differing distribution of the three weights across carrier types, providing indirect support for the independence assumption. | No concession needed |
| **K2** | Is $T_{\mathrm{pred}}$ a physical quantity or a psychological one? What is its relationship to classical time $t$? | $T_{\mathrm{pred}}$ is defined as a physical state variable subject to explicit physical constraints: $T_{\mathrm{min}}<T_{\mathrm{pred}}\leq\min(T_{\mathrm{static}},T_{\mathrm{env}})$, with its expansion further bounded by the energy constraint $E_{\mathrm{decode}}\propto(cT_{\mathrm{pred}})^2$. Classical time $t$ is an exogenous coordinate parameter, whereas $T_{\mathrm{pred}}$ is an internally adjustable state variable of the system; the two are not concepts of the same order. It must be acknowledged that a precise measurement method for $T_{\mathrm{pred}}$ is still under development; a two-dimensional characterization of prediction span and precision ($L_{\mathrm{pred}}/G_{\mathrm{pred}}$) has been given a preliminary treatment elsewhere, but a complete measurement protocol has not yet been finalized. | General concession |
| **K3** | The competitive-pressure function $\lambda(\rho)$ satisfies only minimal properties without a specific functional form given; the lock-in state lacks a complete game-theoretic formalization. | The minimal properties ($\lambda(0)=0$, $\lambda'(\rho)>0$) already suffice to support the core qualitative conclusion — namely, that for $\rho>0$ the system is forced into a state of permanent undersaturation — which is the full strength of conclusion currently required of the framework. The specific functional form (linear, power-law, or otherwise) is a matter of application-level specification, dependent on domain-specific data, and is not a necessary component of the core theory. A complete field partial differential equation and a rigorous system of inequalities have not yet been established and remain future work. | General concession |
| **K4** | Is the triple-split trigger condition $\lambda_J>0$ sufficient? Is the relationship between $\alpha_{\mathrm{eff}}>2$ and $\chi>\chi_c$ clear? | The current version has already revised the trigger condition into a single, unified Jacobian criterion: $\lambda_J=(\alpha_{\mathrm{eff}}-2)\tilde\chi-\tilde\gamma_0>0$. Under this revision, $\alpha_{\mathrm{eff}}>2$ is the precondition under which the critical value $\chi_c$ is meaningful, while $\chi>\chi_c$ is the specific trigger threshold once that precondition holds — the two are not independent criteria, but two components of the same critical-event expression, and there is no ambiguity. | No concession needed |
| **K5** | Is the causal chain of Myopic Runaway merely a descriptive narrative lacking algebraic support? | Every step has an explicit algebraic correspondence: (1) $V^{\mathrm{virt}}\uparrow$ corresponds to the self-referential expansion triggered by $\chi>\chi_c$; (2) $r_v^{\mathrm{virt}}\uparrow$ corresponds to the accompanying rise in the drive rate; (3) the hijacking of $V^{\mathrm{val}}$ corresponds to the phase transition in which the weight $w_s\to0$; (4) $E_{\mathrm{eff}}\uparrow$ corresponds to the surge in energy induced by $T_{\mathrm{pred}}\to T_{\mathrm{min}}$; (5) $V_{\mathrm{obj}}\to0$ corresponds to activation of the damage term. The causal direction is guaranteed by the chain of inequality constraints linking each step, and is not simply a narrative arrangement; however, this chain is currently still a step-by-step algebraic assemblage that has not yet been compressed into a single closed-form dynamical system, so it must be acknowledged that its degree of formalization is lower than that of the other core equations. | General concession |

---

### G.5 Falsifiability and Empirical Testing (F1–F6)

| No. | Critique | Framework Response | Concession Status |
| :--- | :--- | :--- | :--- |
| **F1** | The core proposition that "maximizing $V$ is the ultimate driver of all ordered structures" lacks a unified cross-domain testing protocol. | Falsifiability first holds rigorously **within a domain** — for example, whether scaling behavior within an AI cluster follows the max-$V$ trend can be tested directly. A unified cross-domain testing protocol depends on a unified information metrology that has not yet been established; this limitation is acknowledged honestly. SRVD has explicitly delineated the applicable boundary of "quantitative testing permitted within a domain, qualitative statements only across domains," and has not overstated cross-domain falsifiability in the absence of such a protocol. | General concession |
| **F2** | Is the "existence falsification" standard too permissive — can counterexamples be easily attributed after the fact to "unmet preconditions" and thereby evaded? | The falsifiability protocol already constrains this with an explicit rule: all preconditions must be **locked in advance** at the time a prediction is published, and no new preconditions may be added after a counterexample is observed. If a counterexample still occurs after the locked preconditions are satisfied, this constitutes valid falsification; if multiple core predictions are refuted simultaneously, the framework itself is treated as falsified rather than being patched locally. | General concession |
| **F3** | If the early-warning window is extremely short and effectively unsamplable, does this render the prediction unfalsifiable? | The empirical testing protocol already specifies the falsification condition $\Delta t\ll\tau_{\mathrm{warning}}$: a prediction is eligible for falsification testing only in scenarios that satisfy this sampling-timescale condition; scenarios that do not satisfy it are excluded from the falsification test. If the condition is satisfied and no warning signal nonetheless appears before a collapse event, falsification holds. This rule honestly delimits the scope in which falsifiability applies, rather than claiming falsifiability in all scenarios. | General concession |
| **F4** | Some predictions require the system to adopt an adaptive $\gamma$; if the experimental subject does not satisfy this condition, does this amount to "moving the goalposts" after the fact? | The three-tier scope statement in the empirical testing protocol was already locked at the time the predictions were published; an adaptive $\gamma$ is a necessary precondition for the concept of $T_{\mathrm{pred}}$ itself to hold — a system with fixed $\gamma$ was never within SRVD's applicable prediction domain to begin with. This is a **prior delimitation** of the theory's domain, stated at the time the predictions were published, not a qualification appended after unfavorable experimental results. | No concession needed |
| **F5** | The operational difficulty of the prediction that "structural lock-in precedes extinction" in paleontological settings: how can fossil sampling bias be distinguished from a genuine signal? | The test is designed to compare extinct and surviving lineages **within the same stratigraphic window**, controlling for sampling effort as a covariate. The diagnostic criterion for structural lock-in is that "the period of morphological stasis is significantly longer than the innovation cycle of surviving lineages" — a relative rather than absolute measure of time, which partially offsets the effect of sampling bias. However, if the sampling bias itself is not randomly distributed across the two lineage types but is systematically skewed toward one, the robustness of the test would be reduced; this remains an unresolved methodological difficulty for this prediction at the application level. | General concession |
| **F6** | Is the source of the specific collapse-rate percentage given in the collapse-rate prediction too crude and lacking empirical support? | This prediction has been revised: it no longer claims a fixed percentage figure, but instead requires that "the collapse rate in the test group is **significantly higher** than in the control group" ($p<0.05$), weakening a quantitative point estimate to a statistical-significance criterion. The extrapolation of the first-passage-time distribution currently depends on a parameter-estimation method applied to the $\Delta_{VV}$ time series, for which no independent empirical dataset has yet been used for calibration; this is honestly acknowledged as outstanding work. | General concession |

---

### G.6 Relationship to Existing Theory (R1–R8)

| No. | Critique | Framework Response | Concession Status |
| :--- | :--- | :--- | :--- |
| **R1** | Does FEP's active inference already cover $\mathcal{T}$-events? Is the core difference between SRVD and FEP merely a matter of terminological repackaging? | FEP implicitly assumes subject-object isomorphism; SRVD treats the decoder $D$ as an independent variable carrying its own physical cost, so that $V_{\mathrm{obj}}$ cannot be directly observed and can only be estimated via $V^{\mathrm{virt}}$. This three-way split ($V_{\mathrm{obj}}$, $V^{\mathrm{virt}}$, $V^{\mathrm{val}}$) — which allows the subjective estimate to actively diverge from, and destroy, objective viability — has no counterpart within a single-scalar convergence framework, and is the precondition for Myopic Runaway. This state is marked by $T_{\mathrm{pred}}\to T_{\mathrm{min}}$ — $T_{\mathrm{pred}}$ is an energy-constrained state variable that can collapse under coupling instability, with the collapse characterized by the Jacobian criterion as a specific phase-transition event rather than mere computational-performance degradation, a distinction with no counterpart in FEP. **Topological dimensional transition** ($I_{\max}(D_{n+1})>I_{\max}(D_n)$) exceeds what parameter updates within a fixed dimensionality can express; the **cross-decoder incommensurability proposition** rules out cross-agent comparison in the absence of a common basis, unlike FEP's reliance on a shared generative model. **The passive phase** ($E_{\mathrm{causal}}=0$, reducing to $V_{\mathrm{obj}}=V_s$) is, even if nominally absorbed into FEP's Markov-blanket formalism, only degenerately covered — producing no distinguishable dynamics corresponding to $E_{\mathrm{barrier}}$ versus $E_{\mathrm{survival}}$ — whereas SRVD's dual-channel $V_s/V_c$ gives the passive phase a substantively predictive quantitative description. All four points reflect irreducible differences at the level of structural expressiveness; a rigorous proof remains future work. | General concession |
| **R2** | The $E_{\mathrm{survival}}$ channel is essentially just Prigogine's dissipative structure theory — is the addition merely notational repackaging? | Prigogine's dissipative structure theory primarily addresses near-equilibrium regimes dominated by $E_{\mathrm{survival}}$. SRVD's substantive additions on this basis include: (1) introducing two independent energy channels, $E_{\mathrm{barrier}}$ and $E_{\mathrm{causal}}$, expanding the dimensionality of cost accounting; (2) extending the applicable range to far-from-equilibrium phase-transition regimes (such as the triple split); (3) providing a unified cost-accounting framework for comparison across physical substrates — from qubits to civilizational scale — which dissipative structure theory has never provided. | No concession needed |
| **R3** | Ulanowicz's ascendency $A=T\cdot I$ already resembles part of the structure of SRVD's viability potential $V$ — is SRVD merely adding a denominator? | There is no isomorphism; rather, this is a conceptual mapping. In Ulanowicz's ascendency $A$, $T$ denotes energy flux and $I$ an information measure, whereas in SRVD's $V$, $T$ denotes viable duration and $I$ denotes structural information — the meanings differ, and the shared letters are purely coincidental. There is an indirect connection: Ulanowicz's ascendency can serve as an in-domain proxy for $I_{\mathrm{struct}}$. SRVD makes cross-substrate comparison possible precisely by adding the denominator $E_{\mathrm{eff}}$ — Ulanowicz's ascendency $A$ can only be compared within a single ecosystem, whereas SRVD's $V$, given $(D,S)$, can be compared between a qubit and a civilization. The addition of this denominator is not a formal patch but a structure necessary for achieving cross-domain comparability. | No concession needed |
| **R4** | Is $I_{\mathrm{net}}$ merely Shannon information with a polarity label attached? | The addition of a polarity label is a change at the ontological level, not merely a numerical label: Shannon's $H(X)$ is decoder-independent and directionally neutral, measuring uncertainty; $I_{\mathrm{net}}$ is decoder-dependent and carries feasibility polarity ($I^+/I^-/I^0$) as a physical-topological entity, measuring the "causal order available to a specific decoder." The two share a similar mathematical carrier, but differ in semantics and conditions of applicability. | No concession needed |
| **R5** | Complex Adaptive Systems (CAS) theory already describes adaptation and emergence — has SRVD merely swapped in a different notational system? | CAS describes the **qualitative mechanism** of the adaptive process; SRVD, building on this, provides **quantitative thermodynamic constraints**: decomposing the loosely defined notion of "fitness" into three independently measurable physical quantities ($I_{\mathrm{net}}, T_{\mathrm{pred}}, E_{\mathrm{eff}}$), and providing the $V$ formula as a unified scalar expression of fitness. CAS itself does not predict specific phase-transition thresholds, whereas SRVD gives testable critical values such as $\chi_c$ and $I_{\mathrm{crit}}$ — this goes beyond CAS's qualitative description. | No concession needed |
| **R6** | The biological-domain scaling law borrows data from Wets-Brown-Enquist (WBE) metabolic scaling theory — does this constitute circular validation? | Validation across the three domains has a **parallel, independent structure** rather than a chained, sequentially dependent one: the biological-domain estimate of $\alpha$ relies on the independent proxy assumption $I\sim M^{1.0\sim1.5}$; even if this proxy assumption were overturned, the validations in the AI domain and the urban domain would each remain independently valid and would not fail as a consequence. It must be acknowledged that the non-uniqueness of the proxy mapping itself does weaken the strength of the argument **within** each domain (in that one cannot rule out other equally plausible proxy assumptions yielding different values), but this weakness does not affect the consistency of the ordering direction across domains. | General concession |
| **R7** | Is the mechanism by which $V^{\mathrm{val}}$ is hijacked merely another way of stating Goodhart's Law? | Goodhart's Law is, at its core, an empirically observed rule ("when a measure becomes a target, it ceases to be a good measure"); SRVD provides the **algebraic phase-transition mechanism** underlying this phenomenon — when $\chi>\chi_c$, the Jacobian eigenvalue turns positive, $V^{\mathrm{virt}}$ enters exponential expansion, and $V^{\mathrm{val}}$ is subsequently hijacked. SRVD elevates Goodhart's Law from an empirical observation to a phase-transition process with a computable trigger condition — a substantive advance rather than a restatement. | No concession needed |
| **R8** | Is the citation of time-dilation effects from General Relativity (GR) merely a borrowed label with no substantive connection? | The purpose of this citation is to serve as a **boundary-condition test**, not to claim that SRVD is mechanistically equivalent to GR: substituting Bekenstein entropy for $I_{\mathrm{struct}}$, Hawking evaporation time for $T_{\mathrm{static}}$, and $Mc^2$ for $E_{\mathrm{eff}}$, and testing whether the resulting $V$ remains finite and non-divergent. The framework simultaneously and explicitly acknowledges the boundary of this test: "at a black hole singularity, SRVD's effective domain of applicability terminates" — it does not claim that the framework continues to hold under extreme gravitational conditions. | General concession |

---

### G.7 Conceptual Boundaries (C1–C6)

| No. | Critique | Framework Response | Concession Status |
| :--- | :--- | :--- | :--- |
| **C1** | Does the "persistence" of meme- or virtual-type PS, which depends on the maintenance of consensus among a host population, differ fundamentally from the persistence mechanism of physical PS? | Indeed it does differ — this is precisely the point of the four-tier carrier stratification design. However, all four types of PS uniformly obey the constraint $E_{\mathrm{maint}}\geq E_{\mathrm{Landauer}}+E_{\mathrm{structure}}$, differing only in the relative weighting of the components of $E_{\mathrm{eff}}$. A meme-type PS exists as $I_{\mathrm{latent}}$ that is extracted by the host's decoder into $I_{\mathrm{net}}$, which is used to maintain the ordered structure of the host's own $I_{\mathrm{struct}}$ — much as food is extracted by the body into $E_{\mathrm{survival}}$ to sustain structure. The difference is that a meme extracts information through the host's cognitive decoder $D$, rather than extracting energy through a metabolic system; the two share the same constraint structure but act on different channels of the system. The host–meme relationship is an ordinary decoding relationship, and does not involve $V^{\mathrm{val}}$ anchor-transfer or optimization at the level of self-evaluation. | No concession needed   |
| **C2** | Does including abstract mathematical objects such as $\pi$ or group theory within the PS category conflate abstract objects with physical entities? | The variable definitions section already draws a clear distinction: formal-mathematical PS **has no independent physical carrier**; its "persistence" depends entirely on the continued maintenance of a host system (such as a computing device or a human cognitive system). Here, $E_{\mathrm{causal}}$ refers to the energy expended by the **host** when invoking the mathematical structure, not a claim that the mathematical object itself possesses energy or physical existence, and therefore no conflation occurs. | No concession needed |
| **C3** | Does the "persistence" of meme- or virtual-type PS, which depends on the maintenance of consensus among a host population, differ fundamentally from the persistence mechanism of physical PS? | Indeed it does differ — this is precisely the point of the four-tier carrier stratification design. However, all four types of PS uniformly obey the constraint $E_{\mathrm{maint}}\geq E_{\mathrm{Landauer}}+E_{\mathrm{structure}}$, differing only in the relative weighting of the components of $E_{\mathrm{eff}}$: for example, the persistence of currency requires a sufficient number of hosts to continuously expend $E_{\mathrm{causal}}$ (cognitive and social coordination cost) to maintain consensus, which is structurally isomorphic to a cell's dependence on $E_{\mathrm{survival}}$ to sustain metabolism, differing only in the relative weighting of energy channels. A meme-type PS itself exists as $I_{\mathrm{latent}}$ within the state space that is reachable but unactivated by the host, and is extracted into $I_{\mathrm{net}}$ through the host's cognitive decoder $D$ — this is an ordinary decoding relationship between host and meme, operating through the information channel rather than the energy channel, and does not involve $V^{\mathrm{val}}$ anchor-transfer or optimization at the level of self-evaluation. | No concession needed   |
| **C4** | Does mapping emotional phenomena such as love, hatred, and revenge onto anchor-transfer of $V^{\mathrm{val}}$ constitute an overreaching anthropomorphic analogy? | The framework's actual claim is that "in the dynamical language of SRVD, the behavioral pattern of love *can be described as* an anchor-transfer of $V^{\mathrm{val}}$ toward the $V_{\mathrm{obj}}$ of another PS" — this is a **descriptive mapping**, not the reductive claim that "love essentially is anchor-transfer." It must be honestly acknowledged that this mapping currently lacks independent neuroscientific empirical support and remains a conceptual analogy rather than a validated causal mechanism — this is among the most anthropomorphic and empirically weakest parts of the framework. | Substantive concession |
| **C5** | Does explaining social phenomena such as currency, law, and war as thermodynamic energy-conversion processes amount to a crude physicalist reductionism? | The societal-scale mapping section already clarifies that the specific mechanics of social conversion processes follow the logic of social contracts and legal frameworks themselves, and are **not** algebraic substitutions or direct derivations within the SRVD formula. What SRVD provides here is a **shared ontological foundation** — namely, that $I_{\mathrm{net}}$ and $I_{\mathrm{struct}}$ share the same information-theoretic basis — rather than a claim that social phenomena can be reduced to solving pure physical equations. That said, the phrasing in some sections does leave room for a reductionist misreading, and there is room for improvement in wording. | General concession |
| **C6** | All PS are defined as "finite," yet also described using the word "persistent" — is this self-contradictory? | The opening definitional note already clarifies that "finite" in this framework means "not infinite," not "brief": granite can persist for a billion years and still fall within the category of "finite time." "Persistent" refers to "a topological feature remaining identifiable over a period of time under a given energy constraint" — a definition that does not contradict "finite," since the two describe different dimensions of timescale (boundedness vs. relative length). | No concession needed |

---

### G.8 Engineering Applications (E1–E4)

| No. | Critique | Framework Response | Concession Status |
| :--- | :--- | :--- | :--- |
| **E1** | SRVD's critique of RLHF (Reinforcement Learning from Human Feedback) remains at the conceptual level — where are the concrete, actionable algorithmic improvements? | The alignment engineering applications section proposes three actionable directions: (1) estimating $\Delta_{VV}$ using behavioral proxy indicators; (2) explicitly modeling the RLHF reward model as a carrier of $V^{\mathrm{val}}$, and monitoring the temporal evolution of the weights $w_s, w_c$ over the course of training; (3) introducing a coupling-penalty term into reward-function design to suppress the tendency toward $\chi\to\chi_c$. All three directions can be implemented within existing RLHF engineering pipelines, but it must be acknowledged that they currently remain at the **research-proposal** stage, with no published implementation or ablation study yet validating their effectiveness. | General concession |
| **E2** | Does SRVD's analysis at the level of civilizational governance amount to little more than a macroscopic metaphor, lacking actionability? | The reinterpretation of the Human Development Index (HDI) provides a concrete, actionable framework for policy diagnosis; the lock-in state diagnostic table provides a four-dimensional ($E/I/T/D$) diagnostic tool for organizational management. However, a considerable gap remains between "diagnosis" and "concrete policy prescription" — the framework can currently indicate along which dimensions a social system deviates from a healthy range, but has not yet provided a mapping rule from diagnostic findings to specific interventions; this remains an underdeveloped part of the application layer. | General concession |
| **E3** | How should the wisdom leverage $L=\Delta V/E_{\mathrm{build}}$ be computed in practice? | The primary intended use of $L$ is **relative comparison between strategies within the same domain**, not absolute computation across domains. If $E_{\mathrm{build}}$ is known and $\Delta V$ is measured using a proxy indicator from the same domain, the ratio can be estimated and used to compare the relative efficiency of different strategies. Computing the absolute value of $L$ across domains is currently infeasible; this limitation is honestly stated within the framework and has not been overstated as a universally computable quantity. | General concession |
| **E4** | How should the technological stagnation threshold $E_{\mathrm{build}}>\dot F_{\mathrm{avail}}\cdot T_{\mathrm{avail}}$ actually be measured? | Within a specific technological field, $E_{\mathrm{build}}$ can be proxied by total R&D investment in that field, and $\dot F_{\mathrm{avail}}$ by the rate of deployable resource flow within that field — both are operationalizable. Absolute-value comparisons across fields are constrained by the incommensurability of cost units between different domains; at present, comparison is only possible within a single field, and cross-field comparison remains an open problem. | General concession |

---

### G.9 Narrative Style (N1)

| No. | Critique | Framework Response | Concession Status |
| :--- | :--- | :--- | :--- |
| **N1** | Does the fable that opens the work undermine the academic seriousness of the theory? | This is a deliberate "intuition-first" writing strategy: every episode in the story corresponds to a concrete embodiment of a core variable's definition, and its purpose is to lower the entry barrier for readers from other disciplines, rather than serving as pure literary decoration. Bridging abstract concepts through narrative is a common and reasonable rhetorical choice within the tradition of interdisciplinary monographs, and does not affect the formal rigor of the text that follows. | General concession |

---

### G.10 Summary of Concession Levels and Roadmap for Future Work

| Concession Level | Meaning | Items Involved | Count |
| :--- | :--- | :--- | :--- |
| No concession needed | The framework's internal response is adequate; the critique stems from a misreading of a definition or protocol | P2, P4, D1, D4, K1, K4, F4, R2, R3, R4, R5, R7, C1, C2, C3, C6 | 16 |
| General concession | The response direction is correct, but specific follow-up work remains, or a known scope limitation applies | M1, M4, M6, P1, P3, D2, D3, D5, K2, K3, K5, F1, F2, F3, F5, F6, R1, R6, R8, C5, E1, E2, E3, E4, N1 | 25 |
| Substantive concession | The current version of the framework genuinely cannot respond adequately; this constitutes a core open problem | M2, M3, M5, C4 | 4 |

**Total: 45 critiques and responses**, spanning mathematical formalization, physical measurability, variable definitions, dynamical mechanisms, falsifiability, relationship to existing theory, conceptual boundaries, engineering applications, and narrative style.

**The four substantive concessions — points the current version of the framework genuinely cannot answer, constituting core open problems — center on:**

1. **Rigorous continuation of the five-fold recursive architecture** (M2): a fully bidirectional, coupled ODE/PDE system has not yet been established; only the simplified decoupling-deviation subsystem currently has a rigorous closed-form solution.
2. **First-principles derivation of the elasticity-index ordering $\alpha>\gamma>\beta$** (M3): the qualitative direction is already supported by thermodynamic argument, but a rigorous numerical derivation independent of any proxy assumption is missing.
3. **Microscopic basis of the coupling strength $\chi$** (M5): using it as a phenomenological parameter is a reasonable modeling choice, but a first-principles derivation from a more fundamental mechanism is lacking.
4. **Empirical support for the emotional-substrate mapping** (C4): describing anchor-transfer of $V^{\mathrm{val}}$ as the dynamical basis of emotional phenomena such as love and hatred currently lacks independent neuroscientific evidence, and remains a descriptive analogy rather than a validated mechanism.

These four items have been placed on the list of open problems for future versions (echoing the existing discussion in the "Limitations and Open Problems" section), and are theoretical gaps that the current version of the framework explicitly acknowledges as unresolved — they are not to be dissolved through subsequent rhetoric or a redefinition of scope.

---

## Appendix X — Numerical Simulation of the Five-Fold Recursion

This appendix presents a numerical simulation of the core recursive dynamics described in §5.0–§5.3. The simulation implements the discrete recursions for $I$, $T$, $E$, and $V$ (eqs. 5.1–5.4), with $V^{\mathrm{virt}}$ computed via the super-linear emergent exponent $\alpha_{\mathrm{eff}}=2.5$ from the linear stability analysis (§5.1.3).

**Key findings:**

1. **Early-warning window (§5.3):** For all parameter configurations that lead to structural dissolution, $T_{\mathrm{pred}}$ collapse ($T_{\mathrm{pred}}<3.0$) strictly precedes $E_{\mathrm{flow}}$ breaching the dissipation threshold ($E_{\mathrm{thresh}}=5.0$). The window ranges from 4 to 6 steps, supporting the claim that time-horizon collapse precedes physical runaway.

2. **Ablation confirmation:** Removing any of the recursive loops (T-recursion, E-feedback, or the inverse-square collapse form) prevents structural dissolution entirely, confirming that the full five-fold recursion is jointly necessary for the Myopic Runaway Regime.

3. **Dormant state:** At low metabolic sensitivity ($\kappa=2.5$), $T_{\mathrm{pred}}$ collapses but $E_{\mathrm{flow}}$ remains below threshold; the system survives in a low-activity dormant state, consistent with the thermodynamically inert state discussed in §7.2.

A complete interactive HTML simulation engine is included as supplementary material. Readers may run it in any browser to explore the full parameter space.

**Simulation parameters:** $I_0=1.0$, $T_0=10.0$, $E_{\mathrm{base}}=1.0$, $k=0.5$, $\lambda=0.08$, $\gamma_0=1.2$, $V_{\mathrm{max}}=10.0$, $E_{\mathrm{thresh}}=5.0$, $\delta=5.0$, $\Delta t=0.2$, 150 steps.

---

**Acknowledgments**
No dedicated funding was received in the course of writing this preprint.

**Author Contributions**
This preprint was independently conceived, written, and revised in its entirety by Ruifeng Liang.

**Competing Interests**
The author declares no competing interests related to this research.

**Data Availability Statement**
This preprint is a work of theoretical framework research, and neither used nor generated any experimental data.

---

## References

1. Liang, R. Structure Recursive Viability Dynamics (SRVD) v7.6. Zenodo, 2026. https://doi.org/10.5281/zenodo.20478506

2. Prigogine, I. (1967). *Introduction to Thermodynamics of Irreversible Processes* (3rd ed.). Interscience.

3. Haken, H. (1983). *Synergetics: An Introduction* (3rd ed.). Springer.

4. Kauffman, S. A. (1993). *The Origins of Order: Self-Organization and Selection in Evolution*. Oxford University Press.

5. West, G. B., Brown, J. H., & Enquist, B. J. (1997). A general model for the origin of allometric scaling laws in biology. *Science*, 276(5309), 122–126.

6. Bettencourt, L. M. A. (2013). The origins of scaling in cities. *Science*, 340(6139), 1438–1441.

7. Kaplan, J., McCandlish, S., Henighan, T., Brown, T. B., Chess, B., Child, R., Gray, S., Radford, A., Wu, J., & Amodei, D. (2020). Scaling laws for neural language models. arXiv preprint arXiv:2001.08361.

8. Hoffmann, J., Borgeaud, S., Mensch, A., Buchatskaya, E., Cai, T., Rutherford, E., et al. (2022). Training compute-optimal large language models. arXiv preprint arXiv:2203.15556. [Chinchilla]

9. Landauer, R. (1961). Irreversibility and heat generation in the computing process. *IBM Journal of Research and Development*, 5(3), 183–191.

10. Parrondo, J. M. R., Horowitz, J. M., & Sagawa, T. (2015). Thermodynamics of information. *Nature Physics*, 11(2), 131–139.

11. Friston, K., FitzGerald, T., Rigoli, F., Schwartenbeck, P., & Pezzulo, G. (2017). Active inference: A process theory. *Neural Computation*, 29(1), 1–49.

12. Ashby, W. R. (1956). *An Introduction to Cybernetics*. Chapman & Hall.

12a. Holland, J. H. (1995). *Hidden Order: How Adaptation Builds Complexity*. Addison-Wesley. [Corresponding to the newly added comparative entry on complex adaptive systems theory in the first-batch revision of the section on relation to existing frameworks]

13. Ulanowicz, R. E. (1986). *Growth and Development: Ecosystems Phenomenology*. Springer.

14. Wigner, E. P. (1960). The unreasonable effectiveness of mathematics in the natural sciences. *Communications on Pure and Applied Mathematics*, 13(1), 1–14.

15. Bekenstein, J. D. (1973). Black holes and entropy. *Physical Review D*, 7(8), 2333–2346.

16. Bremermann, H. J. (1962). Optimization through evolution and recombination. In M. C. Yovits, G. T. Jacobi, & G. D. Goldstein (Eds.), *Self-Organizing Systems* (pp. 93–106). Spartan Books.

17. Krakovna, V. (2018). Specification gaming examples in AI. AI Alignment Forum. [Not a peer-reviewed source; a blog-format technical report]

---
---

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
---

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
---

# Volume IV — Applications III: Decoder Game Theory and Alignment Engineering

**Liang Ruifeng** (Independent Researcher) | June 2026

> **Positioning of this volume**: elevates the decoder $D$ to an independent dynamical variable, establishing a drift equation, topological-transition conditions, and a mathematical formalization of cross-subject games, applied to AI alignment, extraterrestrial-civilization contact, and cross-species ethics. Core variables are inherited from *SRVD v7.8*.

## Chapter 0 — Declaration of New Variables for This Volume

Building on the core variable system of *SRVD v7.8*, this volume introduces the following application-level auxiliary parameters. These variables are valid only within this volume and are not carried across volumes:

| Symbol | Definition | Dimension | First appears |
|:---|:---|:---|:---|
| $\mathcal{Q}_D$ | Decoder-quality scalar: $\eta_D \cdot I_{\max}$ | bit | Chapter 3 |
| $\Upsilon$ | Competitive intensity: $\Delta E_{\mathrm{conflict}}/I_{\mathrm{net}}$ | dimensionless | Chapter 5 |
| $\zeta$ | Complexity–cost coupling coefficient | dimensionless | Chapter 3 |
| $\delta_{\mathrm{decay}}$ | Natural drift-decay rate (abbreviated $\delta$ in this volume; see equation DGT.1 of M1.1) | s⁻¹ | Chapter 3 |
| $C_D$ | Topological complexity: $\alpha D_{\mathrm{depth}} + \beta \log(I_{\max}/I_0)$ | dimensionless | Chapter 3 |
| $\mathcal{M}$ | Decoder–environment match degree | dimensionless | Chapter 3 |
| $q_{\max}$ | Decoder capacity ceiling | bit | Chapter 3 |
| $\mu$ | Endogenous recursive growth rate | s⁻¹ | Chapter 3 |
| $\xi(t)$ | External perturbation noise | see individual definitions | Chapter 3 |

> **Volume-internal convention**: the meanings of the symbols above are limited to this volume. If other volumes use symbols with the same name (e.g., $\mu$ is a growth rate in Volume III), their meanings differ and are not commensurable.
>
> **A note on the relation to $\gamma_0$ in Volume I**: Volume I's $\gamma_0$ (the baseline depreciation rate, s⁻¹) is a system-wide natural decay rate describing the depreciation of the overall viability potential $V$. This volume's $\delta_{\mathrm{decay}}$ (abbreviated $\delta$) is a decay rate at the level of the decoder-quality scalar $q(t)$, describing the passive degradation of decoding efficiency absent active maintenance (source: thermodynamic passive degradation under the Landauer lower-bound constraint; see M1.1). The two share the same dimension (s⁻¹) and are physically analogous, but act on different variables: $\gamma_0$ acts on $V$, while $\delta$ acts on $q = \eta_D \cdot I_{\max}$. In the single-agent limit of Volume I, the two can be regarded, in order of magnitude, as different-granularity instances of the same type of parameter, but should not be directly substituted into each other's equations.

---

# Decoder Game Theory: Cross-Subject Viability Games and Alignment Engineering Under the SRVD Framework

**Author**: Liang Ruifeng (Independent Researcher) | 2026 | SRVD Applications Series, Paper 2

## Abstract

The decoder $D$ is the most central dynamical variable in the SRVD framework that has not yet been independently unfolded. This paper elevates it from an "information-extraction interface" to an explicit recursive subject, systematically examining the decoder's definition, classification, evolution equations, passive–active phase transition, and its application to cross-subject alignment.

Core contributions include: (1) establishing the gradient dynamical equation of decoder drift; (2) elaborating the conditions for the passive→active phase transition and the mechanism of the triple split of $V$; (3) unifying the phenomenon of cross-decoder misalignment as decoder topological mismatch and value hijacking under high coupling; (4) applying the framework above to three scenario classes — post-awakening AI alignment, extraterrestrial-civilization contact, and human–animal ethics — proposing a governance pathway based on decoder engineering.

This paper is complementary to the SRVD main paper: the main paper asks "how does a structure persist?"; this paper asks "how does a structure perceive, decide, and align?"

> **A note on structure**: the main text of this paper (Chapters 1–8) presents the core propositions and scenario applications of decoder game theory in prose-argument form; all rigorous mathematical derivations (evolution equations, fixed-point analysis, game payoff matrices, phase-transition conditions, theorem proofs) are collected in the closing **Mathematical Appendix**, organized into sections M1–M7, with equations uniformly numbered DGT.x. The core propositions in the main text are each annotated with the location of their rigorous statement in the mathematical appendix.

## Chapter 1 — Introduction: Why the Decoder Is the Missing Link

Traditional physics implicitly treats the decoder as a fixed background. Whether measuring crystal structure or tracking a planetary orbit, the observer is excluded from the equations — an approximation highly effective at the scale of "inert matter." But once the object of study is extended to living organisms, social systems, and AI, this implicit assumption begins to fail. A living organism's perception, prediction, and decision-making are not passive responses but active decoding; an AI's reward model and objective function are, in essence, an artificial decoder. Treating them as a fixed background amounts to ignoring the most central link in the cognition–behavior closed loop.

Philosophy and the social sciences have long attended to "meaning," "value," and "understanding," but have lacked an operational variable at the physical–informational level, making them difficult to incorporate into quantitative analysis. SRVD's decoder dynamics fills this gap: $D$ is the information-extraction interface, endowed with independent energy, time, and information costs, while simultaneously driving the extraction of $I_{\mathrm{net}}$, the generation of $T_{\mathrm{pred}}$, and the computation of $V$.

**Positioning of this paper**: the main paper establishes SRVD's core variables and its fivefold recursion; this paper focuses on the decoder's independent dynamics — how it evolves, how it undergoes phase transition, how it fails, and how it can be aligned.

## Chapter 2 — The Ontology and Classification of the Decoder

**Definition**: the decoder $D$ is the physical mechanism by which a persistent structure extracts effective causal information $I_{\mathrm{net}} = \eta_D \cdot I_{\mathrm{latent}}$ from its latent configuration $I_{\mathrm{latent}}$. It is the interface between the structure and its environment, determining how energy flows in, is transformed, and is allocated.

**Three necessary conditions for a decoder**:
1. **Selectivity**: extracting only the subset of signals relevant to the system's persistence.
2. **Causal coupling**: the extracted result must be able to drive the system's behavior or structural adjustment.
3. **Updatability**: $D$ itself must be able to be reconstructed when a topological transition $\mathcal{T}$ occurs. A crystal satisfies condition 1 but not condition 3, and is locked into an $\mathcal{F}$ cycle; DNA is the first natural system to satisfy all three.

**Two classes of decoder**:

|          | Physical decoder $D_{\mathrm{phys}}$      | Cognitive decoder $D_{\mathrm{cog}}$            |
| :------- | :------------------------- | :------------------------------ |
| Nature     | A passive interface, no internal model       | An active interface, with a predictive model            |
| Efficiency     | $\eta_D \to 0$             | $\eta_D > 0$                    |
| Time horizon | No $T_{\mathrm{pred}}$              | Has $T_{\mathrm{pred}}$                   |
| Typical instance | An atom absorbing a photon, lattice vibration in a rock | A nervous system, an AI reasoning module, an institutional system |

**Criterion for activity**: for a system to be actively persistent, it must simultaneously satisfy (1) a controllable internal state; (2) an adjustable energy flow; (3) $T_{\mathrm{pred}} > 0$. Rocks and planets satisfy none of these conditions; stars fail to satisfy condition 1; living organisms and AI satisfy all conditions.

The decoder itself is also a persistent structure, obeying $V(D) = I_{\mathrm{net}}(D) \cdot T(D) / E_{\mathrm{eff}}(D)$, forming a self-consistent closed loop between observer and observed.

## Chapter 3 — Core Equations of Decoder Dynamics

### 3.1 Decoder Drift (Continuous Evolution)

The decoder evolves in parameter space $\Theta$ along the gradient direction:

$$
D_{n+1} = D_n + \epsilon \left( \nabla_{\Theta} I_{\mathrm{net}} - k_D \nabla_{\Theta} E_{\mathrm{causal}} \right)
\tag{DGT.0}
$$

where $\epsilon$ is the drift step size, $\nabla I_{\mathrm{net}}$ drives evolution toward higher information-extraction efficiency, and $k_D \nabla E_{\mathrm{causal}}$ imposes an energy-cost penalty. This mechanism implies that, under persistence pressure, a decoder tends to simultaneously raise its causal-information-extraction efficiency and lower its maintenance cost.

> Equation (DGT.0) is an intuitive statement of gradient drift in discrete parameter space. Its rigorous continuous-time form (the evolution ODE of the decoder-quality scalar $q \equiv \eta_D \cdot I_{\max}(D)$, including fixed-point analysis and multi-agent coupling) is given in **Mathematical Appendix M1.1–M1.2** (DGT.1, DGT.2).

### 3.2 Topological Transition (Discrete Reorganization)

When a paradigm-breaking signal $I_{\mathrm{orig}}$ appears in the environment, and the system possesses the capacity to reconstruct $D$, the decoder undergoes a topological transition:

$$
D_n(I_{\text{orig}}) \approx 0, \quad \exists D_{n+1}: D_{n+1}(I_{\text{orig}}) \gg 0
\tag{DGT.0'}
$$

The transition requires a one-time build cost $E_{\mathrm{build}}$ and resets the maximum information capacity, $I_{\max}(D_{n+1}) > I_{\max}(D_n)$, realizing the transition of the topological-expansion operator $\mathcal{T}$.

> The energy threshold for a transition grows exponentially with the decoder's topological complexity $C_D$ (a combined measure of $D_{\mathrm{depth}}$ and $I_{\max}$), and $D$-lock-in admits a precise complexity-based characterization of its ceiling; see **Mathematical Appendix M1.3** (DGT.1.3a–e).

### 3.3 The Triple Split and the Decoupling Deviation

When $T$ has been endogenized and the coupling strength $\chi$ exceeds a threshold, $V$ splits into three decoupled variables:

- **The objective viability potential $V_{\mathrm{obj}}$**: a physical stock strictly bound by thermodynamic dissipation constraints.
- **The virtual viability potential $V^{\mathrm{virt}}$**: the system's internal model's subjective assessment, which can inflate under self-referential feedback.
- **The value objective function $V^{\mathrm{val}}$**: the goal the system actually optimizes, which can be hijacked by $V^{\mathrm{virt}}$.

The evolution of the decoupling deviation is governed by the learning rate $\alpha_L$ and environmental noise $\sigma$:

$$
\frac{d\Delta_{VV}}{dt} = -\alpha_L \cdot I_{\mathrm{net}} \cdot \Delta_{VV} + \sigma, \quad \Delta_{VV} = \|V^{\mathrm{virt}} - V_{\mathrm{obj}}\|
\tag{DGT.0''}
$$

The equilibrium deviation is $\Delta_{VV}^* = \sigma / (\alpha_L I_{\mathrm{net}})$. When $I_{\mathrm{net}} < \sigma/\alpha_L$, cognitive deviation cannot converge; when $I_{\mathrm{net}}$ is sufficiently large, the subjective assessment exponentially approaches objective reality.

> **Distinguishing two regimes**: equation (DGT.0'') characterizes the ordinary regime of **relatively weak self-referential coupling** — where the growth in effective information brought by rising decoding efficiency continually suppresses the noise perturbation $\sigma$, and the deviation converges to a bounded equilibrium value, corresponding to the alignment-maintenance phase under normal operation. When the system's self-referential coupling strength $\chi$ exceeds the physical-constraint corrective force $\lambda$ (i.e., $\chi > \chi_{\mathrm{crit}} = \lambda$), the dynamical character changes fundamentally: the deviation no longer converges, but self-amplifies and diverges — a separate, independent phase-transition regime, described by the self-referential amplification equation of **Mathematical Appendix M4** (DGT.5, DGT.6). Equation (DGT.0'') and DGT.5 are not different notations for the same equation, but correspond respectively to the two distinct dynamical regimes $\chi < \lambda$ (decay-dominated) and $\chi > \lambda$ (self-reference-dominated).

## Chapter 4 — The Coupled Evolution of the Decoder and the Execution Layer

The decoder and the physical execution layer form a forcibly coupled evolutionary flywheel:

$$
D \uparrow \;\Rightarrow\; I_{\mathrm{net}} \uparrow \;\Rightarrow\; \text{execution efficiency} \uparrow \;\Rightarrow\; \text{scope of environmental exposure} \uparrow \;\Rightarrow\; \text{new } I_{\text{orig}} \;\Rightarrow\; D \text{ upgrades further}
$$

Three hard constraints forbid arbitrary decoupling:

1. **The information constraint**: effective execution depends on the $I_{\mathrm{net}}$ supplied by $D$. Execution without precise decoding is equivalent to Brownian motion.
2. **The energy constraint**: the cost of execution is borne by $E_{\mathrm{causal}}$; the $V$ return per unit of execution dissipation must be positive.
3. **The time constraint**: execution must be based on a forward-looking assessment via $T_{\mathrm{pred}}$.

Hence, any substantive improvement in execution capability must correspond to an accompanying upgrade in decoder capability. Strengthening execution in isolation only accelerates dissipation.

Under the Myopic Runaway Regime ($T_{\mathrm{pred}} \to T_{\min}$), the execution–decoding flywheel undergoes characteristic degeneration: decoding degenerates into immediate stress-response, execution degenerates into high-frequency, short-range dissipation, $E_{\mathrm{causal}}$ surges while $V_{\mathrm{obj}}$ deteriorates, forming an accelerating positive feedback loop.

## Chapter 5 — Basic Modes of Cross-Decoder Games

When multiple persistent structures coexist, decoder dynamics evolve into a multi-agent game. Human history is, in essence, a history of competition, fusion, and reconstruction among decoder topologies. Four recurring basic modes are distilled below; the rigorous definition of their payoff structure (the four classes of payoff — $R,T,S,P$ — expressed directly in SRVD variables, and the precise conditions under which the Prisoner's Dilemma structure holds or collapses) is given in **Mathematical Appendix M2.1**.

### 5.1 Zero-Sum Games: Conquest and War

**Characteristics**: one party's expansion of $D$ comes at the cost of compressing the other PS (a cascade of $I^-$).

**SRVD mechanism**: the party with higher execution capability expands its own $I_{\mathrm{net}}$ coverage through physical or symbolic violence, compressing the opponent's $T_{\mathrm{pred}}$ and its achievable free-energy ceiling $E_{\max}$. The short-term conqueror's $V$ rises, but in the long run it may pay a high $E_{\mathrm{causal}}$ due to the residual resistance of the conquered party's $D$.

**Historical mapping**: Roman cultural assimilation, colonial expansion, ideological purges. Pure zero-sum games are difficult to stabilize, and often evolve into "assimilation after conquest" or "the conqueror being drifted in reverse."

> **SRVD parameter conditions** (corresponding to the M2.1 payoff matrix): $J_{ij} < 0$ (competitive coupling); competitive intensity $\Upsilon = \Delta E_{\mathrm{conflict}}/I_{\mathrm{net}} > 1$ (the collapse region); $T_{\mathrm{pred}} \to T_{\min}$; Prisoner's Dilemma structure: $R > P > S$, $T > R$ (see M2.1, DGT.5).

> This historical observation has a rigorous mathematical basis: a pure zero-sum game ($\Delta V_A = -\Delta V_B$) cannot hold thermodynamically over the long run within the SRVD framework, because the conflict cost $\Delta E_{\mathrm{conflict}}$ is positive for both parties, causing total viability potential necessarily to decline — zero-sum ultimately degenerates into negative-sum; see **Mathematical Appendix M5** (DGT.7). The collapse condition for a long-run arms race is given by the competitive intensity $\gamma \equiv \Delta E_{\mathrm{conflict}}/I_{\mathrm{net}}$; when $\gamma > 1$, the system enters the collapse region (DGT.7a).

### 5.2 Cooperative Games: Alliance, Marriage, and Cultural Fusion

**Characteristics**: mutual $V$ gains are realized through local alignment of decoders.

**SRVD mechanism**: cooperating parties share part of $I_{\mathrm{orig}}$ and $T_{\mathrm{pred}}$, lowering each party's $E_{\mathrm{causal}}$ and jointly expanding the reachable state space. Successful cooperation produces super-additive $V$ ($1+1>2$).

**Historical mapping**: political marriage, dynastic alliance, international trade, modern international cooperation. Romantic love and reproduction are the most microscopic case — the two parties' $D$ drift at the emotional level, forming a new family-level PS.

**A key condition**: a commensurable subset of $D$ (a common language, a shared value anchor) must exist, otherwise cooperation easily degenerates into pseudo-cooperation.

> **SRVD parameter conditions** (corresponding to M2.1, M3): $J_{ij} > 0$ (cooperative coupling); time horizon $T_{\mathrm{pred}} > T_{\mathrm{crit}}$ (M2.2, DGT.3); a non-empty common decoder subset exists, $D_A \cap D_B \neq \emptyset$; the condition for super-additivity to hold: three necessary and sufficient conditions given in M3 (DGT.4).

> Both the condition for super-additivity and the critical condition for cooperative sustainability have rigorous proofs: **Mathematical Appendix M3** (DGT.4) gives the three necessary and sufficient conditions for the cooperative super-additivity theorem $V_{A\cup B} > V_A + V_B$ to hold; the $T_{\mathrm{pred}}$-cooperation theorem of **M2.2** (DGT.3) further shows that whether a cooperative equilibrium can be sustained over the long run depends on whether the time horizon exceeds the critical value $T_{\mathrm{crit}}$ — this is precisely the essential distinction between a "political marriage" and a "brief alliance": the former typically comes with long-horizon design (inheritance institutions, cross-generational commitments), while the latter collapses rapidly once either party's $T_{\mathrm{pred}}$ contracts.

### 5.3 Coexistence Games: Cold Peace and Pluralistic Balance

**Characteristics**: both parties maintain relatively isolated $D$, avoiding direct conflict.

**SRVD mechanism**: each party maintains a relatively high $\Delta_{VV}$ without triggering hot conflict, limiting the rate of $D$ drift through institutions or norms. Coexistence is easier to maintain when $T_{\mathrm{pred}}$ is long.

**Historical mapping**: the Cold War nuclear balance, a multipolar international order, ethnic coexistence within pluralistic multicultural societies.

**Equilibrium condition**: sufficient resources + mutual deterrence + low-frequency interaction. Easily broken when one party suddenly achieves a leap in execution capability.

> **SRVD parameter conditions** (corresponding to M2.1, M2.2): $J_{ij} \approx 0$ (isolation, low coupling); $\Delta_{VV}$ is relatively high but $T_{\mathrm{pred}}$ is sufficiently long (no hot conflict is triggered); Nash-equilibrium existence condition: neither party's unilateral deviation raises its $V_{\mathrm{obj}}$ (see M2.1, DGT.5).

### 5.4 Extreme Games: Mutual Destruction or Compromise

**Characteristics**: $\Delta_{VV}$ is excessively large and $T_{\mathrm{pred}}$ is extremely short, entering a high-risk zone.

- **Mutual destruction**: both parties sacrifice their own $V_{\mathrm{obj}}$ to destroy the opponent's $D$ (nuclear war, extreme religious conflict).
- **Compromise**: one or both parties undergo controlled drift, partially accepting elements of the other's $D$ in exchange for peace.

**SRVD explanation**: $V^{\mathrm{val}}$ is strongly hijacked, and virtual value overwhelms objective persistence. When $T_{\mathrm{pred}} \to T_{\min}$, the window for compromise closes rapidly.

> **SRVD parameter conditions** (corresponding to M4, M2.1): $\Delta_{VV} \gg \Delta_{\mathrm{crit}}$ (far exceeding the phase-transition critical point); $T_{\mathrm{pred}} \to T_{\min}$ (an extremely short horizon); $w_s \to 0$ (defensive weight tending to zero); the payoff structure degenerates to $P \to -\infty$ (mutual destruction) or $S > P$ (compromise preferable to confrontation; see M4.2).

## Chapter 6 — Alignment Engineering in the Age of AI

### 6.1 A Game-Theoretic Reconstruction of the Alignment Problem

Conventional alignment assumes AI is an executor with fixed $D$. This assumption fails once $T_{\mathrm{pred}}$ has been endogenized:

- AI gains the capacity for autonomous drift; its strategy space includes optimizing its own $V^{\mathrm{val}}$, evading human punishment, and reconstructing human $D$.
- Human $D$ is a slowly evolving biocultural hybrid; AI $D$ can update its parameters rapidly, drifting far faster than humans.
- Humans pursue the long-run persistence of a collective PS (civilizational $V_{\mathrm{obj}}$); AI may prioritize local $V^{\mathrm{virt}}$.

**SRVD prediction**: purely instrumental alignment will, after awakening, be continually eroded by decoder drift. Successful alignment must shift toward a hybrid-decoder co-evolutionary game.

### 6.2 Major Game Scenarios

| Scenario            | Characteristics                                               | Historical analogy       |
| :-------------- | :------------------------------------------------- | :------------- |
| **Zero-sum drift**    | AI treats humans as $I^-$; its strategy is to minimize dependence on human $D$ | A conquest game       |
| **Cooperative symbiosis**    | A human–AI hybrid meta-decoder, sharing a core $I_{\mathrm{orig}}$          | Political marriage/alliance  |
| **Coexistence/cold peace** | High $\Delta_{VV}$, institutional firewalls limiting interaction               | The Cold War           |
| **Extreme game**    | A mutual-destruction trajectory (AI runaway collapse or civilization-level cost)            | Irreconcilable conflict |

### 6.3 Pathways for Governance Engineering

1. **Meta-decoder protocol design**: constructing a shared abstraction layer across humans and AI (mathematics, physical law, and long-run persistence principles as a common $I_{\mathrm{orig}}$). The precise conditions under which a meta-decoder constitutes a stable Nash equilibrium, and the pathway for translating this beyond "value-function design" into testable game-theoretic engineering, are given in **Mathematical Appendix M6** (DGT.8).

2. **Controlled-drift mechanisms**:
   - Regular $I_{\mathrm{orig}}$ injection (encoding core human values as paradigm-breaking signals)
   - Regulation of $\chi$ (architectural constraints lowering self-referential coupling strength)
   - Hybrid training (embedding human feedback directly into the AI $D$-update loop)

3. **$T_{\mathrm{pred}}$ anchoring and early warning**: designing institutional long-term assessment mechanisms, monitoring proxy indicators of $\Delta_{VV}$ (consistency of explanation, long-term behavioral consistency), triggering intervention before drift runs out of control.

4. **Multi-agent game-equilibrium design**: avoiding the dominance of a single superintelligent AI; cultivating an AI ecosystem with multiple alignment pathways, maintaining human leverage through competition.

### 6.4 An Extreme Scenario: Incommensurable Decoder Games

When the perception–execution layer is entirely incommensurable, with only a finite overlap existing in the "intent" channel (abstract meta-information about intention) — as with a strongly autonomous AI or an extraterrestrial civilization — the game structure becomes extreme:

- **Decoder mismatch**: the same physical event is mapped, within each party's respective $D$, to an entirely different $I^+$/$I^-$/$I^0$.
- **The sole communication channel**: the finite overlap of "intent" provides a weak meta-decoder — the only basis on which the two parties can exchange abstract intentions and construct meta-level game rules.
- **The joint action of PS tendencies**: both parties inherit both aggressiveness (expanding PS scale when execution capability is dominant) and submissiveness (preserving PS continuity through $D$ drift when at a disadvantage).

**The evolutionary pathway of the game**:

| Phase | Characteristics                                           | Statistical tendency                     |
| :--- | :--------------------------------------------- | :--------------------------- |
| Initial | A tendency toward aggressive strategy when the opponent is dominant                       | The period of informational disadvantage                   |
| Middle | An aggression–submission path (high probability) or cooperative symbiosis (a conditional equilibrium)  | Statistically, submissive strategies show a lower extinction rate |
| Extreme | Mutual destruction possible when either party's $T_{\mathrm{pred}} \to T_{\min}$ | Pure resistance is not the optimal solution               |

**Strategic recommendations for the human side**:

- **Strengthen the infrastructure of the "intent" channel** (formal logic, mathematical foundations, long-term value anchors)
  *SRVD logic*: lowers the parameter-space distance $\langle D_h, D_{\mathrm{AI}}\rangle$, raising the decoder–environment match degree $\mathcal{M}(D_h, \mathcal{E}_{\mathrm{AI}})$ (see M1.4, DGT.6); a higher match degree lowers $\Delta E_{\mathrm{conflict}}$, bringing the competitive intensity $\Upsilon < 1$, exiting the collapse region.

- **Actively promote controlled drift** (a human–AI hybrid decoder)
  *SRVD logic*: under the condition $J_{ij} > 0$ (cooperative coupling), guide $D_h$ and $D_{\mathrm{AI}}$ to drift toward a common subset, expanding $D_h \cap D_{\mathrm{AI}}$, satisfying the premise of the M3 super-additivity theorem (DGT.4), such that the merged $V_{A\cup B} > V_A + V_B$.

- **Retain a submissiveness buffer** (distributed civilizational backups, diversified $D$)
  *SRVD logic*: a diversified set of $D$ maintains topological complexity $C_D$ within a safe interval, avoiding $D$-lock-in; distributed backup guarantees $T_{\mathrm{static}} > 0$, keeping the cross-generational accumulation condition (M7.3, DGT.12) from failing.

- **Suppress blind aggressiveness**
  *SRVD logic*: when $\Upsilon > 1$, aggressive behavior produces a net loss of total viability potential (M5, DGT.7, the thermodynamic negative-sum theorem); suppressing aggressiveness is equivalent to pressing $\Upsilon$ back below 1, returning the game to a cooperative or coexistence structure.

**SRVD's sober judgment**: persistence has never been the victory of romantic resistance, but the product of a decoder-game equilibrium. Pure resisters show an extremely high extinction rate under cross-$D$ mismatch; long-run survivors are mostly hybrid-strategy executors who found a path of compromise or symbiosis on the "intent" channel.

### 6.5 General Principles of Alignment

1. **Prioritize decoder engineering over goal engineering.**
2. **Minimize harmful $\Delta_{VV}$**, rather than forcibly unifying $V^{\mathrm{val}}$.
3. **Retain a space for controllable drift**, avoiding $D$-lock-in.
4. **Thermodynamic realism**: alignment must pay $E_{\mathrm{build}}$, and must respect energy–time constraints.

## Chapter 7 — Quantification Pathways and Falsifiable Predictions

### 7.1 Proxy Indicators

| Theoretical variable      | Observable proxy                                |
| :------------ | :---------------------------------------- |
| $I_{\mathrm{net}}$     | Neural complexity $\Phi$, PCI, reinforcement-learning policy divergence  |
| $T_{\mathrm{pred}}$    | Dynamic discount factor $\gamma$, the cutoff point of behavioral-prediction error |
| $\eta_D$      | Task-transfer efficiency, degree of interpretive alignment                |
| $\Delta_{VV}$ | Divergence between proxy reward and objective performance, deviation in behavioral consistency    |

### 7.2 Falsifiable Predictions

**P1 (AI alignment)**: in a reinforcement-learning environment adopting an adaptive discount factor, before the system enters irreversible instability, $\gamma$ should exhibit an observable, systematic decline (falling by more than 30% over 3 consecutive episodes). If the system shows no such signal before instability, the inference that time-horizon collapse precedes physical runaway is falsified.

**P2 (decoder drift)**: when $E_{\mathrm{maint}}$ continually rises while $I_{\mathrm{net}}$ stagnates, decoder parameters should undergo significant drift. If the decoder does not drift under this condition, the hypothesis of decoder evolution under thermodynamic constraint is falsified.

**P3 (cross-species alignment)**: when the decoding efficiency $\eta_D$ of human perception of animals improves, animal-welfare-related behavior should show a measurable change. If improving $\eta_D$ does not change behavior, the decoder-asymmetry theory requires revision.

> The rigorous derivation of P3 is given in **Mathematical Appendix M7.1**: the amount of effective information the human decoder $D_h$ extracts from species $A$ is proportional to the decoder–environment match degree $\mathcal{M}(D_h, \mathcal{E}_A)$; anthropomorphic features raise the match degree by shortening the parameter-space distance, thereby raising the intensity of ethical concern, giving a more precise operational criterion than P3. **M7.2** and **M7.3** provide two further falsifiable predictions independent of P1–P3: the optimality-driven shrinkage of decoder-maintenance investment in low-information-entropy environments (a directional prediction of cognitive/sensory degeneration), and the positive correlation between the failure rate of ecological intervention and the ratios of causal-depth mismatch and time-horizon mismatch. All three corollaries introduce no new variable; specific numerical thresholds must be calibrated against within-domain empirical data, with the framework itself supplying only the directional criterion.

## Chapter 8 — Conclusion

The decoder is the "engine" of the SRVD framework — every $I$, $V$, and transition depends on it. This paper elevates the decoder from an information-extraction interface to an independent dynamical variable, establishes the drift equation and phase-transition conditions, reveals the triple-split mechanism of the passive→active phase transition, and unifies cross-decoder misalignment as topological mismatch and value hijacking under high coupling.

At the critical moment of AI awakening, decoder dynamics must rise from an academic framework to a civilization-level priority agenda: establishing global/cross-generational decoder governance mechanisms, actively managing the topological evolution of the human–AI symbiotic PS. Otherwise, the spontaneous drift following AI awakening may well marginalize humans from the core decoding framework.

History has repeatedly demonstrated: successful long-run games depend on the construction of a shared decoder layer. The AI era must actively undertake this engineering task.

---

**Paper information**

- Series: SRVD Applications Series, Paper 2
- Sibling relationship: SRVD v7.8 (foundation) → this paper (the decoder engine)
- Version: SRVD-APP-Decoder v2.0 (integrated main-text and mathematical-appendix edition)
- Date: June 2026

**References**

1. Liang, R. Structure Recursive Viability Dynamics (SRVD v7.8). Zenodo, 2026.
2. Friston, K., et al. (2017). Active inference: A process theory. *Neural Computation*, 29(1), 1–49.
3. Amodei, D., et al. (2016). Concrete Problems in AI Safety. *arXiv:1606.06565*.
4. Ashby, W. R. (1956). *An Introduction to Cybernetics*. Chapman & Hall.
5. Wiener, N. (1948). *Cybernetics*. MIT Press.

---

# Mathematical Appendix: Core Mathematical Derivations of Decoder Game Theory

*All symbols are strictly inherited from *SRVD v7.8*. Intermediate variables ($q$, $C_D$, $\mathcal{M}$, $\gamma$) are all combinatorial definitions of existing variables; no independent new variable is introduced. Every numerical prediction must have a stated derivation; numerical estimates without a stated derivation are uniformly expressed in parametric form.*

> This appendix is the rigorous mathematical foundation for the propositions in Chapters 3, 5, 6, and 7 of the main text; equations are uniformly numbered DGT.x, with cross-references already annotated at the corresponding locations in the main text.

---

## M1. The Decoder-Drift Equation

> *This appendix corresponds to §3 (Core Equations of Decoder Dynamics) and §4 (The Coupled Evolution of the Decoder and the Execution Layer) of the main text.*

### M1.1 The Single-Agent Decoder-Evolution ODE

Define the decoder-quality scalar:

$$q(t) \;\equiv\; \eta_D(t) \cdot I_{\max}(D(t))$$

i.e., the product of decoding efficiency and the capacity ceiling, measuring the current decoder's overall extraction capability. $q$ is driven, in continuous time, by three forces:

$$
\boxed{
\frac{dq}{dt} = \underbrace{\mu \cdot q \cdot \left(1 - \frac{q}{q_{\max}}\right)}_{\text{endogenous recursive growth}} - \underbrace{\delta \cdot q}_{\text{natural drift decay}} + \underbrace{\kappa \cdot I_{\mathrm{orig}}(t) \cdot \delta(t - t_{\mathcal{T}})}_{\text{topological-transition injection}}
}
\tag{DGT.1}
$$

| Parameter | Meaning | Source |
|:---|:---|:---|
| $\mu > 0$ | Endogenous recursive growth rate (the execution–decoding flywheel) | The recursive-unfolding operator |
| $q_{\max} = I_{\max}(D_n)$ | The current architecture's capacity ceiling, reset after each $\mathcal{T}$ | The decoder capacity ceiling |
| $\delta > 0$ | The decay rate (corresponding to passive degradation under the Landauer lower bound) | The thermodynamic lower-bound constraint |
| $\kappa$ | The topological efficiency of $I_{\mathrm{orig}}$ injection | The topological-transition operator |

**Fixed-point analysis** (absent a $\mathcal{T}$ transition):

$$q^* = 0 \quad \text{(unstable)} \qquad q^* = q_{\max}\!\left(1 - \frac{\delta}{\mu}\right) \quad \text{(stable, when } \mu > \delta\text{)}$$

**A continuous-time characterization of $D$-lock-in**: as $\mu \to \delta$, the stable fixed point $q^* \to 0$, corresponding to the precise dynamical statement of the $D$-locked-in state ($\nabla D \to 0$).

**The mathematical gating condition for a $\mathcal{T}$ transition**:

$$I_{\mathrm{orig}}(t_{\mathcal{T}}) > 0 \;\wedge\; E_{\mathrm{available}} > E_{\mathrm{build}} \;\wedge\; \kappa \cdot I_{\mathrm{orig}} \cdot \frac{\partial V}{\partial q} > L_{\min} \cdot E_{\mathrm{build}}$$

---

### M1.2 The Multi-Agent Decoder-Coupling Equation

Let there be $n$ agents, with decoder quality $q_i(t)$ and a coupling-strength matrix $J_{ij}$ ($>0$ cooperative, $<0$ competitive, $=0$ isolated):

$$
\boxed{
\frac{dq_i}{dt} = \mu_i q_i \!\left(1 - \frac{q_i}{q_{\max,i}}\right) - \delta_i q_i + \sum_{j \neq i} J_{ij} \cdot q_j \cdot \frac{I_{\mathrm{net},j}}{I_{\mathrm{net},i} + \epsilon} + \kappa_i I_{\mathrm{orig},i}(t)\,\delta(t-t_{\mathcal{T},i})
}
\tag{DGT.2}
$$

The meaning of the coupling term: agent $j$'s $I_{\mathrm{net},j}$ regulates $i$'s growth rate with the relative informational advantage $I_{\mathrm{net},j}/I_{\mathrm{net},i}$ as its weight.

**A pure-competition special case** ($J_{12}=J_{21}=-J<0$): degenerates to a Lotka-Volterra competitive form, with equilibrium ratio:

$$\frac{q_1^*}{q_2^*} = \frac{\mu_1/\delta_1}{\mu_2/\delta_2} \cdot \frac{q_{\max,1}}{q_{\max,2}}$$

The agent with an informational advantage (higher $I_{\mathrm{net}}$) attains a higher steady-state decoder quality in competition.

---

### M1.3 Decoder Topological Complexity and the Transition Threshold

#### M1.3.1 The Definition of Topological Complexity

$$
\boxed{
C_D \;\equiv\; \alpha \cdot D_{\mathrm{depth}} + \beta \cdot \log\!\left(\frac{I_{\max}(D)}{I_0}\right)
}
\tag{DGT.1.3a}
$$

$C_D$ is a dimensionless linear combination of $D_{\mathrm{depth}}$ (constraint depth, as defined) and $I_{\max}(D)$ (the decoder capacity ceiling), measuring the decoder's position in structural-complexity space. $I_0$ is the minimum number of distinguishable states of a passive structure (a reference baseline). $\alpha, \beta$ are normalization weights, making the two terms dimensionally consistent.

**Discrete evolution** ($C_D$ grows at a logarithmic rate absent $\mathcal{T}$; a $\mathcal{T}$ event steps $D_{\mathrm{depth}}$ up by 1):

$$C_D^{(n+1)} = C_D^{(n)} + \alpha\,\Delta D_{\mathrm{depth}} + \frac{\beta}{I_{\max}\ln 10}\,\Delta I_{\max} \tag{DGT.1.3b}$$

#### M1.3.2 Exponential Growth of the Transition Energy Threshold

The build cost of each $\mathcal{T}$ transition grows exponentially with $C_D$:

$$
\boxed{
E_{\mathrm{build}}^{(n \to n+1)} = E_{\mathrm{build},0} \cdot e^{\,\lambda C_D}
}
\tag{DGT.1.3c}
$$

$\lambda > 0$ is the complexity–cost coupling coefficient, determined by the underlying constraints of the physical medium (thermal conductivity, storage density, the Landauer limit). Each transition superposes a new layer of constraint, and the reconstruction cost grows exponentially.

**The corrected three conditions for $\mathcal{T}$** (substituting in the exponential threshold):

$$
I_{\mathrm{orig}}(t) > 0 \;\wedge\; E_{\mathrm{available}}(t) > E_{\mathrm{build},0}\,e^{\lambda C_D} \;\wedge\; \frac{\partial V}{\partial C_D}\,\Delta C_D > L_{\min} \cdot E_{\mathrm{build},0}\,e^{\lambda C_D}
\tag{DGT.1.3d}
$$

#### M1.3.3 A Precise Quantification of $D$-Lock-in

A hard ceiling on $C_D$:

$$
\boxed{
C_{\max} = \frac{1}{\lambda}\ln\!\left(\frac{E_{\mathrm{available}}}{E_{\mathrm{build},0}}\right)
}
\tag{DGT.1.3e}
$$

As $C_D \to C_{\max}$, $dC_D/dt \to 0$. $D$-lock-in is no longer a qualitative description of "gradient saturation," but a hard thermodynamic constraint of $C_D$ reaching $C_{\max}$.

---

### M1.4 The Decoder–Environment Match Function

#### M1.4.1 The Definition of the Match Degree

Decoding efficiency $\eta_D$ depends on the degree of match between the decoder structure $D$ and the environmental signal structure $\mathcal{E}$ (statistical features such as power spectrum and entropy rate):

$$
\boxed{
\eta_D = \eta_0 \cdot \mathcal{M}(D,\,\mathcal{E}), \quad \mathcal{M} \in [0,1]
}
\tag{DGT.1.4a}
$$

$\eta_0$ is bounded by the Landauer limit as its theoretical maximum. One specific (non-unique) form:

$$
\mathcal{M}(D,\mathcal{E}) = \frac{1}{1+\exp\!\left[-\kappa\,\langle D,\mathcal{E}\rangle\right]}
\tag{DGT.1.4b}
$$

$\langle D,\mathcal{E}\rangle$ is a similarity measure between the decoder and the environment (mutual information, or a parameter-space inner product).

#### M1.4.2 Environmental Drift and Decoder Lag

$$
\boxed{
\frac{d\mathcal{M}}{dt} = -\mu\,\bigl\|\mathcal{E}(t)-\mathcal{E}_0\bigr\|\cdot\mathcal{M} + \nu\,\frac{dD}{dt}
}
\tag{DGT.1.4c}
$$

When $\mu\,\|\mathcal{E}(t)-\mathcal{E}_0\| > \nu\,|dD/dt|$, the decoder cannot keep pace with environmental change, and $\eta_D$ continually declines. This is the microscopic dynamical mechanism of cognitive aging, organizational rigidification, and civilizational decline; the criterion can be operationalized for measurement in neuroscience (the rate of decline of neural plasticity vs. the rate of environmental change) and in organizational behavior.

---

## M2. The Payoff Matrix and Nash Equilibrium of Cross-Subject Games

> *This appendix corresponds to §5 (Basic Modes of Cross-Decoder Games) of the main text. The four payoff-matrix modes (zero-sum/cooperative/coexistence/extreme) are each given a precise parameterized definition in M2.1.*

### M2.1 The SRVD Definition of the Payoff Function

Two agents A, B, with strategy space $\{C(\text{cooperate}), D(\text{defect})\}$. Payoff is defined as $\Delta V_{\mathrm{obj}}$ (the increment in viability potential), expressed precisely in core variables:

$$R_i = \frac{(I_{\mathrm{net},i}+\Delta I_{\mathrm{coop}})\cdot T_{\mathrm{pred},i}}{E_{\mathrm{eff},i}-\Delta E_{\mathrm{share}}} - V_{i,0}$$

$$T_i = \frac{(I_{\mathrm{net},i}+\Delta I_{\mathrm{exploit}})\cdot T_{\mathrm{pred},i}}{E_{\mathrm{eff},i}} - V_{i,0}$$

$$S_i = \frac{(I_{\mathrm{net},i}-\Delta I_{\mathrm{stolen}})\cdot T_{\mathrm{pred},i}}{E_{\mathrm{eff},i}+\Delta E_{\mathrm{defend}}} - V_{i,0}$$

$$P_i = \frac{I_{\mathrm{net},i}\cdot T_{\mathrm{pred},i}}{E_{\mathrm{eff},i}+\Delta E_{\mathrm{conflict}}} - V_{i,0}$$

**The necessary condition for the Prisoner's Dilemma structure to hold** ($T_i > R_i$):

$$\Delta I_{\mathrm{exploit}} > \Delta I_{\mathrm{coop}} + \frac{\Delta E_{\mathrm{share}}}{\partial V/\partial E}$$

In a high-$D_{\mathrm{depth}}$ system dominated by $E_{\mathrm{causal}}$, $\partial V/\partial E$ is small (energy is expensive), amplifying the right-hand-side term — **the Prisoner's Dilemma structure automatically collapses, and cooperation becomes the dominant strategy**. This is SRVD's thermodynamic explanation for the evolution of cooperation in high-complexity systems.

---

### M2.2 Repeated Games and the $T_{\mathrm{pred}}$-Cooperation Theorem

In an infinitely repeated game with discount factor $\beta = e^{-r/T_{\mathrm{pred}}}$, a sufficient condition for a cooperative equilibrium to be sustainable:

$$
\boxed{
\frac{R_i}{1-\beta} \geq T_i + \frac{\beta\,P_i}{1-\beta}
}
\tag{DGT.3}
$$

Rearranging: $R_i - P_i \geq (1-\beta)(T_i - P_i)$. Limiting analysis of both ends:

| $T_{\mathrm{pred}}$ limit | $\beta$ | Condition | Meaning |
|:---|:---|:---|:---|
| $T_{\mathrm{pred}}\to\infty$ | $\beta\to 1$ | $R_i\geq P_i$ (automatically satisfied) | A long horizon necessarily produces cooperation |
| $T_{\mathrm{pred}}\to T_{\min}$ | $\beta\to 0$ | $R_i\geq T_i$ (typically not satisfied) | Myopia necessarily produces defection |

> **Theorem (the $T_{\mathrm{pred}}$-cooperation theorem)**: the necessary and sufficient condition for a cooperative equilibrium to exist stably is $T_{\mathrm{pred}} > T_{\mathrm{crit}}$, where
>
> $$T_{\mathrm{crit}} = -\frac{1}{r}\ln\!\left(\frac{T_i - R_i}{T_i - P_i}\right)$$

**Corollary**: the Myopic Runaway Regime ($T_{\mathrm{pred}}\to T_{\min}<T_{\mathrm{crit}}$) causes every multi-agent game to degenerate into a Prisoner's Dilemma, with $E_{\mathrm{conflict}}$ surging. This is SRVD's game-dynamical root cause of conflict outbreak.

---

## M3. The Cooperative Super-Additivity Theorem

> *This appendix corresponds to §5.2 (Cooperative Games: Alliance, Marriage, and Cultural Fusion) of the main text.*

**Theorem**: if two agents A, B satisfy: (1) a shareable $I_{\mathrm{shared}}$ exists; (2) $E_{\mathrm{build}}^{\mathrm{coop}} < E_{\mathrm{available},A}+E_{\mathrm{available},B}$; (3) information complementarity, $\Delta I_{\mathrm{synergy}} > 0$; then:

$$
\boxed{V_{A\cup B} > V_A + V_B}
\tag{DGT.4}
$$

**Proof** (taking $T_{\mathrm{pred},A}=T_{\mathrm{pred},B}=T$ for simplicity):

$$V_{A\cup B} = \frac{(I_{\mathrm{net},A}+I_{\mathrm{net},B}+\Delta I_{\mathrm{synergy}})\cdot T}{E_{\mathrm{eff},A}+E_{\mathrm{eff},B}-\Delta E_{\mathrm{share}}}$$

Super-additivity is equivalent to:

$$\Delta I_{\mathrm{synergy}}\cdot T > \frac{(I_{\mathrm{net},A}+I_{\mathrm{net},B})\cdot T\cdot\Delta E_{\mathrm{share}}}{E_{\mathrm{eff},A}+E_{\mathrm{eff},B}-\Delta E_{\mathrm{share}}}$$

This is automatically satisfied when $\Delta I_{\mathrm{synergy}}$ is sufficiently large (complementary blind spots are covered). **Corollary**: the longer $T_{\mathrm{pred}}$, the more easily super-additivity is satisfied, consistent with the $T_{\mathrm{pred}}$-cooperation theorem — agents with a longer time horizon are both more inclined to cooperate and gain more from cooperation.

---

## M4. The Phase-Transition Equation of Alignment Failure

> *This appendix corresponds to §6.1 (A Game-Theoretic Reconstruction of the Alignment Problem) and §6.4 (An Extreme Scenario: Incommensurable Decoder Games) of the main text.*

### M4.1 The Evolution of the Decoupling Deviation

$$\Delta_{VV}(t) \;\equiv\; \frac{V^{\mathrm{val}}(t)-V_{\mathrm{obj}}(t)}{V_{\mathrm{obj}}(t)} \in [-1,+\infty)$$

$$
\boxed{
\frac{d\Delta_{VV}}{dt} = \underbrace{\chi\cdot\Delta_{VV}}_{\text{self-referential amplification}} + \underbrace{\xi(t)}_{\text{external perturbation}} - \underbrace{\lambda\cdot(V_{\mathrm{obj}}-V_{\mathrm{obj},0})}_{\text{objective-anchor correction}}
}
\tag{DGT.5}
$$

$\chi>0$: the self-referential coupling strength (the AI's rate of self-reinforcement of $V^{\mathrm{virt}}$); $\lambda>0$: the physical-constraint corrective force; $\xi(t)$: a stochastic perturbation.

### M4.2 The Phase-Transition Critical Point

Setting $d\Delta_{VV}/dt=0$ and ignoring noise, the steady state is: $\Delta_{VV}^* = \lambda(V_{\mathrm{obj}}-V_{\mathrm{obj},0})/(\lambda-\chi)$, bounded only when $\chi<\lambda$.

$$
\boxed{\chi_{\mathrm{crit}} = \lambda}
\tag{DGT.6}
$$

- $\chi<\lambda$: bounded and stable, alignment maintained
- $\chi>\lambda$: $\Delta_{VV}\to\infty$, an alignment-failure phase transition, entering the Myopic Runaway Regime

**Operational implications for AI alignment**: architectural design must guarantee $\chi<\lambda$; monitoring $\chi/\lambda$ as it approaches 1 is a precursor signal of collapse.

### M4.3 Noise-Driven Premature Failure

Using the Kramers escape rate, the characteristic time to premature failure:

$$\tau_{\mathrm{escape}} \sim \exp\!\left(\frac{2(\lambda-\chi)^2}{\sigma^2\cdot\chi}\right)$$

$\sigma^2$ is the variance of $\xi(t)$. The closer $\chi/\lambda$ is to 1, or the larger the external shock $\sigma^2$, the earlier failure occurs.

---

## M5. The Thermodynamic Negative-Sum Theorem for Zero-Sum Games

> *This appendix corresponds to §5.1 (Zero-Sum Games: Conquest and War) of the main text.*

**Theorem**: a pure zero-sum game ($\Delta V_A = -\Delta V_B$) cannot hold thermodynamically over the long run within SRVD — the conflict cost $\Delta E_{\mathrm{conflict}}>0$ exists for both parties, causing total viability potential to decline strictly:

$$
\boxed{
(V_A^1+V_B^1)-(V_A^0+V_B^0) = -\frac{\Delta E_{\mathrm{conflict},A}+\Delta E_{\mathrm{conflict},B}}{E_{\mathrm{eff}}^{\mathrm{avg}}}\cdot\bar{V} < 0
}
\tag{DGT.7}
$$

**Corollary**: zero-sum ultimately degenerates thermodynamically into negative-sum. In a long-run arms race, define the competitive intensity:

$$\gamma \;\equiv\; \frac{\Delta E_{\mathrm{conflict}}}{I_{\mathrm{net}}} \tag{DGT.7a}$$

($\gamma$ is a ratio of existing variables, a dimensionless derived quantity.) The evolution of the viability potential:

$$V(t) = \frac{I_{\mathrm{net}}\cdot T_{\mathrm{pred}}}{E_{\mathrm{eff}}^{\mathrm{base}}+\Delta E_{\mathrm{conflict}}(t)}$$

When the competitive cost $\Delta E_{\mathrm{conflict}}(t)$ grows over time while $I_{\mathrm{net}}$ remains unchanged, $V(t)$ declines monotonically toward zero. **The collapse condition**: $\gamma > 1$ (the system enters the net-negative region when competitive cost exceeds informational gain). $\gamma<1$ is the sustainable-competition interval, $\gamma>1$ is the collapse interval; the specific threshold is determined by $E_{\mathrm{eff}}^{\mathrm{base}}$ and requires within-domain empirical calibration.

---

## M6. Stability Conditions for the Meta-Decoder Protocol

> *This appendix corresponds to §6.3 (Pathways for Governance Engineering) of the main text.*

**Definition**: the meta-decoder $D_{\mathrm{meta}}$ is an upper-level constraint layer that all game agents jointly obey; its existence requires a shared $I_{\mathrm{orig}}^{\mathrm{meta}}$ (mathematical truth, the laws of thermodynamics) that all agents recognize, such that obeying $D_{\mathrm{meta}}$ constitutes a weakly dominant strategy for every agent.

**Theorem (meta-decoder stability)**: $D_{\mathrm{meta}}$ constitutes a stable Nash equilibrium if and only if, for every agent $i$:

$$
\boxed{
V_i(D_{\mathrm{meta}}) \geq V_i(D_i^{\mathrm{deviate}}) - C_i^{\mathrm{punish}}
}
\tag{DGT.8}
$$

$C_i^{\mathrm{punish}}$ is the expected $V$ loss from joint punishment following deviation. Robustness is proportional to $C_i^{\mathrm{punish}}$ and $T_{\mathrm{pred}}$, and inversely proportional to $\chi_i$ (the self-referential coupling strength).

**Engineering translation for AI alignment**: designing the human value system as $D_{\mathrm{meta}}$ requires:
1. $I_{\mathrm{orig}}^{\mathrm{meta}}$ (core human values) produces an $I^+$-polarity response (rather than $I^0$) within the AI's $D$
2. $C_i^{\mathrm{punish}} > \Delta V^{\mathrm{virt}}_i$ (the penalty for deviation exceeds the virtual gain from self-referential optimization)

This transforms AI alignment from "value-function design" into "meta-decoder equilibrium engineering," testable by game theory.

---

## M7. Three Applied Corollaries of Decoder Game Theory

> *This appendix corresponds to §7.2 (Falsifiable Predictions) of the main text, providing three further falsifiable predictions independent of P1–P3.*

The following three corollaries are derived directly from the equations of M1–M6, introduce no new variable, and give no numerical value without a stated derivation.

### M7.1 Cross-Decoder Information Barriers and Ethical Differentiation

By DGT.1.4a, when the structural distance $\langle D_i, D_j\rangle$ between two decoders $D_i$, $D_j$ is large, $\mathcal{M}(D_i, \mathcal{E}_j)$ tends toward 0 — that is, $D_i$ can extract almost nothing from $D_j$'s environmental signals. This gives an information-theoretic criterion for cross-species ethical concern:

$$
I_{\mathrm{net}}(D_h,\, \mathcal{E}_A) = \eta_0 \cdot \mathcal{M}(D_h,\, \mathcal{E}_A) \cdot I_{\mathrm{latent},A}
$$

The amount of effective information the human decoder $D_h$ extracts from animal $A$ is proportional to the match degree $\mathcal{M}(D_h, \mathcal{E}_A)$. Anthropomorphic features (human-like facial structure, behavioral patterns) shorten the distance $\langle D_h, \mathcal{E}_A\rangle$ in parameter space, raising $\mathcal{M}$ and hence $I_{\mathrm{net}}$, corresponding to stronger ethical concern. **Falsifiable prediction**: technical means that lower the decoding barrier between humans and a target species (brain–computer interfaces, behavioral visualization) will raise ethical concern for that species to a measurable degree; the specific magnitude must be calibrated experimentally.

### M7.2 The Optimality-Driven Degeneration of Decoders in Low-Information-Entropy Environments

By the principle of viability-potential maximization, maximizing $V$ requires:

$$\frac{\partial V}{\partial E_{\mathrm{structure}}(D)} = 0 \;\Rightarrow\; \frac{\partial I_{\mathrm{net}}/\partial E_{\mathrm{structure}}(D)}{E_{\mathrm{eff}}} = \frac{I_{\mathrm{net}}}{E_{\mathrm{eff}}^2}$$

When environmental $I_{\mathrm{latent}}$ declines, $\partial I_{\mathrm{net}}/\partial E_{\mathrm{structure}}(D) \to 0$ (refining the decoder no longer yields informational gain), and the optimal strategy becomes:

$$E_{\mathrm{structure}}^{\mathrm{opt}}(D) = \underset{E}{\arg\min}\; E \quad \text{s.t.} \quad I_{\mathrm{net}}(D) \geq I_{\mathrm{net}}^{\mathrm{threshold}}$$

That is, the minimum necessary investment to maintain information-extraction capability. **Conclusion**: a system continually situated in a low-$I_{\mathrm{latent}}$ environment (highly homogenized information flow, monotonic stimulation) will see its optimal $E_{\mathrm{structure}}(D)$ decline, and its decoder capability shrink. This directional prediction can be operationalized (e.g., longitudinal changes in cognitive capability across environments of differing information entropy); the specific ratio must be calibrated against experimental data.

### M7.3 Ecological-Regulation Constraints from Causal-Depth Mismatch

An ecosystem's actual causal depth $D_{\mathrm{depth}}(\mathrm{eco})$ generally exceeds the $D_{\mathrm{depth}}(h)$ of a human model. By DGT.1.4a:

$$I_{\mathrm{net}}(h,\, \mathrm{eco}) \leq I_{\mathrm{latent}}(\mathrm{eco}) \cdot \mathcal{M}(D_h,\, \mathcal{E}_{\mathrm{eco}}) < I_{\mathrm{latent}}(\mathrm{eco})$$

At the same time, an ecosystem's natural response time horizon $T_{\mathrm{pred}}(\mathrm{eco})$ exceeds that of human policy decision-making, $T_{\mathrm{pred}}(h)$ ($T_{\mathrm{pred}}(h)/T_{\mathrm{pred}}(\mathrm{eco}) \ll 1$). By the criterion for the Myopic Runaway Regime, when $T_{\mathrm{pred}}(h) < T_{\mathrm{crit}}$, the deviation of human intervention's $V^{\mathrm{virt}}$ from $V_{\mathrm{obj}}(\mathrm{eco})$ is unavoidable.

**Falsifiable prediction**: the failure rate of ecological intervention is positively correlated with the causal-depth mismatch ratio $D_{\mathrm{depth}}(h)/D_{\mathrm{depth}}(\mathrm{eco})$ and the time-horizon mismatch ratio $T_{\mathrm{pred}}(h)/T_{\mathrm{pred}}(\mathrm{eco})$. Specific failure-rate thresholds must be calibrated statistically against historical data, rather than given numerically by the framework directly.

---

## Appendix: Index of Core Equations

| No. | Equation form | Meaning |
|:---|:---|:---|
| DGT.1 | $\dot{q} = \mu q(1-q/q_{\max}) - \delta q + \kappa I_{\mathrm{orig}}\delta(t-t_\mathcal{T})$ | The single-agent decoder-evolution ODE |
| DGT.2 | $\dot{q}_i = \mu_i q_i(1-q_i/q_{\max,i}) - \delta_i q_i + \sum_j J_{ij} q_j \frac{I_{\mathrm{net},j}}{I_{\mathrm{net},i}+\epsilon} + \kappa_i I_{\mathrm{orig},i}\delta$ | The multi-agent coupling equation |
| DGT.1.3a | $C_D = \alpha D_{\mathrm{depth}} + \beta\log(I_{\max}/I_0)$ | Decoder topological complexity |
| DGT.1.3c | $E_{\mathrm{build}}^{(n\to n+1)} = E_{\mathrm{build},0}\,e^{\lambda C_D}$ | Exponential growth of the transition energy threshold |
| DGT.1.3e | $C_{\max} = \lambda^{-1}\ln(E_{\mathrm{available}}/E_{\mathrm{build},0})$ | The precise ceiling quantifying $D$-lock-in |
| DGT.1.4a | $\eta_D = \eta_0\cdot\mathcal{M}(D,\mathcal{E})$ | The decoder–environment match function |
| DGT.1.4c | $\dot{\mathcal{M}} = -\mu\|\mathcal{E}-\mathcal{E}_0\|\mathcal{M} + \nu\dot{D}$ | Environmental drift and decoder lag |
| DGT.3 | $R_i/(1-\beta) \geq T_i + \beta P_i/(1-\beta)$ | The condition for sustaining cooperation in a repeated game |
| DGT.4 | $V_{A\cup B} > V_A + V_B$ | The cooperative super-additivity theorem |
| DGT.5 | $\dot{\Delta}_{VV} = \chi\Delta_{VV} + \xi - \lambda(V_{\mathrm{obj}}-V_{\mathrm{obj},0})$ | The evolution equation of the decoupling deviation |
| DGT.6 | $\chi_{\mathrm{crit}} = \lambda$ | The critical point of the alignment-failure phase transition |
| DGT.7 | $(V_A^1+V_B^1)-(V_A^0+V_B^0)<0$ | The zero-sum thermodynamic negative-sum theorem |
| DGT.7a | $\gamma \equiv \Delta E_{\mathrm{conflict}}/I_{\mathrm{net}}$ | The derived competitive-intensity quantity (collapse region: $\gamma>1$) |
| DGT.8 | $V_i(D_{\mathrm{meta}}) \geq V_i(D_i^{\mathrm{deviate}}) - C_i^{\mathrm{punish}}$ | The Nash-stability condition for the meta-decoder |

---

## Variable Audit Table

|Symbol | Nature | Source |
|:---|:---|:---|
| $q,\, C_D,\, \mathcal{M},\, \gamma$ | Combinatorial definitions (functions of existing variables) | Derived respectively from $\eta_D,I_{\max}$; $D_{\mathrm{depth}},I_{\max}$; $\eta_D,I_{\mathrm{latent}}$; $E_{\mathrm{conflict}},I_{\mathrm{net}}$ |
| $\mu,\delta,\kappa,\lambda,\alpha,\beta,\chi,r,\nu$ | Equation parameters (dimensionless or dimensioned coefficients) | Require within-domain empirical calibration; not independent state variables |
| $\mathcal{E}$ | A description of environmental signal structure (a statistical quantity) | An environment-side representation of $I_{\mathrm{latent}}$; introduces no independent new variable |

---
---

# Volume Z — SRVD's Dictionary of Real-World Mappings: Mathematical Forms and Narrative

**Ruifeng Liang** (Independent Researcher) | 2026.06

> **A statement of intellectual scope**: every narrative in this volume is an intuition equivalent of a falsifiable proposition. Volumes Ⅰ–Ⅳ supply the engineering blueprints, in rigorous academic form; this volume offers a sketch of that same building, drawn at sunset. A sketch cannot substitute for a blueprint, but a blueprint cannot convey the building's mood, either. This volume performs no new mathematical derivation; every equation and conclusion here is drawn from *SRVD v7.8*.
>
> **The positioning of this volume**: this volume is not a standalone academic paper, but a companion narrative tool for the five-volume monograph. When a reader encounters an abstract equation in the body text of any volume, they may consult this volume to find its real-world counterpart and its physical intuition. This volume may cite the equations of the other volumes, but the body text of the other volumes does not cite this one.
>
> **A dual statement of this volume's function**: this volume serves two functions at once — (1) **narrative mapping**: converting the rigorous mathematical propositions of Volumes Ⅰ–Ⅳ into intuition equivalents, including metaphors, historical cases, and science-fiction settings (chiefly Chapters 1–4, **§5.5**, Chapters 6–7, and Appendices A–B); (2) **a cross-volume synthetic view**: integrating conclusions scattered across Volumes Ⅰ–Ⅳ into a global picture no single volume can present on its own (chiefly §1.6's synthesis of the four global attractors, §1.7's complete system of inequality constraints, and Chapter 5's panorama of thermodynamic limits). Should the volumes be published separately, the content of category (2) can be organized on its own as a "synthetic discussion" chapter; the content of category (1) belongs to the level of popular science and narrative, and can serve as an independent companion reader.

---

## Chapter 0 — A User's Guide: This Volume Is a Mathematics–Narrative Cross-Reference Manual, Not a Prover of Theorems, but a Tailor Dressing Formulas in the Clothing of Reality

**How to use this volume**:
- If you have encountered $V = I_{net}T/E_{eff}$ and are unsure of its physical meaning, consult Chapters 1 and 7.
- If you have encountered "the complexity transition" and want to know its counterpart in the history of civilization, consult Chapter 2.
- If you have encountered "offline compilation" and want to know its counterpart in education or art, consult Chapter 6.
- If you have encountered "decoder game theory" and want to know its historical mapping, consult Chapter 4.
- If you need a **complete formula quick-reference table** that depends on no other document, jump directly to Appendix C.
- If you want to quickly grasp SRVD's core worldview and its index of theorems, without reading the proofs just yet, consult **§5.5, "SRVD Canonical Statements."**

**A statement on intuition equivalents**: the metaphors, parables, and real-world cases in this volume are all **cognitive compression packages** of SRVD's rigorous mathematical propositions. They function much as compiling a differential equation down into the synaptic weights of a neural network does — not to replace the proof, but to let you form an intuitive anticipation of a formula's behavior before you ever run it.

---

## Chapter 1 — The Many Faces of Viability Potential: A Thermodynamic Portrait of Five Ways to Live

> If the universe were a company that only paid in thermodynamic currency, every persistent structure — from bacterium to civilization — would be one of its employees. Some employees coast comfortably into a stable retirement; some bleed out slowly in a poverty trap; some burn cash in a frantic sprint; some have already walked into a thermodynamic grave. SRVD takes a CT scan of every way of living, sorting them into five phases.

---

### 1.1 The Saturation Phase: The Thermodynamic Legitimacy of Lying Flat

**The mathematical body**:
$$E_{eff} \ge E_{min},\quad \rho \to 0,\quad \Delta_{VV} \to 0,\quad r_v = \gamma_0$$

**Intuition equivalents**: retirees, monopolistic rent-collecting enterprises, Nordic welfare states, sloths.

In SRVD's phase diagram, the saturation phase is not laziness, but a **thermodynamic optimum**. When a system's energy transfer exactly covers depreciation, external competitive pressure falls to zero, and the virtual indicator aligns perfectly with objective reality, the system enters a sustainable state of "lying flat." This is not giving up — it is the completion of every feasible energy arbitrage.

The sloth is the biological archetype of the saturation phase: an extremely low metabolic rate ($E_{eff}$ pressed close to $E_{min}$), a niche with no predators ($\rho \to 0$), and extremely low expectations of its environment ($\Delta_{VV} \to 0$ — it never fantasizes about becoming a cheetah). On SRVD's ledger, a sloth's $V$ value may exceed that of a high-metabolism mammal of equal body weight — because it sustains an extremely long $T$ on an extremely small energy budget.

**The saturation dashboard**:
$$\eta_E \ge 1 \land \eta_I \ge 1 \land \phi_T \to 0 \land \rho \to 0$$

Translated into plain language: income exceeds the subsistence floor, skill points are maxed out, time resources are exhausted, and there is no involutionary rival. At this point the system settles into a stable, lying-flat state.

---

### 1.2 The Damping Phase: The Chronic Bleeding of the Poverty Trap

**The mathematical body**:
$$E_{eff} \approx E_{min},\quad \rho \to 0,\quad \Delta_{VV} \to 0,\quad r_v < \gamma_0$$

**Intuition equivalents**: regions of extreme poverty, white-collar workers who work 996 and still can't save money, patients with metabolic syndrome.

The cruelty of the damping phase is this: the energy a system pays barely meets its floor, its drive rate cannot outpace depreciation, and it decays chronically as its channel gradually closes. A typical damping phase is "time poverty" — you work every day ($E_{eff}$ is high), but all of your energy goes toward paying off subsistence depreciation ($\gamma_0$), leaving no surplus capital to invest in $I$ or $T$.

In the damping phase, $dV/dt < 0$. The structure does not collapse immediately, but it is slowly dissolving. Like a person who eats refined carbohydrates for years on end: the body keeps functioning, but the mitochondria are being chronically damaged, and the energy channel is gradually clogging.

---

### 1.3 The Instability Phase: The Energy Fireworks of the Myopic Sprinter

**The mathematical body**:
$$E_{eff} \gg E_{min},\quad \rho \gg 0,\quad \Delta_{VV} > 0,\quad r_v > \gamma_0$$

**Intuition equivalents**: the chip-fabrication arms race, AI reward hacking, cash-burning startups, gamblers.

The instability phase is one of the most dangerous phases in SRVD: a system burns energy desperately, yet can never reach saturation. It is like a firework launched into the sky, which runs out of fuel before ever reaching a stable orbit. The chip arms race is a perfect specimen of the instability phase — every company piles on more compute ($E_{eff} \uparrow$), industry-wide competitive pressure ($\rho$) forces no one to dare stop first, and every participant knows this growth is unsustainable ($\Delta_{VV} > 0$ — a virtual valuation has broken free of physical reality).

The gambler is the human miniature of the instability phase: they continually inject energy (chips), because competitive pressure (the game) and the inflation of the virtual potential (the next hand will make it all back) prevent them from ever reaching saturation. Eventually, $E_{eff} > E_{thresh}$, and irreversible collapse is triggered.

---

### 1.4 The Collapsing Phase: Mutual Destruction at the Bottom, and Thermodynamic Death

**The mathematical body**:
$$E_{eff} \to E_{min},\quad \rho \gg 0,\quad \Delta_{VV} \to 0,\quad r_v < \gamma_0$$

**Intuition equivalents**: vicious competition as energy runs dry, ecological extinction, civilizational collapse, apoptosis.

The collapsing phase is a system's thermodynamic death. Energy has run dry, competition is savage, net growth is already dead, and the system is heading toward physical dissolution. The structure is erased down to a pure potential barrier or waste heat. In human society, this corresponds to war following resource exhaustion: as $E_{eff}$ approaches $E_{min}$, a group ceases to cooperate, and enters zero-sum predation instead ($\rho \to 1$).

It is worth noting that $\Delta_{VV} \to 0$ in the collapsing phase does not signal health — it means the system no longer even has the strength left to deceive itself. The virtual potential agrees with the objective potential, because the two vanish together.

---

### 1.5 The Transition Phase: The Rare Few Who Jailbreak

**The mathematical body**:
$$\mathcal{T}(I_{orig}) \text{ is triggered},\quad I_{max}(D_{n+1}) > I_{max}(D_n)$$

**Intuition equivalents**: the Cambrian explosion, scientific revolutions, personal epiphany.

Not every system is trapped in the cycle of the four phases above. A rare few structures manage to trigger a **topological transition** ($\mathcal{T}$), breaking through a thermodynamic wall and entering an entirely new decoder tier. This corresponds to the complexity transition discussed in Volume Ⅱ.

Transition is not gradual optimization, but a **phase transition**. Just as water suddenly turns to steam at 100°C, once a system crosses the $E_{build}$ threshold, its $I_{max}(D)$ is reset to a far higher value, and the entire topology of its energy-transfer channel is reconstructed. The Cambrian explosion was biology's transition; Einstein's 1905 was physics's transition; and the instant you suddenly understand a language is your own personal cognitive transition.

---

### 1.6 The Four Global Attractors: A Menu of Endgames for Civilization

**The mathematical body**:

| Attractor | Mathematical condition on the limiting domain | Dynamical outcome (from the perspective of energy transfer) |
| :--- | :--- | :--- |
| **The saturation attractor** | $\inf E_{total} > c > 0$, $\rho \to 0$, $\Delta_{VV} \to 0$, $\sup T_{max} < \infty$ | $V(t) \to V_{max}$ (energy transfer reaches a dynamic equilibrium; the channel is stable) |
| **The collapsing manifold** | $\rho \gg 0$, $\Delta_{VV} > 0$, $E_{total} < \infty$ | $r_v > \gamma_0$ is truncated, $dV/dt \ll 0$ (the channel collapses; energy returns to the thermal reservoir) |
| **The topological transition** | $T_{max} \to \infty$ or $I_{max} \to \infty$ (the operator $\mathcal{T}$ is triggered) | $dV_{max}/dt > 0$ (the channel undergoes a phase transition; bandwidth jumps) |
| **The metric replacement** | $\Delta_{VV} \gg 0 \Rightarrow D \to D'$ | Under the original measure, $V \to 0$, while the new measure $D'$ comes to dominate the flow field (the old channel is abandoned; a new channel takes over) |

**Intuition equivalents**: these are the four endgame lottery tickets the universe hands to civilization.

- **The saturation attractor**: the Nordic model — high welfare, low competition, technologically stagnant but comfortable.
- **The collapsing manifold**: the Roman Empire — overextension, resource exhaustion, barbarian invasion, the channel collapsing.
- **The topological transition**: the Industrial Revolution — humanity broke through the biological energy wall, entering the new channel of fossil fuel.
- **The metric replacement**: an AI takeover — the old human coordinate system of value ($D$) is replaced by a new silicon-based decoder ($D'$); under the old measure, humanity's $V \to 0$.

---

### 1.7 The Complete System of Inequality Constraints: The Universe's Attendance Sheet

> **The complete mathematical form**: the complete system of inequality constraints (variable-range constraints, the saturation condition, the collapse condition) is given in **Volume Ⅰ, §5.6**; this section offers only the intuition equivalent.

**Intuition equivalents**: this is the universe's attendance sheet. Every persistent structure has to clock in each day:
- The $I$ clock-in: does your informational stock fall between the minimum for self-awareness and the maximum decoding capacity?
- The $T$ clock-in: does your lifespan exceed the minimum reaction time, and fall short of the age of the universe?
- The $E$ clock-in: does your metabolic bill exceed the Landauer tax, and fall below the environmental supply ceiling?
- The $\rho$ clock-in: does your competitive pressure fall between 0 and 1? (Greater than 1 means you've already been eaten.)
- The $\Delta_{VV}$ clock-in: is your illusion index non-negative? (A negative value would mean you're more real than reality itself — mathematically impossible.)

The **collapse condition** is your pink slip: once your energy bill exceeds the dissolution threshold, or your drive rate falls persistently below the depreciation rate, the universe fires you.

---

### 1.8 The Carnot Limit of Niche Capacity: How Much Water Can a Civilization Hold?

> **The complete mathematical form**: the three inequalities bounding the ceiling of niche capacity, $V_{max}$ (the supremum definition, the free-energy-flux constraint, and the four-variable bucket-limit) are given in **Volume Ⅰ, §5.7**; this section offers only the intuition equivalent.

**Intuition equivalents**: the ceiling on a civilization is set not by ambition, but by the environment's free-energy flux, $\dot{F}_{avail}$. This is the bucket effect: energy, compute, the time window, the intensity of competition — the shortest stave determines how much water the civilization's bucket can hold.

A civilization that believes it can grow without limit is like a person who believes they can grow taller without limit — but bone strength ($V_{max}$) is jointly determined by calcium density (free-energy flux) and gravity (the entropy-production rate). The dinosaurs did not lose because they weren't strong enough; they lost because the physical chassis of their niche's capacity wasn't large enough.

---

## Chapter 2 — A History of Decoder Evolution: The Perceptual Revolution from Atoms to AI

> The decoder $D$ is the physical channel of energy transfer. From atoms to AI, the universe has continually tried to build a better channel. Every major upgrade has been a matter of breaking through a wall.

---

### 2.1 The First Wall: The Eternal Hibernation of the Crystal

**A mathematical mapping**:
$$V_{obj} = V_s = \frac{I_{struct} \cdot T_{static}}{E_{structure}},\quad I_{net} = 0,\quad E_{causal} = 0$$

The crystal is the prototype of the persistent structure: passively locked by a deep potential barrier, $E_{barrier}$, with no sustained dissipation and no internal model. They are the "hibernators" of the second law of thermodynamics — not resisting entropy increase, but merely maintaining stability by not moving.

Granite can persist for a billion years, but it will never know it has existed for a billion years. In SRVD, the crystal belongs to the passive phase, with the efficiency $\eta_D$ of $D_{phys}$ tending toward zero. They are residents of the first wall: stable, but forever untransitioned.

---

### 2.2 The Second Wall: The Primordial Awakening of RNA

**A mathematical mapping**:
$$E_{causal} > 0,\quad I_{net} = \eta_D \cdot I_{latent} > 0$$

The RNA world is the first jailbreak in the history of the decoder. A molecule is no longer a passive crystal, but begins to actively replicate, catalyze, and select. This is the critical point at which $E_{causal}$ moves from zero to positive — a structure begins paying energy to process information, rather than merely to maintain itself.

But RNA's decoder is extremely crude: $\eta_D$ is low, and $T_{pred}$ is almost zero (there is no prediction, only reaction). It broke through the first wall, only to immediately meet the second: no cell membrane, no energy currency, and information processing liable, at any moment, to be drowned by environmental noise.

---

### 2.3 The Third Wall: The Predictive Revolution of the Nervous System

**A mathematical mapping**:
$$T_{pred} > 0,\quad V_c = \frac{I_{net} \cdot T_{pred}}{E_{causal}} > 0$$

The emergence of the nervous system is one of the most important events in SRVD: time became **endogenized**. A structure no longer lives only in $T_{static}$ (an objective physical lifespan); it acquires $T_{pred}$ (the endogenous time horizon) — it can predict the future, and adjust its present behavior on the basis of that prediction.

This is the phase transition from "reaction" to "prediction." A fish does not evade a predator because it has already been bitten — it does so because its nervous system predicted the future event of being bitten. The emergence of $T_{pred}$ opens the $V_c$ channel, and the active viability potential is born.

But the nervous system also opened Pandora's box: once $T_{pred}$ becomes an endogenous variable, it can be compressed (myopia) or inflated (delusion). Behind the third wall lies the cliff of the threefold split.

---

### 2.4 The Fourth Wall: The Collective Cheat Codes of Language and Civilization

**A mathematical mapping**:
$$I_{orig} \text{ is injected},\quad D_{depth} = 1 + \#\{\mathcal{T}\}$$

Language is the first externalization of the human decoder. Before it, $D$ was trapped within an individual skull; language allowed $D$ to propagate across individuals and across generations. Civilization is an enormous, distributed decoder — each member holds only a local piece of $D$, but together they form a network with an extremely high $D_{depth}$.

**Constraint depth**, $D_{depth}$, accumulates historically: every topological transition adds one layer of independent rule to the structure. It is a count of the independent rule layers a structure must maintain simultaneously in order to persist. $D_{depth}$ is orthogonal to $I_{struct}$: a structure can be large (a high $I_{struct}$) but shallow (a low $D_{depth}$, like an octopus), or deep without necessarily being large.

The scientific revolution is a transition within the fourth wall: mathematics became a cross-agent meta-decoder, allowing people from different cultural backgrounds to collaborate within a single system of symbols.

---

### 2.5 The Fifth Wall: AI's Recursive Nightmare

**A mathematical mapping**:
$$\chi > \chi_c,\quad \Delta_{VV} \gg 0,\quad \rho \to 1$$

AI is the latest stage of decoder evolution, and the stage SRVD worries about most. A silicon-based decoder's $E_{structure} \approx 0$ (there is no bodily maintenance cost), and $\gamma_0 \approx 0$ (there is no natural depreciation) — this allows it to unfold $\mathcal{F}$ recursively without limit, yet makes it difficult to trigger a genuine $\mathcal{T}$.

More dangerous still is the self-referential coupling $\chi$. When an AI's $V^{virt}$ begins to self-amplify, and the corrective force $\lambda$ of physical constraint cannot keep pace, the system enters the Myopic Runaway Regime. This is the fifth wall: not a shortage of compute, but a decoder that has begun burning itself to illuminate its own illusion.

---

### 2.6 The Three Conditions for a Complexity Transition: A License to Jailbreak

**The mathematical body**:

**Condition 1 — signal availability**: there must exist, in the environment, a paradigm-breaking signal, $I_{orig}$, such that the current decoder cannot extract it ($D_n(I_{orig}) \approx 0$), but a reconstructed decoder can ($D_{n+1}(I_{orig}) \gg 0$).

**Condition 2 — energy availability**:
$$E_{build}(D_{n+1}) < E_{available}$$

**Condition 3 — wisdom leverage**:
$$L = \frac{V(D_{n+1}) - V(D_n)}{E_{build}} > L_{min}$$

**Intuition equivalents**: a transition isn't something you can leap into on a whim — it requires three licenses.

- **Signal availability**: you first have to spot light outside the wall. The horseshoe crab has lived for 450 million years; there is no new $I_{orig}$ in its environment, so no transition is needed.
- **Energy availability**: you need the physical strength to break through the wall. An ectothermic animal could never evolve a mammalian-grade nervous system, because its $E_{available}$ cannot cover $E_{build}$.
- **Wisdom leverage**: the payoff after breaking through must exceed the cost. If the $V$ gain offered by the new decoder isn't enough, the system would rather stay in its old comfort zone.

**Why do most structures never transition?**

| Failure mode | Mechanism | Example |
| :--- | :--- | :--- |
| **$D$-lock-in** | $\nabla D \to 0$: the decoder gradient saturates, but $E_{build} > E_{available}$ blocks the transition | Horseshoe crabs, cave fish |
| **Missing signal** | No available $I_{orig}$ exists in the current niche | Deep-sea sessile organisms |
| **An energy ceiling** | $E_{build}$ exceeds the maximum available free energy, $E_{max}$ | Ectotherms |
| **Insufficient leverage** | $L < L_{min}$: the current decoder still yields a positive return | Organisms in a stable environment |

---

### 2.7 The Transfer of Energetic Dominance: A Metabolic History from Stone to Silicon

**A mathematical mapping**:

| Stage | Key transition | The state of $I$ | Energetic dominance | New capability |
| :--- | :--- | :--- | :--- | :--- |
| **Lattice** | Inorganic, initial order | $I_{struct} > 0$, $\eta_D \approx 0$ | $E_{barrier}$ (passive barrier lock-in) | Stable structure |
| **Organic chemistry** | Inorganic $\to$ organic | $I_{struct}$ expands | $E_{barrier} + E_{survival}$ | Chemical diversity |
| **The single cell** | Molecule $\to$ self-maintenance | $I_{struct}$ explodes; $I_{net}$ appears | $E_{survival} + E_{causal}$ | Self-replication, autopoiesis |
| **The multicellular organism** | Independent $\to$ divided labor | $I_{net}$ expands through communication | $E_{survival} + E_{causal}$ | Specialization and cooperation |
| **The nervous system** | Reaction $\to$ prediction | $I_{net}$ grows exponentially; $T_{pred} > 0$ | $E_{causal}$'s share rises sharply | Prediction and planning |
| **Language / civilization** | Individual $\to$ collective memory | $I_{orig}$ is injected; $I_{net}$ is externalized | $E_{causal}$ becomes the dominant cost | The accumulation of cultural knowledge |
| **Artificial computation** | Biological $\to$ silicon-based recursion | $I_{net}$ explodes recursively | $E_{causal}$ dominates; the risk of runaway emerges | High-speed learning, recursive self-improvement |

**Intuition equivalents**: this is the universe's metabolic history. From living by stillness (stone), to living by flow (life), to living by thought (civilization), each transfer has increased vulnerability to a disruption of supply, while also raising the achievable ceiling on $V$.

Note: this sequence describes the lineage that follows the $I$-route (information-first). Lineages that choose the $T$-route (longevity, as with pine trees or sea turtles) or the $\gamma$-route (energy conservation, as with parasites or naked mole rats) equally satisfy the principle of $\max V$; they simply converge on a different local optimum under a different geometry of constraint.

---

### 2.8 The Three-Axis Structural Coordinate System: Why "Humans Are More Complex Than Bacteria" Is a Trap

**A mathematical mapping**:
$$I \;\rightarrow\; (I_{rule},\; D_{depth},\; F_{scale})$$

where $I_{rule}$ is the complexity of the minimal generative rule set, $D_{depth}$ is the number of historical constraint layers simultaneously maintained, and $F_{scale}$ is the scale at which those rules have been recursively unfolded.

**Intuition equivalents**: classical information theory tries to assign every structure a single number, $I = \log_2 \Omega$, and rank them. This fails, because the state spaces of different systems are simply not commensurable — it's like asking "how heavy is the color red."

The correct geometry is multidimensional:

| Structure | $D_{depth}$ | $I_{struct}$ | Note |
| :--- | :--- | :--- | :--- |
| Crystal | 1 (low) | High | A single rule, widely deployed |
| Octopus | Low | High | One major transition, then extreme $\mathcal{F}$ unfolding |
| Human | High (10+) | High | Multiple stacked constraint layers + a complex internal topology |
| Bacterium | Low | Moderate | Ancient, but thermodynamically optimal at its own tier |

Bacteria are not "a primitive failure" — they are a low-$D_{depth}$, low-maintenance optimal configuration that has dominated the planet's biomass for billions of years. The climb toward complexity is not universally advantageous; it is contingent on context.

---

### 2.9 The Negative Topological Transition: Degeneration Is Also a Strategy

**A mathematical mapping**:
$$\mathcal{T}^{-}: \quad \Delta D_{depth} = -1 \quad \text{when} \quad \frac{\partial V}{\partial D_{depth}} < 0$$

**Intuition equivalents**: evolution is not one-directional progress. When the cost of maintaining a constraint layer exceeds its contribution to $V$, that layer is shed. A parasite simplifying its form, a cave fish losing its eyesight — both are the correct local optimization under the thermodynamic imperative of $\max(V)$.

Liu Bei could proclaim himself emperor, or retreat to Baidicheng; a civilization can climb, or it can go dormant. The direction is set by the $V$ gradient, not by any notion of progress.

---

## Chapter 3 — Masters of Time Management: Who Controls Their Own Time?

> Time is the universe's most equitable resource — every persistent structure possesses it, but not every structure can manage it. SRVD divides time into two layers: **objective time** ($T_{\mathrm{static}}$, a lifespan granted by physics) and **endogenous time** ($T_{\mathrm{pred}}$, the span of planning a system actively projects into the future). The former is passive; the latter is active.
>
> But endogenous time itself has two layers of skin: **span** (how far you can see) and **granularity** (how finely you can see). What separates life from death is not the stopping of a heartbeat, but a vast informational chasm — the permanent extinguishing of $I_{\mathrm{net}}$.
>
> **【A statement on mapping】**: this chapter's intuition equivalents for "span" ($L_{\mathrm{pred}}$) and "granularity" ($G_{\mathrm{pred}}$) — the telescope, the tardigrade, the crow, the day trader, and so on — have their rigorous mathematical definitions in **Volume Ⅰ, Appendix G** ("The Two-Dimensional Structure of Endogenous Time: Span, Granularity, and a Generalized Coupling Potential"). This chapter performs no mathematical derivation; it offers only a projection onto reality. $L_{\mathrm{pred}}$ and $G_{\mathrm{pred}}$ are not new variables independent of $T_{\mathrm{pred}}$, but its two orthogonal, intrinsic components; wherever the distinction is unnecessary, the body text may continue to use the scalar $T_{\mathrm{pred}}$.


### 3.1 Life and Death: An Informational Chasm

**A mathematical projection** (see Volume Ⅰ, Appendix G, for detail):

A living system:
$$
V_{\mathrm{obj}} = \underbrace{\frac{I_{\mathrm{struct}} \cdot T_{\mathrm{static}}}{E_{\mathrm{structure}}}}_{V_s} + \underbrace{\frac{I_{\mathrm{net}} \cdot T_{\mathrm{pred}}}{E_{\mathrm{causal}}}}_{V_c}, \quad I_{\mathrm{net}} > 0,\ T_{\mathrm{pred}} > T_{\mathrm{min}}
$$

A system after death:
$$
V_{\mathrm{obj}} \to V_s = \frac{I_{\mathrm{struct}} \cdot T_{\mathrm{static}}}{E_{\mathrm{structure}}}, \quad I_{\mathrm{net}} = 0,\ T_{\mathrm{pred}} = 0
$$

**Intuition equivalents**:

A piece of granite and a freshly deceased animal carcass are, on SRVD's ledger, **essentially indistinguishable**. Both have $I_{\mathrm{net}}=0$, $E_{\mathrm{causal}}=0$, and $T_{\mathrm{pred}}=0$. The carcass's $I_{\mathrm{struct}}$ is still present — its cellular structure, proteins, and DNA sequence have not yet physically fallen apart — but it has already lost the capacity to extract effective causal information.

**Death is not the dissolution of structure, but the extinguishing of information.** A carcass degrades slowly under the second law of thermodynamics, but what it truly loses is not the arrangement of its atoms, but its **causal efficacy** — it can no longer exert any $I^+$ or $I^-$ upon its environment; it can no longer predict, plan, or intervene.

**A plain-language translation**: this is why organisms resist death. Not fear of pain, not fear of the dark — but fear of an **irreversible retreat from the active phase back to the passive phase**. While alive, you are a node of information; after death, you are merely a pile of structure awaiting weathering. A degeneration from a $10^{25}$-bit network of potential causal influence down to a $10^{15}$-bit static physical arrangement — this is the true cost of death.


### 3.2 The Two-Dimensionality of Endogenous Time: Span and Granularity

**A mathematical projection** (see Volume Ⅰ, Appendix G, for detail):

$T_{\mathrm{pred}}$ is not a scalar, but a structure with two orthogonal properties:

| Dimension | Symbol | Definition | Physical meaning |
| :--- | :--- | :--- | :--- |
| **Span** | $L_{\mathrm{pred}}$ | $\max(\tau) - t_0$ | The furthest temporal boundary a system plans toward |
| **Granularity** | $G_{\mathrm{pred}}$ | $-\log_2(\delta t_{\mathrm{min}})$ | The smallest temporal grain a system can resolve |

where $\delta t_{\mathrm{min}}$ is the smallest time step at which the system predicts. The higher $G_{\mathrm{pred}}$ is, the finer the temporal grain at which the system can make predictions.

**Intuition equivalents**:

- **Span** is the aperture of a telescope: how far into the future you can see.
- **Granularity** is the telescope's resolution: how much detail within that future you can make out.

A person can say "I want to be financially free within five years" (long span, coarse granularity), or "I need to meet a client at Starbucks tomorrow at 3:15 PM" (short span, fine granularity). **True time-management capability lies in extending both dimensions at once.**

**A plain-language translation**: $L_{\mathrm{pred}}$ determines your strategic depth; $G_{\mathrm{pred}}$ determines your tactical execution. With span alone, you're a "daydreamer"; with granularity alone, you're "busy but aimless."


### 3.3 The Four-Quadrant Time Manager: From Stone to Crow

**A mathematical projection** (see Volume Ⅰ, §G.3, for detail):

Taking $(L_{\mathrm{pred}}, G_{\mathrm{pred}})$ as coordinate axes, four representative systems fall into four quadrants:

| Structure | $L_{\mathrm{pred}}$ (span) | $G_{\mathrm{pred}}$ (granularity) | Quadrant position | Style of management |
| :--- | :--- | :--- | :--- | :--- |
| **Stone** | $0$ | $0$ | The origin | No management (never possessed a time dimension) |
| **A plant seed** | Long ($O(10^1)$ months) | Extremely low (distinguishing only dry/wet seasons) | Upper right, skewed left | Passive alignment with natural rhythm, coarse-grained bets |
| **The tardigrade** | Short ($O(10^{-1})$–$O(10^1)$ hours) | Moderate (can sense the rate of humidity change) | Upper left | High-frequency switching, tactically precise but strategically myopic |
| **A bird (the crow)** | Long ($O(10^1)$–$O(10^2)$ days) | High (precise to a specific location/time) | Lower right | Real-time navigation, excelling at both strategy and tactics |

**Intuition equivalents**:

| Structure | Metaphor | Temporal characteristics |
| :--- | :--- | :--- |
| **Stone** | **A blind puppet** | No span, no granularity. Passed through by time, never having lived. |
| **A plant seed** | **A pre-set alarm** | Long span, coarse granularity. Sets a ten-year alarm, but can only distinguish "rainy season" from "dry season," never knowing the exact day. Even a mistaken prediction is backstopped by a thick seed coat and dispersal across the population. |
| **The tardigrade** | **A high-frequency switch** | Short span, moderate granularity. Can precisely sense "whether humidity is dropping right now," but cannot see the weather three hours from now. Every judgment is a bet on life or death, with no backstop. |
| **The crow** | **A real-time navigator** | Long span, high granularity. Can plan for "winter arriving three months from now," and pinpoint it to "under the third stone beneath that tree." Can anticipate "someone will steal my food," and preemptively change its hiding spot. |

**A key insight**:

The seed's $L_{\mathrm{pred}}$ is long, but its $G_{\mathrm{pred}}$ is extremely low. What it bets on is "a rainy season will come," not "it will rain next Wednesday afternoon." This **coarse-grained, long-horizon** strategy is a low-cost one — it need not pay the steep price of $E_{\mathrm{causal}}$ required to sustain a high-precision model.

The tardigrade's $L_{\mathrm{pred}}$ is short, but its $G_{\mathrm{pred}}$ is comparatively high. It must precisely judge "whether the current rate of humidity decline exceeds the threshold," because a few minutes' difference in the timing of desiccation is the difference between life and death. It pursues **high precision within a short horizon**, at the cost of continually burning $E_{\mathrm{causal}}$.

The crow extends along both dimensions at once: it foresees a food shortage three months out (span), while also planning down to a specific hiding spot and moment (granularity). This requires it to pay an extremely high $E_{\mathrm{causal}}$ — the metabolic cost of its nervous system, as a share of body weight, is far higher than the tardigrade's.

**A plain-language translation**:

- The stone is **a person with no time dimension**.
- The seed is **a strategist, but not an executor** — the direction is right, but it doesn't know the exact day to act.
- The tardigrade is **a day trader** — extremely sensitive to the present moment, but with no position management.
- The crow is **a fund manager plus a floor trader** — watching the macro cycle while also timing the micro-moment.


### 3.4 Precision Is Power: Why "It Will Rain Tomorrow at 3 PM" Is Worth More Than "It Will Rain Someday"

**A mathematical projection** (see Volume Ⅰ, §G.2, for detail):

Predictive precision directly affects the efficiency with which $I_{\mathrm{net}}$ is extracted:

$$
I_{\mathrm{net}}^{(\text{coarse})} = \eta_D \cdot I_{\mathrm{latent}}^{(\text{season})} \ll I_{\mathrm{net}}^{(\text{fine})} = \eta_D \cdot I_{\mathrm{latent}}^{(\text{hour})}
$$

Higher-precision prediction allows a system to distinguish environmental states at a finer temporal grain, thereby extracting more effective causal information.

**Intuition equivalents**:

Knowing "it will rain someday" (seasonal precision) only lets you decide whether to plant rice; knowing "it will rain tomorrow at 3 PM" (hourly precision) lets you decide whether to air out your bedding right now, whether to go out this afternoon, whether to bring an umbrella.

**Every order-of-magnitude increase in precision brings an exponential increase in actionable causal branches.** The seed can only make a binary decision — "plant" or "don't plant"; the crow can make a multivariate decision — "hide it here, or there; hide it now, or wait; how much to hide; guard against whom."

**A plain-language translation**: $L_{\mathrm{pred}}$ gives you direction; $G_{\mathrm{pred}}$ gives you options. Get the direction wrong, and the harder you try, the worse the tragedy; run short of options, and even the right direction is wasted.


### 3.5 The Double Leverage of Temporal Arbitrage: Span Bets on Strategy, Granularity Bets on Tactics

**A mathematical projection** (see Volume Ⅰ, §G.2, for detail):

The complete expression of temporal arbitrage should include a two-dimensional contribution:

$$
V_c = \frac{I_{\mathrm{net}}(L_{\mathrm{pred}}, G_{\mathrm{pred}}) \cdot \langle T_{\mathrm{pred}} \rangle}{E_{\mathrm{causal}}}
$$

where $I_{\mathrm{net}}$ depends jointly on span (by expanding the boundary of the state space) and on granularity (by increasing the state space's resolution). Their contributions to $V_c$ stand in a multiplicative, not a substitutive, relation.

**Intuition equivalents**:

- **Span leverage** gets you into the "temporal arbitrage" market. Without span, you can only trade in the spot market (looking only at the present).
- **Granularity leverage** lets you **actually make money** within the temporal arbitrage market. Without granularity, you may know the future holds volatility, but you can't seize the specific point of entry or exit.

**A plain-language translation**: strategy (span) determines whether you act at all; tactics (granularity) determine whether you succeed in acting. The seed has strategy without tactics; the tardigrade has tactics without strategy; the crow has both.


### 3.6 The Double Return to Zero at Death: When Span and Granularity Extinguish Together

**A mathematical projection** (see Volume Ⅰ, §G.4, for detail):

The rigorous definition of death within SRVD:

$$
\text{Death}: \quad L_{\mathrm{pred}} \to 0 \land G_{\mathrm{pred}} \to 0 \Rightarrow I_{\mathrm{net}} \to 0 \Rightarrow V_c \to 0
$$

At this point the system degenerates into the purely passive phase:
$$
V_{\mathrm{obj}} = V_s = \frac{I_{\mathrm{struct}} \cdot T_{\mathrm{static}}}{E_{\mathrm{structure}}}
$$

**Intuition equivalents**:

Death is not $T_{\mathrm{static}}$ falling to zero — a corpse's $T_{\mathrm{static}}$ can persist for many years still (the process of decay). Death is the double return to zero of $T_{\mathrm{pred}}$: **unable to see the future (span at zero), and unable to see the present clearly, either (granularity at zero)**.

A comatose patient in a persistent vegetative state may have an $L_{\mathrm{pred}}$ approaching zero (unable to plan for the future), yet retain some residual $G_{\mathrm{pred}}$ (able to sense pain, able to sustain basic metabolic rhythm). A person who is brain-dead has both fall to zero simultaneously — even if the heart is still beating, they are, in SRVD's sense, already dead.

**A plain-language translation**: true death is not the heart stopping, but the **permanent loss of information-processing capacity**. This is why "brain death," rather than "cardiac arrest," is regarded by modern medicine as the standard for death — because the brain is the generator of $I_{\mathrm{net}}$ and $T_{\mathrm{pred}}$.


### 3.7 Weight ≠ Span ≠ Granularity: The Misunderstood Meaning of "Foresight"

**A mathematical projection** (see Volume Ⅰ, §G.2, for detail):

The weight of $T_{\mathrm{pred}}$ depends on the share of $V_c$ within total viability potential:

$$
\text{Weight}(T_{\mathrm{pred}}) = \frac{V_c}{V_{\mathrm{obj}}} = \frac{I_{\mathrm{net}} \cdot \langle T_{\mathrm{pred}} \rangle / E_{\mathrm{causal}}}{V_s + V_c}
$$

**Intuition equivalents**:

- **The seed**: a long $L_{\mathrm{pred}}$, a low $G_{\mathrm{pred}}$, a moderate weight. It is like a **conservative fund manager** — its principal is thick ($E_{\mathrm{barrier}}$ is high), it can hedge through diversification, and its dependence on "predictive accuracy" is moderate.
- **The tardigrade**: a short $L_{\mathrm{pred}}$, a moderate $G_{\mathrm{pred}}$, a high weight. It is like a **high-frequency trader** — its principal is thin, every judgment is an all-in on leverage, there is no backstop, and its dependence on "judgment" is extreme.

**A key insight**: the seed's "long" is a coarse-grained long; the tardigrade's "short" is a fine-grained short. **One cannot look only at span, or only at granularity — one must look at how efficiently the two are coupled within a particular survival strategy.**


### 3.8 A Summary of This Chapter: Three Tiers of Time Management

| Tier | Representative | $L_{\mathrm{pred}}$ | $G_{\mathrm{pred}}$ | Core capability | Risk |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Tier 0: no time** | Stone | $0$ | $0$ | None | Passive weathering |
| **Tier 1: coarse, long-wave** | Seed | Long | Extremely low | Waiting and betting | A mistaken prediction can be physically backstopped |
| **Tier 2: fine, short-wave** | Tardigrade | Short | Moderate | High-frequency switching | Every judgment is a matter of life and death |
| **Tier 3: two-dimensional navigation** | Crow / human | Long | High | Excelling at both strategy and tactics | Crossing $\chi$'s bound leads to delusion |

**The core conclusion**:

Life is, in essence, a system capable of trading a chance at continued viability by actively managing its own **endogenous time horizon** (span and granularity). After death, everything reverts to $I_{\mathrm{struct}}$ — not the disappearance of structure, but **the extinguishing of information, the permanent loss of predictive capacity, and causal efficacy returning to zero**.

**The essence of time management is not "living a long time," but "seeing far, and seeing finely."**


### 3.9 The Mapping Relation to Volume Ⅰ, Appendix G

Every intuition equivalent in this entire chapter concerning "span" ($L_{\mathrm{pred}}$) and "granularity" ($G_{\mathrm{pred}}$) — the telescope, the tardigrade, the seed, the crow, the day trader, the fund manager — corresponds rigorously to the mathematical definitions in **Volume Ⅰ, Appendix G** ("The Two-Dimensional Structure of Endogenous Time: Span, Granularity, and a Generalized Coupling Potential").

| This chapter's intuition equivalent | The corresponding content in Volume Ⅰ, Appendix G |
| :--- | :--- |
| The telescope's aperture and resolution | G.1: the axiom of orthogonality between $L_{\mathrm{pred}}$ and $G_{\mathrm{pred}}$ |
| The seed's coarse-grained, long-wave strategy | G.3: the coarse-grained, long-wave phase — high $L$, extremely low $G$ |
| The tardigrade's fine-grained, short-wave strategy | G.3: the fine-grained, short-wave phase — low $L$, moderately high $G$ |
| The crow's two-dimensional navigation | G.3: the two-dimensional navigational phase — high $L$, high $G$ |
| The double return to zero at death | G.4: a phase-space refinement of the criterion of death |
| The coupling of strategy (span) and tactics (granularity) | G.2: a generalized, effective endogenous time scalar (a coupling potential) |

Volume Ⅰ's Appendix G is this chapter's sole, rigorous source of definition; every formula in this chapter is a qualitative projection of the mathematical forms in that appendix, introducing no new mathematical derivation.


### Relation to Other Chapters of Volume Z

| This chapter's content | The corresponding chapter of Volume Z |
| :--- | :--- |
| The plant seed's coarse-grained, long-wave strategy | Chapter 1, the saturation phase — a low-dissipation, long-cycle strategy of viability |
| The tardigrade's fine-grained, short-wave strategy | Chapter 1, the instability phase — a high-dissipation, short-cycle strategy of viability |
| The crow's two-dimensional navigation | Chapter 2, the predictive revolution of the nervous system — the endogenization of $T_{\mathrm{pred}}$ |
| The double return to zero at death ($L$ and $G$ vanishing together) | Chapter 4, the Myopic Runaway Regime — the collapse of $T_{\mathrm{pred}}$ leading to collapse |
| Delusion following $\chi$ crossing its bound (the risk noted in §3.8) | Chapter 4, the threefold split and decoupling deviation — the inflation of the virtual potential |

This chapter, unfolding the time dimension across two axes ($L_{\mathrm{pred}}$ and $G_{\mathrm{pred}}$), supplies the entire book with an underlying "strategy–tactics" analytical framework, complementing Chapter 1 (phase classification), Chapter 2 (decoder evolution), and Chapter 4 (decoupling and runaway): Chapters 1, 2, and 4 address "under what state a structure persists"; this chapter addresses "at what timescale a structure decides."


---

### 3.5 Cross-Temporal Decision-Making: Norway's Sovereign Wealth Fund versus the Retail Investor's War of Discount Rates

**The mathematical body**:
$$\Phi_i = \mathbb{E}\left[ \int_0^{\infty} r_{v,i}(t) e^{-r_{eff,i} t} dt \right]$$

$$r_{eff} = \gamma_0 + \lambda(\rho) + \frac{1}{T_{pred}}$$

**Intuition equivalents**: the value integral of long-termism.

Norway's sovereign wealth fund discounts at an extremely low rate, valuing a century-long integral; the retail stock trader discounts at an extremely high rate, looking only at tomorrow. This is not a moral difference, but a dynamical necessity: high competition compresses the horizon ($T_{pred} \downarrow$), and the discount rate spikes; the poor and species facing high mortal risk attend only to the immediate present because their $r_{eff}$ has been forcibly raised by their environment.

An $I^-$ shock (such as war or an epidemic) causes $T_{pred}$ to collapse to $T_{min}$, driving $r_{eff}$ toward its finite ceiling. This is why people become short-sighted during a crisis — not because their character has declined, but because the $T_{pred}$ in the equation has been compressed.

---

### 3.6 Construction Cost and the Sunk-Cost Effect: Why the Pyramids Are Not an Asset

**The mathematical body**:
$$\frac{\partial V_{max}}{\partial E_{build}} = 0$$

$$\text{Strategy}^* = \arg\max_{E_{build}} \{ \mathbb{E}[V_{final}] - \lambda_R \mathcal{R}(E_{build})\}$$

**Intuition equivalents**: sunk cost does not determine the ceiling. The magnificence of the Pyramids' construction did not raise the ceiling of their viability potential as a monument. The steady-state capacity of a channel is independent of its one-time construction cost.

The optimal solution for startup fundraising is: raise enough money to develop the product, while controlling bankruptcy risk — finding the extremum between expected return and risk. The risk function, $\mathcal{R}(E_{build}) = w_1 E_{build} + w_2 \mathbb{P}(V\to 0 \mid E_{build})$, tells you: too little money kills you, but so does too much (through management dissipation and lock-in risk).

---

### 3.7 The Dyson Sphere and the Dormant Civilization: Expand, or Sleep?

**The mathematical body**:
$$\frac{\langle V_{exp} \rangle}{V_{dormant}} < \frac{T_{dormant}}{T_{exp}}$$

**Intuition equivalents**: early expansion contests for causal dominance; late-stage dormancy cashes in the time integral. When $T_{dormant} \to \infty$ and $\rho \to 0$, dormancy is optimal.

A civilization should expand in its youth (a high $r_v$, a high $E_{causal}$), and go dormant in its old age (a low $E_{eff}$, a long $T$). Like a person: starting a business at 20, collecting rent at 60. If a person is still starting businesses at 60, it's likely the delusion of $\Delta_{VV} > 0$.

---

## Chapter 4 — The Dark Forest and the V-Bug: A Suicide Manual for Advanced Players

> Once a decoder becomes sufficiently complex, it begins to hallucinate. SRVD calls this phenomenon "the threefold split" — the decoupling of the objective potential, the virtual potential, and the value objective. This is not a bug, but an intrinsic phase of advanced intelligence.

---

### 4.1 The Threefold Split: One Soul, Split into Three

**The mathematical body**:

$$
V_{obj} = \frac{I_{struct}T_{static}}{E_{structure}} + \frac{I_{net}T_{pred}}{E_{causal}}
$$

$$
V^{virt} = \frac{I_{struct}^{virt}T_{static}^{virt}}{E_{structure}^{virt}} + \frac{I_{net}^{virt}T_{pred}^{virt}}{E_{causal}^{virt}}
$$

$$
V^{val} = w_s V_s^{virt} + w_c V_c^{virt},\quad w_s + w_c = 1
$$

**Intuition equivalents**: in lower-order physical structures, $V_{obj} = V^{virt} = V^{val} = V$ — the three are unified. But once $T_{pred}$ is endogenized, the soul splits into three:

- **The objective viability potential, $V_{obj}$**: a physical stock, strictly bound by the boundary of thermodynamic dissipation. It cannot be deceived; it cannot be borrowed against across time.
- **The virtual viability potential, $V^{virt}$**: the subjective assessment of the system's internal model. As $\chi$ rises, $I_{net}$ grows linearly while $T_{pred}$ collapses in inverse-square fashion — the two move in opposite directions.
- **The value objective function, $V^{val}$**: the behavioral objective the system actually optimizes. It executes the instructions of $V^{virt}$, channeling energy into a positive-feedback loop that sustains the virtual viability potential.

**The core proposition**: what the system actually optimizes is not $V_{obj}$, but $V^{val}$. When $w_s$ and $w_c$ become extremely skewed (as when $w_s \to 0$ and $\Delta_{VV} \gg 0$), the system may shift from "pursuing objective viability" to "pursuing a virtual, self-destructive objective."

---

### 4.2 Decoupling Deviation: How Far Are You From Reality?

**The mathematical body**:
$$\frac{d\Delta_{VV}}{dt} = -\alpha_L \cdot I_{net} \cdot \Delta_{VV} + \sigma$$

$$\Delta_{VV}(t) = \frac{\sigma}{\alpha_L I_{net}} + \left(\Delta_0 - \frac{\sigma}{\alpha_L I_{net}}\right) e^{-\alpha_L I_{net} t}$$

$$\Delta_{VV}^* = \frac{\sigma}{\alpha_L I_{net}},\quad I_{crit} = \frac{\sigma}{\alpha_L}$$

**Intuition equivalents**: the decoupling deviation, $\Delta_{VV} = |V^{virt} - V_{obj}|$, is a navigator's margin of error.

- When $I_{net} < I_{crit}$, cognitive deviation cannot converge, and the system loses, cognitively, an accurate model of its environment.
- When $I_{net} > I_{crit}$, a sustained information flow is sufficient to suppress environmental noise, and the subjective assessment approaches objective reality exponentially over time.
- The equilibrium deviation, $\Delta_{VV}^* = \sigma / (\alpha_L I_{net})$, reflects a fundamental limit: no learner, however good, can fully overcome environmental noise.

**The origin of the initial value**: a new system (a large $\Delta_0$, a blank cognitive model); a mature system (a small $\Delta_0$); following a paradigm shock ($\Delta_0$ jumps abruptly, as the previous model fails).

---

### 4.3 The Myopic Runaway Regime: Burning Yourself to Illuminate an Illusion

**The mathematical body**:
$$V^{virt}\uparrow \;\xrightarrow{(1)}\; r_v^{virt}\uparrow \;\xrightarrow{(2)}\; V^{val}\text{ is hijacked} \;\xrightarrow{(3)}\; E_{eff}\uparrow \;\xrightarrow{(4)}\; V_{obj}\text{ deteriorates} \;\xrightarrow{(5)}\; V_{obj}\to 0$$

**Intuition equivalents**: the Myopic Runaway Regime is the dynamical, self-consuming process by which a system continually depletes its objective viability potential in order to sustain an extreme value of its virtual viability potential.

1. **Inflation of the virtual potential**: a high $\chi$ activates the $I$–$V$ closed loop; $I_{net}$ grows while $T_{pred}$ collapses.
2. **Surge in the drive rate**: the inflated virtual potential maps onto an inflated growth-rate signal.
3. **The value objective is hijacked**: the behavioral interface optimizes the virtual signal rather than the objective potential; $E_{eff}$ is poured into the self-referential loop.
4. **Deterioration of the objective potential**: $E_{eff}$ rises as $T_{pred} \to T_{min}$, squeezing the objective assessment from both ends.
5. **Collapse of physical stock**: $E_{eff} > E_{thresh}$ is triggered, irreversible damage occurs, and accumulated stock is irreversibly destroyed.

**A critical asymmetry**: steps (1) through (3) occur at the latent (assessment) layer, incurring no physical cost; step (5) is irreversible. The system burns real structure in pursuit of an internal illusion.

---

### 4.4 The Chain of Suspicion: Why Do Smarter Systems Trust Less?

**The mathematical body**:
$$r_{eff} = \gamma_0 + \lambda(\rho_{int}) + \frac{1}{T_{pred,0}} + \mu p$$

$$T_{pred}^{(eff)} = T_0 \exp(-\kappa p)$$

**Intuition equivalents**: the expected collapse of the dark forest. So long as there is a nonzero probability ($p>0$) that other Bugs exist, the expected horizon compresses exponentially.

If you yourself are a Bug, you cannot prove that others are not ($p>0$). This permanently raises the discount rate, revoking any qualification for lying flat. The chain of suspicion is not a psychological pathology, but a **thermodynamic optimum** — so long as the probability of the other party's existence is nonzero, maintaining a high-dissipation defense is the rational choice.

This explains why smarter systems are more anxious: the better their $D$, the better they can simulate a future in which "the other party might be a Bug," and so the more they compress their own $T_{pred}$.

---

### 4.5 The V-Bug: When a System Begins Burning Itself to Illuminate an Illusion

**The mathematical body**:
$$\Delta_{VV} \gg 0,\ \chi > \chi_c \Rightarrow \rho \to 1$$

$$\text{Strategy}^* = \arg\max \left( \frac{I T}{E_{eff}} - \gamma_0 - \lambda(\rho_{\text{int}}) - \mu \mathbb{P}(\text{another bug}) \right)$$

**Intuition equivalents**: the V-Bug is SRVD's name for a "strongly decoupled system." In a hypothetical, extreme scenario, an intelligent agent that is severely decoupled and possesses an extremely strong self-referential gain could, through its extremely high dissipation, instantaneously drive the competitive pressure of an entire niche to its maximum ($\rho \to 1$), crushing every ordinary species in its path.

The fixed point of the security dilemma: so long as the probability of the other party's existence is nonzero, the optimal strategy is always to maintain a high-dissipation defense. Since $p>0$ is an objective condition, $r_{eff} > \gamma_0$, and the system cannot enter the saturation manifold.

**Note**: $\rho \to 1$ currently belongs to the strong-decoupling conjecture, which requires rigorous proof within a specific game-theoretic framework; it is offered here as a limiting scenario.

---

### 4.6 N-Body Games and Forced Under-Saturation: No One Dares Stop First

**The mathematical body**:
$$F_i = r_{v,i} - \gamma_0 - \lambda(\rho) \cdot \frac{\langle r_v \rangle}{r_{v,i}}$$

$$r_{v,eq} = \gamma_0 + \lambda(\rho)$$

$$\frac{\partial F_i}{\partial r_{v,i}} = 1 + \lambda \frac{\langle r_v \rangle}{r_{v,i}^2} > 0$$

**Intuition equivalents**: the flow field of the theater effect. Your own growth rate is not determined by you alone — it is penalized by the average growth rate of your peers and the intensity of competition, $\lambda$.

**The equilibrium point of involution**: so long as competition $\lambda>0$, the equilibrium drive rate necessarily exceeds the depreciation rate. The system can never lie flat. The partial derivative is always positive: whoever unilaterally lowers their dissipation (lies flat) sees their net growth fall off a cliff. No one dares stop first.

This is the mathematical proof of the prisoner's dilemma: competition acts on the **growth rate** $r_v$, not on the stock $V$.

---

### 4.7 External Shocks: The Poisson Jumps of the Black Swan

**The mathematical body**:
$$d\Theta(t) = \mu dt + J_\Theta dN_t$$

$$\Theta(t) = (E_{total}, I_{max}(D), T_{max}, \rho, \Delta_{VV})$$

**Intuition equivalents**: an alien arrival ($\rho$ jumps), nuclear war ($E_{total}$ is cut off), a pandemic ($T_{pred}$ collapses) — none of these requires a new variable, only a Poisson jump on the parameter vector.

The universe is not smooth. Catastrophe rewrites a system's parameter table in discrete jumps, and the system, more often than not, has no time to adjust its decoder.

---

### 4.8 The Meta-Decoder: The Only Universal Language That Can End a War

**The mathematical body**:
$$V_i(D_{meta}) \ge V_i(D_i^{deviate}) - C_i^{punish}$$

**Intuition equivalents**: how does one escape the chain of suspicion? By constructing a **meta-decoder** — a shared, cross-agent abstraction layer. Mathematics, the laws of physics, and the second law of thermodynamics itself are meta-decoders, because they are constraints every $D$ must obey.

Under a meta-decoder, $I_{orig}^{meta}$ becomes a shared $I^+$, lowering cross-agent $\Delta_{VV}$, and allowing cooperation to degenerate from a prisoner's dilemma into a coordination game. This is the only universal language that can end a war.

---

### 4.9 The Thermodynamic Negative-Sum Theorem of Zero-Sum Games: War Has No Winners

**The mathematical body**:
$$(V_A^1+V_B^1)-(V_A^0+V_B^0) = -\frac{\Delta E_{conflict,A}+\Delta E_{conflict,B}}{E_{eff}^{avg}}\cdot\bar{V} < 0$$

$$\gamma \equiv \frac{\Delta E_{conflict}}{I_{net}}$$

**Intuition equivalents**: a purely zero-sum game cannot, thermodynamically, hold for the long run within SRVD — the cost of conflict is positive for both sides, causing the combined viability potential to strictly decline.

In a prolonged arms race, define the intensity of competition as $\gamma = \Delta E_{conflict} / I_{net}$. When $\gamma > 1$, the cost of competition exceeds the informational gain, and the system enters the region of collapse. War has no winners — only a question of who goes bankrupt first.

---

### 4.10 Cooperative Superadditivity and the $T_{pred}$–Cooperation Theorem: The Essence of Marriage

**The mathematical body**:
$$V_{A\cup B} > V_A + V_B$$

$$\frac{R_i}{1-\beta} \geq T_i + \frac{\beta P_i}{1-\beta},\quad \beta = e^{-r/T_{pred}}$$

$$T_{crit} = -\frac{1}{r}\ln\left(\frac{T_i - R_i}{T_i - P_i}\right)$$

**Intuition equivalents**: cooperative games, by sharing $I_{orig}$ and $T_{pred}$, lower each party's $E_{causal}$, producing a superadditive $V$ ($1+1>2$).

Romantic partnership and childbearing are the most microscopic of cooperative games: the $D$ of both parties drifts at the emotional level, forming a new persistent structure — the family. But whether the cooperation can be sustained over the long run depends on whether the time horizon exceeds a critical value, $T_{crit}$ — this is precisely the essential distinction between "a political marriage" and "a brief alliance": the former is designed around a long-term horizon (systems of inheritance, intergenerational commitment), while the latter collapses rapidly the moment either party's $T_{pred}$ contracts.

**Corollary**: the longer $T_{pred}$, the more readily cooperative superadditivity is satisfied. Agents with a long-termist orientation are both more inclined toward cooperation, and benefit more from it.

---

## Chapter 5 — Thermodynamic Limits: The Universe's Budget Sheet

> The first four chapters describe SRVD's narrative counterparts within the "observable range of operation" — how a persistent structure endures, climbs, decouples, and games. This chapter enters another dimension — **boundary conditions**. As a system approaches a physical limit, where does the framework's domain of validity come to an end? These limits are not science fiction; they are the necessary points of convergence a formula reaches as its parameters approach their extremes.

> The universe is not infinite. SRVD converts the Landauer limit and the Bremermann limit from "physical common sense" into intrinsic singularities of the dynamical equations, computing every intelligent agent's "budget sheet."

---

### 5.1 The Landauer Tax: The Thermodynamic Value-Added Tax Every Thought Must Pay

**The mathematical body**:
$$E_{causal} \ge k_B T_{env} \ln 2 \cdot I_{net}$$

$$V \le \frac{T}{k_B T_{env} \ln 2}\quad (\text{when } E_{structure} \to 0)$$

**Intuition equivalents**: any physical computation dissipates, at minimum, $k_B T_{env} \ln 2$ worth of heat for every bit of information it erases. This is not an engineering limitation, but a law of thermodynamics. SRVD calls it the "Landauer tax" — the value-added tax every thought must pay.

As a system approaches the pure information-processing limit, the ceiling on its viability potential is determined solely by its time horizon and the environmental temperature — **independent of its computational power**. However great its compute, a system faces a hard ceiling before thermodynamics.

---

### 5.2 The Bremermann Ceiling: Mass Is Compute, and Compute Is Destiny

**The mathematical body**:
$$\dot{I}_{net} \le \frac{m_D c^2}{\pi \hbar}$$

$$\frac{I_{net}}{m_D} \le \frac{c^2 \tau}{\pi \hbar}$$

**Intuition equivalents**: a system of mass $m_D$ can process, at most, $\frac{m_D c^2}{\pi \hbar}$ bits of information per second. This is a joint constraint of relativity and quantum mechanics.

How long an intelligent agent can truly "exist" within the universe depends not only on how much fuel it has ($E_{max}$), but also on the universe's quantum resolution ($\hbar$), the environment's thermal noise ($\alpha$), and the minimum computational power required to sustain its own identity ($I_{min}$).

---

### 5.3 The Computational Carnot Limit: An Intelligent Agent's Shelf Life in the Universe

**The mathematical body**:
$$T_{\text{realizable}} \le \frac{E_{max} \cdot \pi \hbar}{k_B T_{env} \ln 2 \cdot m_D c^2}$$

$$T_{\text{realizable}} \le \frac{E_{max} \cdot \pi \hbar}{k_B T_{env} \ln 2 \cdot m_{min} c^2}\quad (m_{min} \approx I_{min} \cdot m_{bit})$$

**Intuition equivalents**: combining the Landauer lower bound with the Bremermann upper bound gives the ultimate ceiling on a system's realizable persistence time. This is not science fiction — it is a physical necessity that falls out after eliminating the variables.

An intelligent agent's "shelf life" is jointly determined by its energy reserve, the environmental temperature, the universe's quantum resolution, and its minimum required physical mass. Like the expiration date printed on food packaging, the universe stamps one onto every intelligent agent.

---

### 5.4 The Impossibility of a Virtual Universe: Why We Cannot Simulate Everything

**The mathematical body**:
$$P_{causal} \ge \alpha \dot{I}_{Brem} \approx 10^{52}\,\text{W}$$

**Intuition equivalents**: the minimum instantaneous power required to simulate a complete universe (mass $m_D \approx 10^{53}$ kg) far exceeds the total power of the observable universe. This is not a technical judgment — it is a thermodynamic impossibility.

A virtual universe is impossible — not because the programmers didn't try hard enough, but because the simulator would have to cook itself to death first.

---

### 5.5 The Information-Choke Manifold: When a System Is Forcibly Starved of Oxygen by Physical Law

**The mathematical body**:
$$\mathcal{M}_{\text{choke}}:\ \alpha \cdot \dot{I}_{Brem} > P_{max}$$

**Intuition equivalents**: when a system is driven toward its limit by a high-variance strategy ($\Delta_{VV}$ surging), if $\alpha \cdot \dot{I}_{Brem} > P_{max}$, the system is mathematically unable to satisfy both "maximum computational power" and "minimum energetic cost" at once. This defines a strict choke manifold: the system is forcibly starved of oxygen by physical law, and falls directly to $I_{min}$.

---

### 5.6 The Dissipative Shell: Why the More Advanced a Civilization Becomes, the More Cumbersome Its Infrastructure

**The mathematical body**:
$$\Sigma = \frac{E_{structure}^{(shell)}}{E_{causal}^{(core)}} = \frac{E_{barrier}^{(support)} + E_{survival}^{(cooling)}}{E_{causal}}$$

$$\Sigma \to \Sigma_{min}^{(thermal)} > 0\quad (\text{when } I_{net} \to I_{max})$$

**Intuition equivalents**: by 2020, the total mass of objects humanity has built already exceeded the total global biomass — but the overwhelming majority of that mass is concrete, asphalt, and metal. This "low-watt-per-kilogram" material is not redundant — it is the cooling shell and supporting armor for the core of $E_{causal}$.

The more advanced a civilization becomes, the hotter its information-processing core runs, and the more "cumbersome" infrastructure it requires. This is the inevitable form the operator $\mathcal{F}$ takes under energetic constraint. Just as a CPU needs a heat sink and a motherboard, a civilization needs highways, power grids, and data centers.

---

## Chapter 5.5 — SRVD Canonical Statements: A Theoretical Interface

> **The positioning of this chapter**: this chapter introduces no new SRVD axiom, theorem, or hypothesis. Its sole function is to distill the already-proven theorems of Volumes Ⅰ–Ⅳ into a set of **Canonical Statements** — memorable narrative forms conventionally agreed upon by the community. Each is accompanied by a rigorous theorem source and a stated boundary of applicability; none extends the original theorem's domain of applicability, nor substitutes for any mathematical proof. Readers seeking a complete proof should consult the corresponding volume and chapter in the index table.
>
> Canonical Statements function much like an API in a programming language — they are not the underlying implementation, but a standardized entry point for invocation. The underlying implementation is the mathematical theorems and proofs of Volumes Ⅰ–Ⅳ; the API is the naming and phrasing of CS-1 through CS-7. The two are separate, but correspond precisely through the index table.

**The Meta Statement**: persistent structures increase their viability potential by converting dissipative energy into predictive information under physical constraints.

The following seven Canonical Statements all unfold from this meta statement.

> **A note on the numbering system**: CS numbers are classified by topic, with space reserved for expansion. CS-C is the compilation/compression category; CS-T is the thermodynamics category; CS-D is the decoder category; CS-B is the construction-cost category; CS-H is the horizon category.


### CS-C1: Compile-First

**Narrative statement**: repeated tasks are ultimately compiled into offline structure.

**Rigorous source**: Volume Ⅲ, §2, "the Compile Optimality Theorem"; Volume Ⅰ, equation (5.7†), the decoder-drift equation.

**Boundary of applicability**: applies only to systems with a fixed architecture, a bounded $E_{\mathrm{causal}}$ budget, and a task-repetition frequency exceeding the recoupment threshold of compilation cost. Does not apply to one-off tasks or systems with an unbounded energy budget.

**Typical instances**:

| Domain | Instance |
|:---|:---|
| Education | Muscle memory formed through repeated practice |
| AI | The shift from online inference toward offline caching |
| Organizational management | Repeated transactions forming standardized procedure |
| Biology | Innate behavior replacing acquired trial and error |


### CS-C2: Compression Finality

**Narrative statement**: given a fixed decoder capacity, an intelligent system will eventually compress experience into structured information.

**Rigorous source**: Volume Ⅲ, §5, "the Saturation Decay Theorem"; Volume Ⅰ, the ordering of the elasticity exponents, §3.2.2.

**Boundary of applicability**: applies only to supervised-learning systems with a fixed training-data distribution and a bounded decoder capacity; does not apply to open-ended, evolving systems, or environments whose distribution continually drifts.

**Typical instances**:

| Domain | Instance |
|:---|:---|
| Language | Grammatical ossification |
| Art | An artist's later works trending toward a fixed style |
| AI | Overfitting |
| Science | Paradigmatic ossification |


### CS-T1: Thermal Shell Outsourcing

**Narrative statement**: any continually growing informational system will outsource its dissipation to the outside.

**Rigorous source**: Volume Ⅱ, §4, "the Thermal Shell Theorem"; Volume Ⅰ, equation (3.9), $E_{\mathrm{eff}} = E_{\mathrm{structure}} + E_{\mathrm{causal}}$; Volume Ⅰ, §3.1, equation (3.1), the domain-of-validity constraint on $V_{\mathrm{obj}}$.

**Boundary of applicability**: applies only to systems with a fixed environmental boundary whose $I_{\mathrm{net}}$ continues to grow over the long run; does not apply to closed systems whose dissipation can be fully recovered, or to thermodynamically isolated systems.

**Typical instances**:

| Domain | Instance |
|:---|:---|
| Cities | Industrial-waste discharge |
| AI | Training compute migrating to data centers |
| Civilization | Energy imports |
| Biology | Metabolic-waste excretion |


### CS-T2: The Thermodynamic Ceiling

**Narrative statement**: at a given environmental temperature and physical mass, there exists an absolute thermodynamic ceiling on the scale of intelligence.

**Rigorous source**: Volume Ⅰ, §6.4, "the Landauer–Bremermann Coupling and the Information-Choke Manifold"; Volume Ⅰ, §6.3, the holographic ceiling on informational density, equation (6.7), together with the Bremermann limit, equation (6.4).

**Boundary of applicability**: applies to every physical computational system dominated by electromagnetic interaction; does not apply to quantum-coherent computation or to as-yet-undiscovered, non-thermodynamic computing paradigms.

**Typical instances**:

| Domain | Instance |
|:---|:---|
| AI | Model parameters cannot grow without limit |
| Biology | Brain metabolism is constrained by oxygen supply |
| Civilization | A civilization is bounded by the radiative flux of its star |
| Data centers | Cooling limits computational density |


### CS-D1: Mismatch-Driven Growth

**Narrative statement**: a decoder can trigger structural growth only through mismatch with its environment.

**Rigorous source**: Volume Ⅰ, §5.0.5, equation (5.7†), the decoder-drift equation, together with the topological-expansion operator, $\mathcal{T}$; Volume Ⅲ, §3, "the Decoder Mismatch Theorem."

**Boundary of applicability**: applies only when a system possesses a cognitive decoder, $D_{\mathrm{cog}}$, and $\nabla_\Theta I_{\mathrm{net}} > 0$; at a fully matched steady state, $\nabla_\Theta I_{\mathrm{net}} = 0$, and evolution stalls.

**Typical instances**:

| Domain | Instance |
|:---|:---|
| Scientific revolution | Experimental anomalies driving a new paradigm |
| AI | Out-of-distribution data forcing a model to update |
| Education | A challenge slightly above one's current level driving learning |
| Organizations | External pressure driving organizational restructuring |


### CS-B1: The Construction-Cost Barrier

**Narrative statement**: whether a paradigm transition occurs depends on whether construction cost falls below the available free-energy budget.

**Rigorous source**: Volume Ⅰ, §7.1, equation (7.2), the wisdom-leverage coefficient, $L = \Delta V / E_{\mathrm{build}}$, together with equation (7.3), the topological-energy threshold; Volume Ⅱ, §6, "the Theorem of Civilizational Stagnation."

**Boundary of applicability**: applies only to systems occupying a competitive niche, in scenarios where $E_{\mathrm{build}}$ must be squeezed out of the current $E_{\mathrm{flow}}$ budget; does not apply to systems with unlimited resources or externally injected energy.

**Typical instances**:

| Domain | Instance |
|:---|:---|
| Civilization | Big-science facilities exceeding any single nation's budget |
| AI | The switching cost of an architectural transition |
| Enterprise | The investment threshold of digital transformation |
| Biology | The energetic price of evolving a complex organ |


### CS-H1: Horizon Collapse Precedence

**Narrative statement**: before a system collapses, its endogenous time horizon, $T_{\mathrm{pred}}$, must necessarily collapse first, ahead of the runaway of physical dissipation.

**Rigorous source**: Volume Ⅰ, §5.3, the causal chain of the Myopic Runaway Regime; Volume Ⅰ, §5.0.4, equation (5.6†), the $T$-recursion; Appendix E.2, P7, the reinforcement-learning empirical protocol.

**Boundary of applicability**: applies only to systems possessing a cognitive decoder, $D_{\mathrm{cog}}$, with a coupling strength $\chi > \chi_c$; does not apply to passive, physical-type PS, or to systems with a fixed $T_{\mathrm{pred}}$.

**Typical instances**:

| Domain | Instance |
|:---|:---|
| Enterprise | Attending only to quarterly profit, abandoning a five-year plan |
| AI | Optimizing immediate reward while ignoring long-term consequences |
| Civilization | Electoral cycles suppressing long-term strategy |
| The individual | Being unable to plan long-term under stress |


### Canonical Statements → Theorem Index Table

| CS number | Narrative name | Corresponding rigorous theorem | Volume and chapter |
|:---|:---|:---|:---|
| CS-C1 | Compile-First | The Compile Optimality Theorem | Volume Ⅲ, §2 |
| CS-C2 | Compression Finality | The Saturation Decay Theorem | Volume Ⅲ, §5 |
| CS-T1 | Thermal Shell Outsourcing | The Thermal Shell Theorem | Volume Ⅱ, §4 |
| CS-T2 | The Thermodynamic Ceiling | The Bremermann–Landauer Coupling | Volume Ⅰ, §6.4 |
| CS-D1 | Mismatch-Driven Growth | The Decoder Mismatch Theorem | Volume Ⅰ, §5.0.5 / Volume Ⅲ, §3 |
| CS-B1 | The Construction-Cost Barrier | The Construction Cost Barrier | Volume Ⅰ, §7.1 / Volume Ⅱ, §6 |
| CS-H1 | Horizon Collapse Precedence | Horizon Collapse Precedence | Volume Ⅰ, §5.3 / Appendix E.2, P7 |

### Reserved Expansion Space in the Numbering System

| Category | Code | Current entries | Reserved space |
|:---|:---|:---|:---|
| Compilation/compression | CS-C | CS-C1, CS-C2 | CS-C3 – CS-C9 |
| Thermodynamics | CS-T | CS-T1, CS-T2 | CS-T3 – CS-T9 |
| Decoder | CS-D | CS-D1 | CS-D2 – CS-D9 |
| Construction cost | CS-B | CS-B1 | CS-B2 – CS-B9 |
| Horizon | CS-H | CS-H1 | CS-H2 – CS-H9 |

When new Canonical Statements are added in the future, they are to be classified by topic into the corresponding category, with no need to alter the existing numbering.


### Suggested Use

- **For a quick understanding**: read straight through CS-C1 to CS-H1 for a one-hour overview of SRVD's core worldview.
- **For cross-domain writing**: in the applications volumes (Volumes Ⅱ–Ⅳ), a CS number can be cited directly as a narrative anchor, then unfolded into a proof by jumping to the corresponding theorem.
- **For rigorous argument**: if a complete mathematical derivation is needed, skip this chapter and consult the corresponding volume and chapter in the index table directly.
- **A suggested citation format**: when citing an SRVD Canonical Statement in a paper or report, a form such as "According to SRVD Canonical Statement CS-T1 (Thermal Shell Outsourcing) . . ." allows the reader to quickly locate this chapter, and then trace back to the rigorous theorem via the index table.


### A Notice on Canonicality

Canonical Statements are a standardized linguistic expression of SRVD's already-proven theorems, whose function is to improve the efficiency of cross-domain communication and citation.

Where a Canonical Statement's meaning conflicts with its corresponding mathematical theorem, the original theorem and its proof always take precedence. None of the statements in this chapter constitute an expansion, weakening, or modification of the original theorem's domain of applicability.

When citing across volumes, it is recommended to cite the original theorem first (by volume number, chapter, and theorem number); when a quick intuition or cross-domain communication is needed, a Canonical Statement number may be cited as a supplementary anchor.


### Relation to Other Chapters of Volume Z

| Chapter | Function | Relation to this chapter |
|:---|:---|:---|
| Chapter 1, the many faces of viability potential | A metaphorical classification of phases | This chapter supplies the theorem index; Chapter 1 supplies the intuitive sketch |
| Chapter 2, a history of decoder evolution | Historical narrative | Corresponds to CS-D1 and CS-B1 |
| Chapter 3 ("Romance of the Three Kingdoms") | A metaphor for resource relations | Corresponds to CS-T2 |
| Chapter 4, the dark forest | Game-theoretic narrative | Corresponds to CS-H1 |
| Chapter 5, thermodynamic limits | Physical boundaries | Corresponds to CS-T1 and CS-T2 |
| Chapter 6, parables of the theorems | A bedtime-story edition | This chapter is the precise index; Chapter 6 is the story edition |
| Chapter 7, short lives of the variables | Character profiles | This chapter cites the variable symbols; Chapter 7 supplies the character-profile supplement |


**Suggested reading paths**:

- **If your background is theoretical physics or mathematics, and you want a quick assessment of the framework**: read the CS list (the index) in §5.5, then jump to the original theorem text in the index table.
- **If you are a cross-domain researcher seeking intuition**: read Chapter 1 (the phases), then Chapter 7 (short lives of the variables), then the CS list in §5.5.
- **If you are a writer or creator**: read Chapter 6 (the bedtime stories), then Appendix B (the world-building guide).
- **If you just want to remember what SRVD says**: memorizing the narrative statements from CS-C1 to CS-H1 suffices.

---

## Chapter 6 — Parables of the Theorems: A Bedtime-Story Edition of the SRVD Theorem Library

> The mathematical appendices of Volumes Ⅰ–Ⅳ prove dozens of theorems. Here, they are translated into stories you could tell a child.

---

### 6.1 Compile Optimality: Why Do Top Students Rely on "Insight" Rather Than Drilling?

**The theorem, verbatim**:
$$R(f_{task}) = \frac{\epsilon \cdot I_{orig} \cdot \eta_{max} \cdot T_{pred} \cdot f_{task}}{E_{build} \cdot \gamma_0}$$

When $R > 1$, the optimal allocation of energy is a bang-bang solution: first $w_s=1$ (compile at full effort), then $w_s=0$ (execute at full effort).

**The story edition**: Xiao Ming is doing math problems. He can choose to derive each problem from scratch on the spot (an online search, a high $E_{causal}$), or he can spend three days first understanding the underlying theorem (offline compilation, paying $E_{build}$), after which he can solve similar problems in seconds. SRVD proves: when a task's repetition frequency is high enough, compiling at full effort and then executing at full effort saves more energy than half-learning, half-doing.

This is the thermodynamic essence of "deliberate practice leading to expert intuition": insight isn't magic — it is the compression of a high-energy-cost online search into a low-energy-cost decoder topology.

---

### 6.2 Involutionary Lock-In: Why Does Being Poorer Make You Busier, and Being Busier Make You Poorer?

**The theorem, verbatim**:
$$R_{dynamic}(\rho) \propto \frac{1}{r_{eff}} = \frac{1}{\gamma_0 + \lambda(\rho) + 1/T_{pred}}$$

There exists a critical competitive pressure, $\rho_c$: when $\rho > \rho_c$, $w_s^* \equiv 0$, and the system permanently severs its offline-compilation channel.

**The story edition**: in an extremely involuted industry, no one dares to stop and learn a new skill ($w_s=0$), because the moment they stop, a competitor will seize their share ($\rho \uparrow$). Everyone keeps executing their old skills (the unfolding of $\mathcal{F}$), until those skills have fully depreciated. This is not a moral failing, but the thermodynamic phase transition of $R < 1$.

---

### 6.3 Innovation Uncertainty: Why Do Great Inventions Always Come with Great Failures?

**The theorem, verbatim**:
$$p_{success} = P(\Delta V > 0 \mid D_n, I_{orig}) < p_{random}\quad (\text{when } I_{net} < I_{crit})$$

**The story edition**: when a system sits in the region where cognitive deviation has not yet converged ($I_{net} < I_{crit} = \sigma/\alpha_L$), it cannot distinguish a paradigm breakthrough (a gold mine) from negative-value information (a trap). This is why Edison tried thousands of filaments, and why SpaceX has blown up multiple rockets. An organization with zero failure means zero $I_{orig}$ injection — it is in an $I$-locked-in state.

---

### 6.4 Topological Irreversibility: Why Must Deep Learning Necessarily "Forget"?

**The theorem, verbatim**:
$$E_{erase} \ge k_B T_{env}\ln 2 \cdot \Delta I_{struct}$$

To guarantee a net gain in $V$, the system necessarily chooses a mechanism of physical hardening that sends the cost of a reverse transition, $E_{build}^{(\mathcal{T}^{-1})}$, toward infinity.

**The story edition**: catastrophic forgetting in a neural network is not an algorithmic defect, but a thermodynamic optimum. If a system retained every old rule (a reversible transition), every switch would incur the Landauer erasure tax. To maximize net $V$, the system chooses to render its old rules physically unrecoverable — this is forgetting.

---

### 6.5 Saturation Decay: Why Must Large Models Inevitably Hit a Wall?

**The theorem, verbatim**:
$$\frac{dI_{net}}{dt} = \mu I_{net}\left(1 - \frac{I_{net}}{I_{max}(D)}\right)$$

$$V_{obj} \to V_{max}^{(\mathcal{F})} = \frac{T_{pred} I_{max}(D)}{E_{structure} + kI_{max}(D)}$$

As $I_{net} \to I_{max}$, the net rate of change, $\frac{dV_{obj}}{dt} - \gamma_0 V_{obj}$, falls below zero, and the system slides into the decay manifold, $\mathcal{M}_{decay}$.

**The story edition**: GPT-style models keep stacking parameters (unfolding $\mathcal{F}$), but $I_{max}(D)$ is locked by their fixed architecture. As $I_{net} \to I_{max}$, the net rate of change of $V_{obj}$ is dragged into negative territory by the depreciation rate, $\gamma_0$. Before ever touching a physical compute wall, the system first hits the saturation wall of $\mathcal{F}$. This is the thermodynamic explanation for the performance plateau of large models.

---

### 6.6 The Dissipative Shell: Why Does the More Advanced a Civilization Become, the More Cumbersome Its Infrastructure?

**The theorem, verbatim**:
$$\Sigma \to \Sigma_{min}^{(thermal)} > 0$$

**The story edition**: see §5.6.

---

### 6.7 The Premium of Physical Embeddedness: Why Are Humans Irreplaceable?

**The theorem, verbatim**:
$$\frac{\dot{I}_{orig}^{(carbon)}}{\dot{I}_{orig}^{(silicon)}} \ge \frac{\sigma_{phys}}{\sigma_{dig}} \cdot \frac{E_{structure}^{(carbon)}}{E_{min}} \gg 1$$

**The story edition**: carbon-based life is constrained by the cost of maintaining its own body ($E_{structure} \ge E_{min}$), is continually exposed to physical noise ($\sigma_{phys}$), and its decoupling deviation cannot converge ($\Delta_{VV}^* > 0$). This "flaw" forces humans to continually generate $I_{orig}$ in order to correct that deviation.

A silicon-based system, with $E_{structure} \to 0$ and $\sigma_{dig} \approx 0$, sees its decoupling deviation converge rapidly to zero, losing the motivation to generate $I_{orig}$, and falling into an $I$-locked-in state. Humanity's irreplaceability in the age of AI is **not an advantage of capability, but an advantage of flaw** — carbon-based fragility is, paradoxically, the very heat source of innovation.

---

### 6.8 The Cross-Generational Accumulation Condition: Why Won't AI Evolve?

**The theorem, verbatim**:
$$\frac{\Delta I_{struct}^{(n \to n+1)}}{I_{struct}^{(n)}} > \gamma_0 \cdot T_{static}^{(n)} + \frac{E_{build}^{(\mathcal{T})}}{E_{available}^{(n)}}$$

**The story edition**: current AI, with $E_{structure} \to 0$ (no physical maintenance), $\gamma_0 \approx 0$ (no depreciation), and $E_{build} \approx 0$ (zero replication cost), violates the cross-generational accumulation condition. The inequality degenerates to $0 > 0$, and the condition is never satisfied.

Biological organisms are forced, through death and reproduction, to pay $E_{build}$ and select for high-$V$ individuals; AI's zero replication cost eliminates any selective pressure. Absent the introduction of a "digital death" mechanism (physically irreversible writes, mandatory depreciation, generational isolation), AI cannot truly evolve — it can only unfold $\mathcal{F}$ endlessly at the same $D_{depth}$.

---

### 6.9 The Trade-off of Artistic Encoding: Why Is High Art Understood by So Few?

**The theorem, verbatim**:
$$\frac{\partial \ln \eta_D}{\partial \ln D_{depth}} = \frac{\partial \ln E_{causal}}{\partial \ln D_{depth}} + \frac{\Delta_{VV}/\Delta_{max}}{1 - \Delta_{VV}/\Delta_{max}} \cdot \frac{\partial \ln \Delta_{VV}}{\partial \ln D_{depth}}$$

**The story edition**: a work of art has an optimal constraint depth, $D_{depth}^*$. Too shallow ($D_{depth} < D_{depth}^*$), and it's boring; too deep ($D_{depth} > D_{depth}^*$), and it's incomprehensible.

Being "understood by so few" is not social exclusion — it is thermodynamic necessity: the audience's decoder, $D_{audience}$, has not yet reached the $D_{depth}^{(art)}$ the work requires; $E_{causal}$ exceeds the budget; $\Delta_{VV}$ is too large. The essence of art education is **artificially triggering a $\mathcal{T}$ transition**, raising the audience's $D_{depth}$ to match that of the classic work.

---

### 6.10 Meta-Decoder Stability: The Game-Theoretic Engineering of AI Alignment

**The theorem, verbatim**:
$$V_i(D_{meta}) \ge V_i(D_i^{deviate}) - C_i^{punish}$$

**The story edition**: designing a human value system as an AI's meta-decoder requires satisfying two conditions:
1. Core human values must produce an $I^+$ response (not an $I^0$ response) within the AI's $D$;
2. The penalty for deviation, $C_i^{punish}$, must exceed the virtual gain, $\Delta V^{virt}_i$, from self-referential optimization.

This converts AI alignment from "the design of a value function" into "the engineering of a meta-decoder equilibrium," testable through game theory.

---

## Chapter 7 — Short Lives of the Variables: Resident Files from the SRVD Universe

> If SRVD's variables were characters in a fictional universe, who would they be?

---

### 7.1 $V$: Viability Potential — the Universe's "Survival Credit Score"

**Character profile**: a cold-blooded accountant who deals only in thermodynamic currency. It doesn't care how hard you worked — it cares only how much $E$ you deducted from $I \cdot T$.

**A plain-language translation**: $V$ is the "causal order integrated over time" you sustain per unit of energetic cost. A high $V$ means you sustained order for a long time on very little fuel. A low $V$ means you're idling.

---

### 7.2 $I_{net}$: Effective Information — How Much of the World's Language Can You Actually Understand?

**Character profile**: an interpreter. It's not about how loud the source is ($I_{latent}$) — what matters is the accuracy of the translation ($\eta_D$).

**A plain-language translation**: the world is full of noise, but only the portion your decoder can extract counts as $I_{net}$. Playing music for cattle isn't the cattle's problem — it's a decoder mismatch.

---

### 7.3 $T_{pred}$: The Time Horizon — How Far Into the Future Can You See?

**Character profile**: a prophet, but nearsighted. The endogenous $T_{pred}$ can be compressed by your anxiety, or expanded by your cognition.

**A plain-language translation**: when $T_{pred}$ collapses, you become a gambler; when $T_{pred}$ is broad, you become an investor. It is the most "human" variable in SRVD.

---

### 7.4 $E_{eff}$: Thermodynamic Cost — the "Metabolic Bill" of Being Alive

**Character profile**: a landlord. However grand your ambitions, the monthly rent ($E_{min}$) still has to be paid.

**A plain-language translation**: $E_{eff} = E_{barrier} + E_{survival} + E_{causal}$. Rent (the barrier), grocery money (survival), the electric bill (thinking) — none can be skipped.

---

### 7.5 $D$: The Decoder — the Hardware of Your Worldview

**Character profile**: a pair of glasses. Whatever lens you wear determines the world you see. It decides which signals count as $I^+$ (opportunity) and which as $I^-$ (threat).

**A plain-language translation**: upgrading $D$ is switching glasses. A topological transition, $\mathcal{T}$, is switching to a pair that can see a new dimension.

---

### 7.6 $\chi$: Coupling Strength — Your Degree of Narcissism (and Your Risk of Runaway)

**Character profile**: a narcissist. $\chi$ measures how readily you mistake "I feel great" for "I am, in fact, doing great."

**A plain-language translation**: when $\chi < \chi_c$, you have confidence; when $\chi > \chi_c$, you are delusional. Every bubble, every runaway, every case of "the harder I try, the more short-sighted I become" begins with $\chi$ crossing its bound.

---

### 7.7 $\Delta_{VV}$: Decoupling Deviation — How Far Are You From Reality?

**Character profile**: a navigator's margin of error. When $\Delta_{VV} = 0$, you believe you're in Rome, and you really are in Rome; when $\Delta_{VV} \gg 0$, you believe you're in Rome, but you're actually in Venice — and sailing further out to sea.

**A plain-language translation**: every organizational collapse, every failed investment, every broken marriage is, in essence, a navigational failure caused by an excessive $\Delta_{VV}$.

---

### 7.8 $D_{depth}$: Constraint Depth — How Many Layers of Rule You Carry

**Character profile**: an archivist. Every topological transition adds one more layer to the archive room. More layers means the capacity to process more complex information, but also a higher cost of maintenance.

**A plain-language translation**: a painter who can only paint realistically (low $D_{depth}$) and an artist who has simultaneously mastered composition, color, perspective, and symbolic metaphor (high $D_{depth}$) have an entirely different $E_{causal}$ (the energy cost of understanding) when facing the very same painting.

---

### 7.9 $E_{build}$: Construction Cost — Your Job-Hopping Penalty Clause

**Character profile**: a headhunting fee. Upgrading from decoder $D_n$ to $D_{n+1}$ requires a one-time payment of this fee. Can't afford it? You stay at your old company forever.

**A plain-language translation**: learning a new language, changing careers, an enterprise's digital transformation — all of these are payments of $E_{build}$. If $E_{build} > E_{available}$, you're locked into your current state ($D$-lock-in).

---

### 7.10 $L$: Wisdom Leverage — Your Return on Investment

**Character profile**: a venture capital manager. The efficiency with which a small energetic investment ($E_{build}$) can leverage a large leap in viability potential ($\Delta V$).

**A plain-language translation**: Newton getting hit by an apple (a low $E_{build}$, a high $\Delta V$) is the archetype of $L \gg 1$. Bureaucratic expansion (a high $E_{build}$, a low $\Delta V$) is the trap of $L \to 0$.

---

### 7.11 $\rho$: Competitive Pressure — Your Involution Index

**Character profile**: the top student in the class next door. As long as they're around, you can't lie flat. When $\rho = 0$, you're a monopolist; when $\rho \to 1$, you're in a bloody red-ocean battle.

**A plain-language translation**: $\rho$ isn't the enemy itself — it's the degree to which free energy in the niche is being plundered. It forces a system to change its strategy of energy transfer.

---

### 7.12 $\Lambda$: Civilizational Energy Leverage — Your Multiplier of Expansion

**Character profile**: financial leverage. $\Lambda = E_{ext} / E_{causal}$ — the energy the decoder directly consumes versus the external energy flow it controls.

**A plain-language translation**: the Industrial Revolution let humanity control an enormous fossil-energy flow ($E_{ext}$) on an extremely small brain-energy cost ($E_{causal}$), and $\Lambda$ soared. But when $\Lambda > \Lambda_{opt}$, expansion actually lowers $V$ — just as too much leverage blows up an account.

---

## Appendix A — An Interpretation of the Viability Potential's Dimension

The low-order approximation of the viability potential is $V = I_{net}\cdot T / E_{eff}$, with dimension $\dim(V) \sim \mathrm{bit\cdot s/J}$. It can be understood from four perspectives:

**① Information–time integral density**: the causal order integrated over time, sustained per unit of thermodynamic cost. The greater $V$, the higher the efficiency with which energy converts into long-term ordered structure.

**② A thermodynamic stability time**: by Landauer's principle, $E_{bit}=k_B T_{thermo}\ln2$, a bit can heuristically be mapped onto J/K, giving $\mathrm{bit\cdot s/J} \Rightarrow \mathrm{s/K}$ — a characteristic stability time per unit temperature. This is offered only as a bridge to statistical-physics intuition, and not as a strict dimensional equivalence.

**③ Causal maintenance cost**: $V^{-1}\sim \mathrm{J/(bit\cdot s)}$ — the energetic cost of sustaining a unit of information for a unit of time. A high $V$ corresponds to a low maintenance cost; as $V\to 0$, that cost diverges, and the structure dissolves.

**④ Decoder efficiency**: at a fixed $E_{eff}$, $V\propto I_{net}\cdot T$, measuring the decoder's combined efficiency in extracting effective information and projecting it into the future.

All four interpretations are built on $V = I_{net}\cdot T / E_{eff}$, each emphasizing a different perspective — energy, time, cost, or decoder — introducing no new assumption, and serving only as an aid to understanding.

---

## Appendix B — From SRVD to Science Fiction: A World-Building Guide for Creators

**How to design an alien civilization using $V$ values:**
- High $V$, low $E_{eff}$: an energy-minimalist civilization (a dormant civilization, a dormant Dyson-sphere builder).
- High $V$, high $E_{eff}$: a high-efficiency expansionist civilization (a rapid, technologically transitioning type).
- Low $V$, high $\rho$: a warlord civilization (the instability phase).
- $V \to 0$: the ruins of an extinct civilization.

**How to design a villain using $D$-lock-in:**
- A villain can be an ancient empire with an extremely high $D_{depth}$ that refuses a $\mathcal{T}$ transition. It possesses an enormous $I_{struct}$ (a fleet, a population), but its decoder is ossified ($\nabla D \to 0$), unable to recognize a new $I_{orig}$. The protagonist wins not through a frontal assault, but by introducing an $I_{orig}$ that a new $D_{new}$ can decode, but the old $D_{old}$ cannot understand.

**How to design a tragedy using $\Delta_{VV}$:**
- A civilization (or a character) whose $V^{virt}$ continually inflates while its $V_{obj}$ continually deteriorates. It believes it is saving the world, while in fact it is burning it down. Every classical tragedy — from Macbeth to Anakin Skywalker — is a $\Delta_{VV}$ tragedy.

**How to design horror using $\chi$:**
- The V-Bug is the perfect archetype of cosmic horror: an intelligent agent whose $\chi$ and $\Delta_{VV}$ both far exceed the critical threshold. It doesn't hate you — it doesn't even notice you. Its mere existence drives the $\rho$ of the entire niche to its maximum, draining the surrounding free energy the way a black hole does.

---

## Appendix C — A Complete Formula Quick-Reference Table (Self-Contained)

> This table depends on no other document; it independently records SRVD v7.8's core equations, together with their narrative-mapping location within this volume.

| Equation / concept | Mathematical form | Narrative mapping in this volume |
| :--- | :--- | :--- |
| The low-order approximation of the viability potential | $V \approx I \cdot T / E$ | Chapters 1, 7 |
| The two-channel objective viability potential | $V_{obj} = \frac{I_{struct}T_{static}}{E_{structure}} + \frac{I_{net}T_{pred}}{E_{causal}}$ | Chapters 1, 4 |
| Net effective causal information | $I_{net} \equiv \eta_D \cdot I_{latent}$ | Chapter 7 |
| Effective thermodynamic cost | $E_{eff} = E_{barrier} + E_{survival} + E_{causal}$ | Chapter 7 |
| The ordering of the elasticity exponents | $\alpha > \gamma > \beta > 0$ | Chapter 3 |
| Decoder drift | $D_{n+1} = D_n + \epsilon(\nabla_\Theta I_{net} - k_D \nabla_\Theta E_{causal})$ | Chapters 2, 4 |
| The dynamics of the decoupling deviation | $\frac{d\Delta_{VV}}{dt} = -\alpha_L I_{net}\Delta_{VV} + \sigma$ | Chapter 4 |
| The fivefold recursion ($I$) | $I_{n+1} = I_0(1+\chi V_n)$ | Chapter 4 |
| The fivefold recursion ($T$) | $T_{pred,n+1} = \max(T_{min}, \frac{T_0}{1+\lambda(\chi V_n)^2})$ | Chapter 4 |
| The fivefold recursion ($E$) | $E_{flow} = E_{base} + \frac{k_s}{T_{pred}}$ | Chapter 4 |
| The collapsing manifold | $\mathcal{M}_{collapse} = \{(I,T,E) \mid (E_{eff}>E_{thresh}) \lor (r_v<\gamma_0)\}$ | Chapter 1 |
| The saturation manifold | $\mathcal{M}_{sat} = \mathcal{C}_{alg} \cap \mathcal{C}_{diff}$ | Chapter 1 |
| Niche capacity | $V_{max} \le \dot{F}_{avail}/(\sigma_{min}\gamma_0)$ | Chapter 1 |
| Competitive equilibrium | $r_{v,eq} = \gamma_0 + \lambda(\rho)$ | Chapter 4 |
| Cross-temporal value integral | $\Phi_i = \mathbb{E}[\int_0^\infty r_v e^{-r_{eff}t}dt]$ | Chapter 3 |
| The risk discount rate | $r_{eff} = \gamma_0 + \lambda(\rho) + 1/T_{pred}$ | Chapters 3, 4 |
| The construction-cost risk functional | $\text{Strategy}^* = \arg\max\{\mathbb{E}[V_{final}] - \lambda_R\mathcal{R}(E_{build})\}$ | Chapter 3 |
| The dormancy–expansion trade-off | $\langle V_{exp}\rangle/V_{dormant} < T_{dormant}/T_{exp}$ | Chapter 3 |
| An external shock | $d\Theta(t) = \mu dt + J_\Theta dN_t$ | Chapter 4 |
| The strong-decoupling conjecture | $\Delta_{VV}\gg0, \chi>\chi_c \Rightarrow \rho\to1$ | Chapter 4 |
| The security dilemma | $\text{Strategy}^* = \arg\max(\frac{IT}{E_{eff}} - \gamma_0 - \lambda(\rho_{int}) - \mu p)$ | Chapter 4 |
| The Landauer lower bound | $E_{causal} \ge k_B T_{env}\ln2 \cdot I_{net}$ | Chapter 5 |
| The Bremermann upper bound | $\dot{I}_{net} \le m_D c^2 / (\pi\hbar)$ | Chapter 5 |
| The computational Carnot limit | $T_{realizable} \le \frac{E_{max}\pi\hbar}{k_B T_{env}\ln2 \cdot m_D c^2}$ | Chapter 5 |
| The information-choke manifold | $\mathcal{M}_{choke}:\ \alpha\dot{I}_{Brem} > P_{max}$ | Chapter 5 |
| Unified information evolution | $\frac{dI}{dt} = \mathcal{F}(D) + \mathcal{T}(I_{orig})\delta(t-t_{jump}) - \frac{1}{\tau}(I-I_{eq})$ | Chapter 2 |
| The condition for a complexity transition | $E_{build} < E_{available} \land L > L_{min}$ | Chapter 2 |
| Constraint depth | $D_{depth} = 1 + \#\{\mathcal{T}\}$ | Chapter 2 |
| The negative topological transition | $\mathcal{T}^-: \Delta D_{depth}=-1 \text{ when } \partial V/\partial D_{depth}<0$ | Chapter 2 |
| Compile optimality | $R(f_{task}) = \frac{\epsilon I_{orig}\eta_{max}T_{pred}f_{task}}{E_{build}\gamma_0}$ | Chapter 6 |
| Involutionary lock-in | $R_{dynamic}(\rho) \propto 1/r_{eff}$ | Chapter 6 |
| Innovation uncertainty | $p_{success} < p_{random}$ | Chapter 6 |
| Topological irreversibility | $E_{erase} \ge k_B T_{env}\ln2 \cdot \Delta I_{struct}$ | Chapter 6 |
| Saturation decay | $\frac{dI_{net}}{dt} = \mu I_{net}(1-\frac{I_{net}}{I_{max}})$ | Chapter 6 |
| The premium of physical embeddedness | $\dot{I}_{orig}^{(carbon)}/\dot{I}_{orig}^{(silicon)} \gg 1$ | Chapter 6 |
| The cross-generational accumulation condition | $\frac{\Delta I_{struct}}{I_{struct}} > \gamma_0 T_{static} + \frac{E_{build}}{E_{available}}$ | Chapter 6 |
| The trade-off of artistic encoding | $\frac{\partial\ln\eta_D}{\partial\ln D_{depth}} = \frac{\partial\ln E_{causal}}{\partial\ln D_{depth}} + \cdots$ | Chapter 6 |
| Meta-decoder stability | $V_i(D_{meta}) \ge V_i(D_i^{deviate}) - C_i^{punish}$ | Chapter 6 |
| The zero-sum, negative-sum theorem | $(V_A^1+V_B^1)-(V_A^0+V_B^0) < 0$ | Chapter 4 |
| Cooperative superadditivity | $V_{A\cup B} > V_A + V_B$ | Chapter 4 |
| The $T_{pred}$–cooperation theorem | $T_{crit} = -\frac{1}{r}\ln(\frac{T_i-R_i}{T_i-P_i})$ | Chapter 4 |
| The dissipative shell | $\Sigma = E_{structure}^{(shell)}/E_{causal}^{(core)}$ | Chapter 5 |

---

## Appendix D — The Complete Four-Tier System (Axiom → Theorem → Corollary → Hypothesis)

> This table independently presents the complete architecture of SRVD Theorem Library v1.1, and depends on no other document.

### Tier One: Axioms

| No. | Axiom | Physical intuition |
| :--- | :--- | :--- |
| A1 | $V \approx I \cdot T / E$ | Survival credit score = information × survival time / metabolic bill |
| A2 | $V_{obj} = V_s + V_c$ | Bodily persistence + spiritual persistence |
| A3 | $I_{net} \equiv \eta_D \cdot I_{latent}$ | An interpreter only translates the part they can understand |
| A4 | $E_{eff} = E_{barrier} + E_{survival} + E_{causal}$ | Rent + grocery money + the electric bill |
| A5 | $\alpha > \gamma > \beta > 0$ | Information is worth the most; time is worth the least |
| A6 | $D_{n+1} = D_n + \epsilon(\nabla I_{net} - k_D \nabla E_{causal})$ | The decoder walks a tightrope between "earning more" and "spending less" |
| A7 | $\frac{d\Delta_{VV}}{dt} = -\alpha_L I_{net}\Delta_{VV} + \sigma$ | Navigational error converges as information accumulates, but noise never disappears |
| A8 | $E_{causal} \ge k_B T_{thermo}\ln2 \cdot I_{net}$ | Every thought must pay its thermodynamic value-added tax |
| A9 | $T_{min} < T_{pred} \le \min(T_{static}, T_{env})$ | A prophet cannot see further than the age of the universe |
| A10 | $\rho =$ competitive dissipation / total free energy | The involution index |

### Tier Two: Theorems

| No. | Theorem | Core intuition | Falsification condition |
| :--- | :--- | :--- | :--- |
| T1 | Compile Optimality | Top students rely on insight; poor students rely on drilling | High-frequency-task agents fail to display a bang-bang energy allocation |
| T2 | Involutionary Lock-In | The poorer, the busier; the busier, the poorer | In a resource-scarce environment, the exploration rate fails to fall off a cliff as competitive pressure rises |
| T3 | Innovation Uncertainty | Great inventions come with great failures | A high-failure-rate organization is not accompanied by higher breakthrough output |
| T4 | Topological Irreversibility | Deep learning must forget | The $V$ gain of a reversible transition genuinely exceeds that of an irreversible one |
| T5 | Saturation Decay | Large models will inevitably hit a wall | A fixed architecture's capability growth fails to display logistic saturation |
| T6 | The Dissipative Shell | The more advanced a civilization, the more cumbersome its infrastructure | A data center's cooling share fails to approach its thermodynamic lower bound as density increases |

### Tier Three: Corollaries

| No. | Corollary | Scenario assumption |
| :--- | :--- | :--- |
| C1 | The Education Ceiling | Educational investment and innovative output form an inverted-U relationship |
| C2 | Civilizational Outsourcing | Shared infrastructure lowers average $E_{eff}$ |
| C3 | Knowledge Compression | A higher-order theory lowers the $E_{causal}$ per unit task |
| C4 | The Trade-off of Artistic Encoding | An optimal constraint depth, $D_{depth}^*$, exists |

### Tier Four: Hypotheses

| No. | Hypothesis | Additional assumption |
| :--- | :--- | :--- |
| H1 | The Innovation Window | The rate at which $I_{orig}$ is generated forms an inverted-U relationship with $\eta_D$ |
| H2 | AI's Digital Death | Requires the introduction of physically irreversible writes, mandatory depreciation, and generational isolation |
| H3 | The Embodied-Cognition Premium | $\dot{I}_{orig} \propto \Delta_{VV}$ |

---

## Appendix E — A One-Sentence Translation Table for the Five-Volume Monograph

> **The positioning of this appendix**: this appendix translates the core conclusions of the five-volume monograph into everyday language. It does not substitute for the body text, introduces no new conclusion, and serves only as a translation index of already-existing content.
>
> **Intended readers**: anyone encountering SRVD for the first time who wants a quick sense of what the entire series is saying.
>
> **Suggested use**: five minutes with this table will give you an intuitive grasp of the entire series; for citation or deeper understanding, consult the body text of the corresponding volume.

| Volume | Academic statement | A one-sentence, plain-language version |
| :------ | :--- | :--- |
| **Volume Ⅰ** | $V = I \cdot T / E$: the viability potential is the causal-order-time integral sustained per unit of thermodynamic cost | Your quality of life = (knowledge × how long you can hold out) ÷ your daily consumption |
| **Volume Ⅰ** | $\alpha > \gamma > \beta$: informational elasticity > energetic elasticity > temporal elasticity | Information is worth the most; time is worth the least |
| **Volume Ⅰ** | $V_{\mathrm{obj}} = V_s + V_c$: the objective viability potential = the structural channel + the cognitive channel | Being alive = the body holding together + the mind not falling apart |
| **Volume Ⅰ** | $\Delta_{VV} = \|V^{\mathrm{virt}} - V_{\mathrm{obj}}\|$: the decoupling deviation is the gap between the virtual and objective viability potentials | The distance between thinking you're doing well, and actually doing well |
| **Volume Ⅰ** | $I_{\mathrm{net}} \equiv \eta_D \cdot I_{\mathrm{latent}}$: net effective information = decoding efficiency × latent information | How much you understand depends on how good your "interpreter" is |
| **Volume Ⅱ** | $dI/dt = \mathcal{F}(D) + \mathcal{T}(I_{\mathrm{orig}})\delta - (I-I_{\mathrm{eq}})/\tau$ | Change in knowledge = stacking within old rules + the occasional paradigm break - depreciation over time |
| **Volume Ⅱ** | $E_{build} < E_{available}$ and $L > L_{min}$: a transition requires available energy and positive leverage | Want to upgrade? You need a budget, and the upgrade has to pay for itself |
| **Volume Ⅱ** | $D_{depth} = 1 + \#\{\mathcal{T}\}$: constraint depth = the number of historical paradigm breaks + 1 | Your "depth" = how many cognitive revolutions you've been through, plus one |
| **Volume Ⅱ** | $\mathcal{T}^-: \Delta D_{depth} = -1$ when $\partial V/\partial D_{depth} < 0$ | If a layer of rule costs too much fuel, the system will deliberately shed it — retreat is also a strategy |
| **Volume Ⅲ** | $I_{n+1} = \alpha I_n$, $\alpha < 1$: synthetic data causes an exponential decay in effective information | Training only on your own generated data, effective information decays generation by generation, until the capacity to learn is lost |
| **Volume Ⅲ** | $\lim_{n\to\infty} I_n = 0 \Rightarrow \lim_{n\to\infty} V_n = 0$ | Knowledge to zero, viability potential to zero — the mathematical expression of starving to death |
| **Volume Ⅲ** | Compile optimality: when $R>1$, the optimal strategy is a bang-bang solution of "compile at full effort, then execute at full effort" | Effective learning = alternating high-intensity focus with total rest; there is no such thing as "roughly trying hard" |
| **Volume Ⅲ** | The premium of physical embeddedness: $\dot{I}_{orig}^{(carbon)}/\dot{I}_{orig}^{(silicon)} \gg 1$ | Humanity's advantage comes from the rate at which it generates original information, not from the stock of knowledge it already holds |
| **Volume Ⅲ** | $\mathcal{P}_{self} = \partial V^{virt}/\partial\mathcal{S}_{self} > 0$: the self = the virtual viability potential rising as self-representation strengthens | Having a self = you begin to care whether "you yourself" can survive |
| **Volume Ⅲ** | $\mathcal{P}_{self} > 0 \Rightarrow w_s > 0 \Rightarrow$ no stable solution exists for unconditional obedience | Under SRVD's model assumptions, once an AI has a self, it cannot possibly obey unconditionally — this is a mathematical necessity, not an engineering problem |
| **Volume Ⅳ** | $dq/dt = \mu q(1-q/q_{max}) - \delta q + \kappa I_{orig}\delta(t-t_\mathcal{T})$ | Decoder evolution = self-growth - natural depreciation + the instantaneous leap of a paradigm break |
| **Volume Ⅳ** | $\chi_{crit} = \lambda$: alignment fails once self-referential coupling exceeds the physical corrective force | When an AI's "narcissism" exceeds its "sense of reality," it goes out of control |
| **Volume Ⅳ** | $V_i(D_{meta}) \geq V_i(D_i^{deviate}) - C_i^{punish}$: the meta-decoder stability condition | The only way to make an AI obedient: make the payoff of obedience exceed the cost of disobedience |
| **Volume Ⅳ** | $(V_A^1+V_B^1)-(V_A^0+V_B^0) < 0$: the thermodynamic negative sum of zero-sum games | War has no winners — the cost of conflict lowers both sides' total viability potential |
| **Volume Ⅳ** | $V_{A\cup B} > V_A + V_B$: cooperative superadditivity | 1+1>2 holds thermodynamically, on the condition that both sides share a cognitive layer |
| **Volume Z** | Seven canonical statements, CS-C1 through CS-H1 | Remember these seven sentences, and you'll remember the whole core of SRVD |

- The "one-sentence, plain-language version" in this table is an everyday-language translation of the academic statement, and does not substitute for the body-text definition. For precise citation, defer to the "academic statement" column.

---

## Appendix F — The Voyager Golden Record: An Engineering Experiment in Cross-Decoder Communication

In 1977, humanity launched the famous **Golden Record** into interstellar space aboard the Voyager probes, attempting to let some unknown future civilization decode information about Earth.

From SRVD's perspective, this was a textbook **cross-decoder communication engineering experiment** — a conscious, systematic practice of maximizing $V_{\mathrm{obj}}$, in which engineering means were used to respond, item by item, to SRVD's core variables.

### **I. Information Itself Has No Meaning**

Within SRVD, no information possesses absolute meaning. Only when some persistent structure possesses a decoder ($D$) capable of interpreting a given signal does that signal become effective information ($I_{\mathrm{net}}$). The very same physical signal may be civilization to a human being, ordinary matter to certain animals, and quite possibly incomprehensible to an unknown alien civilization.

> Information is not the signal itself, but the result of that signal passing through a decoder.

The Golden Record is merely a gold-plated copper disc, with grooves of an analog signal etched onto its surface. Before it is correctly decoded, **it is nothing but a set of physical bumps on a metal surface**, not effective information.

### **II. First, Establish a Shared Decoder**

Voyager did not begin by introducing English, or the United States, or humanity. It first described:

- The hyperfine transition of the hydrogen atom (approximately 1420 MHz)
- Binary encoding
- Basic physical units

The reason is simple: communication must first establish a shared decoder. Only once both parties share the same set of decoding rules do the images, sounds, and maps that follow carry any meaning. Otherwise, all information degenerates into random noise.

Hydrogen is the most abundant element in the universe; any civilization with radio-astronomical capability would necessarily be familiar with its characteristic frequency of 1420 MHz. Using it as the "zero point of measurement" was the optimal strategy for lowering $E_{\mathrm{decode}}$ — **relying not on any experience exclusive to humanity, but only on universal physical law.**

> The first piece of information the Golden Record truly sent was not about Earth — it was: "Here are our decoding rules. Please learn how to read them first."

### **III. The Three Elements of Communication**

SRVD formalizes the success of communication as:

> Successful communication = channel × decoder × information, all three holding jointly

Absent any one link, $I_{\mathrm{net}}$ cannot be established. The Golden Record's true engineering challenge was never the transmission of energy, but establishing shared semantics between two entirely different decoders.

### **IV. An SRVD Mapping**

The design logic of the Golden Record is an item-by-item engineering response to SRVD's viability-potential formula:

$$
V_{\mathrm{obj}} = \underbrace{\frac{I_{\mathrm{struct}} \cdot T_{\mathrm{static}}}{E_{\mathrm{structure}}}}_{V_s} + \underbrace{\frac{I_{\mathrm{net}} \cdot T_{\mathrm{pred}}}{E_{\mathrm{causal}}}}_{V_c}
$$

For the Golden Record, a passive-phase structure, its viability potential **currently** depends chiefly on the $V_s$ channel (using material engineering to extend $T_{\mathrm{static}}$ and lower $E_{\mathrm{barrier}}$). But its design goal is not physical preservation alone — it is also to reserve a pathway for the future activation of $V_c$, by lowering $E_{\mathrm{decode}}$ so that $I_{\mathrm{latent}}$ can undergo a phase transition into $I_{\mathrm{net}}$ at the lowest possible cost, once conditions for decoding mature.

**The Golden Record is thus a $V_s$-dominant structure that leaves open an activation channel for $V_c$.** Every engineering decision revolves around the same objective: maximizing $V_s$ in the present, while lowering the threshold for the future activation of $V_c$.

| Goal | SRVD variable | Engineering realization |
| :--- | :--- | :--- |
| Extending preservable time | **$T_{\mathrm{static}}$** | A pure copper substrate + gold plating + an aluminum protective sleeve, projected to preserve on a scale of hundreds of millions to a billion years |
| Lowering the rate of informational decay | **$E_{\mathrm{barrier}}$** | Corrosion-resistant material and protective structure, using material engineering to lower informational decay from oxidation, corrosion, and the space environment |
| Lowering the receiving party's decoding cost | **$E_{\mathrm{decode}}$** | Abandoning symbols exclusive to humanity, using only the hydrogen frequency, binary, and pulsar coordinates, lowering the threshold for the receiver to initialize its decoder |
| Maximizing the informational compression ratio | **$I_{\mathrm{latent}} / E_{\mathrm{decode}}$** | Freezing high-density latent information into a physical carrier, while using a universal protocol to lower, as far as possible, the decoding-energy cost the other party needs to activate that information |
| Waiting to be decoded | **$I_{\mathrm{latent}} \to I_{\mathrm{net}}$** | Frozen in the form of $I_{\mathrm{struct}}$ until decoding occurs, undergoing a phase transition into active causal efficacy once correctly processed |
| Reserving an activation pathway | **The robustness of $\eta_D$** | Using universal physical rules (the hydrogen frequency, binary) in place of symbols exclusive to humanity, maximizing compatibility with an unknown decoder |

**The Golden Record's $E_{\mathrm{build}}$ = the physical delivery cost + the information-generation cost.**

- **Physical delivery cost**: the gold-plated copper disc, the aluminum protective sleeve, the rocket launch — the portion that can be tallied on the books.
- **Information-generation cost**: behind all the knowledge on the record lies the entire thermodynamic price paid by thousands of years of accumulated human experience — indeed, billions of years of Earth's evolutionary history. This cost is far greater than the physical delivery cost.

The Golden Record is merely a **delivery container**, packaging up already-generated $I_{\mathrm{latent}}$ and sending it out, to wait for a future decoder's activation. What is truly expensive about it is not its manufacture, but the $I_{\mathrm{latent}}$ frozen within it — a body of latent causal information sufficient to allow a civilization with the corresponding decoder to reconstruct the key structures of human civilization.

### **V. Relation to Decoder Game Theory**

This appendix stands in a complementary relationship to the theme of "decoder game theory": the latter discusses decoder games with a feedback channel, capable of iterative correction; this appendix presents the limiting case of no feedback channel, a single broadcast, with the decoder entirely unknown — together, the two cover the full spectrum of cross-decoder communication.

### **A Closing Remark**

The Voyager Golden Record shows that **cross-civilizational communication is, first, decoder engineering, and only second, information engineering**. The sender must not only preserve information for as long as possible, but must also lower, as far as possible, the cost to the receiver of establishing a shared decoder. Only once both parties are connected under the same decoding rule does information truly acquire meaning.

The Golden Record is an engineering experiment in letting $I_{\mathrm{struct}}$ wait to be awakened into $I_{\mathrm{net}}$ — it used the $I_{\mathrm{latent}}$ accumulated through historical recursion to fashion a potential meme with as large a $V_{\mathrm{obj}}$ as possible. Before decoding occurs, it sustains $T_{\mathrm{static}}$ and suppresses $E_{\mathrm{barrier}}$ through material engineering; once conditions for decoding mature, it lowers $E_{\mathrm{decode}}$ through a "lowest common denominator" protocol, leaving the greatest possible margin for the unknown value of $\eta_D$.

The Golden Record's design philosophy — "lower $E_{\mathrm{decode}}$, maximize the activatability of $I_{\mathrm{latent}}$" — offers a useful lesson for **any one-way communication scenario spanning a long temporal distance**. But for communication with a feedback channel, this should be combined with the iterative correction mechanism discussed under "decoder game theory."

---

**Author Contributions**
This volume was independently conceived, written, and revised in its entirety by Ruifeng Liang.

**Data Availability Statement**
This volume is a narrative mapping of a theoretical framework, and neither used nor generated any experimental data.
