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

**Acknowledgments**
No dedicated funding was received in the course of writing this preprint.

**Author Contributions**
This preprint was independently conceived, written, and revised in its entirety by Ruifeng Liang.

**Competing Interests**
The author declares no competing interests related to this research.

**Data Availability Statement**
This preprint is a work of theoretical framework research, and neither used nor generated any experimental data.

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
