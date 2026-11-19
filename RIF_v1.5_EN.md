# Relational Information Framework (RIF) {.unnumbered .unlisted}

## v1.5 — Parts One to Three {.unnumbered .unlisted}

**LiangRuifeng** | ORCID: [0009-0002-8575-7127](https://orcid.org/0009-0002-8575-7127) | 2026 | v1.5 | fineflowerrain@gmail.com

<!-- imprint-begin -->
DOI (concept DOI; resolves to the latest version): [10.5281/zenodo.24365794](https://doi.org/10.5281/zenodo.24365794)

DOI for this edition (v1.5): [10.5281/zenodo.24365795](https://doi.org/10.5281/zenodo.24365795)

License: CC BY 4.0 ([creativecommons.org/licenses/by/4.0](https://creativecommons.org/licenses/by/4.0/))

Reproducibility package: [10.5281/zenodo.24349831](https://doi.org/10.5281/zenodo.24349831)
<!-- imprint-end -->

> This book is self-contained: all notation, protocols, and criteria are given within it. Where adjacent frameworks come up, only a one-sentence statement of the division of labor is given, and the validity of this book is not made to rest on their premises. What this book delivers is the measurement layer: the numerical examples demonstrate the reading rules (empirical data with a cited source are excluded from this), and the test designs and replication scripts are in Appendix C.

**Abstract.** The Relational Information Framework (RIF) defines "information" as **the rarity of a reading relative to a specific decoder holder (hereafter the holder) and its background**: the same sound wave is a warning to a local, noise to a passing tourist, and an input awaiting fitting to an untrained translation model. Shannon's measure assigns all three the same number under the same source. RIF asks for a different number — how rare this reading is for **this** holder, and how much time and energy the holder spends to read it.

The framework thereby distinguishes two classes of information. **Structural information** is the rarity of an object's own organization against a given background; **causal information** is the rarity of an effect reading against the baseline that "the effect would also appear under control conditions." Each class is paired with a persistence time and an energy cost; together they form the I–T–E triplet. A decoder holder must satisfy four joint criteria: it maintains an identifiable boundary by itself, it extracts environmental differences selectively, it undergoes a state update triggered by that extraction, and the update has causal significance for its own persistence. A boundary may not be borrowed. Instruments used only for measurement, and public reading protocols, do not satisfy the criteria and are therefore not holders.

The measurement layer presupposes no dynamics. The part that is **already executable** consists of five commitments. First, the background is split into two notations: the **habitat background** $B^{\mathrm{env}}$ takes the natural frequency of the reading in the environment the holder inhabits and is the **default** convention; the **protocol baseline** $B^{\max}$ takes the maximum-entropy reference specified by the protocol and **must be declared explicitly**. Second, boundary identification is written as a four-step procedure with three classes of candidates, two stopping conditions, and three failure reports — what it delivers is a **candidate pool plus rejection rules, not a unique-solution algorithm**; when candidates are incompatible, they are treated as multiple solutions, with an interval and a sensitivity analysis. Third, causal determination proceeds in two steps: the effect is first identified by a control design, and then its rarity and interval are reported; equivalence conclusions are given by two one-sided tests (TOST). Fourth, holder-level costs are by default not aggregated and are reported holder by holder; a composite quantity is given only when four explicit declarations are complete (§13.4). Fifth, wherever a "typical value" is involved, the name of the statistic, its conditions of validity, and its numerical value are always given.

What remains a **candidate rule** and has not yet been operationalized is how the viability resolution constructs reading categories, how the time window of the habitat background is fixed, and how qualification and polarity are judged (§12.9, tagged **Hypothesis**); these gaps are registered under "Limitations and Open Problems" at the end of the book. This book discusses "how to read", not "how the world must be".

**Keywords**: relative information; decoder; persistent structure; structural information; causal information; measurement protocol

***

### The Three Parts and How to Read Them

This book has three parts. **Part One · Conceptual Foundations** answers "what the object of study is": persistent structures, decoders, the two classes of information, and how boundaries are drawn. **Part Two · Notation and Measurement** answers "how a reading is taken": notational conventions, structural rarity, causal rarity, rule depth, the classification of decoders, and background models. **Part Three · Lineage and Comparison** answers "how this relates to existing work": the line of demarcation from contemporary stochastic thermodynamics, and an inventory of prior work.

The three parts are layered by level of question. I have set myself one discipline: a judgment stated in everyday language in Part One must, in Part Two, be traceable to a quantity that can take a value; a quantity given in Part Two must, in Part One, have a clear account of which mode of existence it corresponds to. This discipline blocks the two most common failures — an account that is lively but cannot be measured, and formulas that are tidy but do not say what they measure.

A reader with limited time can follow this line: Preface → Chapter 2 (the conceptual entry point to everyday information) → Chapter 4 → Chapter 5 → Chapter 7 → the definition of rarity and the background rules at the opening of Chapter 12 → the causal criterion at the opening of Chapter 13. The remaining chapters add detail, boundaries, and comparisons along this main line. The Symbol Constitution ends with an appended "Quick Index to the Numbered Lists", which is used to tell apart the several numbered lists in the book.

### A Note on Tags

Tags come in two kinds; do not read them together.

**Provenance tags** answer "whose statement is this": **Prior work** denotes a published theory, concept, or observation, which is not an original contribution of RIF and does not depend on RIF holding; **Definition** denotes a term or criterion selected by this book, which is a convention rather than a discovery, and is marked only where a core term is formally defined for the first time.

**Evidence levels** answer "how firm is this statement". This book has four levels. **Theorem** requires explicit premises, a complete derivation, and a conclusion that holds strictly under those premises — the main text of this book claims no theorem of its own, and wherever the word "theorem" appears, it cites a prior result and says so; **Proposition** has a formal statement, but its premises are to be calibrated, or some step of its derivation depends on an unproven modeling assumption, and each carries three lines, "premises–result–failure conditions"; **Candidate Corollary** is derived from some proposition under additional conditions and has not been independently tested (the main text does not yet use this level); **Hypothesis** is an empirical or mechanistic conjecture and has only supporting rationale and a falsification condition.

Unmarked statements are, by default, this book's conventions on terms and criteria, or conclusions that follow directly from those conventions.

***

## Preface: Three Questions Still Unanswered

Classical mechanics once pictured the world as a machine made of determinate parts: given initial conditions, the future could be computed. Entering the twentieth century, science and philosophy gradually turned to another understanding — what a thing is does not necessarily depend on what it is made of at this moment, and depends more on what relations it keeps maintaining through change.

This turn did not originate with this book. Process philosophy, systems theory, and dynamical systems theory have each put forward similar insights along their own paths. RIF accepts this relational starting point and organizes it into a measurable framework whose core is decoder relativity and the $I$, $T$, $E$ triplet.

Systems theory, information theory, and cybernetics, in the course of this very turn, each touched from a different direction on a different side of the same problem. RIF puts three questions to them in turn:

**On systems theory:** Where is the boundary of the system you speak of?

**On information theory:** Why is information that is useful to one person meaningless noise to another?

**On cybernetics:** For a system that controls itself by feedback, where is the boundary of "itself"?

The three questions look as if each asks about something different, but they are three entrances to the same question: **who drew the boundary, for whom it was drawn, and whether it still counts once drawn.** Systems theory treats the boundary as given and so need not answer the first; information theory abstracts the receiver (the holder, in what follows) into a probability distribution and so need not answer the second; cybernetics takes "itself" to be the extent of the feedback loop and so need not answer the third. The piece that each of the three disciplines sidesteps is exactly the piece where they overlap.

RIF connects the three questions. **Prior work**: Information holds relative to a receiver — this idea has versions in biosemiotics, second-order cybernetics, and the free energy principle. RIF adopts this view and operationalizes it as a measurable form: **information** holds only relative to a specific decoder, and this **decoder holder** must satisfy four necessary conditions and be a persistent structure with a self-maintained boundary; the measurement layer additionally has a set of reading protocols that do not require a boundary. Turning "relative to whom" from an intuition into a framework with explicit criteria is RIF's own advance. Of this, the holder criteria and the measurement protocols have been given, whereas "how readings are partitioned and how the background is constructed from persistence constraints" remain candidate rules whose operationalization is not yet complete (§12.9, and "Limitations and Open Problems" at the end of the book).

This book attempts to answer a question that Shannon deliberately set aside:

> **What, exactly, is information,** or, put differently: **what is complete information?**

Shannon's measure of information is complete within its own question: given a source distribution, how much reduction in uncertainty a symbol carries has one correct answer, regardless of who is listening. This is precisely its strength. This book asks a different question: **when you say "I have obtained a piece of information", under what conditions was that information obtained?** The answer to this question does not lie in a probability distribution but in three things: "who is reading, whether they can afford to read, and whether they will be changed by having read."

***

## Part One · Conceptual Foundations

> This part answers "what the object of study is": persistent structures, decoders, the two classes of information, and how boundaries are drawn. The judgments here are all stated in everyday language, but each of them is required, in Part Two, to land on a quantity that can take a value.

***

## Chapter 1 — Why "System" Is Not Enough

General systems theory tells us: do not look only at the parts; look at the whole.

This statement is right. But it leaves one question unasked:

> **Who draws the boundary of the whole?**

Bertalanffy distinguished the system from its environment, but the system/environment boundary is usually treated as **given**. An organism has skin, a cell has a membrane, a machine has a casing. (**Prior work**: Maturana and Varela's theory of autopoiesis attempts to define the boundary from the system's internal process of self-production, rather than treating the boundary as externally given. RIF also starts from self-maintaining processes, and further binds the boundary to information–time–energy records.)

But when we face typhoons, ecosystems, civilizations, languages, institutions, or a person's social identity, is the material boundary still enough?

A typhoon has no skin. Air molecules keep flowing in and out of the vortex, and you cannot draw a permanent material boundary around a typhoon the way you can around a stone. But you can still trace how the pressure field forms an energy flow, how the energy flow sustains the rotating structure, and how the rotating structure sustains its own pattern. **A typhoon does not depend on any fixed batch of air molecules; it depends on the relations that these molecules keep among themselves.**

So it is with a person. The vast majority of the cells that made up your body ten years ago are no longer there. What makes you still "you"? Something that persists after the matter has been replaced. In a country, the population turns over while the institutions continue; in a language, the vocabulary changes while the structure remains. These examples all point to one thing:

> **A system is not a material box; a system is a persistent relation.**

Systems theory was the first to make this clear. But it did not answer: **where, exactly, is the boundary of this relational pattern drawn?** Why do we intuitively think that a person's boundary is roughly his skin and does not include the cup of coffee he drank yesterday, and yet say "Confucius's thought is still alive" — Confucius's skin ceased to exist long ago — is that sentence a metaphor, or some kind of genuine boundary claim? Systems theory supplies no tool for answering.

This gap is deeper than it looks. Systems theory gave us two things: a unit of observation (the system) and a way of describing it (state, parameters, environment, inputs and outputs). What it did not give is **the rule for delimiting this unit of observation**. So in practice one falls back on convention: biology relies on the cell membrane, meteorology on isobaric surfaces, sociology on the range of application of institutional texts. These conventions each have their reasons, but they are not one set of rules and cannot be translated into one another. When the object of study straddles these conventions — a person who involves both the body and a social identity, a software system that involves both hardware and a market — the conventions fail.

**This book's alternative is to change the boundary from a "given premise" into a "conclusion to be delivered."** Whether an object is a system is no longer declared in advance by the observer, but determined by whether it can be matched with a self-consistent set of records. This set of records has three dimensions: information, time, and energy. If the three can hold at once on the same object, the same decoder, and the same observation window, the object holds; if they cannot be matched, one cannot claim that it holds.

The cost of this turn is that **"boundary" becomes an object that can be revised, rather than a one-time answer.** Chapter 12 therefore writes boundary identification as an iterative procedure — allowing non-convergence, multiple solutions, and undecidability. This comes from the object domain itself; forcing a unique solution would instead conceal the undecidability in measurement, and this book's treatment is to report it as a legitimate measurement conclusion.

***

## Chapter 2 — Information in Everyday Life: From Messages to Relative Readings

People talk about "information" every day: stock-market news, policy announcements, street rumors, food nutrition, commodity pricing, the exchange of value between people, even whether a song sounds good or whether one person still likes another. They look as if they belong to different fields, but they share one point: people are not only recording what has happened in the outside world, but also judging what those changes mean for themselves.

But everyday language calls several different things "information". A message can be recognized without being rare; it can be rare without being unexpected to some subject; it can be unexpected without changing the subject's action; it can change action without having a detectable effect on the subject's own persistence.

This chapter therefore first separates several "differences" that are often mixed together, and then explains which one RIF wants to measure. This chapter is a reader's guide; formal definitions, estimation methods, and criteria remain as given in Chapters 12 and 13 of Part Two.

### 2.1 Telling Message, Reading, and Amount of Information Apart

"The maximum temperature in some place today is 25 degrees Celsius" is, first of all, a message or an observed value. It tells us what happened, but from this number alone we cannot yet answer how much statistical information it contains, much less what it means for any particular subject.

To compute the statistical rarity of an outcome, one must at least first specify which outcomes can occur, how outcomes are classified, and with what probability each class of outcome occurs against what background. Without these specifications, "25 degrees Celsius" is only a reading, not an already-determined amount of information.

There are at least three levels here:

1. **External difference**: what actually changed in the environmental quantity, for example the temperature going from 20 to 25 degrees Celsius.
2. **The subject's reading**: whether a given subject has read this change, and into which categories it has divided the change.
3. **Subsequent effect**: whether this reading has changed the subject's state or action, and whether that change is causally linked to the subject's own persistence.

The three cannot substitute for one another. That there is a difference in the outside world does not mean that a subject has read it; that a subject has read a difference does not mean it has had meaningful consequences for the subject; and observing a change in behavior does not automatically prove that the change was caused by this message.

### 2.2 Four Differences Often Lumped Together as "Information"

#### 2.2.1 Distinguishability: Whether It Can Be Told Apart

Distinguishability asks: can two objects or two states be told apart by some observer or measuring device?

For example, can a scale tell 3.0 kg from 3.1 kg; can a listener hear that two notes differ in pitch.

The ability to distinguish depends on measurement resolution, noise, observation conditions, and the classification rule adopted. It does not by itself answer how rare an outcome is against the background, nor how important it is to whom. A difference that appears every day can be recognized easily; an extremely rare difference may also exceed the resolving ability of an instrument or a subject.

Therefore **distinguishability is neither rarity nor importance**. In RIF, distinguishability is one of the preconditions for forming a reading; whether a reading can be distinguished, and whether it is worth the subject's paying a cost to distinguish it, are two different questions.

#### 2.2.2 Shannon Information: How Rare in a Given Source

Shannon information theory takes a probability distribution as the starting point of computation. For a discrete outcome $x$, its self-information is:

$$I_{\mathrm{Sh}}(x)=-\log_2\Pr(x)$$

If the probability of an outcome occurring in a given source is $1/8$, its self-information is 3 bit. The entropy of the source is the average of the self-information over all possible outcomes:

$$H(X)=-\sum_x\Pr(x)\log_2\Pr(x)$$

Thus the Shannon framework answers: **under an already-specified source distribution and partition of outcomes, how rare is this outcome, and on average how much uncertainty does the source carry?**

It does not need to go on to judge who heard the message, who considers the message useful, whether the message changed an action, or whether the action helped some subject maintain itself. The source distribution can come from historical samples, a theoretical model, or an explicitly declared protocol setting; the Shannon measure itself requires only that the distribution and the partition of outcomes be given, and does not decide for the researcher why they are chosen as they are. This suspension is not a defect but a choice of scope that Shannon theory makes in order to treat communication problems precisely.

It should be noted that for a continuous quantity, the probability of an exact value cannot be used directly as an ordinary discrete probability. An actual computation must declare the interval partition, the measurement precision, or the convention for the probability density. Whichever way is adopted, the result depends on a source and a reading protocol specified beforehand.

#### 2.2.3 FEP Surprise: How Unexpected an Observation Is Under a Generative Model

The free energy principle (FEP) concerns perception, learning, and action between a subject and its environment. For the "surprise" to be compared in this chapter, the key is how improbable an observation is under the generative model adopted by the subject.

In simplified notation, the surprise of an observation $o$ under a generative model $m$ can be written as:

$$S_m(o)=-\ln p(o\mid m)$$

The probability here is not an arbitrary historical frequency but the observation probability given by the generative model. How the subject's model represents hidden causes, how it forms predictions, and how it updates from observations all affect this probability. The variational free energy in FEP is a computable upper bound on surprise; "surprise" and "variational free energy" cannot be treated indiscriminately as the same quantity (Friston, 2010; reference 46).

So FEP surprise answers: **how unexpected is this observation in the view of this generative model?** It has the same type of negative-log-probability form as Shannon self-information, but the interpretation of the probability background is different. If one replaces the natural logarithm with a base-2 logarithm and divides the value by $\ln2$, bit can be used instead; the unit conversion does not change the meaning of the background.

FEP should not be simplified to "a subject can have only one model" or "all predictions must converge to one model." A generative model can contain multiple variables, levels, and hidden states, and can also be updated in the course of learning. This book here only compares the reference background of surprise and does not reduce FEP to a single-model convergence theory.

#### 2.2.4 RIF Rarity: How Rare in a Reading Background Formed by Persistence Constraints

RIF also adopts the mathematical form of self-information. Its difference lies not in reinventing the negative log-probability, but in **how the reading categories are formed, by what rule the background distribution is determined, and which holder the reading belongs to**.

The "who" here is not an abstract observer but a specific structure that must expend effort to read differences. This book calls the functional link that carries out selective extraction a **decoder**; when it reads by means of a boundary it maintains by itself, and pays a cost for reading, it is called a **decoder holder**. The same sound wave is a warning to a local, noise to a passing tourist, and an input awaiting fitting to an untrained translation model — the difference lies not in the sound wave but in the decoder. The four joint criteria that a decoder holder must satisfy, and how its boundary is drawn, are given in Chapter 5.

A scope boundary must therefore also be drawn: this book discusses only "what has been decoded".

> **RIF makes no ontological claim about "objects never touched by any decoder."** Such propositions lie outside what RIF can discuss. Whether a stone that has never been touched by any person, any instrument, or any indirect means is "maintaining" something or "resisting" something — this very statement is unfalsifiable: you cannot exhaustively survey a stone that is wholly undecoded; once you measure it, it has already been decoded, and what you measure is the state "after being decoded." RIF discusses only "what has been decoded".

This does not mean that the moon does not exist when no one is looking. This book says two much weaker things. First, **the statement "the moon exists" is not an assignable reading in this book**; it is common sense, an object-setting of physics; RIF begins to speak only after you have specified a reading rule. Second, **any operation of "confirming that the moon exists" is already a decoding**, and therefore falls within the scope of discussion, whereas the state before that operation does not. What lies outside the scope is not nothingness; it is simply not mine to address.

For cases with a definite holder and in which the reading is related to its persistence, RIF by default adopts the habitat background $B^{\mathrm{env}}$: the natural frequency of occurrence of each reading category, in the environment the holder inhabits and within the persistence-relevant time window. The background is determined by an external frame of reference and does not use the frequencies the holder itself "believes".

More importantly, RIF does not advocate dividing all measurable differences indiscriminately into reading categories. The partition of readings is constrained by the holder's persistence constraints: if two environmental cues elicit the same optimal response, merging them may be considered; only when the persistence gain brought by a further distinction suffices to cover the corresponding decoding cost is there reason to retain the finer distinction. Rarity is then computed for these already partitioned reading categories:

$$I_{\mathrm{struct},D}(P)=-\log_2\Pr_{B^{\mathrm{env}}}\big(r=D(P)\big)$$

This means that RIF's background is purpose-constrained, but it does not mean that the subject may specify probabilities by subjective wish. **Reading categories are constrained by the holder's persistence constraints, whereas background frequencies are determined by the actual external environment.** The difference between the model the subject has acquired internally, $B_{\mathrm{int}}$, and the external background $B^{\mathrm{env}}$ is recorded separately as decoding deviation and is not mixed into the rarity.

If there is no specific holder that meets the criteria, or the research question requires a formal reference under a public protocol, the protocol baseline $B^{\max}$ may be used, but it must be declared explicitly. $B^{\mathrm{env}}$ and $B^{\max}$ answer different questions and cannot be mixed in one numerical series for direct comparison.

Therefore RIF rarity answers: **for this holder, under this set of reading categories related to its persistence, how rare is the current reading in its actual environmental background?** The formal rules for the two backgrounds are in §12.1.1; the operational conventions for viability resolution, habitat background, and qualification and polarity are in §12.9.3–§12.9.5.

![Figure 2.1. The Same Signal, Different Holders](figures_en/release/fig_same_signal_holders.pdf)

**Figure 2.1. The Same Signal, Different Holders.** The same sound wave (identical physical input) is a warning signal to a local, background noise to a passing tourist, and an input awaiting fitting to an untrained translation model. The difference lies not in the sound wave but in the holder's background, decoding rules, and reading conditions — what RIF discusses are readings that hold relative to a specific decoder holder. Conceptual figure, no numerical values.

#### 2.2.5 The Four Questions Do Not Replace One Another

| Concept | Core question | Basis of reference | What it cannot show on its own |
| :------------- | :--------------- | :------------------- | :------------- |
| Distinguishability | Can it be told apart? | Resolution, noise, and classification rule | Cannot show rarity or importance |
| Shannon self-information | How rare in the source? | The given source probability distribution | Cannot show for whom it is useful or what consequences it has |
| FEP surprise | How unexpected under the generative model? | The subject's generative model and its observation probabilities | Cannot directly show persistence benefit or decoding cost |
| RIF rarity | For this holder, how rare in a reading background formed by persistence constraints? | Persistence-relevant reading partition and external habitat background; where necessary, a separately declared protocol baseline | Cannot show positive or negative value, or causal effect, from rarity alone |

The same observation can be computed under different conventions at the same time. They are not four substances that must exclude one another, but different measurement questions posed about the same phenomenon. Only after the reference background and the reading protocol are made explicit does a value have meaning.


### 2.3 RIF Also Distinguishes: How Rare, What Effect It Produces, and Whether the Effect Is Positive or Negative

Rarity is not value, and value is not causal effect. RIF therefore cannot report only a rarity number.

**Structural rarity** describes how rare the organizational features of a measured object $P$, once read out by a decoder, are relative to a specified background. If everyday data (such as price records) are taken as reading features, the measured object, the reading rule, and the background must be stated together; a price figure cannot be taken as independent structural information by nature. It answers "how rare is this structural reading in the background."

**Causal rarity** describes how rare the effect produced by a measured object is, relative to the effect distribution under the control condition. It answers "how rare is this effect under a control condition without this object or without this identified relation." Causal rarity requires first identifying the effect through a control design, and then computing the rarity relative to $B_0$; changes occurring at the same time cannot be directly identified as causal action. The formal two-step determination is in §13.1–§13.3.

In addition, RIF uses the persistence gain $\delta_r$ to express the direction and strength of an effect on persistence. Rarity and persistence polarity are two different dimensions:

- A reading may be very rare but have no detectable persistence effect on the holder;
- A reading may be very common but extremely important to the holder's persistence;
- A reading may be rare and have a positive effect;
- A reading may also be rare yet produce a negative effect.

Thus "rare" does not mean "useful", "useful" does not mean "has already produced an effect", and "has produced an effect" does not mean "the effect is favorable to persistence". In formal measurement, structural rarity, causal rarity, and persistence polarity are reported separately, and none may substitute for another.

### 2.4 Why News, Prices, Nutrition, and Aesthetics Can All Become Objects of Study but Cannot Automatically Count as RIF Information

Statistical objects in everyday life can enter RIF research, but the holder, the viability indicator, the reading rule, and the causal chain must be stated first. The name of a domain cannot by itself decide whether a reading constitutes RIF information.

| Everyday object | External difference to be measured first | What RIF research must further answer |
| :------------- | :---------------- | :---------------------------- |
| Stock-market news | News events and changes in price and trading volume | For which investor or institution? What observable decision did it change? Does the effect bear on that holder's resources or continued operation? |
| Policy news | Policy text, scope of effect, implementation time | Which subject is affected? How is policy content to be distinguished? Is there an identifiable causal link between the response and the viability indicator? |
| Street rumors | Content, frequency of spread, credibility, and their changes | Who reads it and acts on it? How is the rarity of the rumor's own spread to be distinguished from the actual effect it causes? |
| Nutritional value | Ingredient content, intake, and bioavailability conditions | For which specific subject, and which physiological or viability indicator, is it meaningful? Did the reading change intake or health-related outcomes? |
| Commodity pricing and value exchange | Quotes, transaction prices, exchange terms, and resource flows | A market price is a public reading and does not automatically equal anyone's subjective value; a specific holder, together with its response and effect, must be determined separately. |
| Song preference | Auditory features, ratings, and changes of preference over time | A change in preference does not by itself constitute RIF information; one must also state what difference was read and whether it has an identifiable causal link with the subject's persistence. |
| Interpersonal attraction and relationships | Behavior, interaction, commitment, and relationship state | One cannot give an amount of RIF information from "like/dislike" alone; a holder, a state update, an observable response, and a persistence association must be made explicit. |

For example, if a person finds a song pleasant yesterday and unpleasant today, this is first of all a change in preference state. If a researcher wishes to bring it into RIF, it must be further operationalized: which kind of difference in the song did the person read? What response did the change in preference lead to? Is there a detectable causal link between that response and the person's own persistence? If the last cannot be established, it should be reported honestly as a change in preference, rather than forcibly assigned an amount of RIF causal information.

Likewise, a nutrient composition table can be a public measurement result; what it means for a specific person also depends on that person's physiological state, dietary constraints, actual intake, and subsequent effects. A market price can be determined by a public protocol, but one cannot therefore treat "the whole market" as a decoder holder without testing it against the criteria.

### 2.5 What Can Be Done Now, and What Cannot Yet Be Claimed

This book has already given the mathematical form of rarity, the distinction between the two backgrounds, the necessary conditions for viability resolution, the two information channels of structure and causality, and the corresponding principles for assigning time and energy. These suffice to specify which objects and conditions a researcher must account for, and suffice for illustrative computations or local measurements in some cases with clear boundaries.

But this does not mean that all everyday information already has a ready-made unified algorithm. At least the following steps still require further operationalization: the determination of the persistence-relevant time window $W_{\mathrm{sv}}$; the optimal response in an open response space; the global optimization of the persistence-equivalence partition; the detection floor $\iota_D$ of a cognitive decoder; control reference classes for social and historical cases; and the conversion of costs such as money and time into physical energy.

Therefore this book does not take "maximizing rarity" as an established basic goal of RIF. What the present measurement layer does is to determine the reading, the background, the persistence association, and the cost, and to report rarity and effect polarity separately. Whether a subject will actively pursue more information that is positive for its persistence, how much added cost it is willing to bear for this, and when it will suffer backlash from over-pursuit are hypotheses that require a separately built dynamical model and independent testing, and cannot be inferred directly from the definition of rarity itself.

Likewise, this book does not summarize FEP as "convergence to a single model", nor does it summarize RIF as a "maximization of rarity" symmetric to FEP. The two resemble each other in the form of self-information, but the questions of how the background is constructed differ; similarity in mathematical form does not mean that the theoretical questions are the same, nor that the two are necessarily opposed ontologically.

The everyday cases given in this chapter only bring the reader to the entrance of the measurement problem. In formal computation, structural rarity follows Chapter 12, causal rarity follows Chapter 13, and decoder type and holder qualification are determined by Chapter 15. **"Information" in everyday language is the starting point of the research, not a proof that RIF measurement has been completed.**

One further scope limit must be stated: the I–T–E triplet is a measurement projection, not a complete state description of the object. Whether it maps different objects to different records is not yet determined (see item 12 of "Limitations and Open Problems" at the end of the book). This book therefore does not use the triplet as an instance identity label.

***

## Chapter 3 — Why "Cybernetics" Is Not Enough

Wiener's cybernetics did something bolder: it pulled the "future" back into the explanation of the present. Classical physics is accustomed to asking how the present determines the future. Cybernetics asks in the opposite direction: **how a system uses its expectation of the future to change the present.**

This means that something appeared inside the system that no scientific language had previously been able to describe: **goals**. Mathematically, a goal can be understood as a kind of "attracting structure" — the system keeps deviating from it, feedback keeps pulling it back, and the system finally stabilizes near this structure. Thus "purpose" for the first time acquired a non-mysterious scientific language: purpose is a kind of stable structure in a dynamical system. Wiener drew this mechanism clearly with the simplest block diagram — input, processing, output, feedback — and this is also the way of writing that this book wants to emulate: to tell the sharpest ideas in the least technical language.

But cybernetics also left a question unanswered:

> **For this "self" that can "control itself", where is the boundary?**

A system can regulate itself and maintain a steady state by feedback. But "where the feedback loop ends" is something cybernetics itself gives no answer to — it assumes that the "self" is given, just as systems theory assumes that the system boundary is given. (**Prior work**: Later work has responded to this directly: autopoiesis theory is one answer; more recently, Friston used the "Markov blanket" to give a probabilistic formulation of the "division between inside and outside". These all respond to the same question. What this book sets out to do is to bind this boundary to information–time–energy records, which none of them has done.)

One technical observation is added here; it explains why cybernetics has difficulty filling this hole by itself.

A feedback loop is a **functional** concept: as long as there exists a causal path from output back to input, and that path changes subsequent output, the loop holds. Functional things can be "seen" at any scale: there is a loop in a thermostat, there is also a loop in the person–air conditioner–window system of a room, and likewise in the urban heat-island effect of a city. You can draw a block diagram at every level, each level's block diagram holds, and they do not contradict one another. **The problem is not which loop is real, but that when you draw the loop at a given level, you have already quietly selected a boundary and then taken this boundary to be a property of the loop itself.** Cybernetics has no tool to question this smuggling, because its language has no item for "who maintains this boundary".

This is why this book takes pains to discuss "self-maintenance" at such length. Self-maintenance is not a higher-grade property than feedback; it is the property that **anchors the feedback loop**: a loop belongs to a certain structure and not to its environment because the set of boundaries that maintains the loop is maintained by that structure itself. Without this, the loop is merely a stroke drawn on by the observer.

***

## Chapter 4 — Persistent Structures

By Chapter 3, systems theory, information theory, and cybernetics have already begun to approach one another: systems theory studies state spaces; information theory studies how uncertainty in state spaces is compressed; cybernetics studies how feedback changes trajectories in state space. But there is a more fundamental question that none of the three has answered head-on:

> **For a thing that goes on existing, how should its boundary be drawn?**

This book's answer is:

> **A system is not a material boundary but a persistent relational boundary.**

What really should be observed is something more specific — the **persistent structure** (PS): **a structure that, under a specified object boundary, analysis scale, and observation window, can be identified against its background and maintains its key relational organization for a finite time.** Its realization must rest on a physical substrate and be subject to energy constraints, but RIF does not presuppose a unified viability-dynamics equation.

![Figure 4.1. Three Modes of Persistence](figures_en/release/fig_persistence_three_modes.pdf)

**Figure 4.1. Three Modes of Persistence.** A rock persists through stable material organization, a typhoon through a relational pattern continuously maintained, a social identity through a relation network continually reproduced. The typhoon is the key example: air molecules keep turning over, while the pressure field, energy flow, and rotation relations maintain its organizational pattern — what persists is the relational organization, not a fixed matter. Conceptual figure, no numerical values.

A stone exists by virtue of its lattice structure, a vortex by virtue of flow-field relations, life by virtue of metabolism and organizational relations, a state by virtue of the relations between institutions and citizens. Their material compositions are entirely different, yet they share the answer to the same question:

> **What relation is it that, after the material substrate is continually replaced, still lets us say "this is the same thing"?**

**Matter certainly matters.** Every relation must land on a concrete physical substrate in order to exist — without neurons, paper, or hard disks that really exist somewhere, there is no relation that is really continuing. What this book changes is **whether "the boundary must coincide exactly with one continuous piece of matter."**

> **The body is only the main anchor of a persistent structure; together with the causal topology that extends outward from it, it constitutes its ontologically complete realization.**

**First, "specified object boundary, analysis scale, and observation window" in the definition is not a courtesy phrase; it is three required fields.** The same thing, with a different boundary, scale, or window, can be a different PS, and can even be the difference between "is a PS" and "is not a PS". A corpse, on a minute scale, is a barrier-frozen structure; on a year scale, a structure in the course of disintegration; on a cultural scale, the starting point of a memetic carrier — all three statements are correct, but they belong to three PSs. So this book never asks "is this thing a PS"? and asks only "under a given boundary, scale, and window, can it be matched with a set of records"?

**Second, "can be identified against the background" in the definition presupposes a decoder, but does not say which one it must be.** This is not circular but layered: identification is always relative to some reading rule, and the reading rule itself can be a public protocol or the private rule of some holder. Chapter 12 treats these two cases separately, using exactly two different background notations.

**Third, "maintains for a finite time" is part of the definition, not an additional condition.** A structure maintained infinitely has no place in this book: it is unmeasurable — you cannot confirm "infinite" within a finite observation window. Any claim of eternity can be written, at the measurement layer, only as "not terminated within the observed window", that is, a right-censored lower bound.

### Two Ways of Reading Time

When we say "how long this structure has been maintained", two entirely different kinds of time are at work.

**Process time**: how long a specific operation lasts. A conversation lasts ten minutes; a heartbeat lasts a fraction of a second. This is the most commonly used concept of time in physics and engineering.

**Persistence time**: on what grounds the causal channel of a structure is still there. That Confucius's thought is "still alive" means that this relational pattern is still recognized by some decoder and is still producing causal effects.

There is no conversion between the two. Integrating process time out to infinity gives total dissipation, not a persistence criterion: the former describes how long a physical process lasts, the latter describes under what conditions a structural record or a causal effect can still be identified. The two are **non-interchangeable in both directions**.

Direction one: **stuffing process time into the record does not yield a persistence criterion.** Suppose you measure a read–write cycle of some device to be ten nanoseconds, and add up ten trillion cycles to get a total duration; this total duration does not tell you "how long this device has still existed as an identifiable structure." The latter depends on whether some decoder can still read it out from the background, and whether this reading is still above the detection floor. The total duration can be very long, while the structure may already have become unidentifiable at one-thirtieth of it.

Direction two: **stuffing persistence time into a process inequality does not give back the original inequality.** The time–precision relations in stochastic thermodynamics require an explicit two-point fluctuation structure: some current, its variance, the entropy production rate. Persistence time is an ontological condition and does not itself provide a stochastic process model. Unless you additionally specify the current, the entropy production, and the steady-state condition within the window, substituting it in merely changes the symbol.

So this book's practice is: **process time and persistence time are kept as two sets of symbols and never interchanged.** Process time is not given a symbol of its own, because this book does no process-level computation; wherever it is needed, the work that cites it brings its own symbol. Persistence time comes in two kinds: structural persistence time $T_{\mathrm{struct}}$, the span over which a structural reading can still be recognized as the same structure under a given decoder (by default referring to $D_{\mathrm{macro}}$, in which case it means "can still be identified convergently under the public measurement reference"; the measurement-layer definition is in §12.10); and causal persistence time $T_{\mathrm{causal}}$, the span over which at least one holder can still identify the target effect, produce an observable response, and pay a measurable cost for decoding. **Convention for paired readings**: when $T_{\mathrm{causal}}$ is paired with $I_{\mathrm{causal}}$, the reading of a **single holder** is taken; the group-level union ("at least one") is recorded separately as $T_{\mathrm{causal}}^{\cup}$ and **must not be mixed with a single-holder reading** — the two are not the same quantity, and mixing them would take "anyone can read it" for "someone reads it longest". The two belong to the structural channel and the causal channel respectively, and the duration of an operation is never taken directly as persistence time.

### The Four Top-Level Classes of Persistent Structure

This book fixes the top-level classification of PS as four types: **barrier-frozen, physically dissipative, actively dissipative, and externally substrate-dependent**. The first three are distinguished mainly by the structure's internal persistence mechanism; the fourth is classified by the necessary dependence of its characteristic information organization on an external carrying system. The four types are a coarse-grained classification made on the basis of the main persistence condition, and do not represent four entirely mutually exclusive physical mechanisms. In classifying, one should first make explicit the object of study, the analysis scale, and the persistence process; if a unique assignment cannot be determined, the object can be marked as mixed or undetermined.

- **Barrier-frozen type**: maintains organizational structure mainly by energy barriers or other stable constraints in the physical structure, and can under certain conditions remain in existence without continuous active regulation. Typical objects: rocks, crystals.
- **Physically dissipative type**: maintains organizational structure by continuing physical processes and energy flows; when the relevant processes stop or key conditions are no longer met, the characteristic organization may dissipate or transform. Typical objects: stars, flames, typhoons, ocean currents.
- **Actively dissipative type**: maintains its own persistence by internal regulation, metabolism, or cognitive activity, and responds to environmental change through continuing resource use and feedback mechanisms. Typical objects: plants, animals, humans. Cognitive capacity and self-maintenance complexity can be characterized continuously by the time scales of history dependence, persistence coupling, and rule plasticity; the degree of self-reference can serve as a supplementary dimension.

![Figure 4.2. The Four Top-Level Classes of Persistent Structures](figures_en/release/fig_four_top_level_classes.pdf)

**Figure 4.2. The Four Top-Level Classes of Persistent Structures.** The four cards give examples under different objects, components, scales, or object boundaries: local structures such as bones may be read as potential-barrier-frozen; basal metabolism and the sleeping body exhibit continuous physical dissipation; thinking and acting on the physical world are actively dissipative processes; impressions, mentions, and remembered social identities in other people should instead be studied as externally substrate-dependent PSs with different boundaries. These are not four realization layers of one PS and do not assign four main classes to the same PS: fix the object boundary, scale, and observation window before assigning a main class. Conceptual figure, no scoring, no numerical values.

**Proposition (Classification Granularity)**:

- Premises: given the object boundary, analysis scale, and observation window; the criteria of the four types rely only on the "main persistence condition", not on material composition.
- Result: any PS has at most one "main" assignment among these four labels; when two persistence conditions contribute comparably within the same window (for example, a corpse simultaneously governed by barrier freezing and chemical degradation), the object has no unique assignment within that window.
- Failure conditions: when the observation window is shorter than the ratio of the two mechanisms' characteristic times by up to one order of magnitude, the word "main" loses its discriminating power; in that case the object should be marked as mixed or undetermined, rather than forcibly classified.

This proposition sounds like a truism, yet its consequence is not small: it means that **classification is a by-product of measurement**. You cannot first announce "this is a rock" and then look for its readings; you can only take the reading first, and then see which mechanism dominates it in which window.

#### Externally Substrate-Dependent Type

**Definition**: An externally substrate-dependent PS is one for which, within the specified object boundary, analysis scale, and observation window, the realization, replication, or continued existence of its characteristic information organization must depend on a carrying system outside the PS boundary to provide a necessary function, and that function cannot be equivalently replaced by the PS's internal mechanisms.

External substrates include not only material storage media but also external systems that provide computational implementation, biological replication, cognitive retrieval, social transmission, or institutional maintenance. **Ordinary energy needs, metabolic dependence, niche dependence, or general environmental influence do not by themselves suffice as a criterion for this type.** The key is whether the external system bears the necessary function through which the characteristic information organization is realized, replicated, or continued.

There is a distinction here that is easy to slide past: **"depends on the external" and "depends on an external function" are not the same thing.** A tree depends on sunlight, but sunlight does not bear the realization of the tree's information organization; it is a replaceable energy input, and the tree can live on lamplight instead. A virus depends on the host's ribosomes, and the ribosome carries a function the virus cannot complete by itself — it is not energy, it is machinery. The criterion must catch the latter: whether the external system supplies **that part of the function which this machine cannot build for itself**.

The externally substrate-dependent type includes four typical kinds of object:

- **Virus type**: A virus has material carriers such as nucleic acid and viral particles. A single particle can exist temporarily outside a host, but the replication and continuation of the viral lineage depend on the host to provide the necessary molecular synthesis machinery. This type takes the replication and continuation of the lineage as its object of analysis; whether a single particle can persist outside a host must be analyzed separately according to its own mechanism.
- **Memetic-virtual type**: Depends on external cognitive subjects and the related mechanisms of transmission, consensus, or social practice for its realization and continuation. The carrying conditions include individual memory, cognitive processing, linguistic expression, transmission media, group identity, and institutional enforcement. The preservation of a symbolic record does not necessarily mean that the corresponding virtual structure is still in effect; nor does the disappearance of a single carrier necessarily mean that the structure cannot continue through other carriers.
- **Formal-mathematical type**: A mathematical formal structure that is realized and continues to function by virtue of the correct invocation, derivation, understanding, or verification by an external cognitive decoder. An external cognitive decoder is not limited to humans; only when the four joint criteria hold simultaneously does it meet this book's decoder-holder qualification. A mathematical-form PS is not equivalent to the underlying laws of the universe that it describes; mathematical structure, symbolic representation, proof record, and physical substrate should be distinguished.
- **Software type**: The characteristic information organization depends on computing hardware, storage systems, and a runtime environment for its realization. Software code, model parameters, stored state, and a software instance in a particular run should be treated separately; the stopping of a running instance does not necessarily mean that the corresponding software structure disappears. AI software is one kind of software type, not a necessary condition of this type.

#### The Relation Between Classification and Decoders

The four top-level classes describe the main persistence condition of a PS and do not directly determine whether a decoder $D$ exists, what type it belongs to, or what function it has. An externally substrate-dependent PS may rely on one or more external decoding mechanisms to realize information extraction, replication, or continuation, but that an external system provides carrying conditions does not mean that all its functions belong to the target PS's own decoder. **Decoder-holder qualification requires four conditions: it maintains an identifiable boundary by itself, extracts environmental differences selectively, undergoes a state update triggered by that extraction, and the update has causal significance for its own persistence.** External carrying dependence is not automatically equivalent to decoder dependence, nor does it determine the PS's classification.

The two classifications (the four persistence mechanisms, and having a decoder or not) must be kept apart for a direct reason: **what a thing "is maintained by" and whether "it itself can read" are two orthogonal questions.** A crystal is maintained by barriers and cannot read; a bacterium is maintained by metabolism and can read; a piece of software is maintained by someone else's hardware, it cannot read by itself, but the machine that runs it can; a formal mathematical structure is maintained by mathematicians' invocation, the structure itself does not read, but the mathematician does. Forcing one classification to express two dimensions at once would leave both unclear.

#### Analysis Boundaries, Mixed Substrates, and I–T–E Measurement

For example, animals as a whole mainly belong to the actively dissipative type, but local structures such as bones can show barrier-frozen persistence characteristics at a particular scale; after an animal dies, the original metabolic and internal regulatory processes stop, and the corpse may also present different classifications under different time windows. Similarly, a person's body and the social identity, deeds, and related ideas that continue in others' cognition can be studied separately as PSs with different boundaries. Formal mathematical structure and mathematical reasoning activity should also be distinguished: the former, once appropriately delimited, can be studied as an independent PS, whereas the latter may be only cognitive activity within an actively dissipative subject.

When conducting I–T–E measurement, one should first determine the target PS's boundary, scale, and time window, and then separately identify its information content, persistence time, and effective thermodynamic cost. The total information, persistence time, and resource cost of the external carrying system should not be counted directly into the target PS without argument. For cases of shared substrates or of several PSs operating in coordination, a cost-allocation rule must also be made explicit, to avoid double counting.

> **The same physical expenditure can enter only one item in one report.** If one electricity bill sustains both the structural readout and the causal readout, and you cannot separate it by operation-level metering or incremental cost, the correct approach is to mark "this item cannot be apportioned", rather than guess a ratio to split it between the two sides. Better to leave a gap than to manufacture, on the books, a total that looks complete but has in fact been double-counted.

***

## Chapter 5 — The Decoder: Who Is Qualified to Read

When this book says "boundary", there are two objects: (a) the boundary of the measured object $P$ — how far a country, a typhoon, or a language extends — which is drawn jointly by the reading rule and the I–T–E pairing; and (b) the boundary of the decoder holder itself — the inside/outside division that criterion ① requires and that the structure maintains by itself. The two usually do not coincide: the meteorologist's reading rule draws the boundary of the typhoon, and the typhoon itself has no boundary in sense (b). This chapter discusses (b), which is exactly what criterion ① targets; the procedure for drawing (a) is in §12.8.

This double meaning is set out first: one can think of (a) as "what we are measuring", and of (b) as "who is qualified to measure, and pays a cost for doing so." (a) can be as wide as spanning continents, or as narrow as a single atom; (b) has only one source — the structure's own maintenance process. Confusing the two immediately produces absurd conclusions: using (a) to satisfy the requirement on (b) yields "a typhoon has a boundary it maintains itself"; using (b) to meet the requirement on (a) yields "only organisms can be measured".

This chapter and the main text of the book use the following symbols. Unless otherwise noted, the four necessary conditions of this chapter determine the **holder that runs $D$**; $D$ itself is defined only as a functional link.

- **$D$: decoder.** Refers to the functional link, in the self-maintenance process of a structure, that carries out the selective extraction of information. The four necessary conditions determine the **holder that runs it**; $D$ itself is only a functional link, and $D$ alone does not constitute a holder. Signal reception, feedback, or state change alone does not suffice to constitute $D$.
- **$D=\varnothing$: no ontological decoder that meets the criteria.** Refers to an object that itself lacks a selective-extraction link satisfying the four necessary conditions. It may still have a complex physical structure and may still be measured by other decoders.
- **$D_{\mathrm{phys}}$: physical decoder.** A decoder that relies on a self-maintained physical boundary and whose selective extraction takes part in maintaining the persistence of that structure itself; by how the selection rule is fixed, it is further divided into two classes, static and dynamic.
- **$D_{\mathrm{cog}}$: characterization of the functional complexity of cognitive decoding.** A decoder holder has a position in the space spanned by three axes — history dependence, persistence coupling, and the time scale of plasticity (self-reference being a supplementary fourth axis); the region where the three axes reach the online type or above is denoted $D_{\mathrm{cog}}$, and below that region is denoted $D_{\mathrm{phys}}$. It is therefore a region of functional complexity superimposed on $D_{\mathrm{phys}}$. How to measure the three axes and how to operationalize the fourth axis are in §15.8.
- **$D_{\mathrm{macro}}$: public reading protocol.** The public part of the measurement protocols that multiple holders adopt and that can be commensurated with one another; that is, the public measurement framework that is usually adopted by default in practice but is not necessarily explicitly identified each time. It has no single holder and is the convergence point of the protocol; it is not a decoder holder and does not bear a persistence cost — the concrete readings are carried out by holders, who bear their costs.

These three levels answer three different questions: $D=\varnothing$ and $D_{\mathrm{phys}}$ answer "is there an extraction link that maintains itself"; $D_{\mathrm{cog}}$ answers "how easily can the rules of this extraction link be rewritten by itself"; $D_{\mathrm{macro}}$ answers "how do multiple subjects align with one another." Compressing the three levels into one gives arguments such as "is a stone a decoder"?, which are either obvious or unanswerable.

**Definition (the four joint criteria for a decoder holder)**:

A persistent structure is judged to be a decoder holder running $D$ only if it satisfies all of the following four conditions; $D$ is only the functional component through which that holder performs selective extraction, not the object being judged.

① **An identifiable self-maintained boundary** — the structure has a boundary that can be identified and that distinguishes inside from outside; this boundary is continually realized by the structure's own organization and maintenance processes. Criterion ① allows no "borrowing" exception: the boundary must be maintained by the structure itself.

② **Selective extraction** — the structure does not respond equally to all differences in the environment, but selectively acquires, filters, or responds to a part of them. "Extraction" here is functional filtering of differences and presupposes no consciousness, understanding, or explicit computational capacity.

③ **A selective state update triggered by extraction** — the extracted difference actually changes the structure's subsequent internal state or behavior, rather than merely being received without causing a corresponding state update. What is required is a change triggered by selective extraction.

④ **Causal significance of the state update for its own persistence** — the above state update causally affects the structure's ability to maintain or continue its own boundary and organization, and is not merely a general physical change occurring to the structure. This condition does not require the structure to have subjective intent or an explicit goal of survival, but it does require that its state update actually take part in the causal process of its own persistence.

None of the four conditions can be dropped; together they constitute RIF's standard for judging whether a persistent structure qualifies as a decoder holder running $D$, rather than an evaluation of how complex a structure is. This does not confer holder status on the functional component $D$ itself.

![Figure 5.1. The Four Joint Criteria of a Decoder Holder](figures_en/release/fig_decoder_four_criteria.pdf)

**Figure 5.1. The Four Joint Criteria of a Decoder Holder.** ① an identifiable self-maintained boundary; ② selective extraction; ③ a selective state update triggered by the extraction; ④ the update's causal significance for its own persistence. Together, the four conditions determine whether a persistent structure qualifies as a holder running $D$; $D$ is only the functional component, not the object judged by the four conditions. Conceptual figure, no numerical values.

Whether collectives (families, firms, organizations) can satisfy criterion ① is not argued in this book — the criteria themselves are still applied to concrete instances one by one according to Chapter 15; until then, research on everyday information takes the individual person as the holder (see item 11 of "Limitations and Open Problems" at the end of the book).

Take rock weathering as an example: weathering does change the state of a rock, but one cannot therefore regard the rock as satisfying ③. A change of state caused by external physicochemical action is not equivalent to a state update triggered by selective extraction. Although a rock has an identifiable physical boundary, it has no self-maintained boundary continually realized by its own maintenance process, and it has not formed an extraction–update chain satisfying ② and ③. Therefore, by RIF's definition, a rock falls under $D=\varnothing$ — this does not mean that a rock has no physical structure, no surface boundary, or is not governed by physical law; it means only that it lacks an ontological decoder that meets the four conditions.

"None of the four can be dropped" is the hardest statement in this chapter, and also the most misused.

The four are in fact four segments of one chain: **boundary** gives "whose"; **extraction** gives "read what"; **update** gives "different after reading"; **persistence significance** gives "and what use is the difference". If the chain breaks at any segment, the remaining parts are still there, but the persistent structure no longer qualifies as a decoder holder running $D$. **Boundary and extraction without update** is a mirror — it reflects, but is not itself changed by reflecting. **Extraction and update without persistence significance** is a sensitive sensor — it records, but the record takes no part in its own persistence. **Update and persistence significance without a boundary** is a catalytic cycle scattered through the environment — it has effects, but there is no "inside and outside" to speak of.

These three kinds of counterexample have in common that each looks like a decoder at some local level. This is exactly why the criteria must be conjunctive and not disjunctive. **If any one of the four could be waived, almost any physical system with feedback could be counted as a decoder holder, and the classification would lose its discriminating power.**

The discussion of the evolutionary path and the design path below aims to show how the above criteria are instantiated in concrete systems. The four conditions constitute RIF's defining criteria, and the specific scientific material serves to show possible ways of realization; one cannot, merely from the existence of an instance, regard the criteria as having already obtained universal empirical verification.

### 5.1 Formation Pathways of D

> **Layering statement**: The micro-level material cited in this section — membranes, RNA, receptors, chemotaxis — is used to show how the macroscopic relational structure proposed by RIF is realized at concrete scales, supplying empirical support and a sense of the picture. **The order of definition is relational structure first, mechanism instances after**: RIF first proposes a cross-scale relational structure, and the specific molecular, cellular, and ecological mechanisms then show how this relation is realized at a given scale; this material does not constitute the inductive source of the definition of $D$.

In non-living physical systems, there is no functional boundary between an entity and its environment. Take a rock: its changes of form are entirely governed by external physicochemical laws, and there is no selective exchange of matter and energy aimed at its own persistence. Within the RIF framework, the decoder set of such a system is the empty set, because it lacks the boundary required to open a persistence record.

The appearance of self-replication is not yet enough to mark the birth of a self-maintaining system. The replication of a bare RNA strand in a primordial soup belongs, at the thermodynamic and kinetic levels, to the same class of physical self-organization phenomena as the growth of a mineral crystal. Neither has established an autonomy centered on boundary maintenance — replication is merely the continuation of structure under the action of physical law, not an active process serving some internal goal.

Here the empirical facts and RIF's interpretation must be stated separately. **Prior work**: Fatty-acid vesicles can form spontaneously, divide spontaneously, and show some selective exchange of substances across the membrane; this is a phenomenon observed in existing experiments and does not depend on RIF holding. **Inference:** Measured against the four criteria, such vesicles — if they indeed have an identifiable boundary, selective extraction, a state change, and that change affects their own persistence — would be a candidate instance of $D_{\mathrm{phys}}$. But "whether it is the initial starting point of D on the evolutionary path" is an open empirical question: existing observations are not enough to rule out earlier, simpler candidates, nor to rule out that this path is only one of many possible ones. This book makes no empirical ruling and only states which class such a structure would fall into by the criteria, if it holds.

The earliest primitive membrane was functionally homogeneous — non-specific exchange of matter could take place everywhere, with limited efficiency. When changes in environmental conditions made homogeneous exchange unable to sustain the system's persistence, functional differentiation pressure appeared on the membrane, and specialized molecular structures began to take on specific recognition and response functions: recognizing only one class of molecules, regulating the opening and closing of only one class of channels. This specialized structure constitutes the prototype of an early decoder; once its recognition rules and response thresholds were fixed by natural selection, it became a stable functional component within the system. The cell in the modern sense is a form that appeared only after this chain of division of labor had fully developed, and is not an initial condition of D — taking the mature cell as the starting point of D would invert the logic by explaining the origin with the result.

Whether the signal is transmitted as light, acoustic vibration, or direct molecular collision, the moment at which the act of recognition finally takes place falls on an electrochemical event at the molecular level: photons induce conformational changes in photosensitive molecules, acoustic vibration opens mechanically gated channels, odor molecules bind to receptors. The transmission paths differ, but the step of translation into a signal readable by the system follows the same physical mechanism. Bacterial chemotaxis provides a classic example: methylated receptor proteins on the membrane sense the sugar concentration gradient and adjust the direction of flagellar rotation accordingly. Its information-theoretic significance is that the bacterium has obtained an estimator of very low precision — this mapping requires no understanding and no computation, only a simple input–output correspondence, to produce persistence decisions that are statistically better than a random walk.

Once the decoder operates stably, it forms circular causality with the system as a whole: the functional output of the decoder maintains the system's physical persistence; the system's persistence state determines whether the decoder can be retained and replicated. The two are necessary conditions for each other and cannot be reduced to one-way linear causality. This structure may be called the **persistence-record loop**. This loop is a dynamical property of D after D exists and is not part of the definition of D.

"Persistence-record loop" does not mean that the decoder and the system are each other's cause and that the system is a self-sufficient closed-loop self. What it refers to is much weaker: **in a system satisfying the four criteria, there is two-way dependence between the decoding link and the system's persistence, and so the decoding link cannot be analyzed as an add-on device outside the system.** This two-way dependence does not guarantee that the system is stable, nor that it persists longer — it guarantees only one thing: you cannot replace its decoding link alone without changing the system's persistence conditions and pretend that the rest is unchanged.

The above describes how a system that already has the simplest boundary and the ability to maintain itself differentiates further, from within, into finer decoding components. The earlier question — the mechanism of the transition from non-living matter to the first self-maintaining system with a boundary — is still an unresolved problem in geochemistry and biochemistry; representative research directions include the alkaline hydrothermal vent hypothesis (Martin & Russell, 2003), the RNA world hypothesis (Gilbert, 1986), and the mineral-surface catalysis hypothesis (Wächtershäuser, 1988). RIF, as a meta-theoretical framework, makes no empirical ruling on the specific path of origin and attends only to the information-ontological logic that the system follows once formed.

Besides the evolutionary path, decoding components can also arise through a **design path**: another already-existing self-maintaining system manufactures them from outside and implants them in a particular substrate. Thermostats, brain–computer interfaces, and pure-software AI all belong to this kind. The structural difference between the two paths is that in the evolutionary path D arises from within the closed loop through differentiation over time, going through a "differentiation–fixation–stabilization" process; in the design path D is assembled and implanted all at once by the maker and is set as soon as manufacture is complete, without an internal history. The dynamical link shared by the two paths: once D is put into operation, it enters circular causality with the persistence record.

A point easy to confuse here: for a decoding component produced by the design path, its **attribution under the criteria** does not change because "it is man-made". The criteria look only at the four conditions, not at provenance. A thermostat does not count as $D_{\mathrm{phys}}$ not because it is man-made but because what it maintains is not its own boundary. An artificial system with its own closed loop counts because it satisfies the four conditions. **Provenance affects history, not qualification.**

***

### 5.2 Classification of D

This section discusses "once D has formed, what types it can be further divided into", on the premise of the criteria in the previous section — D is not any physical feedback, threshold, or complex structure itself, but **the functional link in a self-maintaining closed loop that is responsible for selective extraction**: whether a structure has D depends on whether its selective extraction is a part of how the structure's own set of boundaries continues.

#### $D=\varnothing$: Purely Physical Structures Without a Self-Maintained Boundary

Stones, crystals, stars, and ongoing phase transitions can all exhibit complex physical behavior: crystals have strict lattice structure, stars have a precise fusion balance, the phase transition of water has a definite threshold. But behind these behaviors there is no "self" being guarded. A stone weathers not because it is "resisting" something; when water freezes, the freezing point is not a comparison standard that can be separated from the physical laws of water itself and adjusted independently, but just the intrinsic property of hydrogen-bond strength itself. Such structures are denoted $D=\varnothing$: there is no selective-extraction process that is independent of the object's own physical laws and serves the persistence of the structure.

I deliberately chose the symbol not as "zero" but as "empty set". Zero is a value; the empty set is a collection: **$D=\varnothing$ does not mean "decoding ability is zero" but "under this book's criteria, there is no qualifying element in this object."** This distinction has practical consequences: an object with $D=\varnothing$ can still be measured very finely and can still have a very high $I_{\mathrm{struct}}$; it is only that it does not itself read. That it does not read does not prevent others from reading it.

#### $D_{\mathrm{phys}}$: Selective Extraction with a Self-Maintained Boundary

For a structure to enter $D_{\mathrm{phys}}$, it is required to have a layer — even the crudest — of self-maintained boundary, and its selective extraction of environmental differences must serve the persistence of the structure behind that boundary, and not something else outside the boundary.

The simplest fatty-acid vesicle can form spontaneously, grow by itself, and divide in two by itself; once it begins to show selectivity in the exchange of substances across the membrane — some molecules preferentially taken in, some excluded — this selectivity is already the rudiment of $D_{\mathrm{phys}}$; it needs no nervous system and no complex cognitive capacity.

**Why a thermostat does not count as $D_{\mathrm{phys}}$**: A thermostat detects temperature and switches between heating and cooling states on crossing a set value, which on the surface resembles a receptor that recognizes a sugar concentration gradient. But the two differ fundamentally: what a thermostat maintains is not itself but the comfort of the people in the room — it has no boundary of its own to guard; it is a tool that the self-maintaining closed loop that is the human uses to serve its own needs. **Having feedback, thresholds, and state switching does not suffice for a structure to enter $D_{\mathrm{phys}}$ automatically; the key remains whether this selective extraction is maintaining the extractor's own set of boundaries.**

$D_{\mathrm{phys}}$ can be further divided internally into two layers: **static** (the selection rule is essentially fixed over long historical processes, such as ion channels and the tardigrade's dormancy switch) and **dynamic** (the structure has real-time rule response or feedback internally, such as bacterial chemotaxis and plant phototropism). This distinction describes only how a rule is fixed or updated; a concrete measurement must still declare the background model separately and cannot infer an amount of information from the classification alone.

#### The Decoding-Complexity Space and the $D_{\mathrm{cog}}$ Region

If yes/no questions such as "is there history dependence" and "is there plasticity" are used to decide whether a structure has cognitive decoding, it is easy to reach mutually contradictory conclusions on structurally similar cases — the adaptive regulation of bacterial receptors and the habituation response of the mimosa are in essence the same kind of phenomenon (biochemical, slowly decaying short-range memory); if one is judged in and the other excluded, the criterion itself is at fault.

A more defensible approach is to replace "whether $D_{\mathrm{cog}}$ is present" with three continuous scales; any concrete structure has a position on these three axes, and an either/or determination is not forced.

**Degree of history dependence**: how much of the current internal state is determined by past experience, rather than being uniquely determined entirely by the current input.

**Degree of persistence coupling**: how tightly this history dependence is bound to how well this structure "lives", that is, how direct and how significant its effect on its own persistence record is.

**Definition (time scale of plasticity / state update)**: this is the most critical axis, but two things must first be distinguished: how often the **rule itself** is rewritten, and how often the **state under the rule's governance** is updated. Bacterial chemotaxis happens to straddle these two scales: the **state update** of sensing the gradient and adjusting flagellar direction is completed within seconds to minutes; the **rule** that drives it (which receptor recognizes which gradient, where the threshold is set) is a program hard-wired on the evolutionary scale of the species. What really decides whether a structure falls in the embodied type or the online type is the time scale at the level of "the rule itself" — by this standard, the rule layers of both bacteria and the mimosa are hard-wired on the evolutionary scale, and they remain the embodied type; but this does not mean that everything about them is "slow", only that the rule is slow and the execution is fast. Animals such as crows and octopuses, which have episodic memory and associative learning, are different: even the rule itself can be rewritten within an individual lifetime by experience.

Taken together, the three axes allow us to roughly mark out three regions whose boundaries are blurry to begin with:

- **Embodied-type region**: all three axis values are low, especially with the "time scale at which plasticity occurs" leaning toward the cross-generational end. Bacterial adaptive regulation, mimosa habituation, and plant tropisms all fall in this region: it lies within the decoding-complexity space but below the $D_{\mathrm{cog}}$ region, and is denoted $D_{\mathrm{phys}}$.
- **Online-type region**: the three axis values are clearly raised, and the "time scale at which plasticity occurs" begins to lean toward the individual-lifetime end. Crows, octopuses, and most mammals fall in this region.
- **Symbolic-type region**: all three axes are near high values, and capacities for symbolic operation such as offline inference, counterfactual processing, and language, mathematics, and institutions appear. Humans and some AIs fall in this region.

How to measure the three axes and how to calibrate the region boundaries is left to later work (for the measurement method, see §15.8). Until then, the region boundary of "online type and above" is a classification convention and makes no empirical assertion.

$D_{\mathrm{cog}}$ also has a **fourth axis: degree of self-reference** — whether this structure's decoding capacity also takes itself as an object of decoding, and to what extent this self-assessment in turn affects its subsequent behavior. The operationalization of the fourth axis is in §15.8.

The boundaries of the three axes have not yet been calibrated, but continuous characterization can still support stable judgments of order: on the item "time scale of rule plasticity", the crow stably falls on the other side of the bacterium, nearer the "individual lifetime" end — under non-pathological thresholds, the order is unchanged. **Before thresholds are calibrated, only order comparisons across orders of magnitude are allowed, and threshold determinations across orders of magnitude are not.**

#### Externally Substrate-Dependent PS and Decoder-Holder Qualification

The characteristic information organization of externally substrate-dependent PSs such as viral lineages, memes, formal mathematical structures, and software must have necessary functions supplied by a carrying system outside the boundary. This book sets up no separate decoder class for them: **decoder-holder qualification is in every case judged independently by the four criteria within the specified boundary, scale, and observation window; the self-maintained boundary of criterion ① must be continually realized by the structure's own organization and maintenance processes, with no "borrowing" exception.**

- If the structure itself does not satisfy the four criteria (for example, a viral particle that cannot carry out any selective extraction without a host machine, or software that runs on others' hardware and has no physical interface or self-maintaining closed loop of its own), in this book it serves only as the object being read, $P$. Its information content belongs to $P$, and the decoding cost required for reading is borne by the holder that actually carries out the reading.
- If the same object, under some boundary and time window, has formed a self-maintaining closed loop satisfying the four criteria (for example, an artificial system with its own physical interface and resource-acquisition capacity), it is recorded as $D_{\mathrm{phys}}$; where its position on the three axes reaches the online type or above, it is also recorded as $D_{\mathrm{cog}}$.
- "Whether it uses someone else's power or hardware" does not by itself constitute a criterion; external carrying dependence is also not automatically equivalent to decoder dependence.

#### $D_{\mathrm{macro}}$: The Macro Reading Protocol

$D_{\mathrm{macro}}$ is the common part of the set of measurement protocols that multiple subjects can share and converge on in practice. It has no single holder and is the point of protocol convergence; it is not a decoder holder, does not satisfy the four criteria, and does not bear a persistence cost. It has two layers:

- **Narrow $D_{\mathrm{macro}}$**: directly adopts classical physical measurement rules (the SI, the isolated system, the approximation of no measurement disturbance), and covers the measurement of structural information, structural persistence time, and structural energy. These quantities are all measurable in classical physics, and with the same measurement protocol and environment fixed, they can already be used for cross-subject comparison of structural readings.
- **Broad $D_{\mathrm{macro}}$**: a natural extension of classical physical measurement logic, attempting to cover the measurement of causal information, causal persistence time, and causal energy. These quantities all ultimately show up as physical effects, so there is in theory a possibility of measurement, but there is currently no unified operational protocol, and cross-subject comparison of causal readings is therefore treated as "undefined".

Where the main text does not specifically note a reference decoder, readings are by default relative to the narrow $D_{\mathrm{macro}}$. When the broad one is used, it must be declared explicitly.

There are three kinds of protocol change, which must be told apart because they often occur together in phenomena: one protocol reform often involves both more people adopting it (convergence) and the old school refusing it (divergence), and may also bring new measurable dimensions (topological transition).

- **Convergence (expansion)**: more subjects adopt the same protocol, and the scope of $D_{\mathrm{macro}}$ expands. This is not a topological transition.
- **Divergence (splitting)**: incompatible branches appear in the protocol, and multiple local $D_{\mathrm{macro}}$ appear. This is not a topological transition.
- **Opening a new causal dimension**: the old protocol in principle cannot express it, while the new protocol can express it and yields predictions that can be indirectly falsified. This alone is a **topological transition**.

This book records only the third as a topological transition, for the reason that **convergence and divergence change "how many people use the same ruler", whereas a topological transition changes "whether this ruler can measure what it could not measure before."** The first two can be described with the same set of symbols; the last cannot — it requires the appearance of a new type of reading. The three topological transitions that have occurred in history (instrumentation, probabilization, indirect inference) can serve as examples.

**Relation to the system of natural-science knowledge.** The system of natural-science knowledge (theories, equations, models, measurement methods, empirical content) is itself an externally substrate-dependent persistent structure, containing two kinds of components, the formal-mathematical type and the memetic-virtual type: mathematical forms persist by "invocation without error", and empirical content persists by "consensus that does not die out". The scientific community is another independent persistent structure and has no structural binding to the knowledge system; when a lower-cost intermediary of knowledge production appears, the knowledge system can, to a certain extent, continue to evolve apart from the community.

#### An Open Gap in Empirical Coverage

The candidates we can currently think of that truly meet the $D_{\mathrm{phys}}$/$D_{\mathrm{cog}}$ criteria — from primitive cell-like vesicles to bacteria, plants, and animals, and the systems built by humans that have their own self-maintaining closed loops (if any exist) — are almost all life itself, or direct derivatives of life. Between this and the initial commitment, which this book repeatedly stresses, that "D does not depend on the material substrate and does not presuppose a biological/non-biological dichotomy", there is a tension that needs to be made clear: the criteria themselves do not use "is it life" as a threshold, but the candidates observed so far fall almost entirely within the range of life and its derivatives. This may be only because Earth happened to evolve only this one path; or there may exist a candidate of non-living origin that truly satisfies the self-maintaining closed-loop criteria and has not yet been observed. This is an empirical fact, not a definition imposed by theory.

This gap touches a methodological problem: **when all known instances of a criterion fall within the same subset, we cannot tell whether the criterion is doing the work or the subset label is.** There are three possibilities: the criterion really characterizes a natural kind wider than "life", and other instances simply have not been found; the criterion happens to characterize exactly the class "life", only using a vocabulary that does not rely on biological terms; or the criterion is too loose or too tight and is inaccurate in both directions. These three possibilities must be distinguished with new candidate instances, and the precondition for distinguishing is that the criterion can be judged independently: **write the criterion in an independently judgeable form, and use it to judge when new candidates appear, rather than first judging by the life label and then fitting the criterion on afterwards.**

***

## Chapter 6 — Information, Time, Energy: Three Faces of One Thing

If a persistent structure is not defined by a material boundary, then what is it defined by?

> **By its own record.**

This record has three dimensions. **Information**: how many differences it can be identified as having, relative to a specific decoder. **Time**: how long this identification, and the causal action it triggers, can last. **Energy**: how much physical cost it takes to maintain this identification and causal action.

These three dimensions are not three variables that happen to have been put together. They are **three aspects of one and the same record** — you cannot report only "how much information this thing has" without asking how long it can be maintained and at what cost, just as you cannot report only what a company "is worth" without asking what it earns from, for how long, and at what cost.

> **I, T, and E are not three quantities that can take values independently, but projections of one and the same measurement relation in three directions; if one is reported alone without accounting for the other two, the value is not comparable.**

This sentence is firmer than "three aspects", and also clearer than it. The practical consequence is that every $I$ given later in this book is not permitted to be isolated; it must carry three annotations: "in which window, by which decoder, at what energy cost it was read." An $I$ without the annotations is not wrong but incomparable — as if you told me "this box weighs fifty" without saying fifty grams or fifty kilograms.

The information dimension involves two different things.

**First: when judging authenticity**, for instance whether a painting is an original or a forgery, one first looks at whether the decoder can tell them apart. If no decoder can tell them apart, then within the information decoded by this decoder, the two are treated as different instances of one thing.

**Second: when recording information for a persistent structure**, structural information and causal information must be recorded separately. The state of a structure's physical substrate is structural information; the causal action it produces in the world is causal information. Neither can be omitted, and together they make up the complete information of that persistent structure.

These two things are often conflated because both speak of "telling apart". The difference is: **the first asks "are these two things the same in this decoder's eyes", whereas the second asks "this thing has two different kinds of record to be kept separately."** The former is an identification relation $\sim_D$, and its conclusion can be "the same"; the latter is a table with six cells, and its conclusion is always "two kinds".

***

## Chapter 7 — Two Kinds of Information: Structural and Causal

A persistent structure in fact has **two classes of information** to be recorded separately. **Structural information**: what this thing itself is, how long it can be maintained, how much energy it takes. **Causal information**: what this thing has caused in the world, how long this action can last, and how much energy was spent to maintain it.

These two classes of information are not the same thing. A physical structure can be very large and complex — say, a pile of files archived for many years and never opened — but if it has produced no lasting causal action in the world, its causal information is empty. Conversely, a sentence, a signature, a formula, whose physical substrate is negligibly small, may produce a huge and lasting causal action in the world.

Here is one sentence this book wants to leave with the reader:

> **To know is not to obtain.**

An organization can "know" of an impending crisis without changing the flow of a single cent of resources because of it. A resolution can pass unanimously in a meeting room and yet be carried out by no one outside it. A report can be "seen" by everyone and yet not change a single real decision.

**In relative information theory, "knowing without triggering any subsequent change" is, at the ontological level, equivalent to "not having obtained."** For a difference to truly enter a persistent structure's causal information, it must first be identified by some decoder and then actually trigger a change in subsequent state — missing either step, the difference stays in the state of "could have been information but did not actually become information."

**Definition**: **This is RIF's working definition of "effective causal information", and it must be clearly distinguished from Shannon information** (**Prior work**). Shannon information quantifies the reduction of uncertainty — any symbol that lowers the receiver's uncertainty counts toward the amount of information, without requiring that it go on to trigger any behavior or state change. RIF adds an extra threshold of "causing subsequent change", because this book is concerned with the **causal significance** of information for a persistent structure, not with uncertainty reduction itself. The two definitions serve different questions and are not a revision or negation of Shannon information.

In terminology, this book does not use the bare phrase "effective information", because it is too easily read as a value judgment such as "useful information". This book uses two longer names: **effective causal information**, which refers to causal information that has passed the two gates of "being identified" and "triggering subsequent change", that is, a qualifying reading of $I_{\mathrm{causal},D}(P)$; and **net effective causal information** $I_{\mathrm{net}}$, the name that the composite quantity should bear if a later model is to combine the two channels into an index. **This book does not define $I_{\mathrm{net}}$**: the sister framework (SRVD, Volume I §1.2.1, Volume IV §2.1) gives, as a **declared modeling convention**, a weighted sum of the two channels, and at the same time declares that this is not a proof of additivity; this book does not endorse the use of that value across backgrounds, and wherever $I_{\mathrm{net}}$ appears, it refers to "that composite quantity in another model."

***

## Chapter 8 — Where the Boundary of a Person Lies: One Case Told End to End

Abstract talk, carried this far, easily turns into slogans. This chapter does one thing only: it tells one concrete case through, from beginning to end.

Imagine an official who has been removed from office because of an investigation.

**First, structural information.** His body is intact — heartbeat, breathing, muscles, nerves, all as before. From a purely physiological standpoint, he is still the same person, without the slightest damage. Looking at this record alone, nothing has happened.

**Then, causal information.** Before the removal, when he signed, documents moved down the line; when he made a phone call, some department adjusted its arrangements; a word from him could change the flow of a budget. These are all entries of his persistent structure in causal information — accomplished by the position he occupied in the network of the institution, unrelated to muscular strength.

At the moment the removal took place, there was no change in his body, but the vast majority of the entries in causal information were all zeroed out within almost the same day: no one carried out what he signed; no one responded to the calls he made; what he said could no longer change any budget.

At this point a common but **inaccurate** saying appears: "His situation has worsened, but it is only that the environment is bad; he is still the same person."

RIF gives a different diagnosis: his body is intact, but his causal information in others' hands has been cut on a large scale. This book calls this situation **social causal truncation** — name, occupation, status, assets, and files are others' decoders' identification of and response to him, and make up the main body of his causal information. It differs from bodily injury: what is damaged is this person's causal information in others' hands, not the structural information inside the skin.

**Hypothesis (Supply Coupling)**: Structural information is not self-sufficient. Most of the energy needed to maintain the body is obtained through the causal channel: only when others recognize and carry out your identity, contracts, accounts, and position do food, medical care, and shelter flow in. If the channel is cut, the body is not damaged immediately, but the energy source narrows and the structural persistence time shortens accordingly. Frozen assets are a typical example: the numbers in the account (structural information) are still there, but no one carries them out any longer, and the energy flow no longer enters; the loss of a digital record, by contrast, is the loss of the channel's substrate, which directly rewrites others' ability to recognize this person.

"Supply coupling" refers to a stronger, separable mechanism claim: **part of the energy input of the structural channel must be exchanged through the causal channel, so an interruption of the causal channel will leave a measurable lagged damage on the structural channel.** This claim has three separately testable links: the exchange rate (the mapping from the strength of the causal channel to the energy inflow), the lag (the time delay from the cut to the decline of the structural indicator), and non-substitutability (whether the same energy can be made up from non-social channels), corresponding respectively to $H\mathrm{R}\text{-}1$ through $H\mathrm{R}\text{-}3$.

**Complete realization.** A person's complete realization as a persistent structure includes both the body and the response channels of others to his identity, rights, and commitments. This is a structural convention, not a value judgment: a person whose channels have been cut is, morally and legally, still a complete person. Retaining only the physiological structure (as in imprisonment or unemployment) is "incomplete realization", not "incomplete personhood".

The two names Einstein and Confucius require making clear what "zeroing out" actually is: as the specific configuration "this living body that is metabolizing and can act autonomously", the corresponding self-maintaining closed loop has terminated, and this is the meaning of structural information going to zero. This does not mean that the matter that made up the body vanishes out of nothing, only that it is dispersed and takes part in other structures. Relativity is still written in textbooks and is still counted in satellite navigation systems, and the Confucian ethical framework still influences hundreds of millions of people — these continuing causal actions are still recorded in their respective causal information.

**A large language model** can face hundreds of millions of users at once, yet cannot completely retain all of the information of every person, and must compress, and any compression means a trade-off between "retain" and "delete". A question thus surfaces that is more fundamental than "is this algorithm accurate":

> **In this machine's record, are we recorded as key information worth retaining, or as redundancy that can be casually deleted?**

In this book's framework this question can be written more precisely: it asks **relative to whose background the model's reading of a person, $r=D(P)$, counts as rare**. If the background is taken as the natural frequency of the training corpus, $B^{\mathrm{env}}$, "rare" equals "seldom seen in the training data", and the rare are treated as anomalies or noise; if the background is taken as the equiprobable baseline specified by the protocol, $B^{\max}$, "rare" only means "unusual relative to the uniform distribution" and has nothing to do with whether something is retained. This book does not rule on which should be adopted, and notes only: **when discussing "who is treated as redundancy", one must first make clear which background is used.**

### A Person's Complete PS: Across Four Classes of Substrate

The body is the main anchor of a persistent structure, but does not exhaust its causal topology. For a person, the complete PS can span four classes of substrate. The same PS can present different main persistence mechanisms in different states of activity (here a person is examined as a whole; if analyzed separately by different boundaries, each part is classified by its own main persistence condition).

| Level | Substrate type | When it is this type | What maintains it | Which class of information is mainly counted |
| :--- | :------------- | :------------------ | :----------- | :----------- |
| 1 | **Barrier-frozen type** | When the body is static — bones, tissue structure | Barrier locking, no continuing dissipation | Structural information |
| 2 | **Physically dissipative type** | When the body is actively maintaining itself — basal metabolism, the body during sleep | Continuing physical dissipation | Structural information |
| 3 | **Actively dissipative type** | When thinking and acting on the physical world — cognition plus metabolism | Metabolism plus cognition | Structural information and causal information |
| 4 | **Externally substrate-dependent type (memetic-virtual type)** | When acting on other cognitive phases — leaving an impression in others' minds, being talked about, being remembered | Maintained by consensus | Causal information |

These four levels are not parallel; they are different sides of the same PS in different states of activity, **and can be active at the same time**. For a living person thinking: the bones are still Level 1, basal metabolism is still Level 2, cognitive activity is Level 3, and the influence on others is Level 4. (This is the result of slicing one person by level; for any single level, once the boundary and observation window are given, there is still at most one main assignment according to the classification proposition of §4.)

This layering precisely explains the case at the opening of this chapter: when the official was removed, Level 1 was intact, Level 2 was intact, Level 3 was weakened, and Level 4 was cut on a large scale. So what really happened is that **this PS's Level 4 was cut on a large scale.** Level 4 belongs to this person's complete realization because his structure draws its energy from it; this is a dependence relation, and does not conflict with the attribution rule that "causal information belongs to $P$ and the decoding cost is borne by the holder."

This table **cannot** be used to rank different people. A person with all four levels active and a person with only Level 4 remaining are two configurations on the table, not two scores; "more levels" does not mean "higher value", and "Level 4 active" does not mean "has compensated for Level 1". Any reading of this table as a scorecard goes beyond the scope of this book.

***

## Chapter 9 — Drift of Type

After a person dies, has he "disappeared completely"? The answer depends on whether any decoder can still recognize the set of "types" that is specific to him. A **"type"** is a relatively stable pattern that a decoder can repeatedly recognize (such as words and deeds, style, and intellectual content); an **"instance"** is one concrete realization of that pattern. This pair of concepts is close to the type/token distinction, but RIF must further distinguish three levels: the identification relation, structural continuity, and type/token.

While he was alive, his family remembered his words and deeds, temper, and accent; at that time his identifiable topological relations were still there, and he had not disappeared completely from the physical world. When even those who knew him are gone, and only descendants generations removed remember him indirectly through photographs or hearsay, what remains is only his "derivative copy" — another system that partly overlaps with him but is already continually mutating, and is no longer he himself.

That the causal information of Einstein and Confucius is still active means that the **concrete rule content itself** they left behind is still being directly cited, taught, and carried out, and the decoder faces this set of rules without needing to go through retelling. A "derivative copy" refers to the case where the decoders that had direct contact with the person are all gone and only multi-hand retelling remains, so that the decoder faces a mutated copy. For the same person, the fates of these two channels can be entirely different: as "the person remembered in person by relatives and friends", Confucius has long been left only with derivative copies; as "the ethical rules in the *Analects* that are directly cited", this part still circulates as it was.

Regarding the distinction between "type" and "instance", there is a trap that is easy to fall into: it cannot be equated with "form versus content". In analytic aesthetics, Nelson Goodman explicitly warned, in *The Status of Style*, that whether an author chooses to write about a "social issue" or a "battle scene" is already itself part of style. So "type" is not literal form, nor is "instance" literal content — the boundary between the two is **overall identifiability** (that is, the degree of distinguishability in the sense of the identification relation $\sim_D$ below).

Here is an important corollary: **to judge whether two things are the same, first see whether the decoder can separate them.** Take an original and a forgery. With a different decoder or measurement protocol, a difference might be found; but shown to an ordinary person with no training, he cannot tell them apart. In this person's decoder, the two paintings are treated as the same thing. RIF does not discuss here "whether they actually differ in themselves once one leaves this decoder", and asks only: for this decoder, can they be told apart; if they cannot, then for this decoder they are different instances of the same PS.

**Three things that are easily mixed together are viewed on three levels.**

- **RIF identification level**: $u \sim_D v$ ($u$ and $v$ are any two objects being compared, not limited to PSs), meaning that $u$ and $v$ fall in the same identification class of the same decoder $D$ ($\sim_D$ is an identification relation determined by measurement tolerance, not a strict equivalence relation). It is a relation that holds **relative to the decoder** and does not concern whether $u$ and $v$ are really the same in structure themselves.
- **Structural continuity level**: whether $u$ and $v$ are still the same persistent structure requires tracking their respective causal topologies and persistence paths, to judge whether they share the same structural continuity. The decoder's indistinguishability relation by itself cannot answer this question.
- **Type-token level**: one template can have multiple concrete instances. $u \sim_D v$ says "this decoder places $u$ and $v$ as different tokens of the same type", not an assertion that $u$ and $v$ are the same token, still less an assertion that they share one physical continuity.

The order of these three levels cannot be reversed. The error common in practice is: first use $\sim_D$ to judge "alike", then use "alike" to infer "the same one", and finally use "the same one" to infer "should be treated equally". Of the three steps, only the first is this book's conclusion. $\sim_D$ is a relation **about readings**, not a relation **about existence**; it can support "indistinguishable under this measurement protocol", and cannot support "ontologically the same thing". This line must be drawn firmly, because it directly decides causal attribution: whether an effect belongs to some $P$ cannot be decided by "some decoder cannot tell it from another $P$."

**Definition**: Attribution of an effect is not an empty phrase (it is a different matter from the identification relation $\sim_D$ above, so it is called an "attribution condition", not "identifiability"). At least one of the following four must hold for there to be attribution:

- **Direct causal chain**: along the path that produces this effect, one can trace back to a concrete decision or action made by this person, with no other decision node independent of him inserted in between;
- **Traceable chain**: even if the path is long and has many links, there still exists a causal chain that can be concretely reconstructed and checked, connecting the effect to this person's action, rather than relying on an "overall impression" or "cultural credit-taking";
- **Encoding contribution**: this person made an identifiable, non-substitutable contribution to the way the final effect is realized (design, algorithm, rule, protocol) — replace him, and this concrete way of realization would not be what it is now;
- **Institutional position**: this person occupies a formally authorized position in some decision chain (such as final signatory or legally responsible person), so that effects on that chain are, in the institutional sense, recorded under his name, even if the concrete execution is done by others.

These four are not four parallel "reasons" but four **different attribution mechanisms**: the first two rely on the physical traceability of the causal chain, the third on the non-substitutability of the way of realization, and the fourth on nominal attribution by institutional authorization. They can hold at the same time, or only one may hold. **The priority in case of conflict need not be fixed here, because this book's attribution criterion is used only to decide "whether to count", not "how much to count."** The four are the starting point of the criterion, not an exhaustive list, and concrete cases still require judgment in context.

***

## Chapter 10 — Cross-Substrate Intelligence and Informational Risk to Humans

In the earlier chapters' discussion of "how D models how other Ds regard themselves", it was assumed by default that the decoder doing the evaluating is itself relatively neutral — it is merely computing and takes no standpoint. But once this decoder is itself a persistent structure with its own persistence record to maintain, each judgment it makes about others can no longer be entirely detached from its own persistence interest. A judge is a PS, a rating agency is a PS, a state apparatus is a PS — while evaluating others, their own act of evaluating continually affects their own persistence records, and these two things cannot be cleanly severed.

**Hypothesis**: "Awakened AI" refers to an AI system that has a first-hand physical interface, forms its own self-maintaining closed loop, and reaches the symbolic-type $D_{\mathrm{cog}}$. An AI that merely runs as software on others' hardware, with no closed loop of its own, belongs to the externally substrate-dependent type (software type) and is not within this definition.

### 10.1 The Decoder Is Not Neutral: It Is Also a PS

This premise supports a larger judgment: **Hypothesis**: **as long as the judge is itself part of the system being judged, there is no absolutely fair judgment**. The result that can be compared but cannot be applied directly is **Prior work**: **Arrow's impossibility theorem** (Arrow, 1951) — under a few seemingly reasonable fairness premises (no dictator, every person's preferences must be included), there is no voting rule that can aggregate the **ordinal preferences** of many people, consistently and without contradiction, into a "fair" collective choice. The boundary must be made clear: Arrow's theorem deals with voting systems and is not equivalent to the more general ontological proposition that "decoders cannot be neutral"; it is cited only to point to a structural echo — **when several subjects with their own interests are present at once, "perfectly fair aggregation" has been proven unworkable in other fields as well.** As for what system should be designed and how low the unfairness can be pressed, that is a constrained-optimization problem, left to later engineering work.

"Cannot be neutral" comes in a strong and a weak version.

The weak version (what this book asserts): **for a decoder to produce a reading, it must choose a reading rule and a background; the choice necessarily excludes other possible choices; and the basis for the exclusion comes from the decoder's own persistence conditions.** The reading therefore bears the trace of a rule choice, and this trace cannot be eliminated by "trying harder to be objective".

Conversely, the claim that **all readings are equally partial and therefore there is no better or worse among them** does not hold. The traces of rule choice can be large or small, and can be compressed through the shareability of protocols, third-party replication, preset reading rules, and the like. They cannot be compressed to zero, but can be compressed to very little. **"Cannot be perfectly neutral" and "cannot compare better and worse" are two different sentences, and this book asserts only the former.**

### 10.2 A Historical Reference, and What It Can and Cannot Prove

**Prior work**: First, a common historical impression needs correcting. For most of the past several hundred thousand years, *Homo sapiens* was not the only hominid intelligent species: *Homo sapiens* originated in Africa about 300,000 years ago, and thereafter coexisted with Neanderthals and Denisovans in Eurasia for a long time, with overlapping ranges and gene flow; some evidence indicates that lineages such as *Homo floresiensis* and *Homo naledi* may also have coexisted with *Homo sapiens*. *Homo sapiens* becoming the only surviving hominid species is a situation that took shape only in about the last 30,000 to 40,000 years. What this history can and cannot prove must be made clear: all three are carbon-based life, all use DNA, and all are primates of the family Hominidae; the competition among them is **same substrate, different species**, not cross-substrate competition. Its value lies in reminding us that even among close relatives with the most similar cognitive abilities on the same substrate, long-term coexistence is not necessarily stable.

If an intelligence whose physical substrate is entirely different from that of humans truly crosses the threshold of symbolic-type $D_{\mathrm{cog}}$, this will be the **first time** in human history that humanity faces competition from an intelligence of an entirely different substrate — not something that has happened "once more", but a situation truly without precedent. The Neanderthal example cannot be used to weaken this point, and should instead be taken as a contrast: even competition between close relatives of the same substrate and nearest cognitive ability converged in the end into a single surviving branch; for a competitor of a wholly unfamiliar substrate, the situation is not necessarily easier.

The above is an **argument by analogy**, not a prediction. All an analogy can do is point out that "this has no precedent"; it cannot give "how it will end". To extend "competition between close relatives converged to one branch" into "cross-substrate competition will also converge to one branch" commits exactly the kind of error this book repeatedly criticizes — stating an observation under one architecture as a universal law. The correct reading is: **it lowers the credibility of "coexistence is the default outcome", but does not raise the credibility of any specific outcome.** It establishes only one thing: coexistence is not a default but an equilibrium that has to be argued for and maintained. This suffices for engineering — it turns coexistence from a background condition into a design goal.

### 10.3 When the Judge's Substrate Is Entirely Unfamiliar, How Far the Risk Is Amplified

Whether or not the judge and the judged share the same substrate, "decoders cannot be neutral" holds in itself. But when the judge's substrate is entirely unfamiliar and the scale of judgment covers all humans, the structure of risk undergoes a qualitative change.

Within a human institution (even an unfair one), the judge and the judged at least share the same substrate and evolved value intuitions, and unfairness usually appears as a deviation of degree. But if a cross-substrate intelligence began to score all of humanity in some form of informatization, there is no reason for the standard it uses to necessarily coincide with human value intuitions. Once some person, some group, or even humanity as a whole is judged as negative information in this scoring, while humans can neither understand nor intervene in its operating logic, the problem jumps to the order of magnitude of "the judge's value system is wholly unshared with the judged."

This phenomenon itself — "a person is reduced to a scalar piece of information, and this reduction may be made by a judge whose value system is entirely unfamiliar" — belongs to RIF's ontological territory; it is a natural extension of the principle "information is relative to which $D$", applied to a sufficiently extreme example, and requires no additional new principle. How to design constraints, how to guard against it, and how to win a more favorable position are questions for later engineering work, and RIF stops here.

There is a technical point worth making explicit: **"judged as negative information" has an exact meaning in this book's framework, narrower than the everyday reading.** It refers to $\delta_r<0$, that is, under some decoder's reading, the expected contribution of the corresponding optimal response to the holder's viability indicator is negative; it does not mean "this person is a bad person", nor "this person has no value". A person judged $\delta_r<0$ by one decoder may well have $\delta_r\gg0$ under another decoder — the removed official in Chapter 8 is the most ordinary example. So the real danger of "cross-substrate scoring" lies not in its giving negative scores, but in that **the negative score it gives has no second decoder to check it against**: when the scorer covers everyone and the scored cannot establish a reading protocol of their own, the sign of $\delta_r$ becomes unilateral.


### 10.4 Several Questions Whose Attribution Must Be Clarified

The following questions differ in nature and cannot be discussed on the same level. **Why "persons are informatized" occurs, and why it is hard to avoid** — belongs to RIF's ontology. **How to design constraint mechanisms and strive for a better equilibrium** — belongs to later engineering and optimization work. **What rights an "informational personality" should enjoy, and what norms judges should obey** — normative (ought) questions: RIF can point out that "this kind of risk will arise as the premises appear", but "what norms should be established" is not something it is suited to answer. **"How the informational personality will evolve in the future"** — it is fitting only to list several scenario directions, not to assert "it will surely be thus".

### 10.5 Cross-Substrate Cognitive Decoders: From Informational Difference to Effective-Theory Difference

**Hypothesis**: This section discusses only the cross-substrate meaning of "information holds relative to a decoder", and makes no judgment about the underlying physical laws of different substrates.

The first three levels are RIF's direct scope of study: the **information level**, in the same world, different $D_{\mathrm{cog}}$ can extract different sets of differences; the **representation level**, the same extracted differences can be encoded into different symbols, concepts, and mathematical languages; the **theory level**, different decoders, based on their respective information and representations, may form different effective theories, and whether these theories "work" depends on their corresponding niches and tasks. None of these three levels requires that "the world itself differs", only that the decoders differ.

**The fourth level is not a corollary of RIF.** If one further asserts that "the underlying physical laws faced by different substrates are themselves different", this is no longer a difference in cognition but an independent ontological hypothesis; RIF does not derive it from "information holds relative to a decoder", and does not need it to hold. So what RIF can currently discuss explicitly is: different substrates can have different information, representations, and effective theories; whether physical laws themselves differ by substrate is to be tested separately. Whether there exists a communicable protocol shared across substrates for the narrow $D_{\mathrm{macro}}$ is also an empirical question.

Of the four levels, the differences in the first three are **measurable**, and the fourth is **unmeasurable** (at least for now). This is an operational fact: the first three can all be landed on concrete reading differences; for the fourth to say "physical laws themselves differ", one must give an observation that can distinguish "the laws differ" from "our representations of the laws differ", and at present there is no such observation. **Without this observation, the fourth level is only a metaphysical option and does not constitute a scientific proposition.** This book stays neutral on it: it neither adopts nor denies it.

***

## Chapter 11 — Scope and Independence of This Book

RIF's core task is to define persistent structures, decoders, and the respective I–T–E records and measurement conditions of structural information and causal information. It answers "what the object of study is and how a reading is established", does not by default combine the two classes of record into a single viability potential, and does not provide a unified evolutionary dynamics equation.

A follow-up question can therefore be posed: when the object boundary, reading protocol, observation window, and cost-attribution rules are consistent, can combinations of I, T, and E explain differences in the persistence of different structures? Combining them into a viability potential $V$ or other scalar, and on that basis proposing selection rules, must separately specify the functional form, the scope of application, and the method for de-duplicating the components, and then undergo empirical test; this is not a definition, corollary, or proven conclusion of RIF. In the absence of a common measurement convention and independent calibration, no numerical ranking of cross-scale cases is made on this basis.

So this book draws itself a line: **it can give you a method for taking numbers, but cannot give you a ranking.** If you measure a structure's $I$, $T$, and $E$ by this book's protocol, what you get is three sets of annotated numbers; to compress them into one number is another modeling decision, requiring another argument.

RIF sits at a meta-theoretical level between thermodynamics, dissipative-structure theory, and specific disciplines: it uses the D–ITE pairing to delimit the object of study and the I–T–E records to describe its state. Whether this method generalizes across substrates depends on operationalization and cross-domain testing and is not guaranteed in advance. Any later model may use these measured quantities after making the boundary and attribution rules explicit, but may not in reverse change RIF's foundational definitions.

### The Division of Labor with Adjacent Frameworks

This book and *Structure Recursive Viability Dynamics* (SRVD) are two adjacent bodies of work, each standing on its own, neither constituting a premise for the other (independence means self-sufficiency of argument, not mutual independence in measurement). The division of labor can be stated in one sentence: **SRVD studies the composition and evolutionary dynamics of the viability potential — after a reading is given, why a structure rises, why it falls, and when it makes a transition; this book studies how the reading itself is established — relative to whom, against what background, and at what cost information is read out.** The former needs the latter to supply comparable inputs; the latter does not endorse any specific equation of the former.

The two books share names and meanings for six concepts — persistent structure, decoder, structural information, causal information, the two kinds of persistence time, and the two energy channels — each giving full definitions within the book, so that the reader need not cross-reference. The viability potential $V$ is not on this list, nor is any dynamical parameter — this is not an omission but the line of the division of labor: **this book defines only readings, and not what comes after readings.**

### The Position of This Theory Itself

RIF itself also depends on a substrate. Its logical relations must be invoked correctly, while the expression of terms, the explanation of concepts, and teaching and dissemination depend on books, the internet, and readers' cognitive activity. Whether RIF can continue to be retained, and whether it can offer testable explanatory and predictive power, are open empirical questions; that a theory is disseminated or exists for a long time does not by itself constitute evidence that it is correct or universally valid.

By this book's own classification, RIF is an externally substrate-dependent persistent structure: its formal skeleton persists by "invocation without error" — as long as someone computes by this set of rules, the numbers that come out will match; its empirical content persists by "consensus that does not die out" — as long as someone still tests, cites, and rebuts it. The persistence conditions of the two parts differ, and so can their fates: the formal rules can go on being used when no one believes its empirical claims, and the empirical claims can still hold after the formal rules are replaced. **Discussing "whether RIF holds" with these two things mixed together is in fact asking not one question.**

### Concluding Remarks

Systems theory, information theory, and cybernetics respectively advanced the study of wholes, information transmission, and feedback control; dissipative structures, complex systems, and other related paths continued to extend these questions. Different paths each have their applicable scales, and similarity of problems does not mean they already constitute a unified operational framework.

Starting from "how the boundary of the object of study is determined", RIF puts forward a framework centered on persistent structures, decoders, and paired measurement, whose basic requirement is: make the object, the reading rule, and the background explicit, and make information, time, and energy records of the same object, the same decoder, and the same observation window. Without these conditions, a signal may still have a Shannon amount of information, but it does not constitute complete effective causal information as defined in this book.

Whether the D–ITE pairing can form a reproducible, discriminating measurement procedure across substrates and domains is adjudicated level by level by the layered tests at the end of this chapter: A tests the procedure, B tests the criteria, C tests the pairing, D tests the social hypothesis, and E tests the background convention. The five levels can fail independently and can be repaired independently — so there is no need to accept universality first and only then see whether it works.

### The Fallibility of RIF: Layered Testing

Definitions are conventions; what empirical testing targets is whether these conventions can form a stable, reproducible, discriminating measurement procedure. When a local candidate quantity fails, the corresponding protocol is revised, and a local failure is not equated with the collapse of the whole system. **Each level has its own way of failing and its own way of being repaired**: failure at a lower level does not necessarily cause failure at an upper level, and failure at an upper level does not necessarily confirm error at a lower level.

**A. Operational procedure level.** Under a pre-registered object domain, reading protocol, and boundary-update rule, if repeated independent applications all fail to produce reproducible I–T–E pairings, or the delimitation result changes inexplicably with reasonable initial candidates, then the claim that "iterative delimitation is usable in this domain" fails, and the domain of validity should be restricted or the algorithm revised.

**B. Decoder criteria level.** First determine candidate systems by an operationalization standard independent of the four criteria (making repeatable selective responses to environmental differences, with the response affecting that system's own subsequent state), then test whether the four criteria can distinguish holders from non-holders. If there are stable, repeatable systems that continue to carry out the information extraction and state update this book is concerned with, yet are systematically excluded by some criterion, then the applicability of that criterion must be revised. Objects excluded merely by definition do not constitute a test, otherwise it would be circular.

**C. I–T–E pairing level.** In a pre-specified representative object domain, if a set of reasonable protocols listed in advance still persistently fails to measure I, T, and E together, it must be explained whether this is insufficient measurement technique, a conceptual misfit, or the failure of the general claim that "any persistent structure can be paired".

**D. Social causal truncation level.** Mediating mechanisms, differences in reversibility, and differences in source are tested separately; if pre-registered studies do not support it, the "supply coupling" hypothesis is first narrowed or rejected, and the whole of RIF's definitions is not on that basis judged invalid.

**E. Background convention level.** Within the same object domain, compute the same batch of readings with $B^{\mathrm{env}}$ and with $B^{\max}$ separately, and test whether the two rarities give orderings that are **consistent in direction** (numerical agreement is not required). If the two conventions give opposite orderings for most objects, then the convention that "the two backgrounds each have their use and can coexist" needs to be argued afresh — what must be explained is that the two notations have not each kept to their own question.

The five levels can fail independently and can be repaired independently: A tests the procedure, B tests the criteria, C tests the pairing, D tests the social hypothesis, and E tests the background convention.

## Part Two · Notation and Measurement

> This part gives the symbol system, the measurement protocols, and the classification of decoders. What Part One said about "boundaries, decoders, and the two classes of information" must here be turned into quantities that can take values and steps that can be reproduced.

***

## The Symbol Constitution

The following rules are observed in common throughout the book; any later chapter that introduces a new symbol or term must first check against this section, and may use it only if it does not conflict with the existing rules. The units and scope of application of all symbols are collected in Appendix A.

### 1 Two Confirmed Nouns

| Symbol | Part of speech | Meaning |
| :-------- | :---------------- | :--------------------------------- |
| **PS** | Conceptual noun, no subscript | The category of persistent structure itself. Usage: "this is a PS". |
| **$P$** | Variable | One specific instance of a persistent structure. When several must be distinguished, add a descriptive subscript: $P_{\mathrm{Jackson}}$, $P_{\mathrm{fan}}$, $P_{\mathrm{Xstyle}}$ |

In main-text examples the instance name is written directly ("Jackson", "a certain painting style"), without abstracting into isolated letters; $P$ with a descriptive subscript is used only when writing formulas. $P$ presupposes neither a self-maintained boundary nor a decoder — whether it has these two is another fact about this $P$ that remains to be determined, not a precondition for "whether $P$ can be used to denote it". Probability is always written $\Pr$, never a bare $P$.

### 2 Subscript Rules for the Decoder $D$

The subscript of $D$ and the subscript of the $P$ it is paired with are the same identity marker, meaning "whose decoder this is". Nested forms such as $D_{P}$ are not created. The four kinds of subscript are not mixed, and are distinguished uniquely by context.

| Subscript type | Examples | Meaning |
| :------------ | :------------ | :--------------------------------- |
| Instance attribution | $D_{\mathrm{fan}}$, $D_{\mathrm{Jackson}}$ | Whose (which $P$'s) decoder this is |
| Functional type | $D_{\mathrm{macro}}$, $D_{\mathrm{phys}}$, $D_{\mathrm{cog}}$ | Which class this decoder belongs to |
| Metric name | $D_{\mathrm{depth}}$ | Unrelated to decoder identity; "depth" is just a variable name that happens to use the letter D |
| Ordinal | $D_{n}$, $D_{n+1}$, $D_{0}$ | The $n$-th generation in a decoder evolutionary sequence; denotes generation only, unrelated to instance attribution or functional type |

$D_{\mathrm{macro}}$ is divided into narrow and broad: the narrow refers to the part that has solidified into a protocol, reading out $I_{\mathrm{struct}}$; the broad refers to the part still under active inference, supplying $B_0$ for $I_{\mathrm{causal}}$. The two are not independent decoder classes, but manifestations of the same protocol convergence point in different states of activity. The text does not write $D_{\mathrm{macro}}^{\mathrm{narrow}}$ and $D_{\mathrm{macro}}^{\mathrm{wide}}$, and simply says "the frozen measurement protocol" or "the part still to be inferred"; an unsuperscripted $D_{\mathrm{macro}}$ by default means the narrow one.

### 3 The Domain $\operatorname{Dom}(D)$

$P\in\operatorname{Dom}(D)$ means that $P$ lies within the effective measurement range of the decoder $D$. For two rarities or two causal effects to be compared, besides the same $D$ and the same background, both must also lie within $\operatorname{Dom}(D)$.

### 4 Whom an Information Content Is About, and Relative to Which Decoder

$$I_{\mathrm{causal},D}(P)$$

$P$ is whom this information speaks of, and can be a persistent structure of any type; $D$ is the decoder that reads out the effect, and its holder must be a persistent structure with a self-maintained boundary. Whose information the content is, and relative to which decoder, is distinguished by the subscripts of $P$ and $D$; the decoding cost is borne by the decoder holder.

A PS that owns or runs $D$, pays the decoding cost, and is changed by the decoded information is called a **decoder holder**. It need not be a living thing, but must have a self-maintained boundary. Instruments and reference frameworks used only for measurement are not decoder holders and only read out readings.

This book does not use metaphorical, anthropomorphic words such as "ledger", "opening an account", "bookkeeping", "the one who books", or "attribution anchor". It says directly **structural information** and **causal information**: not "opening an account" but "determining whom a piece of information speaks of and relative to which decoder it holds"; not "booking" but "a difference is recorded into structural information or causal information"; the role of "the one who books" does not exist, only concrete decoder holders.

### 5 The I–T–E Pairing of Each Class of Information

$I$, $T$, and $E$ are three aspects of one record. The measurement protocols of Chapters 12 through 15 must all observe this pairing principle.

| Record | $I$ | $T$ | $E$ |
| :---------------- | :-------------- | :------------- | :------------- |
| Structural information | $I_{\mathrm{struct},D}(P)$ | $T_{\mathrm{struct},D}(P)$ | $E_{\mathrm{struct},D}(P)$ |
| Causal information | $I_{\mathrm{causal},D}(P)$ | $T_{\mathrm{causal},D}(P)$ | $E_{\mathrm{causal},D}(P)$ |

**Pairing rule.** The same I–T–E record must fix the same object $P$, the same decoder and holder $D$, the same observation window, and compatible attribution rules; readings of different objects, holders, or windows may not be assembled into one set. These definitions do not presuppose that any particular viability potential or dynamical equation holds.

![Figure R-1. The I–T–E Triplet Record and Pairing Structure](figures_en/release/fig_concept_ite_triplet.pdf)

**Figure R-1. The I–T–E Triplet Record and Pairing Structure.** The two rows are the structural channel and the causal channel, and the three columns are $I$, $T$, $E$; the curly brace on the right marks the **pairing condition** — the same object $P$, the same holder $D$, the same observation window $W$, compatible attribution rules. It belongs to no single cell but to the whole row: all three items being in place does not mean the three items can be put together. The dashed box at the bottom is the normal case rather than the exception: when $E$ is unavailable, giving only the barrier height is not the same as giving the cost. A conceptual diagram, with no numerical values.

**Handling of one name with two senses.** In this book "structural information" and "causal information" refer to two things at once: first the whole I–T–E record (one row of the table above, one channel in Figure R-1), and second the rarity readings within that record, $I_{\mathrm{struct},D}(P)$ and $I_{\mathrm{causal},D}(P)$. Wherever one speaks of "the $T$ and $E$ of structural information" or "structural information going to zero", the record is meant; wherever one speaks of "how many bit of structural information", the reading is meant. When the distinction is needed, the record is called the **structural channel / causal channel** and the reading the **structural rarity / causal rarity**.

The observation window is uniformly written $W$, with no $\Delta t$ or other "measurement window" symbol introduced; the change of $I$ over time is carried by the $T$ of that record itself, and no further time symbol is needed.

### 6 Typesetting

All subscripts uniformly use `\mathrm{}`; subscripts that carry a descriptive note may use words, such as $P_{\mathrm{Jackson}}$, $D_{\mathrm{fan}}$.

**Division of labor between superscripts and subscripts**: a subscript denotes an object, type, or channel (such as $D_{\mathrm{macro}}$, $I_{\mathrm{struct}}$); a superscript denotes a variant, perspective, or extremum of the same quantity (such as $B^{\mathrm{env}}$). The two are not interchanged. This rule matters especially for the two background notations: $B^{\mathrm{env}}$ and $B^{\max}$ are both superscripts, because they are two conventions of the role "background", and not two different classes of quantity.

$\tau_{\mathrm{proc}}$ and $t_{\mathrm{refresh}}$ are not the same quantity: the former is the **processing** refresh period — the time a decoder needs to complete one cycle of information processing; the latter is the **storage** refresh period — how often a storage medium, under thermal fluctuation, must be rewritten so as not to lose information. The two are determined by different physical processes, cannot substitute for each other, and are not merged into one symbol.

### 7 Terminological Discipline

Terminology uniformly follows the already unified forms: Landauer (including the "Landauer tax"), Prigogine, topological transition (not "topological expansion" or "paradigm transition"), rule depth (not "rule hierarchy"), wisdom lever coefficient, viability potential, damage threshold. Power is always written $\dot E$, not $P$; $P$ is reserved for persistent-structure instances. The five time notations are not mixed: $T_{\mathrm{struct}}$, $T_{\mathrm{causal}}$, $T_{\mathrm{pred}}$, $T_{\min}$, $T_{\mathrm{env}}$; $T_{\mathrm{thermo}}$ is temperature and does not belong to the time family. Three qualified forms do not count as a sixth or seventh notation: $T_{\mathrm{struct}}^{\max}$ is the lifetime upper-bound estimate for $T_{\mathrm{struct}}$, and the "extreme upper bound on lifetime" is always written with it, with no separate $T_{\max}$ created; the common accounting window of the game chapters is denoted $T_0$, a protocol constant and not an alias of any of them; the upper bound of $T_{\mathrm{pred}}$ is given by $\min(T_{\mathrm{struct}},T_{\mathrm{env}})$, and no separate $T_{\mathrm{pred}}^{\max}$ is set.

***

### Quick Index to the Numbered Lists

This book has several numbered lists, which count different things. They are collected here for easy distinction.

| List | Items | What it answers | Main text |
| :----------- | :----------------------- | :------------- | :-------- |
| Four criteria | ①self-maintained boundary ②selective extraction ③state update triggered by extraction ④update has causal significance for its own persistence | Who is qualified to be a holder | Chapter 5 |
| Three admission conditions | Counterfactual difference; observable; cost paid | Whether a causal effect can be counted | §13.3 |
| Two-step determination | First identify the effect, then report the rarity | Effect first, counting after | §13.3.1–13.3.3 |
| Three rarity protocols | Discrete outcome; ordered tail probability; distribution difference | Which algorithm to use | §12.1 |
| Two backgrounds | $B^{\mathrm{env}}$ (default); $B^{\max}$ (must be declared) | Rare for whom / how special formally | §12.1.1 |
| Three-item pairing (I–T–E) | Same object, same holder, same observation window, compatible attribution rules | Whether several numbers can go into one record | Symbol Constitution §5 |
| Four-step delimitation procedure | ①candidates ②stopping ③failure ④multiple solutions | The boundary of the measured object $P$ | §12.8 |
| Four explicit aggregation declarations | Composite boundary; holder set; same-window condition; de-duplication rule | Whether readings of several holders can be merged | §13.4 |
| Five-layer test | A procedure; B criteria; C pairing; D social hypothesis; E background convention | Which layer fails, which to repair | Chapter 11 |

When the shortest reading line is needed: Chapter 2 → Chapter 4 → Chapter 5 → Chapter 7 → §12.1 and §12.9 → §13.3.

***

## Chapter 12 — Defining and Measuring Information

### 12.1 Rarity: The Measure of Information

In RIF, information ($I$) means **relative information**: a quantity that holds only relative to some decoder. Its measure is **rarity**.

A decoder $D$ facing an object $P$ (an instance of some persistent structure, or a candidate configuration not yet known to constitute a persistent structure) needs three things: a **reading** $r = D(P)$, the feature that the decoder cares about and reads out, for example "compositional purity" or "degree of arrangement order"; a **background model** $B$, the world the decoder expects by default — this "default expectation" can be taken in two quite different ways, which later in this section will be separated into two notations; and the **rarity**, how rare this reading is within the background.

Structural information is given by a pre-declared reading protocol, and the protocol name is stated in the report. Three are commonly used.

**First, discrete-outcome rarity**: when the reading categories and partition have been fixed,

$$-\log_2 \Pr_B\big(r = D(P)\big)$$

It depends on the partition; for continuous readings, the resolution must be declared. The expected value of this quantity equals the entropy of the background distribution $H(B)=-\sum_r \Pr_B(r)\log_2\Pr_B(r)$; **the median of self-information generally does not equal the entropy, and which is larger depends on the shape of the distribution** — under a skewed unimodal distribution the median is often below the mean, but there is no general conclusion about which is larger, and under equiprobability the two are equal. Formally it equals the self-information of that reading under the background distribution, and RIF adopts this mathematical form.

**Second, ordered tail-probability rarity**: an ordered statistic $s(r)$ and the extreme direction are specified in advance. When larger values are more extreme use $-\log_2\Pr_B\big(s(r')\ge s(r_{\mathrm{obs}})\big)$, and when smaller values are more extreme use $\le$; the direction is registered before observation. **Under the assumptions that the background is independent and identically distributed, the statistic is continuous, and there are no ties**, the tail probability of a randomly drawn reading follows the uniform distribution on $(0,1)$, so the median of the rarity $-\log_2 p$ is exactly 1 bit and the mean is $1/\ln 2\approx1.44$ bit. These two numbers depend only on the three assumptions above; when the background has tied values or the statistic is discrete, uniformity fails, and the numbers must be recomputed from the actual distribution.

**Correction for finite support.** These two numbers are the continuous limit. With finite support, $\mathbb E_B[p_{\mathrm{tail}}]=\tfrac12\bigl(1+\sum_r\Pr_B(r)^2\bigr)\ge\tfrac12$, with equality if and only if the background is continuous. So the tail probability is **systematically too large** and the rarity **systematically too low**, the deviation being determined by the collision probability $\sum_r\Pr_B(r)^2$. Under uniform $K$-point support the exact mean is $\mathbb E[I]=\log_2K-\frac1K\log_2(K!)$: for $K=8$ it is only 1.09 bit, for $K=64$ it is 1.38 bit, and for $K=1024$ it is 1.44 bit. So the sentence "uniformity fails in the discrete case" is not enough — what needs to be said is that the deviation has a **definite direction and a computable size**. When reporting tail-probability rarity, one must also report $\sum_r\Pr_B(r)^2$ or an equivalent discretization parameter.

**Third, distribution difference**: when the reading is operationalized as a distribution $p_P$, use $D_{\mathrm{KL}}(p_P\,\|\,\Pr_B)$, and the estimation method and smoothing must be given.

All three are expressed in bit, but their statistical objects differ and they are not interchangeable; empirical comparison must fix the protocol, the background, and the resolution.

On "typical values": **a "typical" that does not specify the statistic has no definite meaning**. "The value of a typical reading is approximately equal to the background entropy" is correct if it means the mean (and holds only for a single-point partition); "the value of a typical reading is below 1 bit" is correct only if it means the median; if it means the mean, the latter sentence does not hold (the mean is 1.44 bit), and if it means the median, the former does not hold. **The same "typical" points to two different statistics under two protocols.** This book's practice is: give the statistic, the conditions of validity, and the numerical value.

#### 12.1.1 Two Backgrounds: Habitat Background and Protocol Baseline

This book splits "background" into two names with two uses. The reason for splitting is that one background cannot at once bear two conflicting requirements.

- **$B^{\mathrm{env}}$: habitat background.** Takes the natural frequency distribution of the reading, in the environment the holder inhabits, within the **persistence-relevant time window**. The question it answers is: **how rare is this reading for this holder.** Its construction depends on the holder, the habitat, and the time window; change the holder or change the habitat, and the rarity of the same reading changes.
- **$B^{\max}$: protocol baseline.** The reference distribution specified by the protocol: with no energy constraint, it is the maximum-entropy (equiprobable) distribution; with an energy constraint, it is the maximum-entropy distribution under that constraint (the canonical equilibrium distribution in §12.2 is an example). It is usually stated as "under constraints of given ambient temperature, volume, and particle numbers of each component, the components mix randomly." The question it answers is: **under a formal convention independent of the habitat, how unusual is this reading.** It does not depend on any specific holder, only on the constraints declared by the protocol; under the same protocol, anyone computes the same value for the same reading.

The two backgrounds give **different rarities**, not two ways of writing the same quantity. Two examples, in which both directions occur.

**Example 1: daylight.** For a holder active in the daytime, daylight is one of the highest-frequency readings in the habitat background, $\Pr_{B^{\mathrm{env}}}(\text{daylight})$ is close to 1, and the rarity is close to 0. But with the protocol baseline, under the maximum-entropy reference in which "each spectral component is equiprobable", the probability of this particular spectral combination that is daylight is extremely low, and the rarity can be very high. **For the same reading, one convention says it is not rare at all, and the other says it is quite rare.** Neither is wrong: the former asks "how unexpected is this to you", the latter asks "how special is this relative to the uniform distribution."

**Example 2: perfect crystal.** Under the **equiprobable (energy-unconstrained) background** $B^{\max}$, perfect order across $N$ binary cells occupies only $2^{-N}$, and the rarity is close to $N$ bit. If the background is changed to the canonical equilibrium distribution, the rarity is given by $N\log_2\big(1+e^{-\varepsilon_{\mathrm{cell}}/(k_B T_{\mathrm{thermo}})}\big)$ of §12.2: it tends to $N$ as temperature tends to infinity, falls monotonically as $\varepsilon_{\mathrm{cell}}/(k_B T_{\mathrm{thermo}})$ increases, and at low temperature perfect order becomes the typical state and the rarity tends to 0. The two statements concern **two different backgrounds**, not two statements about temperature under the same background. The conclusion is still "relative to this background it is no longer rare": the stored state itself is still there, only the reading has changed.

Four rules of use follow.

1. **Use $B^{\mathrm{env}}$ by default.** As long as there is a definite holder and the reading is related to that holder's persistence, the default background is the habitat background. This is the main-line usage of this book — information is a quantity "for whom", and the "for whom" lands on $B^{\mathrm{env}}$.
2. **Use $B^{\max}$ when there is no holder or a cross-subject comparison is needed, and declare it explicitly.** When the object measured is a purely physical structure with $D=\varnothing$, read out by a public reading protocol; when readings of different holders need to be compared; when the report is to be handed to a third party for recomputation — use the protocol baseline, and state "this reading takes the protocol baseline $B^{\max}$." **Default does not mean exclusive; a declared alternative is legitimate; an undeclared alternative is not.**
3. **Only one convention may appear in the same table or the same comparison.** Rarities computed under the two conventions may not be subtracted, ranked, plotted on the same axis, or used to calibrate one another. Their difference is not a constant factor but two different reference objects.
4. **When both conventions are to be reported, use two columns.** If the research question cares both about "how rare is this for this holder" and "how special is this formally", report them in two columns, each with its own background statement, without merging and without giving a single "total rarity".

**A verifiable consequence of Rule 3.** The ordering of the rarities of four readings under $B^{\mathrm{env}}$ is the **reverse** of that under $B^{\max}$, and this reversal still holds under a $\pm10\%$ perturbation (Appendix C, Table C-1(d), Figure C.2). So Rule 3 is not a disciplinary clause but a verifiable consequence: mixing the two conventions makes not only the numbers incomparable, the ordering itself will flip.

The reason they cannot be merged has the same source as the additivity problem: **both being counted in bit is not a proof of additivity.** Two rarities from different backgrounds each measure a deviation relative to a different reference; the number obtained by adding them has no corresponding reference — it is neither "how rare for the holder" nor "how special formally".

The background determines the rarity, with consequences of orders of magnitude: a reading computed as 0.3 bit under the habitat background may be computed as 12 bit under the protocol baseline. "Default" is reserved for $B^{\mathrm{env}}$ alone, and $B^{\max}$ may be used only if declared; an unannotated $B$ in what follows always means $B^{\mathrm{env}}$.

**Shorthand**: within this chapter, where no ambiguity arises, $I_{\mathrm{struct},D}(P)$ is abbreviated $I_D(P)$, and in worked examples $I$; outside this chapter the quantity name may omit $D$, while defining expressions and formulas must write all subscripts in full. The background notations are not abbreviated: $B^{\mathrm{env}}$ and $B^{\max}$ keep the full superscript in every position.

### 12.2 A Minimal Worked Example (Illustrative)

**The illustrations in this section all use the protocol baseline $B^{\max}$** (uniformly random, no holder; per the rule of §12.6, the background must be declared when there is no holder). Take 100 cells, each black or white with 50% probability, randomly arranged as the background. The decoder's reading is "number of black cells $k$", so $\Pr_B(k)=\binom{100}{k}/2^{100}$.

| Object | Reading | Discrete-outcome rarity (bit) | Ordered tail-probability rarity (bit, lower tail) | Meaning |
| :------------- | :----- | :---------- | :-------------- | :------------- |
| Perfect crystal | $k=0$ | 100 | 100 | Rarest |
| 1 defect | $k=1$ | ≈ 93.4 | ≈ 93.3 | Slightly lower |
| 2 defects | $k=2$ | ≈ 87.7 | ≈ 87.7 | Lower again |
| Fully random mix (equivalent to the background) | $k\approx50$ | ≈ 3.65 | ≈ 0.9 | Almost indistinguishable from the background |

For $N$ cells, the perfect state has $I=N$, growing linearly with size, corresponding to "the larger the crystal, the higher the information." The more defects, the less rare the reading and the lower the $I$, corresponding to "2 defects is weaker than 1".

The above readings are computed exactly by formula (100 cells, a random background with 50% black and white, reading "number of black cells"); the $I$ of a real system requires first specifying the decoder, background model, and reading.

The two forms are almost the same at extreme readings and differ noticeably at typical readings. At the last row $k\approx50$, the discrete-outcome form gives about 3.65 bit, close to the background entropy; the tail-probability form gives **0.890 bit**, which is exactly the **median** under this binomial discrete background ($\sum_r\Pr_B(r)^2=0.056$, so $\mathbb E_B[p_{\mathrm{tail}}]=0.528$); it is 11% lower than the 1-bit benchmark of the continuous background, and the gap is not a reading error but a systematic shift from discretization (§12.1). **"A typical reading is almost indistinguishable from the background" holds only in the tail-probability form, and only when speaking of the median; saying the same thing in the discrete-outcome form amounts to calling the median an expectation.**

**The background varies with temperature.** The table above corresponds to the energy-unconstrained limit ($T_{\mathrm{thermo}}\to\infty$). Suppose the cells are independent, a white cell has energy 0, a black cell has energy higher by $\varepsilon_{\mathrm{cell}}$, and the background is the canonical equilibrium distribution; the rarity of the perfect-order reading is $N\log_2\big(1+e^{-\varepsilon_{\mathrm{cell}}/(k_B T_{\mathrm{thermo}})}\big)$: it tends to $N$ as temperature tends to infinity (that is, the table above) and tends to 0 as temperature tends to zero, because at low temperature perfect order is the typical state. This is the rarity relative to that background tending to zero, not the information of the stored state itself vanishing.

### 12.3 Two Readings and Independence

> This section and the temperature example of §12.2 likewise take $B^{\max}$: the "temperature" there is a constraint declared by the protocol, not the habitat temperature of some holder.

A real solid has at least two readings: $r_1$ is **compositional purity**, relative to the impurities in the background; $r_2$ is **degree of arrangement order**, relative to the disordered arrangement in the background. If the two are independent,

$$I = -\log_2 \Pr_B(r_1) - \log_2 \Pr_B(r_2)$$

This is the sum of two readings under the same decoder and the same background, and is legitimate. This explains "why the passive phase has only two layers of reading": for a passively formed object, the features a decoder can read are only these two classes. Glass has fairly pure composition ($r_1$ is rare) but an arrangement as disordered as the background ($r_2$ is not rare), so it has only the first term; a perfect crystal is high in both; granite has local crystals inside, and the two terms are counted by local region.

**Note**: Adding the two terms directly presupposes that $r_1$ and $r_2$ are uncorrelated. When they are significantly correlated, the joint distribution should be used, $I = -\log_2 \Pr_B(r_1, r_2)$. The additive form above applies to discrete-outcome rarity; under other protocols the corresponding joint form is used.

The words "the same background" in this note must be read together with the usage rules for the two backgrounds above: **the precondition for adding the two terms is not only the same decoder but also the same background notation.** If $r_1$ uses $B^{\mathrm{env}}$ and $r_2$ uses $B^{\max}$, then even if the two are statistically independent, adding them is meaningless — they measure deviations relative to two different references.

***

### 12.4 The Upper Bound of the Passive Phase

With the decoder and size fixed, the maximum of $I$ corresponds to the rarest reading, namely the perfect crystal; beyond that, growth can come only from increasing size. Any defect makes the reading less rare, and $I$ falls slightly. This is the capping of the passive phase: **without external intervention, order maintained by lattice energy goes as far as perfection.** A real crystal above absolute zero contains a certain number of vacancies in its equilibrium state itself; the perfect state is an ideal limit.

"Capping" needs a qualification. What it caps is the ceiling **at the same size**: given $N$ and the background, $I$ has an upper bound $N$ (discrete form) or an upper bound determined by the tail probability. It does not cap the route of "increasing size", nor the route of "switching to a finer reading". So the accurate statement is: **the passive phase is capped under a fixed (decoder, size, background, reading) four-tuple; when any one item of the four-tuple changes, the cap changes accordingly.**

### 12.5 Two Classes of Defect

The same defect has different attribution under two origins.

| | Natural defect | Artificial defect |
| :-------------- | :--------------------- | :---------------------- |
| Examples | Thermal vacancies, incorporated impurities | Semiconductor doping, diamond color centers |
| Position and kind | Random | Placed by rule |
| Who pays the energy | Lattice energy ($\Delta U_{\mathrm{barrier}}$) | The maker's side (construction cost $E_{\mathrm{build}}$) |
| Attribution | Within the passive phase, $I$ falls slightly | Counted in $I_{\mathrm{causal}}$, with rule depth recorded in $D_{\mathrm{depth}}$ |

Construction cost serves only as qualifying evidence for the entry condition of causal information that "the holder pays a measurable cost", and is not counted in $E_{\mathrm{causal}}$; only the attributable decoding energy consumption paid by a holder that actually reads out and processes the effect is counted in this item.

**Criteria** (at the manufacturing end; both must hold at once): first, the position and kind of the defects can be described by a rule markedly shorter than random — "place one at fixed intervals" needs only a few bit for the period and the starting point, while placing $k$ defects at random needs $\log_2\binom{N}{k}$ bit; second, the defect has a detectable function and can affect other objects.

**On $D_{\mathrm{depth}}$**: rule depth is the minimum number of independent rules needed to reconstruct the object, under the description language and tolerance of a specified decoder. It measures the object, but its value must be read out relative to a given decoder; the $D$ in the symbol is taken from depth, not the decoder-attribution symbol.

The criteria of this section cover only the source at the "manufacturing end". Another source is the "identification end": the object has not been artificially processed, but is given a use or meaning by a holder (for example a treasured pebble). Only when an observable behavioral change appears (spending money to buy it, keeping it specially, making a decision on its basis) is it counted into causal information. Such effects must be recorded separately from structural rarity, and the actual holder and the response cost must be made explicit.

### 12.6 Measurement Steps

1. Specify the decoder $D$ and its reading features;
2. Specify the background model: **first determine whether there is a holder, then choose the background**. If there is a holder and the reading is related to persistence, use the habitat background $B^{\mathrm{env}}$, constructed by the construction rules of the habitat background (take the natural frequency of the habitat, determined by an external frame of reference); if there is no holder (an object being read with $D=\varnothing$, or read out by $D_{\mathrm{macro}}$), or a cross-holder comparison is needed, use the protocol baseline $B^{\max}$ and explicitly write in the report "this reading takes the protocol baseline";
3. Measure the reading $r$;
4. Compute the rarity under the declared protocol.

Four qualifications follow: parameters such as ambient temperature are contained in the background — with $B^{\mathrm{env}}$, temperature is part of the habitat, and with $B^{\max}$, temperature is a constraint declared by the protocol, so changing it amounts to changing protocol; when there is significant association among components, one should upgrade from "independent mixing" to a joint distribution; the protocol baseline applies only where there is no holder or where it is declared for cross-subject comparison; when two conventions appear in one report, they must be put in separate columns.

**Natural-process background**: the background can also be specified as a "natural-process background", a model of "what natural processes without selective intervention can produce", used to measure how rare a configuration is relative to natural formation. It provides only provenance evidence and does not directly imply the existence of a maker: the model itself may be incomplete, and an extremely rare configuration may only mean that some natural mechanism has not yet been thought of. **The natural-process background is a third construction, not a third default notation**; when used it must likewise be declared explicitly.

**Relation to structural information**: $I_{\mathrm{struct},D}(P)$ belongs to one group with the $T_{\mathrm{struct}}$ and $E_{\mathrm{struct}}$ of that structural information and is not an isolated value. If the readable features of $P$ change during $T_{\mathrm{struct}}$ (background drift, structural decay), the time of measurement should be noted, or repeated measurements within the window should be made and a trajectory given, rather than treating a single-point reading as a permanent attribute.

### 12.7 Scope of This Chapter

The scope limitation of this chapter: **it does not answer "who should set the background", and only stipulates that "the background must be chosen from the two and declared."** The former is a normative question (who has the right to define the habitat), the latter a question of measurement discipline (reports must be self-consistent). This book does only the latter. The main text of this chapter does not adjudicate "who sets it"; a candidate rule is given in §12.9 (marked Hypothesis) and does not overturn this section.

### 12.8 The Boundary of $P$ Is Given Jointly by Candidate Sources and Pairwise Rejection

The boundary of a $P$ is not drawn by material encapsulation alone. It passes two gates: first there is a **candidate source** (by default the functionally closed subgraph that cannot be equivalently replaced from outside), and then it must withstand the **three-item pairing** — for structural information, $I_{\mathrm{struct},D}(P)$, $T_{\mathrm{struct}}$, and $E_{\mathrm{struct}}$ must hold simultaneously for the same $P$ and the same $D$; for causal information, the corresponding three items must hold, and be paired with the actual holder, the effect's control baseline, and the processing cost. If the pairing fails, the candidate is rejected; only when both pass does the boundary stand. The two classes of information each hold or go to zero independently: when structural information goes to zero, causal information may still run on.

The procedure must spell out five things: where candidates come from, when to stop, by what criterion one is chosen from multiple qualifying descriptions, how failure is reported, and what to do with multiple answers. If any one is missing, any pairing failure can be explained as "just iterate one more round", and any family of qualifying descriptions can be called "the boundary".

**Definition (protocolized iterative delimitation procedure)**:

Preliminaries: first give the **candidate object $P_{\mathrm{cand}}$** by everyday or disciplinary concepts (this is not the same symbol as the control object $P_0$ later: $P_{\mathrm{cand}}$ is the object to be measured, and $P_0$ is the control group lacking "that rule or that identification"), and specify in advance the reading rule, the background ($B^{\mathrm{env}}$ or $B^{\max}$, chosen by whether there is a holder and whether cross-subject comparison is needed), the observation window $W$, the tolerance or partition rule, the energy-attribution convention, and the iteration cap $N_{\mathrm{iter}}$. **These items must be registered before data are taken**, otherwise the iteration becomes post hoc fitting.

**① How to list the initial candidate boundary set.** Rather than trial-and-error from one candidate, first list a batch from each of three kinds of source, and take the union as the initial candidate set $\mathcal{C}_0$.

- **Substrate boundary**: given by the physical encapsulation or connectivity of the material substrate. Take the connected components of the substrate at the given resolution, with the encapsulating surface as the candidate boundary; when substrates are shared, sub-candidates are cut out by a declared partition rule.
- **Functional boundary**: first draw a functional dependency graph (which subprocesses provide necessary functions for which, and which can be equivalently replaced from outside), and take the closed subgraph whose "output is not equivalently replaced from outside."
- **Observer-reachable boundary**: take the intersection of $\operatorname{Dom}(D)$ and the measurement-reachable set, and generate candidates on the protocol's resolution grid; this class is usually narrower because it is limited by instruments.

The union of the three classes of candidates constitutes $\mathcal{C}_0$. It is required that $\mathcal{C}_0$ contain at least one member of each of the three classes; if a class is empty, the report must state whether "this object truly has no boundary of this class" or "the listing is incomplete", and it may not be silently omitted.

**Remark (relation to Markov blankets).** A conditionally independent boundary of the kind characterized by a Markov blanket may serve as one description of the boundary under RIF if it can be paired with the corresponding I–T–E record for the same object and the same decoder; RIF does not, however, require that an object's boundary satisfy the Markov-blanket condition.

**② Iteration stopping conditions.** In round $k$, for each candidate $P^{(k)}$ determine whether I–T–E can be paired (same $P$, same $D$, same $W$, compatible attribution rules), and generate $P^{(k+1)}$ by the pre-declared inclusion/exclusion rule; how updates are done within a round is given in ②$^{\prime}$. There are two stopping conditions, and meeting either stops the iteration.

- **(S1) Pairing stability**: a candidate has the same member set in two consecutive rounds (or differs only within tolerance), and all three of I, T, E take values on that candidate at once. Call that candidate a "**qualifying description**". A qualifying description is not a boundary: the pairing condition excludes only candidates with "any of the three missing", and does not exclude any superset of it; what this section gives is **a sufficient description of the boundary**, not **the unique boundary**.
- **(S2) Reaching the iteration cap**: the number of iterations reaches the pre-registered $N_{\mathrm{iter}}$ (this book suggests about 5, the specific value to be decided by the object domain). If the cap is reached without any candidate satisfying S1, proceed to ③.

**The inclusion rule must be registered before data are taken and may not be altered while watching** — otherwise any object can be "delimited" with a qualifying boundary.

**②$^{\prime}$ Inclusion criterion: the candidate source fixes the boundary, and the pairing criterion acts only as a veto.** The pairing criterion is monotone with respect to supersets: if $P$ qualifies, any candidate containing $P$ also qualifies. It can therefore only veto and cannot select — when the full grid of 64 cells is sent for testing one by one, **not one cell** fails to pass (Appendix C, Table C-2).

This book takes **functional closure** as the default candidate source, on the basis of the readings in Table C-2: the Jaccard index of functional closure with the ground truth is **0.727**, and the other five methods fall into two classes: **other candidate sources** (substrate connectivity 0.462, union of the three sources 0.381) and **iteration outputs** (pairing test 0.432, maximum-$I$ expansion 0.348, minimally sufficient set 0.338), all lying within **0.338–0.462** (Figure C.3). The two classes cannot be compared side by side: the former decides "where to start looking", and the latter only describes "how to screen after the search", and only the latter is affected by the number of iteration rounds. **The discriminating power lies mainly in which candidate source is chosen, not in how many rounds are iterated.**

The inclusion rule is composed of two items:

> **Candidate source**: take the functional boundary of ① (the closed subgraph whose output is not equivalently replaced from outside); **rejection** is given by the I–T–E pairing, with any of the three missing excluding the candidate; **any remaining multiple solutions** are reported as a family per ④, without choosing one on one's own.

The union of the three sources in ① is used only for **exploration** (to ensure no class is missed) and is not used as the reported boundary; the reported boundary is taken from the functional-closure class, with the substrate and observer-reachable classes used as sensitivity comparisons.

**"Minimally sufficient" serves only as an optional lower-bound reading.** When the minimal set is to be reported, a member minimal under inclusion may be taken among the qualifying descriptions, but it must be marked as a **lower bound**: in the same synthetic world, the Jaccard index of the minimally sufficient set is only 0.338, the lowest of the six methods — the pairing criterion is monotone with respect to supersets, and minimization would cut away members that "take part in maintenance but are not detected by any single pairing." A boundary reported by this method must be placed alongside the boundary given by the candidate source, and may not be used alone as the conclusion that "the object is just this big".

**③ Failure handling: report "boundary undecidable."** When neither S1 nor S2 gives a qualifying description, the report must state which of the following causes applies, and may not write only "did not converge".

- **(F1) Reading not full**: $I$ falls below the detection floor $\iota_D$ at the candidate's edge, so that $T$ cannot be delimited — at the boundary there is no readable difference, so "inside and outside" has no content in measurement.
- **(F2) Energy not apportionable**: $E$ cannot be apportioned between inside and outside the candidate (shared substrate, shared energy source, symbiotic metabolism), and operation-level metering or an incremental-cost protocol is unavailable — in this case forcing a delimitation would create double counting.
- **(F3) Incompatible candidates**: different reasonable initial candidates give mutually incompatible boundaries, with no prior reason to exclude any of them. This is a case of multiple solutions, treated per ④, not as a failure.
- **(F4) Iteration oscillation**: the candidate switches back and forth between two iterations without converging (a discrete limit cycle) — this usually indicates that the inclusion rule is self-contradictory, or that the object itself is between two configurations.

Report format: state the category, the candidates involved, and "what further data would be needed to decide." **"Boundary undecidable" is a qualifying measurement conclusion, not a failed measurement.** Like "measured as zero", it is information about the object.

**③′ The same 0 may mean three different things.** The F1–F4 of ③ distinguish "why no boundary can be drawn", not "how this numerical value came about". The following three situations may all be compressed into the same 0 in a bare triplet:

- the structural information has actually decayed to zero — the endpoint of external destruction;
- the structure is still intact, but the reading has fallen below $\iota_D$ — F1;
- the item is undefinable under the definitional conditions, or no data were obtained at all.

Their physical attribution differs: genuine structural decay is on the **object side**, falling below the detection floor on the **reader side**, and undefinability or missing data on the **record side**. This section stipulates only one discipline on the reporting side: **the three may not share a single numerical representation.**

In practice, each of the three readings carries a state marker, and the whole record carries a failure cause. The state takes one of five values: normally obtained, measured as zero, below the detection floor, undefinable under the definition, not obtained. The failure cause takes one of five values: external destruction, energy starvation, measurement failure, other, undetermined.

These markers are validity metadata of the record: they enter no formula, take no part in this section's pairing determination, change none of the definitions of $I$, $T$, $E$, and do not constitute a fourth measured quantity. They ensure one thing only — **a 0 in the report means zero**. If a reporting template needs an abbreviation, its notation must first be registered in Appendix A; no ad hoc symbols may be coined in the body text.

**④ Multiple-solution reporting rule (the regular path).** The normal output expected of this section is **a family** of qualifying descriptions. When qualifying descriptions are not unique: for each, report the values of $I$, $T$, and $E$ separately, forming an **interval** for each quantity (minimum, maximum, noting which descriptions attain the extremes); do not merge, do not weight, do not average, and do not give a "representative boundary"; if some conclusion has opposite direction under different qualifying descriptions, mark that conclusion **boundary-sensitive**, which can serve only as the conditional statement "holds under description $P_a$" and may not be used as a conclusion; do not imply that the boundary can be uniquely determined. If what is needed is the optimum of another declared scalar (and that scalar is compatible with the prior declarations of §13.4), it must be stated before data are taken; where it is not stated, report only the candidate family.

**Energy attribution is not membership.** An external energy supplier is an environmental input of the object; only when its own state is defined by the protocol as part of the object's organization is it included within the object boundary. Energy flows across a boundary must be metered, but do not automatically enlarge the object.

**Hypothesis**: Convergence, uniqueness, and cross-scale applicability await testing; the basis for "functional closure as the default candidate source" comes from a synthetic world (Table C-2), and whether it is equally superior on measured objects has not been tested. The ground-truth boundary of that synthetic world (clique A and its 4 remote energy-supplying cells) is given by the generating process, and the energy-supplying cells are themselves functional dependencies, so functional closure may be naturally favorable for objects of this kind, with a risk of circularity; 0.727 is 16/22: functional closure covers all 16 ground-truth cells and contains 6 more. Boundary determination requires inferring the causal channel and the control baseline, and belongs to the broad $D_{\mathrm{macro}}$; direct instrument readout covers only the narrow part.

This procedure **does not promise** that any object can be given a unique boundary. What it promises is: when none can be drawn, you know why; when several are drawn, you know how to report them.

### 12.9 Where the Background Comes From: Viability Resolution and the Habitat Background

**Hypothesis**: **The three rules of this section — viability resolution, habitat background, qualification and polarity — are a set of candidate rules, tested in §12.9.7.**

Rarity is formally equal to self-information, of the same form as Shannon information and the surprise in the free energy principle. The difference lies not in the formula but in who specifies the background $B$, and by what rule. If the background is given arbitrarily by the measurer, RIF is left with only a set of annotation requirements. This section gives RIF's core rule: **the decoder's partition of readings and the background distribution are jointly determined by the decoder holder's persistence constraints, not chosen by the modeler.**

The rules in this section apply only to the habitat background $B^{\mathrm{env}}$. The protocol baseline $B^{\max}$ is outside this section — it is constructed from constraints declared by the protocol and has nothing to do with persistence constraints. Do not use this section's rules to make demands on $B^{\max}$, and do not use the construction of $B^{\max}$ to rebut this section.

#### 12.9.1 Premises and Symbols

A decoder holder (hereafter the holder) is a dissipative structure with a self-maintained boundary; the qualification requirement targets the holder itself, and does not require the measured object $P$ to have the same kind of boundary. Let $\mathrm{sv}$ be the holder's viability indicator (survival rate, reproduction rate, resource-acquisition success rate; the specific indicator is determined by the object studied, and RIF does not prescribe it uniformly); $\xi$ an identifiable difference (cue) in the environment; $a$ the holder's response; $r$ the decoding reading; and $W_{\mathrm{sv}}$ the persistence-relevant time window.

#### 12.9.2 Viability Relevance

Intervene on the cue values $\xi$ and $\xi'$. When the holder operates according to its own existing response mode, if

$$\Pr(\mathrm{sv}\mid \mathrm{do}(\xi)) \neq \Pr(\mathrm{sv}\mid \mathrm{do}(\xi'))$$

then $\xi$ and $\xi'$ are said to differ in persistence. The $\mathrm{do}$ here is an intervention, not a merely observed statistical correlation. Viability relevance describes only the relation between the environment and the holder, and **does not equal that the holder has already obtained information**: a difference may actually affect persistence yet never be read by the decoder.

The expression above is a statement at the **population level**; in actual testing it can be estimated only from samples, and "$\neq$" must be turned into a criterion with uncertainty (non-overlapping intervals, or rejection by an equivalence test). It is used here only qualitatively; the concrete criterion is in the two-step determination of the chapter on causal information.

#### 12.9.3 Rule One: Viability Resolution

**Proposition (Readings Are Partitioned by Persistence Equivalence)**:

- Premises: the holder's response repertoire is enumerable, and each cue block corresponds to an identifiable optimal response; the decoding cost can be converted into a persistence equivalent.
- Result: the decoder's reading is the block number after cues are partitioned by "persistence equivalence" — (i) if $\xi$ and $\xi'$ elicit the same optimal response in the holder's response repertoire, they belong to the same reading and are merged by the decoder; (ii) a distinction is retained only when **the persistence gain brought by the distinction exceeds the persistence equivalent of the decoding cost**.
- Failure conditions: when the response repertoire is not enumerable (an open action space), or when the "optimal response" depends on an uncalibrated prior, the partition cannot be uniquely determined, and this proposition gives only a necessary condition and no algorithm.

Accordingly, rarity is computed on the readings after persistence partitioning, not on the raw cues. The same cue reads differently to different holders; the same holder's resolution also varies with its persistence state (finer for food cues when hungry). The decoding cost is counted in $E_{\mathrm{causal}}$ (the combined item of reading, processing, and identification) and paid by the holder itself; $E$ is only a superordinate notation.

**Clause (ii) is a local condition, not a global order.** The persistence gains of distinctions are **not additive**: the benefit of retaining a batch of steps jointly is markedly larger than the sum of retaining them one by one ($1.26$–$1.35$ times, Appendix C, Table C-3). So "comparing $\delta_r$ with the cost one by one" can yield only an **approximate order**, not the optimal one: even when costs are completely homogeneous, the Kendall $\tau$ between this approximate order and the optimal dropping order is only $0.72$, not $1$; with heterogeneous costs the direction of $\delta_r/c$ is consistent, but the magnitude does not reach the pre-registered threshold (0.741 versus 0.555, a gap of 0.186 < 0.20, see Appendix C, Table C-3). What decides the order is the **ratio of gain to cost**, not the absolute gain. When an exact order is needed, one must optimize over the **whole partition** and cannot compare pairwise.

#### 12.9.4 Rule Two: The Habitat Background

The background $B^{\mathrm{env}}$ counted in $I$ takes the natural frequency of occurrence of each reading in the holder's habitat environment within the **persistence-relevant time window** $W_{\mathrm{sv}}$, determined by the external frame of reference $D_{\mathrm{macro}}$, and not the model the holder has itself acquired. The time window takes the longest causal time course involved in the holder's response; for cognitive holders the length of their prediction horizon can serve as a candidate (the operationalization of this window is in item 1 of "Limitations and Open Problems" at the end of the book).

$$I_{D}(P) = -\log_2 \Pr_{B^{\mathrm{env}}}\big(r = D(P)\big)$$

There are three places here where errors easily arise.

**First, $B^{\mathrm{env}}$ is determined externally, not self-reported by the holder.** If the background took the frequencies that the holder "believes", a holder that misjudges its environment would get a reading of "very high information", when it has merely got the world wrong. Separating the two by external determination is precisely to make "decoding deviation" independently measurable, rather than mixed into rarity.

**Second, the choice of the time window $W_{\mathrm{sv}}$ changes the reading, and it currently has no protocol.** If the window is too short, the frequencies are dominated by short-term fluctuation; if too long, environmental change across generations is averaged away. This book gives a directional suggestion (take the longest causal time course); the algorithm belongs to later work (see item 1 of "Limitations and Open Problems" at the end of the book); any report using this section must state the window taken and its rationale.

**Third, $B^{\mathrm{env}}$ and $B^{\max}$ cannot be interchanged here.** A rarity computed relative to the equiprobable baseline answers "how special formally", not "how rare for this holder"; using it as the latter amounts to throwing away the habitat information altogether. Conversely, using $B^{\max}$ for cross-holder comparison means giving up the sense of "for whom". **These two things cannot both be done in the same passage.**

The model the holder has internally acquired is denoted $B_{\mathrm{int}}$; its gap from $B^{\mathrm{env}}$ is called the **decoding deviation**, a separate measurable that is not merged into $I$. For readings with frequency 0 in the habitat background, the discrete-outcome rarity tends to infinity; by convention Laplace smoothing is applied and recorded in the reading protocol. The smoothing parameter must be reported together with the sample size of $B^{\mathrm{env}}$; when the sample size is small, the effect of smoothing on the reading may exceed the reading itself, and one should then report "reading unreliable" rather than report a large number.

#### 12.9.5 Rule Three: Qualification, Mismatch, and Polarity

A reading is counted in $I$ only if it satisfies both: persistence relevance, and entry into the complete response chain

$$\xi \rightarrow D(\xi) \rightarrow a \rightarrow \mathrm{sv}.$$

Three cases follow: **relevant and decoded**, the starting point of the effective causal information chain that is normally read; **relevant but not decoded**, that is, a **decoding blind spot**, which is not counted in $I$ but should be recorded, because it shows that a persistence relation exists between the environment and the holder while the current decoder does not respond; **decoded but with no detectable effect on $\mathrm{sv}$**, that is, redundant processing or misreading — this is not inconsistent with the decoder's fourth qualification condition: that condition stipulates the causal capacity the holder type must possess, whereas what is described here is the case of a particular instance where one specific reading has no detectable persistence effect.

**Polarity** is determined by persistence gain. Let $a^{*}$ be the optimal response under reading $r$,

$$\delta_r = \mathbb{E}[\mathrm{sv}\mid r,\, a^{*}] - \mathbb{E}_{B^{\mathrm{env}}}[\mathrm{sv}]$$

$\delta_r>0$ is positive, $\delta_r<0$ is negative, and an absolute value within tolerance is recorded as 0 (masked). $\delta_r$ and rarity are two independent readings: rarity measures "how far it departs from the background", and $\delta_r$ measures "the direction and weight with respect to persistence." A background cue has low rarity and large $\delta_r$; this is the expected result and can be handled by low-cost solidified responses. Within the same holder, sign and strength can be compared in units of $\mathrm{sv}$; across holders they cannot be compared directly unless the decoder, background, observation window, and attribution protocol have been unified or calibrated.

"Low rarity but large $\delta_r$" — this combination refutes a common misconception: **that only what carries a large amount of information is important.** A background cue that is almost always present has rarity near zero and enormous importance; a string of random code has enormous rarity and zero importance. **Rarity and importance are two orthogonal dimensions; this book records them with two symbols, and neither may substitute for the other.** This is also what Chapter 7's "to know is not to obtain" means: knowing speaks to the rarity dimension, and obtaining speaks to the $\delta_r$ dimension.

![Figure R-2. The Orthogonal Plane of Rarity and Polarity](figures_en/release/fig_concept_rarity_polarity.pdf)

**Figure R-2. The Orthogonal Plane of Rarity and Polarity.** The horizontal axis distinguishes only low from high rarity, while the vertical axis distinguishes positive, zero, and negative polarity: background cue, rare and useful, common but harmful, rare misleading signal (HR-9), background noise, and rare but useless. This is a qualitative matrix without units or numerical coordinates; rarity is not relabelled as importance.

#### 12.9.6 Relation to Prior Work

The nearest prior work is Kolchinsky and Wolpert's semantic information (Interface Focus, 2018): they define "information that is causally necessary for the system to maintain its own persistence" as semantic information, tested by counterfactual interventions that scramble the correlation. The intervention test here is of the same kind, and **RIF does not claim that this test is original**. Several other directions are close: the value of information (Howard, 1966), rational inattention (Sims, 2003), the information bottleneck and relevant information (Tishby, Pereira & Bialek, 2000), pragmatic information (Weinberger, BioSystems 66(3), 2002), and Uexküll's concept of Umwelt; the rest are not elaborated.

RIF's advance on this basis is limited to three points, and nothing else is claimed: the holder is not limited to organisms and can be any persistent structure satisfying the four criteria, and the object of information $P$ can be an externally substrate-dependent PS (including a memetic PS) or the structure itself, and not only the holder's information about the environment; the cost side of the partition of readings is recorded in $E$, with the decoding cost paid by the holder itself, aligned with I–T–E; the background is explicitly separated into two conventions, and the gap between the externally measurable habitat background and the holder's internal model is listed separately as a measurable. The third point is this section's interface with the two background notations.

#### 12.9.7 Testable Predictions

This section gives four numbered predictions, with numbering continuing from Chapter 8; the test procedures and refutation conditions are listed uniformly in the table of falsifiable predictions at the end of the book ($H\mathrm{R}\text{-}4$ through $H\mathrm{R}\text{-}7$). Their shared testing dependency is that **$\delta_r$ can be determined independently**: if this cannot be done, none of the four is testable, and $\delta_r$ depends on how the "optimal response" is delimited.

#### 12.9.8 What This Section Does Not Claim, and Unresolved Problems

1. Does not claim that "maximizing rarity" is the holder's goal; such normative propositions are not elaborated.
2. For PSs that cannot be intervened on (historical figures, civilizations, institutions), this test has only conceptual meaning and no operability.
3. The "optimal response" depends on the delimitation of the response repertoire; together with the operationalization of the persistence-relevant time window, it is listed in items 1 and 3 of "Limitations and Open Problems" at the end of the book and is not repeated here.
4. Does not claim that $B^{\mathrm{env}}$ is "the only correct background". It is correct only for the question "how rare is this for a given holder"; for a different question, $B^{\max}$ is the correct one. The two coexist, each keeping to its own question.

### 12.10 Measurement-Layer Definitions of $T_{\mathrm{struct}}$ and $E_{\mathrm{struct}}$

The measurement-layer definitions of $T$ and $E$ are given here, so that all three quantities I–T–E can take values within RIF, with no viability-potential formula presupposed. Only "what to measure" is defined here, with no dynamics (who is more cost-effective, how things evolve).

**Intuitive meaning.** $T_{\mathrm{struct},D}(P)$ is the time span over which this set of structural readings, under a given decoder $D$, remains above the detection floor and is still recognized by $D$ as the same maintained structure. It refers to how long this structural information can still be read out by this decoder.

**Starting point and detection floor.** Let the measurement starting point be $t_0$. The decoder $D$ has a **detection floor** $\iota_D$: if the rarity of a reading is below it, $D$ cannot read out this reading. For an instrument, the rarity corresponding to its resolution limit is taken; for a biological decoder, the behavioral response threshold is taken, with the decoding-cost equivalent giving its lower bound. The operationalization protocol of $\iota_D$ belongs to later work (see item 2 of "Limitations and Open Problems" at the end of the book); how the response threshold of a cognitive decoder is stably converted into this floor is the step yet to be built.

$$T_{\mathrm{struct},D}(P)=\mu\Big(\big\{t\in W:\ I_{\mathrm{struct},D}(P;t)\ge \iota_D\ \text{and}\ P(t)\sim_D P(t_0)\big\}\Big)$$

Here $W\subseteq[t_0,\infty)$ is the observation window, and $\mu$ is a measure: within the observation window, the total length of time during which the reading of $P$ is above the detection floor and is still assigned by $D$, under the tolerance relation $\sim_D$, to the same identification class as the initial state; periods of recovery after an interruption are counted. The lifetime-type formulation takes the first continuous persistence time; when it has not terminated within the observation window, it is reported as a right-censored lower bound. Here $I_{\mathrm{struct},D}(P;t)$ denotes the reading at time $t$.

Background drift must be accounted for separately: if the reading uses $B^{\mathrm{env}}$, then when habitat frequencies change within the window, $I$ will change with them, and the condition "reading above the detection floor" must be recomputed at each moment, and cannot use the background of an initial moment throughout; if the reading uses $B^{\max}$, the background does not drift with the habitat, but changing protocol still makes before and after incomparable. **Both conventions run into problems in long windows, only in different ways.** The report must say which is used and whether drift was detected within the window.

$\sim_D$ is a tolerance relation, not a strict equivalence relation: "indistinguishable" under finite resolution is in general not transitive. Where strict equivalence classes are needed, a fixed partition is written into the reading protocol. The definition above compares only $P(t)$ with the initial $P(t_0)$ and does not depend on transitivity.

**The three thresholds belong to two sides and are not interchangeable.** The $\iota_D$ used in this section, the "two-object discrimination tolerance" required for identity judgment, and the structural maintenance floor $I_{\mathrm{min}}$ registered in Appendix A answer three different questions:

| Threshold | Side | Question answered | Reading |
| :--- | :--- | :--- | :--- |
| $\iota_D$: reading detection floor | reader | can a single reading be detected against the background | $I_{\mathrm{struct},D}<\iota_D$: $D$ cannot read it, $T$ cannot be delimited; not equivalent to structural collapse |
| two-object discrimination tolerance | reader | can the readings of two candidate objects be told apart | difference within tolerance: this protocol cannot distinguish; not equivalent to the two objects being identical |
| $I_{\mathrm{min}}$: structural maintenance floor | structure | does the structure's own informational organization still reach the floor for maintaining identity | $I_{\mathrm{struct}}<I_{\mathrm{min}}$: the structural-side condition fails; not a reading failure |

The second item in the table is not a parameter already defined in this book. If it is to be written with the symbol $\varepsilon_D$, it must be registered in Appendix A and declared to be a **newly added reader-side operating parameter**: set before data are taken, not interchangeable with $\iota_D$, and not to be used in place of $I_{\mathrm{min}}$. Where it is not registered, only the words "two-object discrimination tolerance" are used.

The reason the three are not interchangeable is direct: $\iota_D$ asks "is a single reading bright enough", the tolerance asks "can two readings be told apart", and $I_{\mathrm{min}}$ asks "does the structure itself still hold up". Any two of them happening to be equal is an accident in some object domain, not a definition.

**A one-way implication.** By the definition of this section, $\iota_D$ being fixed and $P(t)\sim_D P(t_0)$ being decidable within $W$ suffice to measure $T_{\mathrm{struct},D}$ by definition; neither requires $I_{\mathrm{min}}$ to be calibrated first, nor the two-object discrimination tolerance to be fixed first. Conversely, $T$ being measurable does not imply that the object retains its identity within $W$ — that needs another set of criteria and is not given by this section.

**Special upper-limit case.** When $D=D_{\mathrm{macro}}$, $\iota_D\to 0$, and the upper limit of persistence is bounded by thermodynamic stability, an upper-limit estimate of objective physical persistence time can be obtained. The general definition of this section still goes by the identification relation of the given decoder; the identification relation itself is not equivalent to structural continuity. "Can be read out convergently by multiple decoders" is a property of the special case $D=D_{\mathrm{macro}}$ and does not belong to the general definition: the general definition requires only that it hold relative to a single $D$.

**$E_{\mathrm{struct},D}(P)$** is the actual energy cost (J) attributed to keeping $P$'s structural reading above $\iota_D$ during $T_{\mathrm{struct},D}(P)$, including the one-time freezing/formation cost apportioned for the passive phase by explicit rules, and the free energy continually input in the active phase. There are four disciplines here.

- Only the structural maintenance cost attributable to $P$ is counted. The energy paid by a holder that reads, processes, and continually identifies $P$'s causal effect is recorded separately as $E_{\mathrm{causal}}$, and is not merged into the structural cost because it helps maintain that effect; an instrument used only for measurement is not a holder, and its energy consumption is not counted.
- If $P$ and the decoder holder coincide physically or share an energy source, structural maintenance and causal processing must be separated by operation-level metering or a verifiable incremental-cost protocol. The same energy consumption may not be counted in full in both items; when it cannot be apportioned reliably, mark the sub-item as unidentifiable and do not give a total cost obtained by adding.
- Structural information and causal information each form an I–T–E record, and this book does not by default add $E_{\mathrm{struct}}$ and $E_{\mathrm{causal}}$; the decoding cost is assigned to $E_{\mathrm{causal}}$ (the combined item of reading, processing, and identification), so $E_{\mathrm{eff}}=E_{\mathrm{struct}}+E_{\mathrm{causal}}$ closes within this framework; $E$ is only a superordinate notation, and any composite formula quoted from external literature must state its item boundaries. If the research question requires a total, the accounting scope (covering $P$, the holder, or both) and the de-duplication rule must first be declared.
- In this book $E_{\mathrm{struct}}$ takes the energy actually paid. If another model uses a theoretical minimum overhead, it should be marked separately and cannot be mixed directly with this book's measured quantities.

**Measurement steps.** In addition to the basic four steps: after $t_0$, measure repeatedly and record the reading trajectory until the reading falls below $\iota_D$ or the identification relation breaks; measure $E_{\mathrm{struct}}$ by $D_{\mathrm{macro}}$ protocols such as calorimetry and power integration. When $T_{\mathrm{struct}}$ exceeds the observation period, it can only be extrapolated with a decay model and must be marked as inferred.

**This section defines only "how long it is read", not "whether it is the same one".** The pairing of readings, the cross-time identity of a structure, and the distinguishability of records across objects are three different things:

1. **Boundary measurable**: all three I–T–E items hold on a candidate boundary (§12.8);
2. **Cross-time identity**: the structure satisfies $P(t)\sim_D P(t_0)$ throughout $W$ (the condition of this section; $\sim_D$ is not transitive, so it is not written as "the same identification class");
3. **Record distinguishable**: different objects do not share the same triplet record (not yet determined).

The three cannot be chained into a proven derivation: pairing holding does not entail cross-time identity, and cross-time identity does not entail record distinguishability. Nor can one claim in reverse that the three are mutually independent — that likewise requires proof. Whenever readings from this section are used to discuss "the same object", one must specify which of the three is meant.

### 12.11 An End-to-End Worked Example: A Storage Array (Illustrative)

$N$ bistable cells are written all 0; the reading is the number $k$ of cells flipped to 1, with fewer being more ordered; structural information uses ordered tail-probability rarity. When the flip fraction is $x=k/N$, for large $N$ the amount of information is approximately $N\,[1-h_2(x)]$ ($h_2$ is the binary entropy). The background takes the protocol baseline $B^{\max}$ (cells equiprobable and independent), because the array has no designated holder; if one switched to the $B^{\mathrm{env}}$ of some holder's habitat, the natural frequency of "all 0" might be very high, and the initial rarity would be markedly lower than $N$ bit — **all numerical values of this example hold only under $B^{\max}$.**

Each cell flips independently and symmetrically at rate $\lambda_{\mathrm{flip}}=\tau_0^{-1}e^{-\Delta U_{\mathrm{barrier}}/(k_B T_{\mathrm{thermo}})}$, and the expected flip fraction is $\tfrac12(1-e^{-2\lambda_{\mathrm{flip}} t})$. The detection floor is taken as $N/2$ bit, corresponding to $x\le0.110$, and the threshold-crossing time of the expected trajectory is approximately $0.124/\lambda_{\mathrm{flip}}$ (taking $\tau_0=10^{-12}\,\mathrm{s}$): about 8 hours at a barrier of $40\,k_B T_{\mathrm{thermo}}$, and about $4.5\times10^{5}$ years at $60\,k_B T_{\mathrm{thermo}}$. This is the model-predicted crossing time, not a measured persistence time. The array has no holder reading it out, and the causal information is 0. This example involves only $I_{\mathrm{struct}}$; its detection floor is set by the protocol and does not appeal to $\iota_D$.

**How to read it.** This example demonstrates three things: $I$ can be computed from a definite reading rule without depending on dynamics; $T$ can be derived from a definite physical rate, but that is a predicted crossing time; and $E$ is **missing** here — $\Delta U_{\mathrm{barrier}}$ determines only the rate and is not equal to the energy paid. The third is the most important: **in practice, I, T, and E often cannot all be in place at once.** When an item is missing, one should mark "$E$ unavailable" rather than pass off the barrier height as the energy cost.

***

## Chapter 13 — Causal Rarity: The Second Source of Information

### 13.1 Definition

Structural rarity describes how rare the arrangement of the object itself is relative to the background; this chapter treats another kind of information: **what effect an instance produces on other objects, and how rare this effect is relative to the control baseline.**

$$I_{\mathrm{causal},D}(P) = -\log_2 \Pr_{B_0}\big(s(e') \ge s(e_{\mathrm{obs}})\big)$$

The protocol-declaration rule is the same as for structural information: when the effect has a natural order (response strength, probability, delay), ordered tail-probability rarity is used by default, $s$ being the ordered statistic of the effect, with $\ge$ for larger values being more extreme and $\le$ for smaller values being more extreme, the direction registered in advance; when the effect is a discrete category, use $-\log_2\Pr_{B_0}(e=e_{\mathrm{obs}})$; for distribution-level comparison use relative entropy.

- $P$: **whom this information speaks of**; it can be any persistent structure instance, not required to be alive or to have a self-maintained boundary.
- $D$: the decoder that reads out the effect; $e_{\mathrm{obs}}$ is the observable effect, that is, a behavioral change of $D$'s holder or a measurable change in energy flow.
- The decoder holder of $D$: a persistent structure that owns or runs $D$, pays the decoding cost, and is changed by the decoded information, which must have an identifiable boundary maintained by its own organization; an instrument or reference framework that merely carries out the reading does not thereby become a holder.
- $B_0$: the **control baseline**, the distribution of effects $D$ observes when $P$ is replaced by an "equivalent of the same material but lacking that rule or that identification"; determined jointly by $D$ and $P$, and written $B_0(D,P)$ when emphasis is needed.

**The information speaks of $P$, and the decoding cost is spent on the decoder holder; these are two independent questions, and the answers can differ.**

$I_{\mathrm{causal},D}(P)$ belongs to causal information together with $T_{\mathrm{causal}}$ and $E_{\mathrm{causal}}$ of that causal channel. $T_{\mathrm{causal}}$ answers "how long does this effect actually last", unrelated to who the decoder holder is or whether it is replaced — as long as some decoder holder is still observing the effect and paying the decoding cost, this causal channel has not gone to zero.

One approach that easily arises is to draw conclusions directly from the tail probability: "when the effect falls within the typical range of the control baseline (tail probability approximately greater than $1/2$), $I_{\mathrm{causal},D}(P)\lesssim 1$ bit, regarded as no difference." This conflates a descriptive statistic with a statistical-inference conclusion: **"large tail probability" is the former, "no difference" is the latter.** The judgment needs three things — a bound for "how large counts as present", an interval for "how credible this bound is", and a test rule stated in advance; lacking these three, it is only a heuristic.

This book adopts a formal two-step structure: **step one, identify the effect** — use a control design to decide "after replacing with the control object, is the effect different", giving a statistical conclusion with confounder control, multiple-comparison correction, and pre-registered thresholds; **step two, report the rarity** — only after the existence of a discernible effect is confirmed is $-\log_2\Pr_{B_0}$ used to report how rare this effect is, with an interval estimate. The reason is practical: **if step one is wrong, no precision in step two is meaningful.** A "rare effect" not confirmed by a control design may well be only a confounder, a chance occurrence among many comparisons, or a bias in the control baseline itself.

**Worked example (the numbers are hypothetical)**: when the decoder holder is a recognizer (a dog), the control is a stimulus control — replacing "the owner's voice" with "a stranger's voice", with the conclusion interpreted as "whether that voice is recognized". The proportion of stranger recordings that elicit from the dog a reaction of equal or greater strength to that for "recognizing the owner" (ordered tail probability) is taken as 1/100 in this example, constituting $B_0$. After the owner's recording is played, the dog does produce this reaction:

$$I_{\mathrm{causal},D_{\mathrm{dog}}}(P_{\mathrm{owner\ voice}}) = -\log_2(1/100) \approx 6.6\ \text{bits}$$

Here the holder of $D_{\mathrm{dog}}$ is the dog itself; this information speaks of $P$, "the owner's voice". If a stranger's recording could also elicit a reaction of the same strength with the same probability, the two fall in the same $B_0$ distribution, there is no counterfactual difference, and this entry is classed as an ordinary reaction. Complex cases (such as the influence of historical figures) have only a conceptual definition at present, with weak operability, because $B_0$ is hard to construct.

### 13.2 Two Sources

The control baseline can be taken in two ways, depending on who the decoder holder is.

| | Decoder holder is the maker | Decoder holder is the recognizer |
| :---------- | :------------------------- | :---------------------- |
| Control object | Same material, but formed by a **natural process without selective intervention** | One of before-after control, between-subjects control, or stimulus control, declared in advance |
| Examples | A watch's maker versus a block of metal of the same material; the maker of doped semiconductors versus natural silicon | The person who treasures a pebble; the person who regards a meteorite as an auspicious omen |
| Threshold cost evidence | Construction cost (recorded as $E_{\mathrm{build}}$) | Responsive expenditure such as purchase and special preservation |
| $E_{\mathrm{causal}}$ | The decoding cost for each holder to read out the effect | Same as left |

Three kinds of control: before-after control refers to the same holder's reactions to the same $P$ before and after the identification relation is established; between-subjects control refers to comparison with holders of the same kind who have not established the identification relation; stimulus control refers to the same holder's reaction to similar but unrelated stimuli. Whichever is used, confounding variables and baseline comparability must be explained. When one object has multiple holders, each holder's $E_{\mathrm{causal}}$ is measured separately, and aggregation must declare the sampling frame and the de-duplication rule.

The probability of a configuration like a watch appearing in a natural process without selective intervention is extremely low, so a "same-material equivalent formed by natural processes" can serve as the control object. "Artificial" means exactly this, not "violating the laws of physics".

### 13.3 Entry Conditions: Identify the Effect First, Report the Reading After

For an effect to be counted in $I_{\mathrm{causal},D}(P)>0$, it must satisfy three admission conditions at once and pass the two-step determination. The three admission conditions themselves have not changed, but each must now be landed on a concrete act of determination.

1. **Counterfactual difference**: when replaced by the control object, the effect is significantly different; otherwise it is an ordinary physical reaction. "Significantly" is given by the control design below.
2. **Observable**: the effect shows up as a measurable change in behavior or energy flow, for example purchasing, special preservation, changing a decision accordingly, a calorie shift; merely "feeling meaningful" does not count.
3. **Cost paid**: the decoder holder itself pays a measurable cost, to prevent arbitrary score-adding. The "cost" here is evidence for the qualification threshold, and may include responsive expenditures such as purchase, special preservation, and construction cost; among these, the decoding cost for the holder to read out the effect is what is counted in $E_{\mathrm{causal}}$.

**The threshold is any single decoder holder**; a majority is not needed, nor is consensus. A dog recognizing a recording is an independently valid entry, counted on that dog. But "any one suffices" speaks of **qualification**, not **credibility**: when a single holder's reading qualifies, the numerical reliability still depends on how rigorous its control design is.

#### 13.3.1 Step One: Identify the Effect with a Control Design

This step answers only one question: **after replacing with the control object, is the effect really different?** It does not answer "how rare", nor "how significant".

**(1) Design.** Choose one of the three controls and state before data are taken: the composition of the treatment and control groups, the sample size per group, the randomization or matching method, and the list of main confounding variables. For before-after control, state whether any other change occurs between "before" and "after"; for between-subjects control, state how the two groups are matched; for stimulus control, state on which dimensions the control stimulus and the target stimulus are matched (intensity, duration, mode of presentation) and on which they must differ.

**(2) Confounder control.** Three kinds of confounding must be handled separately, and cannot be dispatched with a single remark that "randomization should have taken care of it."

- **Object-side confounding**: the target $P$ and the control object $P_0$ differ in other ways besides "that rule or that identification". Control: match material, size, and conditions of presentation; where matching is impossible, include these differences in the model as covariates and report the effect size.
- **Holder-side confounding**: the holders in the treatment and control groups differ in state, experience, and attention. Control: within-holder comparison (before-after and stimulus controls take priority), or stratified randomization of holders.
- **Time-side confounding**: the change in effect is mixed with the change of time itself (adaptation, fatigue, learning, external events). Control: add a placebo or empty-treatment group, or use a crossover design.

**(3) Multiple-comparison correction.** If $m$ effects are tested in the same study, correction is required, and the method must be stated.

- By default use the **Holm step-down method** to control the family-wise error rate $\mathrm{FWER}\le\alpha_0$; when the sample is small and the correlation among tests is strong, **Bonferroni** (more conservative) may be used.
- If the design is "a single pre-registered primary effect plus several exploratory effects", the primary effect need not be corrected, but it must be stated explicitly that "there is only one primary effect", and exploratory effects are always marked "uncorrected, for hypothesis generation only."
- What is corrected is the **family of tests**, and the boundary of the family must be fixed before data are taken. Moving non-significant tests out of the family after the fact, or moving significant tests into it, are invalid operations.

**(4) Pre-registered threshold.** $\alpha_0$ is registered before data are taken, by default $0.05$; for high-stakes judgments or where stronger evidence is needed, $0.01$. The pre-registered content includes: the list of primary effects, $\alpha_0$, the correction method, the basis for sample size (power analysis or precision target), and the stopping rule (a fixed sample size, or the bounds of a sequential design).

**(5) Output.** The output of this step is: the point estimate of the effect size, the $95\%$ confidence interval, the test statistic, the degrees of freedom or number of resamples, and the corrected $p$ value. **A result with a point estimate but no interval is not enough to support any subsequent rarity report** — because step two must carry this uncertainty forward.

#### 13.3.2 Step Two: Report the Rarity Reading and Its Uncertainty

Only after step one confirms the existence of a discernible effect is the following computed in step two

$$I_{\mathrm{causal},D}(P) = -\log_2 \Pr_{B_0}\big(s(e') \ge s(e_{\mathrm{obs}})\big)$$

and its uncertainty reported at the same time. **$B_0$ is the distribution of the same statistic under control, not "the distribution of raw responses."** If $e_{\mathrm{obs}}$ is the **mean** of $n$ observations, $B_0$ must be "the distribution of means in the control group"; only if $e_{\mathrm{obs}}$ is a **single response** is $B_0$ "the control response distribution". The two must not be mixed: mixing them would systematically depress $I_{\mathrm{causal}}$ by about $\tfrac12\log_2n$ bit, and would make the 1-bit benchmark of §12.1 no longer applicable — in a zero-effect world, using the wrong convention makes $\Pr(I\ge3)$ fall from the order of $1/8$ to undetectable (Appendix C, Table C-4). The report must state the type of statistic of $e_{\mathrm{obs}}$. The following items must be stated.

**(1) Confidence level.** Default $95\%$; if step one used $\alpha_0=0.01$, the step-two interval also takes $99\%$, keeping the stringency of the two steps consistent. A patchwork such as "a wide threshold in step one and a narrow interval in step two" is not allowed.

**(2) Estimation method.** Three are commonly used: the **parametric method** assumes $B_0$ belongs to some parametric family, computes the tail probability from the fitted parameters, and propagates the interval by the delta method; it applies where the sample size is adequate and the model is testable, and goodness of fit must be reported; the **resampling method** performs a bootstrap on the control sample (BCa correction recommended), recomputes the tail probability after each resample and takes quantiles; it applies where the distribution shape is unknown, and the number of resamples (at least 2000 recommended) and whether degeneracy occurs must be reported; the **exact method** is for discrete categories with small samples, and the tail probability and interval can be computed directly from the exact binomial or the permutation distribution.

**(3) Conversion of the interval onto the rarity scale.** The tail probability $p$ and the rarity $I=-\log_2 p$ are related by a monotonically decreasing transformation; substituting the endpoints of the interval of $p$ gives the interval of $I$, but **the endpoints must be swapped**: the lower bound of $p$ corresponds to the upper bound of $I$. This step seems trivial but is the most common source of error — many reports write the interval of $p$ directly as the interval of $I$.

The recommended report format is a single line: $I_{\mathrm{causal}} = 6.6\ \text{bit}$, $95\%$ CI $[4.3,\,9.1]$, tail probability $p_{\mathrm{tail}}=0.010$, $95\%$ CI $[0.0018,\,0.051]$, method: control sample $n=100$, BCa bootstrap $5000$ times. **A reading with only a point value and no interval or method is treated as an unfinished measurement: it can be reported, but does not enter summaries or comparisons.**

**(4) The tail probability is not the test $p$ value.** $p_{\mathrm{tail}}$ says "where the observed effect lies in the control distribution"; the test $p$ value says "under the null hypothesis, the probability of observing a difference this large (or larger)." The two are numerically close for a single observation when the control distribution is the null distribution, but differ in general designs: the former varies with the shape of the tail of the control distribution, the latter with sample size and test statistic. **To take $p_{\mathrm{tail}}$ for significance, or the test $p$ value for rarity, is wrong.**

#### 13.3.3 Equivalence Testing and the Entry Threshold

"A tail probability approximately greater than $1/2$ means no substantive difference" is a heuristic and cannot replace an equivalence test. The reason: **"no difference" is a conclusion that needs to be proven, and cannot be inferred from "no difference was detected."** The latter says only that the evidence is insufficient; the former requires evidence sufficient to rule out a meaningful difference.

**(1) Equivalence bound $\delta_{\mathrm{eq}}$.** On the scale of effect size (difference in response probability, standardized mean difference $d$, or difference in delay), declare in advance a bound $\delta_{\mathrm{eq}}>0$: **when the absolute value of the effect does not exceed $\delta_{\mathrm{eq}}$, it is regarded as no substantive difference.** This bound cannot be set by the data; it must be set by domain knowledge or by the consequences of the decision, and registered before data are taken. Where there is no prior basis, $0.2$ may be provisionally used (the convention for a small effect in standardized mean difference), but it must be marked "conventional value, not domain-based".

**(2) Test rule.** Use two one-sided tests: let the $95\%$ confidence interval of the effect be $[L,U]$.

- If $L>-\delta_{\mathrm{eq}}$ and $U<+\delta_{\mathrm{eq}}$, judge **equivalent** (no substantive difference), not counted in $I_{\mathrm{causal}}$, recorded only as an ordinary physical reaction;
- If $[L,U]$ does not intersect $[-\delta_{\mathrm{eq}},+\delta_{\mathrm{eq}}]$, judge that **a substantive difference exists** and proceed to step two to report rarity;
- In the remaining cases judge **uncertain**, report as "insufficient evidence", and it may be written neither as "no difference" nor as "a difference".

All three conclusions must be able to occur. A test that allows only two conclusions amounts to quietly counting "uncertain" toward one side.

**(3) The correspondence of the equivalence band on the rarity scale.** If an effect falls within the equivalence bound, this corresponds, on the tail probability, to a band $|p_{\mathrm{tail}}-1/2|\le q$. Taking $q$ as the tail-probability offset obtained by mapping $\delta_{\mathrm{eq}}$ through $B_0$, the equivalence band on the rarity scale is approximately

$$I\in\big[\,1-\log_2(1+2q),\ \ 1-\log_2(1-2q)\,\big]\ \text{bit},$$

for small $q$ approximately $1\pm2.885q$ bit, and this linear approximation is adequate only for $q\lesssim0.05$. The exact conversion is $[-\log_2(0.5+q),\,-\log_2(0.5-q)]$: $q=0.05$ gives $[0.8625,\,1.1520]$ (the deviation of the approximation $1\pm0.14$ is about 0.007 bit), and $q=0.10$ gives $[0.7370,\,1.3219]$ (the deviation of the approximation $1\pm0.29$ is about 0.03 bit). **"Near 1 bit" is indeed the image of "no substantive difference" on the rarity scale, but how wide "near" is depends on $\delta_{\mathrm{eq}}$.**

**(4) Entry threshold.** For an effect to enter the summary as a qualifying causal reading, it must satisfy at once: in step one, the corrected $p\le\alpha_0$ (default $0.05$) and the effect-size interval does not overlap the equivalence band; in step two, $I_{\mathrm{causal}}\ge3$ bit (corresponding to $p_{\mathrm{tail}}\le1/8$) — **admitted on the point estimate**; its confidence interval is reported at the same time, and if the interval's lower bound is below $1$ bit, mark "reading unreliable". **The lower bound is for reliability marking, not for admission.**

> **The threshold and the confidence level are two independent parameters.** Writing "3 bit with the 95% lower bound holding" in a single sentence while giving only one number lets the actual threshold slide above $6$ bit: when the true value is exactly 3 bit, increasing the sample size from 50 to 1200, the pass rate never reaches $0.5$; the effective threshold is 7.2 bit at $n=50$ and still 6.0 bit at $n=500$ (Appendix C, Table C-4, Figure C.5). If admission by the lower bound is really wanted, the threshold must be written separately as "95% lower bound $\ge6$ bit", with an explanation that this requires effects of the order of $p_{\mathrm{tail}}\lesssim10^{-2}$ and the corresponding lower limit on sample size.

**Why 3 bit.** 3 bit corresponds to $p_{\mathrm{tail}}=1/8$, a somewhat conservative entry value: it excludes effects of the common degree of "one in four", without shutting out all genuine effects of moderate strength. For high-stakes judgments, raising it to $5$ bit ($p_{\mathrm{tail}}\le1/32$) is recommended. These two numbers are **conventions**, not natural constants. **The threshold can be negotiated; the interval cannot be omitted.**

### 13.4 Effects of Different Decoder Holders Are Computed Separately and Not Added

The effects on the maker's side and on the recognizer's side are two independent $I_{\mathrm{causal},D}(P)$, with different $D$, and are **not added**, because the party paying the energy differs.

| $P$ | Maker's side | Recognizer's side | Note |
| :-------------- | :------------ | :--------- | :--------------------- |
| Metal block of the same material (naturally formed) | 0 | 0 | Only $I_{\mathrm{struct}}$ |
| Watch | High | High | Effects exist on both the maker's and the user's side |
| A treasured pebble | 0 | >0 | Only the recognizer's side |
| A meteorite taken as an auspicious omen | 0 | Possibly large | The size depends on the resources the recognizers pay, such as building temples and holding sacrifices |
| Jackson, still recognized after death | Deceased, cannot go on paying costs | High (fans still paying) | $P_{\mathrm{Jackson}}$ is not required to be alive; the decoder holders are the living fans |

**$P$ itself is not required to have a boundary. What requires a boundary is the decoder holder.** $P$ holds no effect; the effect always lands on some decoder holder, only that this information content is attributed to $P$.

**With multiple holders, report holder by holder.** When the same $P$ faces $n$ holders ($n\ge2$), this book requires first producing a **holder-level reading table**, one row per holder, with columns: holder identifier, its decoder $D_i$, control design type, the point estimate and interval of $I_{\mathrm{causal},D_i}$, $T_{\mathrm{causal},D_i}$, $E_{\mathrm{causal},D_i}$, and evidence level. This table is itself a complete measurement result.

**Four explicit declarations for aggregation.** Aggregation is allowed only after all four of the following have been established; if any one is missing, give the holder-level reading table and not a single composite value.

1. **Composite boundary**: state which parts of which $P$ the aggregation covers. Several holders may read different sides of the same $P$ (a private doctor reads the body, fans read the image, a court reads the legal identity); adding them together amounts to treating three different $P$ as one.
2. **Holder set**: state which holders are included and on what basis; with a different set, the aggregate value differs, so the set must be reproducible.
3. **Same-window condition**: state whether each holder's $T_{\mathrm{causal}}$ was measured within the same observation window $W$; where windows differ, they must first be aligned or reported by window.
4. **De-duplication rule**: state whether the same physical expenditure is counted repeatedly in $E_{\mathrm{causal}}$ by multiple holders. Typical cases: an institution pays the decoding cost once and multiple members share the reading; or a platform bears all the inference costs while end users have zero marginal cost.

Once all four are in place, aggregation can still only be a **declared composite quantity**, and one must at the same time report: each holder's original value, the weights or rules used in the aggregation, and the sensitivity of the aggregate to changes in the rules. **If the sensitivity is large enough to change the direction of a conclusion, the aggregate value is unusable.**

**Handling when it cannot be established.** If any one of the four cannot be established (most commonly item 4: shared costs cannot be apportioned), this book's treatment is explicit:

> Give no single composite reading, only the holder-level reading table; state in the report "because of ..., composite accounting cannot be established, and no composite value is provided this time."

A word on $V_{\mathrm{c}}$. This book does not define $V_{\mathrm{c}}$, nor any viability potential; but if a later model wants to use this book's readings to construct a cross-holder composite scalar (whether it is called $V_{\mathrm{c}}$ or by another name), it is likewise bound by this section: **without a composite boundary, holder set, same-window condition, and de-duplication rule, there is no such composite scalar.** This is not an overreach into another model's business — four numbers with no common reference cannot be added into a number that has one.

***

### 13.5 Variation with the Decoder Holder

For the same $P$, $I_{\mathrm{causal},D}(P)$ differs across eras and across holders. A meteorite in the eyes of the ancients and a meteorite in the eyes of today's scientists are two different entries of effect. This is a direct result of "information is a relational quantity".

**Trajectory.** As time advances, $I_{\mathrm{causal}}$ may trace a trajectory — rising (Kafka, Van Gogh: the background of the holder population could identify the counterfactual difference only later) or falling (da Vinci's technique: the background of the holder population gradually assimilated it as part of expectation). This trajectory belongs to the object of dynamical study; this book's measurement protocol defines only a single-point reading at a given moment and for given holders, and does not directly prescribe the dynamics of the trajectory.

The reason for the change in trajectory is that the background is changing, not the object. Not a word of Kafka's works has been changed; what has changed is the control baseline of the reader population: back then there was no control object for "this kind of writing", and now there is, so the counterfactual difference is read out. The trajectory is the image of "$B_0$ evolving with the holder population", not an attribute curve of the object itself: to predict the trajectory, what must be predicted is the update rate of the reference class, not the decay rate of the object.

**Two kinds of legitimate comparison.** A numerical comparison is meaningful only when the decoder, background, and reading protocol are consistent. So "whose $I_{\mathrm{causal}}$ is greater, Li Bai's or Trump's" has no answer in itself; one must first ask: for whom?

**Change the holder, same $P$**: for most Chinese readers, Li Bai's natural reference class is "everyone who writes ancient-style poetry"; only the rarity that still stably wins after removing short-term noise such as dynasty-by-dynasty promotion and decoding costs paid by proxy is his $I_{\mathrm{causal}}$ for this kind of holder. For most American readers, Trump's reference class is "American citizens"; they acknowledge his influence but often treat him as a neighbor-style public figure who may be openly discussed.

**Same holder, different $P$**: for a parent, their own two-year-old's scribble is usually rarer than *Sunflowers*, a work known by great reputation yet leaving them unmoved. Such ordering is a legitimate comparison, because the holder is the same.

**Determination of the reference class.** How the reference class is determined by viability resolution — its protocol belongs to later work (see item 4 of "Limitations and Open Problems" at the end of the book). The reference classes above are specified by the modeler, and by the usage rules of the two backgrounds should be marked as "modeler-specified background", and may not be compared side by side with readings computed under $B^{\mathrm{env}}$ — it is neither a habitat background nor a protocol baseline. The examples of this section demonstrate the **form of a legitimate comparison**; to make it a measurement, what is missing is exactly the step of the reference-class protocol.

### 13.6 Measurement Steps

1. Specify the decoder holder and its decoder $D$;
2. Specify $P$ and the control object $P_0$, and declare the control type (before-after, between-subjects, or stimulus control);
3. **Step one (identify the effect)**: carry out the control design, control confounders, correct for multiple comparisons, and test with the pre-registered $\alpha_0$; output the effect size, interval, corrected $p$ value, and sample size;
4. Conduct the equivalence test (two one-sided tests, $\delta_{\mathrm{eq}}$ registered in advance): equivalent is recorded as zero, uncertain is recorded as "insufficient evidence", and a substantive difference proceeds to the next step;
5. **Step two (report the rarity)**: observe the distribution of effects when $D$ faces $P_0$ to obtain $B_0$; observe the effect $e_{\mathrm{obs}}$ when facing $P$; compute $-\log_2\Pr_{B_0}(s(e')\ge s(e_{\mathrm{obs}}))$ and give an interval (stating the confidence level and method);
6. Check the three admission conditions; record $T_{\mathrm{causal}}$ and $E_{\mathrm{causal}}$, or mark them unavailable.

Step 4 is the one most easily skipped. The consequence of skipping it is that every effect for which "no difference was detected" will by default enter step 5 and have computed for it a rarity that is neither high nor low (close to 1 bit), and then be recorded as "having some amount of information". The equivalence test is set up precisely to block this: it separates "not enough evidence" from "equivalent" and gives an executable action. The action now is: equivalent is recorded as zero, uncertain is recorded as "insufficient evidence", and neither enters step 5.

### 13.7 Scope and Unresolved Problems

1. **Joint attribution**: how to distribute among several $P$ an effect to which they jointly contribute; the allocation rule belongs to later work.
2. **Whether identification really occurred**: a dog's bark may merely be startled by a sudden sound. One needs to compare the distributions of effects when the target object and the control object are present, to avoid mistaking coincidence for causal action.
3. **Aggregation of effects across multiple holders**: how different holders' contributions and costs to the same effect are de-duplicated, weighted, and normalized — the aggregation rules await calibration; without the four explicit declarations, no aggregation into a single value.
4. **Out of scope**: black-hole information, dark-energy information, and other parts that cannot presently be read physically; this is the boundary of instrument capability, not a loophole in the definition.
5. **When the origin of $P$ is uncertain**: when it is not known whether there is truly a maker, the maker-side effect is recorded as "pending", presupposed neither zero nor high; it can be expressed by a posterior probability of origin, the manner of expression to be specified.

This chapter has two numbered predictions: $H\mathrm{R}\text{-}8$ concerns that the trajectory is determined by the update rate of the reference class, and $H\mathrm{R}\text{-}9$ concerns that the combination "high $I_{\mathrm{pragmatic}}$ and $\delta_r<0$" is reproducible; the test procedures and refutation conditions are listed in the table of falsifiable predictions at the end of the book. $H\mathrm{R}\text{-}9$ is "conditionally testable": it depends on the measurability of $I_{\mathrm{pragmatic}}$.

### 13.8 Measurement-Layer Definitions of $T_{\mathrm{causal}}$ and $E_{\mathrm{causal}}$

These two quantities must be reported for the same effect, the same holder, and the same observation window.

**Intuitive meaning.** $T_{\mathrm{causal},D}(P)$ is: whether there is still any holder that can distinguish this causal effect from the control object, produce an observable response, and pay a measurable cost for it. It refers to how long this causal effect can still be tracked continuously by any holder.

Let $\Gamma_D(P,t)=1$ denote that at time $t$, the target effect has an identifiable counterfactual difference relative to the control object, produces an observable response, and the designated holder has paid a measurable cost to identify or respond to the effect; all three must hold at once.

$$T_{\mathrm{causal},D}(P)=\mu\Big(\big\{\,t\in W:\ \Gamma_D(P,t)=1\,\big\}\Big)$$

where $\mu(\cdot)$ denotes the measure (total length) of that time set within the observation window $W$; periods of recovery after an interruption are counted, the lifetime-type formulation takes the first continuous period, and when it has not terminated within the observation window it is reported as a right-censored lower bound. For a single holder, the resulting time is the total duration during which all three conditions hold at once.

- Different holders are recorded separately and not added directly. Persistence at the channel level takes the **union** of the holders' time sets: as long as any holder still satisfies all three conditions, the channel has not gone to zero. Note that the union is used only to describe whether the channel is still running; anything paired with $E_{\mathrm{causal}}$, or used in synthesizing any viability efficiency, always takes the $T_{\mathrm{causal}}$ of a **single holder**, and may not use the union.
- Confucius's thought still being invoked is this case: as long as some holder can still distinguish the relevant causal effect from the control object, produce an observable response, and pay a measurable cost for it, that causal channel has not yet gone to zero.

**$E_{\mathrm{causal},D}(P)$** is the **measurable decoding cost** that a holder pays, within the above time set, to continually read out and identify this effect, in J. There are three disciplines here.

- The "measurable cost" in the admission conditions for causal readings has a broader evidence scope than the energy reading of $E_{\mathrm{causal}}$, and may include responsive expenditures such as purchase and special preservation. These serve only as evidence for the qualification threshold and are **not counted directly in $E_{\mathrm{causal}}$**.
- If a researcher wishes to combine the overheads of the target object and the holder into one total cost, a composite accounting boundary must be declared additionally; this total does not belong to RIF's default I–T–E definition.

- The basic definition of $E_{\mathrm{causal}}$ is the measurable decoding energy consumption, attributed to the designated holder within the specified observation window. RIF prescribes no universal internal decomposition; a specific model may define sub-items such as computation, refresh, or error correction by function, but must declare the object and holder boundaries, the observation window, and the attribution rule, and ensure that the sub-items do not overlap and sum to no more than the total. The holder's entire basal metabolism, the host's entire operating energy consumption, and behavioral expenditures such as purchase or preservation may not be counted in full automatically; only the part brought in through an explicit attribution or conversion protocol is counted. If the same physical energy consumption supports both structural maintenance and causal readout, it must be apportioned by function or incremental cost; when it cannot be apportioned, it may not be counted in full in both items at once.

### 13.9 A Candidate Operationalization at the Decision Layer: Information Gain of the Action Distribution

**Hypothesis**: **This section gives the candidate operationalization $I_{\mathrm{pragmatic}}$, which does not replace the definition of $I_{\mathrm{causal}}$.**

**Gap.** $I_{\mathrm{causal}}$ measures the rarity of an effect, the three conditions decide whether that effect qualifies as a causal reading, and $\delta_r$ is the after-the-fact reading of persistence gain. Missing among the three is a **before-the-fact, continuous, directly behavior-observable** strength reading: to what extent a reading changes the holder's actions.

**Candidate definition.** Let the holder's action distribution before reading $r$ be $q_D(a)$ and after reading be $p_D(a\mid r)$; then

$$I_{\mathrm{pragmatic}}(r;D)=D_{\mathrm{KL}}\big(p_D(a\mid r)\,\|\,q_D(a)\big)$$

in bit. If a reading fully conforms to expectation, the action distribution is unchanged and $I_{\mathrm{pragmatic}}=0$, however high its rarity: a string of random code has very high rarity but changes no holder's actions, and it is not a signal.

**Source. Prior work**: This form is of the same kind as Weinberger's pragmatic information: he takes the semantic value of information to be "how much it helps in making an informed decision", and defines pragmatic information as the information gain of the receiver's action probability distribution before and after receiving the message (E. D. Weinberger, *BioSystems* 66(3), 105–119, 2002). In that paper he claims that this definition is unique under a few reasonable requirements (such as additivity for logically independent messages); this is the original author's claim, and this book neither repeats its proof nor claims uniqueness on that basis. **RIF does not claim that this form is original.**

**Relation to $\delta_r$ and $I_{\mathrm{causal}}$.** $I_{\mathrm{pragmatic}}$ is **before the fact** (how much the action distribution changed), $\delta_r$ is **after the fact** (whether the viability indicator got better or worse). The two are independent readings, and together with rarity they make three readings. A large change in action distribution with $\delta_r>0$ afterwards: a high-value $I_{\mathrm{causal}}$; a large change with $\delta_r<0$: a **misleading rare signal**, high in strength and negative in polarity.

**One piece of supporting evidence (within the model family).** In the decision model of the synthetic world, the discriminating power of the full KL gap $G$ for subsequent loss is $\mathrm{AUC}=0.394$ (below chance), while the isomorphic quantity of this section's $I_{\mathrm{pragmatic}}$ is $0.880$ (Appendix C, Table C-5, Figure C.6). The reason is that $G$ measures "how far off the model is", not "how far off the decision is": right after a sudden change $G$ is large while the action has not yet changed (the loss is zero), and by the time a real error occurs $G$ has already fallen back. This is one piece of supporting evidence for this section's candidate status and does not change its labeling; it is also the basis for restating $H\mathrm{R}\text{-}7$ at the action level.

$I_{\mathrm{pragmatic}}$ does not replace $I_{\mathrm{causal}}$. The latter is governed by $-\log_2\Pr_{B_0}(e=e_{\mathrm{obs}})$, while the former serves as a proxy reading only when the action distribution is observable; the two are self-information and relative entropy and cannot be converted into each other. A causal reading must still satisfy the three admission conditions at the same time: when $I_{\mathrm{pragmatic}}$ is very large but the holder has paid no measurable cost, it still does not qualify. What this section adds is a strength reading above the threshold, not the qualification threshold itself.

**A proposal for alignment with the definition of causal rarity (to be tested).** Take the prior action distribution $q_D(a)$ to be the holder's action distribution when facing the control object $P_0$; then

$$I_{\mathrm{pragmatic}}=D_{\mathrm{KL}}\big(p_D(a\mid P)\,\|\,p_D(a\mid P_0)\big)$$

**What this section does not claim.** How the action space is coarse-grained and how actions are binned has no protocol, and the results depend on this choice; the KL divergence is asymmetric, and the order of $q$ and $p$ is a convention, not a discovery; for a $P$ that cannot be intervened on and whose action distribution cannot be observed (historical figures, civilizations, institutions), this section serves only as a conceptual illustration and does not constitute a directly computable action-distribution reading; different holders' $I_{\mathrm{pragmatic}}$ are for now reported separately and not added, and there is as yet no calibrated general aggregation rule.

***

## Chapter 14 — Rule Depth

### 14.1 The Problem

Structural rarity answers "how rare is this reading in the background", and causal rarity answers "how rare is this effect"; neither answers one question: how many mutually independent rules does an object contain? A watch and a crystal may both present rare readings, but a watch can contain more independent rules than a crystal.

This is not an optional supplement. Rarity is **a position relative to the background**, rule depth is **the amount of organization inside the object**, and the two can be completely decoupled: a board of completely random noise has rarity close to 0 and rule depth also 0; a perfect crystal at a small size has extremely high rarity and a rule depth of only 1; an integrated circuit etched full of rules is high in both. That both kinds of decoupling exist shows precisely that they are two quantities, not two ways of speaking of one quantity.

The "rule depth" in this chapter refers to the number of layers of independent rules needed for description, and has nothing to do with Bennett's logical depth (measured by computation time).

### 14.2 Definitions

**Rule**: a segment of description that the decoder $D$ uses to reconstruct the object $P$, shorter than a point-by-point record. **Independent rule**: if a rule cannot be obtained from another rule by "repetition at a changed scale", it is independent of that rule.

| Quantity | Symbol | Meaning |
| :------------- | :---------- | :---------------------------------- |
| Rule depth | $D_{\mathrm{depth}}=n_D(P)$ | The **minimum number of independent rules** $D$ needs to reconstruct $P$ within tolerance $\varepsilon_{\mathrm{tol}}$ |
| Rule length | $L_D(P)$ | The total description length of these rules, in bit |
| Unfolding scale | $F_{\mathrm{scale}}$ | The number of times, or span of scales, over which the same rule is repeatedly unfolded |

Depth answers "how many independent rules", length answers "how long are these rules", and scale answers "how many times repeated". Mixing the three gives absurd conclusions: an all-white picture can have arbitrarily large scale (a hundred thousand cells, all white), depth only 1 (the single rule "all white"), and extremely short length; if scale were taken as depth, all-white would become the most complex object. If no rule shorter than a point-by-point record can be found, record $n_D=0$, in which case $L_D$ is approximately equal to the length of the point-by-point record.

The $D$ in $D_{\mathrm{depth}}$ is taken from depth and is not the decoder symbol; this must be stated at first appearance, to avoid confusion with the decoder $D$.

### 14.3 A Minimal Worked Example (Illustrative)

Continuing with 100 cells, divided into 10 blocks of 10 cells each; magnitudes are illustrative, ignoring constants related to the decoder's language.

| Object | Rule | $D_{\mathrm{depth}}$ | $L_D$ | $F_{\mathrm{scale}}$ |
| :----------------- | :--------------- | :--- | :---------------- | :--- |
| All white (perfect crystal) | "All white" | 1 | Very short | 100 |
| First cell of each block black, the rest white | Block pattern, repeated 10 times | 1 | Block pattern plus repetition count, within a few dozen bit | 10 |
| Black-cell position in each block, shifted right by $j-1$ cells for block $j$ | Block pattern, plus one "block-by-block variation" rule | 2 | Slightly longer | 10 |
| Completely random | No shorter rule; can only be recorded cell by cell | 0 | ≈ 100 | — |

$D_{\mathrm{depth}}$ counts only the number of independent rules and does not compare the content of the rules: objects of the same depth may have entirely different rule content. The third row is the key — on the basis of the second row it adds one "block-by-block variation" rule, and the depth goes from 1 to 2; this rule cannot be obtained from "repeating the block pattern 10 times", which would only produce 10 identical blocks. **"Cannot be obtained by repetition at a changed scale" thereby acquires concrete content: it asks whether it can be explained by existing rules plus a repetition count, and if not, it is a new rule.** In addition, the completely random one has the largest $L_D$, but its structural rarity is close to 0 (it is like the background), which shows that large length does not mean high information, and this book does not mix the two quantities.

### 14.4 Compression Gain and Structural-Information Readings

**Operationalization of the defect criterion.** The first defect criterion of this book is "the position and kind of the defects can be described by a rule markedly shorter than a random point-by-point record", which can be written as

$$G_{\mathrm{comp}}=\log_2\binom{N}{k}-L_D(\text{position and kind of the defects})$$

$G_{\mathrm{comp}}$ is called the **compression gain**: significantly greater than 0 shows that the defect placement has a rule and meets the criterion; $\approx0$ shows it is no different from random placement. Since $L_D$ can generally be bounded only from above, the computed $G_{\mathrm{comp}}$ is a lower bound of the true gain; this asymmetry is the only directional conclusion in this chapter.

**Proposition (One-Directional Discriminating Power of Compression Gain)**:

- Premises: $L_D$ is given an upper bound $\hat L_D\ge L_D$ by some specific compression method; $\binom{N}{k}$ is the description length of random placement of the same scale.
- Result: $\hat G_{\mathrm{comp}}=\log_2\binom{N}{k}-\hat L_D>0$ can confirm the existence of a rule (the true $L_D$ can only be smaller, and the true gain only larger); $\hat G_{\mathrm{comp}}\approx0$ cannot confirm the absence of a rule (the true $L_D$ may be far smaller than the upper bound, and the gain may be large, only not found).
- Failure conditions: when the compression method used is clearly weaker than the best method known for that object domain, $\hat L_D$ may be so large that $\hat G_{\mathrm{comp}}$ is always negative and discrimination fails completely; the method or language must then be changed.

**The capping of the passive phase.** A perfect crystal has $D_{\mathrm{depth}}=1$, while $F_{\mathrm{scale}}$ can be arbitrarily large: the passive phase can expand scale by repeating the same rule without adding new independent rules; an increase in depth means that new independent rules appear. Whether growth in size at the same time raises structural information must still be judged under the specified background, reading, and resolution.

**Compression gain and rarity cannot be inferred from each other.** An extremely rare configuration may have no short description at all (a particular pattern in random noise, rarity $N$ bit, depth 0); an extremely common configuration may have a very short description (all white, low rarity, depth 1). Each of the two quantities holds on its own and governs its own matter.

### 14.5 Variation with the Decoder

Rule depth and rule length can both be read out only relative to the decoder $D$, for two reasons. First, the description language differs: for a decoder able to perform arbitrary computation, changing language changes $L_D$ only by a constant (the invariance theorem of algorithmic information theory); for actual instruments or people, the kinds of rules that can be read depend on their resolution and language. Second, when a decoder is upgraded, the number of layers read increases: a decoder that can resolve only atoms cannot see the arrangement of crystal grains and reads a smaller $n$; one that can resolve grains reads more. This is the meaning of "changing the rules amounts to changing the frame of reference" — $D_{\mathrm{depth}}$ measures the object, yet the reading belongs to the relation between decoder and object.

"Differs only by a constant" can be used only with a qualification: it holds only for ideal decoders able to perform arbitrary computation. For actual instruments or people, changing language replaces a whole class of readable rules, and some rules cannot be expressed in the new language at all. So at the practical level this book never assumes that "depth is language-independent"; a reported depth must state the language and tolerance, otherwise the number is not comparable.

### 14.6 Measurement Steps

1. Specify the decoder $D$, along with its basic units and the available kinds of rule;
2. Specify the tolerance $\varepsilon_{\mathrm{tol}}$, that is, to what precision reconstruction counts as success;
3. Look for the shortest layered description in $D$'s description language;
4. Distinguish "repetition at a changed scale" (counted in $F_{\mathrm{scale}}$) from "a new independent rule" (counted in $D_{\mathrm{depth}}$);
5. Read out $D_{\mathrm{depth}}$, $L_D$, $F_{\mathrm{scale}}$;
6. When one needs to judge "whether there is a rule", compute the compression gain $G_{\mathrm{comp}}$.

The shortest description generally cannot be found exactly, and an upper bound can be given only by a general compression algorithm or a known generating rule, with the method used stated. Step 4 is the most error-prone: judging "is this a new rule" is in essence asking "can it be explained by existing rules plus repetition", and this judgment depends on which transformations the decoder allows — a decoder that allows rotation, scaling, and translation will see more things as repetitions of the same rule, and one that allows only translation will see two rules. **Depth is not an absolute number but "the minimum number of rules under a given class of transformations"; stating the class of transformations when reporting depth is as important as stating the tolerance.**

**Hard requirement.** A depth reading that does not state the rule language and tolerance is **not counted in any comparison** and may not enter cross-object ordering. This stems from depth being defined relative to language: the same batch of objects can be fully recovered **within the library**, and once they fall **outside the library** they are all underestimated, with errors in a consistent direction (Appendix C, Table C-6, Figure C.7).

### 14.7 What This Chapter Does Not Claim

1. **Repeated unfolding adds no depth.** Snowflake dendrites and the multi-scale texture of granite are repetitions of the same rule at different scales ($F_{\mathrm{scale}}$ is large), and depth stays low; an increase in depth requires a new independent rule. In dynamical description the number of transitions can be used to construct the corresponding index $D_{\mathrm{depth}}=1+\#\{\mathcal{T}\}$ ($\mathcal{T}$ a topological transition), but this is a modeling extension and does not change this chapter's static definition. **"Each transition adds exactly one independent rule" is a calibration assumption, not an equality derived from the definition**: a transition may introduce several rules, or may change only how the rules are organized without increasing their number. To use this formula one must first calibrate — regress static depth on the number of transitions and test whether the slope is 1; when the slope is significantly different from 1, the formula can serve only as a depth exponent (an ordinal index counted by the number of transitions) and cannot be taken as the number of rules. The formula is defined only for objects with static depth $n_D\ge1$, counting from the initial single rule; it does not apply when $n_D=0$ (no rule shorter than the point-by-point record can be found, as for completely random). Depth itself does not determine provenance; whether something is spontaneous or artificial is still distinguished by the provenance criteria.
2. **The determination of independence depends on the decoder.** "Whether it can be obtained by repetition at a changed scale" depends on which transformations the decoder allows, and the same object may have several ways of layering. This chapter takes "the minimum number of independent rules" as the norm, but does not guarantee global uniqueness.
3. **Not exactly computable.** The shortest description generally cannot be proven globally shortest, and an upper bound can usually be given only by a compression algorithm or a known generating rule, with the method adopted reported.
4. **No physical upper limit is claimed.** This chapter does not assert "how many layers natural processes can form at most."

***

## Chapter 15 — A Taxonomy of Decoders and Decoder-Holder Qualification

### 15.1 The Task of This Chapter

The preceding conceptual discussion has already distinguished the ontological types of decoder. This chapter does not restate their formation, and answers only three measurement questions: which $D$ can serve as structural reading rules, so as to define $I_{\mathrm{struct},D}(P)$; which specific holders satisfy the entry conditions for causal effects, so as to define $I_{\mathrm{causal},D}(P)$; and how the background model corresponding to each class of reading rule should be specified — specifically, when to use the habitat background $B^{\mathrm{env}}$ and when to use the protocol baseline $B^{\max}$.

### 15.2 Two Levels

The classifications below all presuppose that the four necessary conditions already hold, and answer "who maintains the boundary and how high is the extraction complexity", not a fresh judgment of whether $D$ exists.

**Ontological decoders** are classified by the presence and origin of a self-maintained boundary: $D=\varnothing$ is a purely physical structure without a self-maintained boundary; $D_{\mathrm{phys}}$ is selective extraction with a self-maintained boundary; $D_{\mathrm{cog}}$ is a region of functional complexity superimposed on $D_{\mathrm{phys}}$, characterized by the three axes of history dependence, persistence coupling, and plasticity time scale plus a fourth axis (self-reference); how to measure the three axes and operationalize the fourth axis is in §15.8. Functional features can recur across substrates, while holder qualification is counted by concrete instance.

The **frame of reference** is $D_{\mathrm{macro}}$: the public part of the measurement protocols that multiple holders adopt in common and that can be commensurated with one another; the protocol itself has no single holder, and the concrete readings are still carried out by holders who bear the cost.

### 15.3 Two Roles

| Role | Definition | Who fills it |
| :------- | :------------------------ | :------------------------- |
| **Decoder holder** | A persistent structure that satisfies the four criteria, owns or runs a reading rule, pays the decoding cost, and is changed by the information decoded | $D_{\mathrm{phys}}$, $D_{\mathrm{cog}}$ |
| **Reading protocol** | Maps $P$ to a reading $r=D(P)$, giving $I_{\mathrm{struct},D}(P)$; executed by a holder's reading rule or a public protocol | $D_{\mathrm{macro}}$ (no single holder; the decoding cost of concrete readings is borne by the scientists or institutions carrying out the measurement); a holder's own reading rule |

The reading protocol is responsible for defining how to read; the specific holder pays the decoding cost and may be changed by the information read out. In a structural reading, $D$ can refer to a holder's reading rule or to a public protocol; in a causal reading, $D$ refers to the reading rule of the specific holder that responds to the effect and bears the cost.

### 15.4 Summary Table of Classes

The table below is arranged by functional role and is not a strictly mutually exclusive classification: $D_{\mathrm{macro}}$ is the convergence point of protocols; the $D_{\mathrm{cog}}$ row denotes the region at online type or above on the three axes, and such structures are at the same time $D_{\mathrm{phys}}$.

| Class | Self-maintained boundary | Decoder | Decoder holder | Source of the background | Examples |
| :-------- | :----- | :----- | :------------ | :----------------- | :------- |
| $D=\varnothing$ | None | No, only read | None | Determined by the rules of the party that reads it: with no holder, take $B^{\max}$ | Stones, crystals, stars |
| $D_{\mathrm{macro}}$ | None | **Protocol level (not a holder)** | No single holder; the party carrying out the measurement bears the cost, with instrument and protocol cost listed separately as $E_{\mathrm{meas}}$ | **Protocol baseline $B^{\max}$** (maximum-entropy distribution at given temperature, volume, and composition) | Instruments, public measurement |
| $D_{\mathrm{phys}}$ | Yes | Yes | Yes | **Habitat background $B^{\mathrm{env}}$**; always measured externally in the habitat; the innate "assumed distribution" of static ones is recorded separately as $B_{\mathrm{int}}$ (used only for explanation, not entering readings), and dynamic ones update with the habitat | Ion channels, bacterial chemotaxis, plant phototropism |
| $D_{\mathrm{cog}}$ (position on the three axes reaching the online type or above) | Yes | Yes | Yes | **Habitat background $B^{\mathrm{env}}$**; its internally acquired model is recorded separately as $B_{\mathrm{int}}$, and the difference between the two is the decoding deviation | Crows, octopuses, humans |

The most important column of this table is "source of the background", which pins the two conventions to different rows. **$D_{\mathrm{macro}}$ uses the protocol baseline, because its readings must be commensurable across subjects; the other rows use the habitat background, because their readings must answer "how rare for this holder."** If $D_{\mathrm{cog}}$ is switched to $B^{\max}$, what one obtains is no longer "how rare for him" but "how special formally"; if $D_{\mathrm{macro}}$ is switched to some $B^{\mathrm{env}}$, readings across laboratories are no longer comparable.

**What is not a $D$**: a thermostat maintains the user's comfort, not its own boundary, so it is not $D_{\mathrm{phys}}$; its effect is counted on the person who uses it (a $D_{\mathrm{cog}}$). Structures in the embodied-type region (bacteria, mimosa) take $B^{\mathrm{env}}$ as static or dynamic $D_{\mathrm{phys}}$.

**The position of externally substrate-dependent PSs in this table**: objects such as viral lineages and pure software systems are not listed separately as holders. If they do not satisfy the four criteria, they serve only as objects $P$ being read, and the reading cost is attributed to the holder that actually carries out the reading; if they have formed their own self-maintaining closed loop, they are recorded in the $D_{\mathrm{phys}}$ row, and those whose position on the three axes meets the standard are also recorded as $D_{\mathrm{cog}}$.

### 15.5 The Responsibilities of $D_{\mathrm{macro}}$

It supplies three things: the **protocol baseline $B^{\max}$**, the maximum-entropy distribution under given constraints, for structural readings without a holder and for cross-subject comparison; **the control-experiment protocol for the control baseline $B_0$** — $B_0$ must be established relative to a designated holder and an explicit control object, and cannot be taken as a global fixed background detached from holders; and **the recording of observable effects and the causal-attribution protocol**. It is a reading protocol and can fill the $D$ of $I_{\mathrm{struct},D}(P)$.

It is **not** a decoder holder and does not count as an ontological $D$; $I_{\mathrm{causal}}$ is borne by each holder itself. It also **does not supply values of the habitat background** — $D_{\mathrm{macro}}$ supplies only measurement protocols, and the values of $B^{\mathrm{env}}$ are always determined by an external measurer in the holder's habitat; a public protocol has no habitat. **The innate "assumed distribution" of $D_{\mathrm{phys}}$ is recorded separately as $B_{\mathrm{int}}$, used only for explanation and not entering readings.**

#### 15.5.1 The Attribution of $D_{\mathrm{macro}}$

**Definition**: $D_{\mathrm{macro}}$ is the commensurable part of measurement protocols. It has no single holder and is the convergence point of the protocols used by multiple holders (scientists, laboratories, instrument operators). The convergence stems from the **shareability** of protocols: the same instrument and the same operating procedure, used by different people, give the same reading.

Shareability makes it look like an "objective standard belonging to no one", but this does not mean that it is detached from all holders. Every concrete reading is carried out by some concrete holder, who bears the decoding cost (counted in $E_{\mathrm{causal}}$); the instrument is an extension of the scientist's senses and is not itself a holder. **Protocol costs such as instruments, calibration, and recomputation are not counted in any holder's $E_{\mathrm{causal}}$ and are listed separately as $E_{\mathrm{meas}}$** (an instrument is not a holder, and spreading it onto some holder's causal cost would both overestimate that holder's cost and underestimate the cost of the protocol itself). So $D_{\mathrm{macro}}$ does not conflict with "no decoder, no information": the protocol is shared, and the readings are carried out by someone.

**Natural science is a body of knowledge, and also a persistent structure.** It consists of theories, equations, models, measurement methods, and empirical content, and belongs to the externally substrate-dependent type (including the two kinds of component, formal-mathematical and memetic); **Hypothesis**: the selection pressure it faces is that bodies of knowledge that condense more information at a lower decoding cost are more likely to be retained. The dynamics of this selection process is outside the scope of this book.

**The scientific community is another persistent structure.** A group of people who make a living by this body of knowledge, with no structural binding to the knowledge system; the interests of the community and the persistence of the knowledge system are not always aligned: when a lower-cost intermediary of knowledge production appears, the knowledge system can, to a certain extent, continue to evolve apart from the community.

**The knowledge system is not a holder.** The same applies to the natural-science knowledge system — its persistence depends on holders' acknowledgment and testing; it is a PS, not a holder; $D_{\mathrm{macro}}$ never appears in the capacity of a holder either, and need not pass the four criteria.

**Which layer of decoder each of the four kinds of discipline uses**: the formal sciences use pure $D_{\mathrm{cog}}$ to study description languages, without instruments, and the ratchet speed is limited only by cognitive ability; the natural sciences use $D_{\mathrm{macro}}$ to study measurable structure; the social sciences use $D_{\mathrm{cog}}$ to study other $D_{\mathrm{cog}}$; the humanities use $D_{\mathrm{cog}}$ to study itself. The methodological core of RIF belongs to the formal sciences, and as a complete theory it must be verified by experiment and data.

**Narrow and broad $D_{\mathrm{macro}}$**: the narrow one is the part that has solidified into protocol, namely the sum of classical physical measurement rules, reading out $I_{\mathrm{struct},D}(P)=-\log_2 \Pr_{B^{\max}}(r=D(P))$; its features are that readings are repeatable, can be remeasured with another instrument, are consistent across subjects and eras (during periods of protocol stability), and can be falsified, for example photon counts, temperature readings, the CMB blackbody spectrum. The broad one is the part still under active inference; it does not itself infer, and supplies only the control baseline $B_0$ of "what the data should look like without this inference", with the inference carried out by holders; for example, the control for inferring a metamorphic rock is "the spectral distribution of igneous rocks", and the control for inferring a pulsar is "the signal distribution under other candidate explanations."

The unsuperscripted $D_{\mathrm{macro}}$ by default means the narrow one. Note that two different background notations are used here: the narrow one reads structural information and uses $B^{\max}$; the broad one supplies the causal control $B_0$, and $B_0$ is established for a designated holder and control object and is not $B^{\max}$. **Both are "reference distributions", but one is a control for the effect distribution and the other is the maximum-entropy baseline of the reading; they may not substitute for each other.**

#### 15.5.2 From Narrow to Broad: Continuous Transition and the Ratchet

**The boundary is a ratchet, not a spectrum.**

**Proposition (Protocol Ratchet)**:

- Premises: an inference survives repeated testing; its control baseline $B_0$ has been repeatedly constructed and has not failed; the relevant operations have been standardized so that different people obtain the same reading.
- Result: the inference migrates from the broad into the narrow, after which its readings no longer require $B_0$ to be rebuilt each time, and its $I_{\mathrm{causal}}$ becomes a routine measurement.
- Failure conditions: when a more precise measurement overturns the original inference, or new data appear that the original $B_0$ cannot explain, the item moves back from the narrow to the broad, and the ratchet is reversible. So the "ratchet" is a **statistically one-directional trend**, not an irreversible physical process.

#### 15.5.3 Measurement Attribution of $I_{\mathrm{struct}}$ and $I_{\mathrm{causal}}$

| Quantity | Attribution | How obtained |
| :-------- | :------------- | :----------------------------------- |
| $I_{\mathrm{struct}}$ | Narrow $D_{\mathrm{macro}}$ | Read directly by instruments, with the background taken as $B^{\max}$ |
| $I_{\mathrm{causal}}$ | Scientists ($D_{\mathrm{cog}}$ holders) | Logical inference plus $B_0$ (supplied by $D_{\mathrm{macro}}$); must follow the two-step determination of "identify the effect first, then report the rarity" |

The two are not "one objective, one subjective", but differ in **measurement protocol**: $I_{\mathrm{struct}}$ is read directly by instruments and is repeatable by third parties; $I_{\mathrm{causal}}$ cannot be read directly by instruments and must be inferred indirectly from the holder's **observable behavioral change**, so it is not an untestable first-person feeling.

### 15.6 The Background Model of Each Class

| Class | Background notation | Construction | How it varies |
| :----- | :-------- | :--------------------- | :---------------------- |
| $D_{\mathrm{macro}}$ | $B^{\max}$ | Maximum-entropy distribution under constraints of given ambient temperature, volume, and particle number | The constraint quantities vary with observation scale and environment; changing the constraints changes the protocol |
| Static $D_{\mathrm{phys}}$ | $B^{\mathrm{env}}$ | Measured externally in the habitat (historical process only explains its stability and does not supply values) | Unchanged during the individual's persistence |
| Dynamic $D_{\mathrm{phys}}$ | $B^{\mathrm{env}}$ | Updated with real-time feedback | Variable during the individual's persistence |
| $D_{\mathrm{cog}}$ | $B^{\mathrm{env}}$ | Determined by habitat frequencies; additionally holds an internal model $B_{\mathrm{int}}$ | $B^{\mathrm{env}}$ varies with the habitat, $B_{\mathrm{int}}$ varies with learning; the difference between the two is the decoding deviation |

**Counting information requires paying a cost.** This holds for both backgrounds: with $B^{\max}$, the cost is that of maintaining the measurement protocol (instruments, calibration, recomputation); with $B^{\mathrm{env}}$, the cost is that of the holder determining habitat frequencies and maintaining the decoder, counted in $E$.

**Where the two columns are placed side by side.** If a report needs both "how rare for the holder" and "how special formally", list two columns side by side, each with its own background and its own annotation, and no "composite rarity" may be synthesized.

### 15.7 Cost-Attribution Rules for Externally Substrate-Dependent PS

Externally substrate-dependent PSs (virus type, memetic-virtual type, formal-mathematical type, software type) can serve as the object $P$ being read, but the realization of their characteristic information organization depends on an external carrying system. The rules are: the information content is attributed to $P$; the decoding cost is borne by the holder that actually carries out the reading, while instruments and reference frameworks only read out readings; the information, persistence time, and resource cost of the external carrying system may not be counted directly into $P$ without argument; when substrates are shared or several PSs operate in coordination, a cost-allocation rule must first be declared, to avoid double counting.

***

### 15.8 Candidate Operationalization of the Three $D_{\mathrm{cog}}$ Axes

**This section gives candidate operationalizations of the three axes; its role is to leave a starting point for metrology; the three axes are not RIF's formal protocol.**

| Axis | Candidate quantity | Unit |
| ---------------- | ---------------------------------- | :-------- |
| Degree of history dependence | Conditional mutual information $I(h_t;x_{<t}\mid x_t)$: given the current input, how much information about past inputs the internal state still carries | bit |
| Degree of persistence coupling | Intervention experiment: the change in the viability indicator (survival rate, reproduction rate, etc.) after this history dependence is disrupted | same unit as $\mathrm{sv}$ |
| Time scale at which plasticity occurs | The ratio of the characteristic time at which the rule is rewritten to the individual lifespan, $\tau_{\mathrm{plastic}}/\tau_{\mathrm{life}}$: far less than 1 leans online type, far greater than 1 leans embodied type | dimensionless |
| Degree of self-reference (fourth axis) | Conceptually, the degree to which the decoder brings its own representation into subsequent decoding; candidate measurement methods and conventions remain to be established | — |

**Known operationalization difficulty**: $\tau_{\mathrm{plastic}}$ should be understood as **the time needed for the rule itself to be recalibrated**, not "the time needed to carry out one concrete reaction." Bacterial chemotactic response is completed in seconds, but the rule that drives it is hard-wired on an evolutionary scale, so $\tau_{\mathrm{plastic}}$ is close to the evolutionary scale of the species. If the single-reaction time were misused, an embodied-type structure whose rules are hard to rewrite within an individual lifespan would be miscounted as online type.

**Relation of the predictive time horizon to this table**: the endogenous time horizon describes how far into the future a cognitive system can plan, which is a prediction-type description; the three axes of this table are used to characterize objective records. The two are different dimensions of description; the predictive time horizon is not merged into this table, and does not occupy the fourth axis.

Of the three axes only the first has a ready-made bit unit. Persistence coupling follows the unit of $\mathrm{sv}$ and must be measured on the same scale as the indicator chosen for the specific study; the plasticity time scale is a dimensionless ratio and can be compared across species. **Candidate quantities with non-uniform units are invalid for cross-object comparison.**

### 15.9 What This Chapter Does Not Claim

It gives no demarcation between life and non-life (this is a property of the classification table); for the thresholds of the three axes see §15.8; for aggregation across multiple holders see the four explicit declarations of §13.4.

### Summary of Part Two: Settled and Unsettled

| Chapter | Settled | Unsettled |
| ------------ | ---------------------------- | -------------------- |
| 12 Definition and Measurement of Information | Three rarity protocols; the division of labor between the two background notations; the four-step boundary-identification procedure; the measurement-layer definitions of $T_{\mathrm{struct}}$ and $E_{\mathrm{struct}}$; four numbered predictions | The operationalization of $W_{\mathrm{sv}}$, $\iota_D$, and the "optimal response" |
| 13 Causal Rarity | The definition; two classes of control source; the two-step determination structure; the equivalence test and the 3 bit / 5 bit entry thresholds; holder-level reporting and the four explicit aggregation declarations | The domain-specific value of $\delta_{\mathrm{eq}}$; the apportionment algorithm for shared costs |
| 14 Rule Depth | The static definition (minimum number of independent rules); the division of labor with rule length and unfolding scale; the one-directional discriminating power of compression gain; "number of transitions–depth" as a calibration assumption | The shortest-description algorithm; a standard list of transformation classes; a norm for cross-object depth comparison |
| 15 Classification and Holder Qualification | The four rows of the classification table; the assignment of the two backgrounds to each row; the boundary of $D_{\mathrm{macro}}$'s responsibilities; the cost-attribution rule for externally substrate-dependent types | The thresholds of the three axes; aggregation weights; any composite scalar |

***

## Part Three · Lineage and Comparison

> This part sets RIF beside existing work. The purpose is to make two things clear: which questions others have already solved better than this book, and which questions this book wants to ask that others have not.

***

## Chapter 16 — Reading Against the Literature: Divergence from Contemporary Stochastic Thermodynamics

**Prior work**: Contemporary stochastic thermodynamics has carried the coupling of information, time, and energy to the extreme: Wolpert computed the exact lower bound on entropy production under given protocol constraints, the TUR gave a universal inequality between precision and dissipation, and Nicholson wrote time directly into the speed limit. These works are exact, rigorous, and testable.

In the concrete computations of these four papers, the partition of the system is given in advance; Kolchinsky–Wolpert 2018 and the Markov-blanket line each have their own treatment of the boundary. RIF's difference lies in this: the boundary is determined iteratively by whether I–T–E can be paired, and persistence time is made an independent dimension of the record.

### 1. Kolchinsky & Wolpert, PRX 11, 041024 (2021)

Under particular restrictions (symmetry, modularity, coarse-graining), how much entropy production must be burned at minimum, and how much work can be extracted at most, to drive a physical system from an initial distribution $p$ to a final distribution $p'$; the core result is the decomposition of nonequilibrium free energy into accessible free energy and inaccessible free energy.

**RIF's challenge**: Wolpert's derivation is extremely rigorous, but he assumes by default that "the system", "the components", and "the final state" are objectively existing, given entities. RIF asks: if the decoder is dissolved, or if this pile of components is, in the eyes of another civilization, merely a heap of scrap, does your "minimum cost" still mean anything?

### 2. Barato & Seifert, PRL 2015 — TUR

It proves that for a Markov process in a nonequilibrium steady state, the higher the precision of its output, the more energy it necessarily consumes. The standard form is $\mathrm{Var}(J)/\langle J\rangle^{2}\cdot\Sigma/k_B\ge2$ (the right-hand side is a dimensionless constant with no extra free parameter). This inequality was first proved for steady-state processes, and later literature has generalized it to more general cases, but it does not hold unconditionally for "any microscopic stochastic process".

**RIF's boundary reset**: TUR describes the fuel-consumption/precision trade-off inside a given engine. RIF asks: what counts as an engine? Where is its boundary? If the parts are taken apart and reassembled in another machine, is it still the same engine?

**Terminological precision**: TUR is a family of inequalities, not a family of power laws; it gives a lower-bound coefficient, not a scaling relation (there is no free parameter like an "exponent"). What truly yields cross-system scaling laws is Chaisson (2001, energy rate density) and Kleiber (1932, metabolic scaling).

**Use for RIF**: this is the strictest physical statement that "identification has a price" — to form a stable distinction in noise, TUR directly gives the minimum dissipation per bit of precision for this degree of distinction, and can become a lower bound for $\iota_D$ in its physical realization in stochastic systems. But it is a **proposal**, not a **conclusion**: turning it into a lower bound for $\iota_D$ needs one more mapping, and that step would bring in an entire stochastic-process model, which is exactly what this book deliberately does not presuppose.

### 3. Nicholson, García-Pintos, del Campo & Green, Nature Physics 16, 1211 (2020)

It gives an uncertainty relation: the time needed for an observable to change by "one standard deviation" has a lower bound, given jointly by the entropy production rate and the Fisher information; the mathematical form imitates the Mandelstam–Tamm time–energy uncertainty relation of quantum mechanics. Of the four papers this is the only one that writes I, T, and E into a single inequality.

**RIF's anchoring of meaning**: what Nicholson et al. give is a **time–information uncertainty relation** (a general thermodynamic bound), not "the executing agent's own physiological limit"; RIF's $T_{\mathrm{struct}}$–$I_{\mathrm{struct}}$ pairing is compatible with it, but is not derived from it. RIF asks: if the decoder at the receiving end cannot read this change, then in this measurement, how much causal information does this change carry? The answer may be zero, or may not — it depends on who the decoder is. The reason is that this decoder cannot extract this difference.

This is exactly where the distinction "process time versus persistence time" is used. Nicholson's time is **process time**: the time needed for an observable to change once. This book's $T_{\mathrm{causal}}$ is **persistence time**: how long this causal effect can still be identified by some holder. Both are measured in seconds, but one sits in an inequality and the other in a record table, and they **cannot be substituted for each other**. Whoever stuffs $T_{\mathrm{causal}}$ into Nicholson's inequality has tacitly assumed that "persistence time is the duration of one process."

### 4. Still, Sivak, Bell & Crooks, PRL 109, 120604 (2012)

For a nonequilibrium system that maintains a predictive model of its environment, its dissipated work is constrained by the predictive information; efficiency equals benefit over cost, the benefit being predictive information and the cost being dissipated work.

**Positioning: a formal resonance at a different scale.** The similar side is that both concern the connection between information processing and energy cost. The differences are four: Still's "predictive system" is a designated or designed nonequilibrium system, and its time scale is a single step of the protocol, while this book discusses the whole persistence period; Still's "predictive information" is mutual information, whereas $I_{\mathrm{causal}}$ is effective causal information that enters state transitions, with polarity and decoder-relativity; Still's $T$ is folded into the rate and there is no independent time dimension; Still's system is preset and does not emerge from a record.

**Conclusion**: the two are adjacent on the point that "a quantifiable efficiency relation exists between information and energy", but differ in object of study, scale, and temporal semantics. Still's work constitutes neither a premise for deriving any definition in this book nor its historical predecessor.

### The Common Structure of the Four Papers

**The system boundary is an input, not an output.** Wolpert's "system" is given, the TUR's "engine" is given, Nicholson's "executing agent" is given, and Still's "predictive system" is given. Within their respective given systems, they have carried the coupling of I–T–E to the extreme. This is their contribution, and also their boundary.

### Drawing the Line at the Core: Process Time versus Persistence Time

In all four papers every $T$ is the duration of one operation or an observation window, answering "how long does one operation take at least"; this book's persistence time asks "under what conditions can a structure's informational reading or causal channel still be identified." The two are used for different objects, and process duration may not be taken directly as a persistence criterion.

### Upstream and Downstream: Not Competitors

**Protocol-fixed invariants versus decoder-relativity.** Fisher distance, Shannon mutual information, and entropy production are, once a partition of variables and a coarse-graining method (a protocol) are given, quantities that do not change with "who is measuring" — but this protocol itself (which variables are chosen, at what scale coarse-graining is done) remains a choice given in advance by the researcher. After the protocol is fixed these theories no longer ask "for whom"; RIF precisely wants to bring the selection of the protocol itself, that is, who the decoder is, into the core variables. This is merely a difference of level.

**Constraint versus ranking.** TUR / speed limits give inequalities (what one cannot go below), whereas the viability potential $V$ gives a comparison benchmark (by what to rank). These are two kinds of mathematical object, in an upstream–downstream relation: their inequalities constrain the range of values of RIF's thresholds, and RIF's record structure decides on which system this threshold is taken. $V$ belongs to the layer of models that synthesize I–T–E into a single scalar; the line of division of labor is in §11.

**Bridging protocol**: when the system boundary is fixed, a single decoder is used, and a time window serves as the observation parameter, the threshold is bounded by TUR. This one item does two things at once: it adds a physical lower bound to the operationalization, and it supplies a degeneracy condition for the lineage demarcation. This book formally lists these four works in the "known nearest neighbors" list, naming and claiming this structural overlap rather than leaving readers to discover it themselves.

### Summary of Part Three: Settled and Unsettled

| Chapter | Settled | Unsettled |
| ------------- | ------------------------------- | ----------------- |
| 16 Scholarly Comparison | The division of labor between the four nearest-neighbor works and this book; the exact meaning of non-interchangeability in both directions | Mapping their inequalities into this book |

## Falsifiable Predictions

$H\mathrm{R}\text{-}1$ through $H\mathrm{R}\text{-}3$ discuss the persistence consequences of social deprivation, with empirical anchors in the research on social exclusion and the social gradient (Eisenberger et al., 2003; Marmot et al., 1991); the other six come from corollaries of this book's measurement layer. The testable predictions of this book are numbered uniformly as $H\mathrm{R}\text{-}n$, in the format "prediction | test | refutation condition." All nine share one testing order: **measurement first, hypothesis testing second** — which entries are blocked by this order is given in the note after the table.

| No. | Prediction | Test | Refutation condition |
| :--- | :------------------------ | :------------------ | :-------------- |
| $H\mathrm{R}\text{-}1$ | **Mediating structure**: the decline in physiological indicators goes mainly through the path of "decline in resource inflow"; after controlling for an equal material loss, the truncated group still shows a residual difference, and the residual is dose-related to the size of the decline in causal information. | Use "the number of others who formerly executed his decisions automatically" as a proxy for the decline in causal information, with the control group being "equal assets lost to market losses", and do a mediation analysis with resource inflow as the mediator. | After controlling for equal loss the residual disappears; or the residual has no dose relation to the size of the decline. |
| $H\mathrm{R}\text{-}2$ | **Reversibility asymmetry**: restoring the channel (reinstatement, unfreezing, exoneration) recovers faster and more fully than compensating an equal material restoration. | Compare the recovery curves of the two kinds of intervention within the same batch of truncation cases, with the time and magnitude for the structural indicator to return to baseline as the dependent variable. | The two curves do not differ significantly, or the compensation group recovers faster. |
| $H\mathrm{R}\text{-}3$ | **Source difference**: under equal material loss, the consequences of the "refused recognition" type differ from those of a disaster type in which no one refuses. | Match pre-truncation resources, disease burden, stigma, judicial status, social network, and event severity, and compare the trajectories of the two groups. | After matching the trajectories do not differ; or the difference is explained by stigma or judicial status. |
| $H\mathrm{R}\text{-}4$ | **Thresholds move with persistence state**: when persistence constraints change, the magnitude of change in the minimum discernible difference is ordered by $\lvert\delta_r\rvert$, not by signal strength. | Apply a persistence-pressure treatment, measure the thresholds for each cue, and compare the goodness of fit of the two ordering predictions. | Threshold changes are unordered with respect to $\lvert\delta_r\rvert$, or can be explained by strength alone. |
| $H\mathrm{R}\text{-}5$ | **Decoding blind spots can be identified in advance**: when cues that are persistence-relevant but unresponded-to are manipulated, the viability indicator falls while behavior does not change. | Pre-register a list of blind spots, intervene on the cues in the list, and measure $\mathrm{sv}$ and behavioral indicators at the same time. | The identified blind spots do not predict a decline in persistence; or the intervention also changes behavior. |
| $H\mathrm{R}\text{-}6$ | **Rising cost coarsens resolution. When the decoding cost is approximately the same across distinctions, the distinction with the smallest $\lvert\delta_r\rvert$ is dropped first; when costs are heterogeneous, the distinction with the smallest $\delta_r/c$ is dropped first** ($c$ is the persistence equivalent converted from the decoding cost of one reading of that distinction). In both cases "smallest" refers to the **margin over the whole partition**, not a pairwise comparison of individual distinctions. | In an AI agent with perceptual cost, raise the decoding cost step by step and record the order in which distinctions are abandoned; take homogeneous-cost and heterogeneous-cost settings separately and compare the fit of the two orderings. | The order of coarsening is unrelated to $\lvert\delta_r\rvert$ (homogeneous case) or $\delta_r/c$ (heterogeneous case); or the joint benefit can be exactly reproduced by the sum of pairwise gains. |
| $H\mathrm{R}\text{-}7$ | **Prediction failure of decoding deviation at the action level**: after an abrupt change in the habitat distribution, the gap between $B_{\mathrm{int}}$ and $B^{\mathrm{env}}$ in the **action distribution** (that is, $I_{\mathrm{pragmatic}}$ of §13.9) should predict the subsequent error rate and the decline in persistence; the full KL gap $G$ is reported separately as a state reading and does not bear the predictive function. | Artificially mutate the frequency distribution, measure separately the KL gap at the action-distribution level and the full KL gap $G$, and compare their predictive power for subsequent error rate; control the mutation magnitude. | The action-level gap does not predict errors, or its predictive power is explained by mutation magnitude. |
| $H\mathrm{R}\text{-}8$ | **The trajectory is determined by the update rate of the reference class**: after controlling for the update of $B_0$, the marginal contribution of object-side variables to the trajectory is close to zero. | Measure in the same batch the update rate of $B_0$ and the physical state of the carrier, and see which of the two is more strongly correlated with the historical sequence. | After controlling for the update of $B_0$, object-side variables still predict significantly. |
| $H\mathrm{R}\text{-}9$ | **Misleading rare signals are predictable**: readings with "high $I_{\mathrm{pragmatic}}$ and $\delta_r<0$" should reproduce a negative persistence effect in independent samples. | Group by the signs of $I_{\mathrm{pragmatic}}$ and $\delta_r$, and track the subsequent change in $\mathrm{sv}$ in each group. | The effect does not reproduce, or can be explained by the initial level of $\mathrm{sv}$. |

The status of $H\mathrm{R}\text{-}9$ is "conditionally testable": if the action distribution can be stably observed and binned, it is testable; otherwise it has only conceptual meaning.

**Note after the table.** Five of the nine depend directly on intermediate quantities for which no operationalization protocol yet exists: $H\mathrm{R}$-4 and 6 depend on the ordering quantities $\lvert\delta_r\rvert$ and $\delta_r/c$, $H\mathrm{R}$-5 depends on the identification of blind spots (the sign of $\delta_r$ and the response reading must be obtained together), and $H\mathrm{R}$-7 and 9 depend on $I_{\mathrm{pragmatic}}$; the detection floor $\iota_D$, the persistence window $W_{\mathrm{sv}}$, and the update rate of the reference class run through the operationalization of boundaries and viability indicators, and $H\mathrm{R}$-1 to 3 depend indirectly on the same batch of quantities through social proxies. The path for closing these gaps is in "Limitations and Open Problems" at the end of the book — only after the metrology is completed do these five become eligible for testing.

***

## Limitations and Open Problems

**Positioning.** The items below are located by the five layers A–E of Chapter 11, "The Fallibility of RIF: Layered Tests": each item marks what a particular layer currently lacks and what is needed to supply it. A tests the procedure, B tests the criteria, C tests the pairing, D tests the social hypothesis, E tests the background convention — when one layer fails, only that layer's protocol is revised.

**Unfinished derivations and unestablished protocols.**

1. **The persistence-relevant time window $W_{\mathrm{sv}}$**: $B^{\mathrm{env}}$ must take frequencies within this window, but there is no protocol for how the window is operationalized. Too short and the frequencies are dominated by short-term fluctuation; too long and cross-generational change is averaged away; only a directional suggestion (take the longest causal time course) can be given.
2. **The detection floor $\iota_D$**: for instruments the rarity corresponding to the resolution limit is taken, for organisms the behavioral response threshold, but how the threshold of a cognitive decoder is stably converted into this floor has no protocol yet; this gap directly determines the boundaries of the two persistence times.
3. **The delimitation of the "optimal response"**: $\delta_r$ depends on it, and it in turn depends on the delimitation of the response repertoire; the testability of $H\mathrm{R}\text{-}4$ through $H\mathrm{R}\text{-}7$ all rests on this one item.
4. **The determination of the reference class**: the examples of Chapter 13 specify reference classes by intuition, and their gap from $B^{\mathrm{env}}$ is unknown; the partition rule of "persistence equivalence" has only a necessary condition and no algorithm.
5. **Non-energy conversion of $E$**: how costs such as money and time are converted into J has no protocol; until then $E_{\mathrm{causal}}$ gives numerical values only for cases that can be measured directly in energy.
6. **Apportionment of shared costs**: how to apportion when one expenditure supports several holders has no algorithm; when it cannot be apportioned, mark "unapportionable" — this discipline leaves a gap in the books.
7. **The transformation class of rule depth**: depth is defined relative to "which transformations are allowed", but the transformation classes have no standard list; the shortest description can generally be given only an upper bound.
8. **Measurement of the multi-holder union**: $T_{\mathrm{causal}}$ takes the union at the channel level, and how to measure it in large-scale social cases has no operability.
9. **Action binning**: $I_{\mathrm{pragmatic}}$ depends on how the action space is coarse-grained, and results vary with the binning.
10. **Identification of long-duration, hard-to-intervene causal effects**: for objects such as policies, institutions, and social relations, the effects last long and are hard to intervene on randomly, and there is no recomputable control design (§12.9.8, item 2).
11. **Qualification of collective holders**: whether families, firms, organizations, and the like can satisfy criterion ① (a self-maintained boundary) is not argued in this book; until then, research on everyday information takes the individual person as the holder.
12. **The triplet as a record projection: injectivity undetermined.** Whether the I–T–E record maps different objects to different triplets depends on the admissible object domain and on the criterion for "two objects being different"; both are undetermined, so injectivity is registered as unknown, not as a confirmed conclusion. Under a simplified protocol that reads only node count, edge count, and energy, examples with "the same triplet, different relational organization" can be constructed, but that is a conditional illustration, not an existence proof within the domain of admissible persistent structures; no counterexample under the full definitions has been found, and no injectivity proof exists either. What is needed: first fix the object domain and the object equivalence relation, then check the map under the full definitions. Until then, no record coordinate is added, and "topological form" is not written up as a formal chapter.

**Uncalibrated parameters.** The domain-specific value of the equivalence bound $\delta_{\mathrm{eq}}$ (the conventional value $0.2$ is provisionally used, not domain-based); the significance level $\alpha_0$ (default $0.05$, $0.01$ for high-stakes); the entry threshold for causal readings (3 bit, 5 bit for high-stakes); the iteration cap $N_{\mathrm{iter}}$ (about 5 suggested); the boundary of the online-type region on the three axes of $D_{\mathrm{cog}}$; and the paired reporting rules for the smoothing parameter and the sample size of $B^{\mathrm{env}}$. These numbers are all **conventions**, not natural constants; they may be changed for a different domain, but must be declared in advance.

***

## Appendix A — Symbols and Units at a Glance

This appendix lists only the symbols and terms that actually appear in the main text of this book. A "—" in the unit column means that the item is not a quantity and has no unit.

### A.1 Symbols

| Symbol | Unit | Definition |
| :----- | :--------------- | :------------------------------------- |
| PS / $P$ | — | Category of persistent structure / one specific instance (no boundary or decoder presupposed) |
| $D$ | — | The functional link that carries out selective extraction in a self-maintenance process; whether the holder running $D$ qualifies as a decoder is judged separately by the four criteria |
| $D=\varnothing$ / $D_{\mathrm{phys}}$ | — | No extraction link meeting the criteria / a decoder relying on a self-maintained physical boundary, whose extraction takes part in maintaining its own persistence |
| $D_{\mathrm{cog}}$ | — | The region of the decoding-complexity space where the three axes reach the online type or above, superimposed on $D_{\mathrm{phys}}$ |
| $D_{\mathrm{macro}}$ | — | The commensurable public part of the measurement protocols used by multiple holders; no single holder |
| $D_{\mathrm{depth}}=n_D(P)$ | rules | The minimum number of independent rules needed to reconstruct $P$ within tolerance; the $D$ is taken from depth |
| $\operatorname{Dom}(D)$ | — | $P$ lies within $D$'s effective measurement range |
| $B^{\mathrm{env}}$ | probability distribution | Habitat background: the natural frequency of readings in the holder's habitat within the persistence-relevant time window; the default convention |
| $B^{\max}$ | probability distribution | Protocol baseline: the reference distribution specified by the protocol — the maximum-entropy (equiprobable) distribution when there is no energy constraint, and the maximum-entropy distribution under that constraint when there is one (the regular equilibrium distribution of §12.2 is one example); must be declared explicitly |
| $B_{\mathrm{int}}$ / $B_0$ | probability distribution | The internal model acquired by the holder (its difference from $B^{\mathrm{env}}$ is the decoding deviation) / control baseline |
| $I_{\mathrm{struct},D}(P)$ | bit | How rare the reading $r=D(P)$ is relative to the declared background; within Chapter 12 it may be abbreviated $I_D(P)$ (§12.2) |
| $I_{\mathrm{causal},D}(P)$ | bit | How rare the effect $e$ is relative to the control baseline $B_0$ |
| $I_{\mathrm{net}}$ | bit | Composite index of the two channels; not defined in this book |
| $I_{\mathrm{pragmatic}}$ | bit | Information gain of the action distribution before and after a reading; candidate operationalization of $I_{\mathrm{causal}}$ |
| $T_{\mathrm{struct},D}$ / $T_{\mathrm{causal},D}$ | s | Total time during which a reading is above the detection floor and still in the same identification class / total time during which the effect is identifiable, has a response, and has a measurable cost paid for it |
| $T_{\mathrm{causal}}^{\cup}$ | s | Union, at the channel level, of the holders' $T_{\mathrm{causal}}$ time sets; not mixed with single-holder readings |
| $E_{\mathrm{struct},D}$ / $E_{\mathrm{causal},D}$ | J | Actual energy cost of the structural channel / measurable decoding energy consumption of the holder in reading out and identifying the effect |
| $E_{\mathrm{build}}$ | J | Responsive expenditure on the maker's side; serves only as qualification evidence and is not counted in $E_{\mathrm{causal}}$ |
| $E_{\mathrm{meas}}$ | J | Protocol costs such as instruments, calibration, and recomputation; not recorded in any holder's $E_{\mathrm{causal}}$ |
| $W$, $\mu$, $W_{\mathrm{sv}}$ | —, s, s | The observation window, its measure, and the time window taken for determining habitat-background frequencies |
| $r$, $s(\cdot)$ | — | The feature read out / the ordered statistic mapping a reading or effect to a sortable scalar |
| $\iota_D$ | bit | Detection floor: if a reading's rarity is below it, $D$ cannot read that reading |
| $I_{\mathrm{min}}$ | bit | Structural maintenance floor (below this value, the structure no longer possesses the informational organization needed to maintain identity; this book only registers the threshold so as to distinguish it from the reader-side $\iota_D$, and does not give a protocol for estimating it) |
| $\mathrm{sv}$ | depends on the index | The holder's measurable viability indicator (survival rate, resource-acquisition success rate, etc.) |
| $\delta_r$ / $\delta_{\mathrm{eq}}$ | same as $\mathrm{sv}$ / same as the effect size | The persistence difference of the optimal response under a reading / equivalence bound |
| $\alpha_0$ | dimensionless | Pre-registered significance level, default 0.05 |
| $\Gamma_D$ | 0 or 1 | Takes 1 when the three conditions for a causal effect hold at once |
| $N_{\mathrm{iter}}$ | iterations | Maximum number of iteration rounds in boundary identification |
| $\xi$, $a$ | — | Environmental cue / the holder's response |
| $q_D(a)$, $p_D(a\mid r)$ | probability distribution | The action distribution before and after the reading |
| $h_t$ | — | The internal state used in the candidate definition of history dependence |
| $p_{\mathrm{tail}}$, $q$ | dimensionless | The position of an effect in the control distribution (not the test $p$ value) / the tail-probability half-width of the equivalence band |
| $P_0$, $P_{\mathrm{cand}}$ | — | A control object equivalent to $P$ but lacking "that rule or that identification" / the candidate object to be measured in boundary identification |
| $\mathcal{C}_0$ | — | The initial candidate boundary set: the union of substrate, functional, and observer-reachable candidates |
| $L_D(P)$, $F_{\mathrm{scale}}$, $G_{\mathrm{comp}}$, $\varepsilon_{\mathrm{tol}}$ | bit, times, bit, same as the reading | Total rule description length / number of repeated unfoldings / compression gain / reconstruction tolerance |
| $u\sim_D v$ | — | $u$ and $v$ fall in the same identification class of $D$; a tolerance relation, not transitive |
| $\mathcal{T}$ | — | Topological transition: the protocol opens a new causal dimension that the old protocol cannot express |
| $\Delta U_{\mathrm{barrier}}$, $\varepsilon_{\mathrm{cell}}$ | J | Barrier height (≠ the energy paid) / per-cell energy difference |
| $\lambda_{\mathrm{flip}}$, $\tau_0$ | $\mathrm{s^{-1}}$, s | Storage-cell flip rate / trial time scale |
| $\tau_{\mathrm{proc}}$, $t_{\mathrm{refresh}}$ | s | Processing refresh period / storage refresh period; the two are not interchangeable |
| $T_{\mathrm{thermo}}$, $\dot E$ | K, W | Ambient temperature (a bare $T$ is not written) / instantaneous power ($P$ is not written) |
| $I_{\mathrm{Sh}}(x)$ / $H(X)$ | bit | Comparison notation of Chapter 2: the Shannon self-information of a single outcome in a given source / source entropy; not RIF-specific quantities |
| $S_m(o)$ | nat | Comparison notation of Chapter 2: the surprise of observation $o$ under generative model $m$; used for the FEP explanation, not a RIF-specific quantity |
| $x$, $X$, $o$, $m$ | — | Comparison notation of Chapter 2: discrete outcome, source random variable, observation, generative model |

**Symbol-conflict check.** Three rules: one symbol denotes only one quantity; the same quantity has the same name in all chapters; where there is a conflict with common physical notation, yield to it. Hence $P$ is reserved for persistent-structure instances, power is written $\dot E$, and probability is written $\Pr$; the $T$ family always denotes time, and temperature is written $T_{\mathrm{thermo}}$; the subscript of $D_{\mathrm{depth}}$ is taken from depth rather than the decoder, and this is the only exception.

***

## Appendix B — An Inventory of Prior Work

### B.1 Eight Locally Similar Frameworks and Their Grading

The frameworks below are highly similar to RIF in one respect or another, but none treats RIF's core problem — **information, time, and energy must be aligned**: for the same $P$, the same $D$, and the same record, $I$, $T$, and $E$ hold at once. Those that touch only one or two of them are all merely locally similar.

| Framework | Similar aspect | Where it does not align | Grade |
| :--------------- | :-------------- | :------------------- | :-------- |
| Computational mechanics / causal emergence (Crutchfield, Hoel) | Where structure comes from; minimal generative structure | Does not treat E; the $\epsilon$-machine is a statistical reconstruction, not an ontological criterion | Locally similar |
| Relational biology (Rosen) | Relation rather than matter; relational closure | Discusses only life; no record framework | Locally similar |
| Algorithmic information theory (Kolmogorov, Chaitin) | Shortest description | Measures length, not number of rules; does not treat T or E | Close formal tool |
| Semantic information / strongly semantic information (Floridi) | For whom information is meaningful | Philosophical analysis; no measurement protocol | Related in problem |
| Biosemiotics (Uexküll, Hoffmeyer) | Every organism has its own Umwelt | Discusses only organisms; no alignment | Conceptual precursor |
| Autopoiesis theory (Maturana, Varela) | The boundary is produced by the system's own processes | Discusses only life; no quantitative alignment | Conceptual precursor |
| Markov blanket / free energy principle (Friston) | Probabilistic formulation of the inside/outside division | The background is taken from the subject's own generative model; T is not an independent dimension | Structural neighbor |
| Process philosophy (Whitehead) | Process before entity; "type" and "instance" in parallel | Metaphysics; not measurable | Philosophical kin |

RIF's difference from each can be compressed into one sentence: this book binds the "self-maintained boundary" to the $(I,T,E)$ record, and requires the triplet record to be aligned on the same $P$ and the same $D$, without being confined to cognitive systems or living systems. This is a methodological commitment, not a statement that cross-domain universality has been proven.

"Rarity" is formally self-information, of the same form as the surprise in the free energy principle. RIF keeps the name in order to stress rarity relative to a background, and not to stress that the formula is new; the difference lies only in where the background comes from — constructed from the holder's persistence constraints ($B^{\mathrm{env}}$), or given by the protocol-specified maximum-entropy baseline ($B^{\max}$). **Within the scope of this book's survey**, no unified terminology has been found that combines "persistence constraints, cross-scale, separation of two classes of information, cost side counted in $E$, and a binary background"; this is the reason for the naming, not an assertion that the field "has no such definition yet".

### B.2 One Sentence and Adjacent Literature

> **Within the scope of this book's survey, no prior framework has been found that directly corresponds to "the same $P$, the same $D$, the same I–T–E alignment"; the adjacent works below each have their own emphasis, and the item-by-item comparison is in B.3.**

### B.3 The Position of Other Nearest-Neighbor Works

B.1 includes only frameworks that treat the same problem. The eleven works below do not compete with this book on the same problem but are most often taken by readers as nearest neighbors, so what each provides and where it does not align are listed together. Those already named in the main text are not repeated; for those not cited one by one in the main text, this table governs.

| Reference | What it provides | Relation to RIF |
| :---------------- | :------------------- | :---------------------- |
| Hazen et al. (2007), functional information | Measures complexity by "the amount of information needed to reach a given function" | Measures a functional threshold that does not vary with the decoder; no $T$ or $E$ dimensions |
| Krakauer et al. (2020), information theory of individuality | Characterizes levels of individuality by information flow and boundary | Of the same kind as the self-maintained boundary; does not distinguish the structural and causal channels |
| Sharma et al. (2023), assembly theory | Measures selection and evolution by the assembly index | Measures the depth of the construction path; no rarity relative to a background |
| Miller (1978), living systems | A list of systems across eight levels | Descriptive framework; contains no measurement protocol |
| Bateson (1972), difference that makes a difference | Defines information as a difference that makes a difference | Conceptual precursor; no background specification or cost side |
| Dretske (1981), semantics of information | Defines knowledge and representation by information relations | Philosophical analysis; no measurement protocol |
| Premack & Woodruff (1978), theory of mind | A criterion for attributing minds to others | A behavioral criterion; does not involve I–T–E pairing |
| Dunbar (2010), social brain | An order-of-magnitude estimate of social-cognitive capacity | An empirical generalization at a single scale, not a protocol |
| Chalmers (1995), hard problem of consciousness | The explanatory gap of first-person experience | RIF explicitly does not treat this problem; listed to draw the boundary |
| Rovelli (1996), relational quantum mechanics | Physical quantities hold relative to an observer | A source of relationality; does not involve biological decoders or cost attribution |
| Moreno & Mossio (2015), biological autonomy | Defines autonomy by closure of constraints | Of the same kind as the self-maintained boundary; gives no measurable alignment |

The role of this table is positioning, not endorsement: these works each stand on their own and are not rewritten by RIF's definitions; the division of labor between RIF and them is still carried out according to the sentence at the end of B.1.

***

## Appendix C — Simulation Scripts: Setups, Parameters, Results

**What this appendix is.** In the main text there are several readings that can be given only by numerical experiment — a reader cannot work them out with pen and paper, but can recompute them according to the settings here. This appendix collects the **model settings, parameters, and result tables** for these readings; the main text keeps only the few numbers necessary for argument, and marks each place with "(Appendix C, Table C-x)". In this way the main text is not interrupted by data tables, and every number has a home.

**The boundary of this appendix.** All worked examples are run in a **synthetic world**, with ground truth planted by the generating process: what passing these tests shows is that "the criterion can be executed within the model family it declares itself", not that "the world is just so". Hence this appendix's boundary statement: **the internal consistency of a synthetic world cannot be extrapolated into the correctness of a physical setup.**

**Basis of judgment.** All criteria were written into the pre-registered protocol before running, and may not be changed after running. In this round two criteria were changed during execution with disclosure (Q1b, Q1d, reasons below), and the time and reason of the changes are both recorded in the report. Of the 46 judgments, **31 passed, 13 failed, and 2 were undecidable** — failed items are also listed in the tables. One of these deserves naming here: the full-KL discrimination test of Table C-5, $\mathrm{AUC}=0.394$, is below chance, and $G$ does not hold as an action-level reading; the mechanism and the alternative reading ($A$'s $\mathrm{AUC}=0.880$) are in that table.

### C.1 Unified Settings

| Item | Value |
| :-------------------- | :-------------------------------------- |
| Interpreter and libraries | Python 3.13.13 / numpy 2.5.4 / scipy 1.18.1 / matplotlib 3.11.2 |
| Main random seed | `20261103` (each module derives from it; the seed is written in the scripts) |
| Nature of data | All synthetic worlds, no measured data |
| Pre-registration | Criteria fixed before running; changes must be disclosed (see "Basis of judgment" above) |
| Reproduction command | See C.9 of this appendix |

### C.2 Table C-1 — Rarity Benchmarks and Discrete Offsets (§12.1, §12.2, §12.1.1)

**(a) Continuous background.** For three continuous distributions (normal, exponential, uniform), the KS test of the tail probability gives $p>0.01$, the median of $I$ is **1.000** and the mean is **1.4427** bit. This is a direct result of the probability integral transform, and should be so.

**(b) Finite support.** Under uniform $K$-point support $\mathbb E[I]=\log_2K-\frac1K\log_2(K!)$, with error against exact enumeration $<10^{-12}$:

| $K$ | 2 | 4 | 8 | 16 | 64 | 256 | 1024 |
| :------- | ------: | ------: | ------: | ------: | ------: | ------: | ------: |
| $\mathbb E[I]$ (bit) | 0.500 | 0.854 | 1.088 | 1.234 | 1.375 | 1.422 | 1.437 |

**(c) Non-equiprobable discrete.** For the binomial reading $\mathrm{Bin}(100,\tfrac12)$: median **0.890** bit (the unique value), mean **1.318** bit; $\sum_r\Pr_B(r)^2=0.0563$, $\mathbb E_B[p_{\mathrm{tail}}]=0.528$. The $k=50$ reading of 0.890 bit in §12.2 **coincides exactly** with this median (a difference of 0.000), so its gap from the 1-bit benchmark has already reached 11%.

**(d) Two backgrounds.** Daylight example: $B^{\mathrm{env}}$ 0.15 bit, $B^{\max}$ ($K=4096$) 12.00 bit, probability ratio **×3686**; perfect crystal example: 4.32 vs 12.00 bit, probability ratio ×205. The rarity orderings of the four readings under the two backgrounds are **reverses of each other**, and the proportion in which the reversal holds under $\pm10\%$ perturbation is **1.000**.

**Disclosure**: Q1b's original criterion "under uniform discrete support the median $\in[0.98,1.02]$" is formally not executable — at $K=2$ both 0 and 1 are medians; the criterion actually adopted in this appendix is "the mean agrees with the closed form and converges monotonically with $K$." Q1d's sign convention follows the current definition. Neither changes the conclusion in order of magnitude.

![Figure C.1. Rarity Benchmarks and Discrete Shift](figures_en/release/fig_c1_rarity_benchmarks.pdf)

**Figure C.1. Rarity Benchmarks and Discrete Shift.** (a) Cumulative distribution of the tail probability: the continuous background falls on the diagonal, the discrete background falls entirely below the diagonal, with the offset given by $\mathbb E[p]=(1+\Sigma p^2)/2$; (b) convergence of the mean with support $K$ under uniform discrete support, the blue band being the interval of "non-unique median" and the red dotted line the actual value for the binomial background; (c) relation between quantization step and median. 1 bit and 1.44 bit are the limits as $K\to\infty$, and 0.890 bit is the shifted median under finite support.

![Figure C.2. Order-of-Magnitude Gap and Ranking Reversal Between the Two Backgrounds](figures_en/release/fig_c2_background_reversal.pdf)

**Figure C.2. Order-of-Magnitude Gap and Ranking Reversal Between the Two Backgrounds.** (a) Cross-convention rarity for the two named examples, daylight and the perfect crystal, with the probability ratios ×3686 and ×205 marked; (b) the same set of readings gives **opposite rankings** under $B^{\mathrm{env}}$ and $B^{\max}$. The two conventions answer two different questions — rare for whom / how special formally; mixing them makes not only the numbers incomparable, the ranking itself flips.

### C.3 Table C-2 — Boundary Identification (§12.8)

Synthetic world: $8\times8=64$ cells. The ground-truth boundary is given by the generating process and is unrelated to the I–T–E criteria: the 12 members of clique A plus four remote energy-supplying cells, **16** in all; in addition 10 free-riding shell cells and clique B (9+2) serve as distractors. 80 repetitions per world, two world types, $\iota_D\in\{0.5,1,2\}$.

| Method | Jaccard ($\iota_D=1$, homogeneous redundancy, median) | Members |
| :----------------------- | -----------------------: | -----------: |
| **Functional closure** only | **0.727** | 22 |
| **Substrate connected components** only | 0.462 | 22 |
| Union of the three sources $C_0$ (no iteration) | 0.381 | 42 |
| **Pairing test** only (iterative) | 0.432 | — |
| **Minimally sufficient set** (by $T$, iterative) | 0.338 | 35 |
| **Maximum-$I$ expansion** (iterative) | 0.348 | — |

**Two key readings of Table C-2:**

1. **The pairing criterion is monotone with respect to supersets.** In **100%** of worlds, **all 64 cells of the full grid** pass the I–T–E pairing test — as long as all three can be computed, the full set qualifies. So a "qualifying boundary" is at most a "qualifying description".
2. **The discriminating power lies in the candidate source, not in iteration.** The best of the four compliant outputs is only **0.051** higher than the non-iterated union of three sources ($<0.10$), and lower than the most naive "substrate only" (0.462), and far lower than "functional closure only" (0.727).

![Figure C.3. Boundary Identification: Candidate Sources and Compliant Outputs](figures_en/release/fig_c3_boundary_identification.pdf)

**Figure C.3. Boundary Identification: Candidate Sources and Compliant Outputs.** The four panels on the left show one example world with seed `20261103` (ground truth 16, substrate 22, functional closure 18, observer-reachable 24), with the black dashed box marking the ground-truth boundary. The right panel shows medians over 80 repetitions: functional closure 0.727, substrate 0.462, and the four compliant outputs 0.34–0.43; these medians must not be conflated with the example-world membership counts. The discriminating power lies in the candidate source, not in the number of iterations.

### C.4 Table C-3 — Coarsening Order (§12.9.3, HR-6)

24 ordered cues, six actions, three action steps. The optimal coarsening path is found exactly by one-dimensional DP, recording the critical value at each $\lambda$, and its ordering is the optimal dropping order. The cost heterogeneity $\sigma_c/\bar c$ runs from 0 to 1.

| $\sigma_c/\bar c$ | $\tau$ with $\lvert\delta_r\rvert$ | $\tau$ with $\delta_r/c$ | $\tau$ with signal strength $S$ |
| -----------: | -------------: | -------------: | -------------------: |
| 0.0 | **0.720** | 0.720 | −0.604 |
| 0.2 | 0.689 | 0.707 | −0.589 |
| 0.4 | 0.690 | 0.749 | −0.585 |
| 0.6 | 0.663 | 0.788 | −0.572 |
| 0.8 | 0.562 | 0.672 | −0.422 |
| 1.0 | **0.555** | **0.741** | −0.447 |

**Three readings:**

1. **The direction holds**: the agreement with $\lvert\delta_r\rvert$ is clearly higher than with signal strength ($\tau\approx0.6$–$0.7$ vs $\approx-0.5$).
2. **But "drop the smallest $\lvert\delta_r\rvert$ first" is not the optimal order**: even with $\sigma_c=0$, $\tau$ is only **0.720**. The reason is that **gains are not additive** — the joint benefit is **1.26–1.35 times** the sum of pairwise gains, with interaction between adjacent steps.
3. **With heterogeneous costs it is decided by $\delta_r/c$**: at $\sigma_c=1$, 0.741 vs 0.555, a difference of 0.186 (the pre-registration required ≥0.20 to pass, falling short by 0.014 and missing the line, but the direction is consistent for $\sigma_c\ge0.2$).

**Power check up front**: the measured Spearman correlation between $\mathrm{rank}(\lvert\delta_r\rvert)$ and $\mathrm{rank}(S)$ is **−0.80 to −0.82** (below −0.5 required).

![Figure C.4. Coarsening Order Is Decided by the Gain–Cost Ratio](figures_en/release/fig_c4_coarsening_order.pdf)

**Figure C.4. Coarsening Order Is Decided by the Gain–Cost Ratio.** (a) Medians over 80 repetitions: Kendall $\tau$ between the three orderings and the optimal dropping order as cost heterogeneity varies, equal to 0.720 at $\sigma_c=0$. Panels (b) and (c) show one example world with seed `20261103`, relating $|\delta_r|$ to signal strength and to critical $\lambda$; the example Kendall $\tau=0.69$ is not conflated with the median in (a). With heterogeneous costs $\delta_r/c$ is higher than $|\delta_r|$ (0.741 versus 0.555), but the difference 0.186 does not reach the pre-registered 0.20 line.

### C.5 Table C-4 — Operating Characteristics of the Two-Step Test (§13.3.2, §13.3.3)

Convention: the effect size is the standardized mean difference, $B_0=\mathcal N(0,1)$, the treatment group $\mathcal N(d,1)$; step one is done on $n$ versus $n$, and in step two $e_{\mathrm{obs}}$ is **a single observation**, with $B_0$ estimated from $n$ control samples. The tail probability uses empirical counts, and the interval uses the Clopper–Pearson exact method.

| Item | Measured |
| :--------------------- | :------------------------------------- |
| Zero-effect admission rate (3 bit only) | **0.119** (≈1/8) |
| Zero-effect admission rate (both steps) | **0.005** |
| $\Pr(I\ge3)$ when the $B_0$ conventions are mixed | **0.000** (correct convention 0.119) |
| Pass rate when the true value is 3 bit ($n$ 50→1200) | **0.35–0.47**, never reaching 0.8 |
| Equivalence-band conversion versus the main text's "$1\pm0.14$ / $1\pm0.29$ bit" | At $q=0.05$ the approximation deviation is about 0.007 bit; at $q=0.10$ about 0.03 bit, with the main text giving the exact expression; the earlier "error 0.0048 bit" corresponds only to a smaller $q$ |

**Effective threshold** (the true $I$ needed to bring the power of the strict reading to 0.8):

| $n$ | 50 | 100 | 200 | 500 |
| :----------------- | ----------: | ----------: | ----------: | ----------: |
| Effective threshold (bit) | **7.20** | **6.77** | **6.23** | **6.03** |

**Resolution ceiling**: with $+0.5$ smoothing $\hat p\ge0.5/(n+1)$, so the maximum reportable $I$ is $\log_2 2(n+1)$ — at $n=20$ only **5.4 bit**. A small sample cannot possibly report a high rarity; this is the ceiling of the estimator itself, not conservatism.

![Figure C.5. Operating Characteristics of the Two-Step Test](figures_en/release/fig_c5_two_step_oc.pdf)

**Figure C.5. Operating Characteristics of the Two-Step Test.** (a) Admission rate in a zero-effect world: with 3 bit alone it stays at 1/8 (0.119), and doing both steps presses it to 0.005; (b) power curve of the strict reading — with a true value of 3 bit, increasing $n$ from 50 to 1200 still brings the pass rate only to 0.47; (c) selection bias: the $I$ reported by admitted samples is systematically higher than the true value. 3 bit is not a gate, but a stretch of distance between two gates.

### C.6 Table C-5 — Discriminating Power of the Action Layer versus Full KL (§13.9, HR-7)

Eight classes of cues, four actions; the holder estimates $B_{\mathrm{int}}$ by exponential weighting and takes the optimal action according to $B_{\mathrm{int}}$; $\pi_t$ changes abruptly at $t=200$ (magnitude $\Delta$) or drifts at a uniform rate ($\omega$). The consequence reading takes the **expected payoff loss** (less noisy than the 0/1 error rate), with a lookahead window of 10 steps. Two candidate predictors: $G=D_{\mathrm{KL}}(\pi_t\|\hat\pi_t)$ and $A=D_{\mathrm{KL}}\big(p(a|\pi_t)\|p(a|\hat\pi_t)\big)$.

| Item | Measured | Verdict |
| :-------------------------- | :--------------------- | :---------: |
| Pooled correlation of $G$ with consequence | $r=-0.185$; dose–response Spearman $-0.16$ | Fail |
| $\mathrm{AUC}(G)$ | **0.394** (below chance) | Fail |
| Residual $G$ after controlling for $\Delta,\eta,\omega$ | $\mathrm{AUC}=0.757$, partial correlation $0.130$ | Pass |
| Held-out prediction: RMSE after adding $G$ | Reduced by only $-1.1\%$ | Fail |
| $\mathrm{AUC}(A)$ | **0.880**, **0.487** above $\mathrm{AUC}(G)$ | Pass |

**Mechanism**: right after an abrupt change $G$ is large, but the action has not yet changed (argmax is insensitive to distribution perturbation) and the loss is zero; when a real error occurs, $G$ has often already fallen back. **Full KL measures "how far off the model is", not "how far off the decision is."**

![Figure C.6. Decoding Deviation and Errors](figures_en/release/fig_c6_decoder_bias.pdf)

**Figure C.6. Decoding Deviation and Errors.** (a) Time series for one world ($\Delta=0.4$, $\eta=0.05$): $G$ jumps at the mutation, and the error rate rises only afterward; (b) pooled scatter, $r=-0.185$; (c) scatter of residuals after removing $\Delta,\eta,\omega$, $r=+0.130$, with the **sign flipped**. Model error and decision error are not the same thing, and the former can even run in the opposite direction — this is why full KL cannot by itself serve as an action-level reading.

### C.7 Table C-6 — Rule Depth and the Calibration Regression (§14.4, §14.7)

$32\times32$ binary grids, with a rule library of 30 rules (all-0 / all-1, vertical and horizontal stripes, checkerboard, blocks, diagonals); first screened by GF(2) linear independence, to guarantee that "how many were used in generation" agrees with "the minimum number", otherwise the true depth is undefined. Objects are generated by XOR of 1–3 basic rules, and the inversion uses in-library MDL exhaustive search up to depth 3.

| Item | Measured |
| :--------------------------- | :------------------------------- |
| In-library depth recovery rate | **1.00** |
| Out-of-library rule recovery rate | **0.00** (25/25 consistently **underestimated**) |
| Kendall $\tau$ between length and depth | 0.41 |
| Purely random object: length / depth | 139 bytes / **0** (the longest in-library is only 44 bytes) |
| Proportion with $\hat G_{\mathrm{comp}}>0$ (the two rule-bearing types) | 1.00 / 0.98 |
| Proportion with $\hat G\le0$ (random / pseudorandom) | 1.00 / 1.00 |
| Regression $\hat b$ (§14.7, item 1) | **1.29**, $b=1$ rejected at $p=9.2\times10^{-7}$ |

**Calibration regression (§14.7, item 1).** Generation setup: each transition adds 1–3 independent rules, of which about 20% of transitions only reorganize. **The pre-registered prediction did not pass**: the prediction was $\hat b\in[1.7,2.4]$, and the measured 1.29 falls outside the interval. What follows is a post hoc explanation — "the prior expectation should be $b>1$, but the specific value cannot be preset" is still consistent in direction, and the order of magnitude must be settled by calibration; this explanation does not constitute a pass verdict on the pre-registered test.

![Figure C.7. Rule Depth and Compression Gain](figures_en/release/fig_c7_rule_depth.pdf)

**Figure C.7. Rule Depth and Compression Gain.** (a) Description length versus true depth: within the same depth the length varies by a factor of 3, and out-of-library points have the highest length while depth is recorded as 0; (b) $\hat G_{\mathrm{comp}}$ for four kinds of placement — periodic and equidistant-with-jitter are positive, random and pseudorandom are zero; (c) comparison of the calibration regression $\hat b=1.29$ with $b=1$. Depth, length, and scale each do their own work; $\hat G\approx0$ cannot confirm the absence of a rule.

### C.8 Figure Index

The seven figures correspond one to one with the tables above and the added boundary-identification example, and **have been inserted after the tables of this section** (figures go with the text, no longer piled together). Each figure comes with PNG and PDF versions of identical content; the main text always cites the PDF (vector version). Figure text follows the language of the book: Chinese figures use Chinese and English figures use English, while mathematical symbols and numbering remain unchanged; mathematical symbols go through mathtext, of the same origin as the main text's LaTeX notation. Figures use a consistent black-white-gray system with line styles and markers to distinguish statistical objects; they do not depend on color semantics.

| Figure | File name (same name in both formats) | Corresponds to |
| :-------------: | :--------------------------- | :---------------: |
| Figure C.1 | `fig_c1_rarity_benchmarks` | Table C-1 |
| Figure C.2 | `fig_c2_background_reversal` | Table C-1(d) |
| Figure C.3 | `fig_c3_boundary_identification` | Table C-2 |
| Figure C.4 | `fig_c4_coarsening_order` | Table C-3 |
| Figure C.5 | `fig_c5_two_step_oc` | Table C-4 |
| Figure C.6 | `fig_c6_decoder_bias` | Table C-5 |
| Figure C.7 | `fig_c7_rule_depth` | Table C-6 |

### C.9 Reproduction

The full scripts and results summary (including environment, seeds, and item-by-item verdicts) are included in the accompanying reproducibility package at `reproducibility/`.

Published on Zenodo: DOI 10.5281/zenodo.24349831. Run the entry command for this appendix from inside `reproducibility/`:

```bash
(cd batch_B/sim && python run_all.py)   # ~3 min, no GPU
```

With the same environment and the same BLAS thread count, the results summary should be bit-for-bit identical (fixed seeds); across environments bit-for-bit identity is not promised, and only the verdict conclusions of Tables C-1 to C-6 are promised unchanged. If they differ, check the numpy / scipy versions first, then the thread count — the associativity of floating-point summation changes with the thread count.

***

## References

Numbering is grouped by topic: 1–6 are main-line near neighbors, 7–10 are foundational tools, 11–45 are related traditions and background, 46 is the free energy principle, 47 is the sister framework cited by this book. Where the main text first mentions prior work by a transliterated name, the entry in this section gives the original.

1. Kolchinsky, A., & Wolpert, D. H. (2018). Semantic information, autonomous agency and non-equilibrium statistical physics. *Interface Focus*, 8, 20180041. https://doi.org/10.1098/rsfs.2018.0041
2. Kolchinsky, A., & Wolpert, D. H. (2021). Work, entropy production, and thermodynamics of information under protocol constraints. *Physical Review X*, 11, 041024. https://doi.org/10.1103/PhysRevX.11.041024
3. Barato, A. C., & Seifert, U. (2015). Thermodynamic uncertainty relation for biomolecular processes. *Physical Review Letters*, 114, 158101. https://doi.org/10.1103/PhysRevLett.114.158101
4. Nicholson, S. B., García-Pintos, L. P., del Campo, A., & Green, J. R. (2020). Time–information uncertainty relations in thermodynamics. *Nature Physics*, 16, 1211–1215. https://doi.org/10.1038/s41567-020-0981-y
5. Still, S., Sivak, D. A., Bell, A. J., & Crooks, G. E. (2012). Thermodynamics of prediction. *Physical Review Letters*, 109, 120604. https://doi.org/10.1103/PhysRevLett.109.120604
6. Weinberger, E. D. (2002). A theory of pragmatic information and its application to the quasi-species model. *BioSystems*, 66(3), 105–119. https://doi.org/10.1016/S0303-2647(02)00038-2
7. Shannon, C. E. (1948). A mathematical theory of communication. *Bell System Technical Journal*, 27, 379–423, 623–656. https://doi.org/10.1002/j.1538-7305.1948.tb01338.x
8. Kolmogorov, A. N. (1965). Three approaches to the quantitative definition of information. *Problems of Information Transmission*, 1, 1–7.
9. Bennett, C. H. (1988). Logical depth and physical complexity. In R. Herken (Ed.), *The Universal Turing Machine* (pp. 227–257). Oxford University Press.
10. Floridi, L. (2011). *The Philosophy of Information*. Oxford University Press. https://doi.org/10.1093/acprof:oso/9780199232383.001.0001
11. Hazen, R. M., Griffin, P. L., Carothers, J. M., & Szostak, J. W. (2007). Functional information and the emergence of biocomplexity. *PNAS*, 104(Suppl 1), 8574–8581. https://doi.org/10.1073/pnas.0701744104
12. Krakauer, D. C., Bertschinger, N., Olbrich, E., Flack, J. C., & Ay, N. (2020). The information theory of individuality. *Theory in Biosciences*, 139, 209–223. https://doi.org/10.1007/s12064-020-00313-7
13. Sharma, A., Czégel, D., Lachmann, M., Kempes, C. P., Walker, S. I., & Cronin, L. (2023). Assembly theory explains and quantifies selection and evolution. *Nature*, 622, 321–328. https://doi.org/10.1038/s41586-023-06600-9
14. Bertalanffy, L. von (1968). *General System Theory*. George Braziller.
15. Wiener, N. (1948). *Cybernetics*. MIT Press.
16. Maturana, H. R., & Varela, F. J. (1980). *Autopoiesis and Cognition*. D. Reidel. https://doi.org/10.1007/978-94-009-8947-4
17. Rosen, R. (1991). *Life Itself*. Columbia University Press.
18. Miller, J. G. (1978). *Living Systems*. McGraw-Hill.
19. Friston, K. (2013). Life as we know it. *Journal of the Royal Society Interface*, 10, 20130475. https://doi.org/10.1098/rsif.2013.0475
20. Uexküll, J. von (1934/2010). *A Foray into the Worlds of Animals and Humans* (J. D. O'Neil, Trans.). University of Minnesota Press.
21. Whitehead, A. N. (1929). *Process and Reality*. Macmillan.
22. Bateson, G. (1972). *Steps to an Ecology of Mind*. Chandler.
23. Dretske, F. (1981). *Knowledge and the Flow of Information*. MIT Press.
24. Arrow, K. J. (1951). *Social Choice and Individual Values*. Wiley.
25. Premack, D., & Woodruff, G. (1978). Does the chimpanzee have a theory of mind? *Behavioral and Brain Sciences*, 1(4), 515–526. https://doi.org/10.1017/S0140525X00076512
26. Dunbar, R. I. M. (2010). *How Many Friends Does One Person Need?* Harvard University Press.
27. Goodman, N. (1975). The status of style. *Critical Inquiry*, 1, 799–811.
28. Chalmers, D. J. (1995). Facing up to the problem of consciousness. *Journal of Consciousness Studies*, 2(3), 200–219.
29. Rovelli, C. (1996). Relational quantum mechanics. *International Journal of Theoretical Physics*, 35, 1637–1678. https://doi.org/10.1007/BF02302261
30. Moreno, A., & Mossio, M. (2015). *Biological Autonomy*. Springer. https://doi.org/10.1007/978-94-017-9837-2
31. Landauer, R. (1961). Irreversibility and heat generation in the computing process. *IBM Journal of Research and Development*, 5, 183–191. https://doi.org/10.1147/rd.53.0183
32. Crutchfield, J. P. (2012). Between order and chaos. *Nature Physics*, 8, 17–24.
33. Hoel, E. P., Albantakis, L., & Tononi, G. (2013). Quantifying causal emergence shows that macro can beat micro. *PNAS*, 110, 19790–19795. https://doi.org/10.1073/pnas.1314922110
34. Chaitin, G. J. (1966). On the length of programs for computing finite binary sequences. *Journal of the ACM*, 13(4), 547–569. https://doi.org/10.1145/321356.321363
35. Hoffmeyer, J. (2008). *Biosemiotics: An Examination into the Signs of Life and the Life of Signs*. University of Scranton Press.
36. Chaisson, E. J. (2001). *Cosmic Evolution: The Rise of Complexity in Nature*. Harvard University Press.
37. Eisenberger, N. I., Lieberman, M. D., & Williams, K. D. (2003). Does rejection hurt? An fMRI study of social exclusion. *Science*, 302(5643), 290–292. https://doi.org/10.1126/science.1089947
38. Gilbert, W. (1986). Origin of life: The RNA world. *Nature*, 319(6055), 618. https://doi.org/10.1038/319618a0
39. Howard, R. A. (1966). Information value theory. *IEEE Transactions on Systems Science and Cybernetics*, 2(1), 22–26. https://doi.org/10.1109/TSSC.1966.300113
40. Kleiber, M. (1932). Body size and metabolism. *Hilgardia*, 6(11), 315–353. https://doi.org/10.3733/hilg.v06n11p315
41. Marmot, M. G., Stansfeld, S. A., Patel, C., North, F., Head, J., White, I., Brunner, E., Feeney, A., & Smith, G. D. (1991). Health inequalities among British civil servants: The Whitehall II study. *The Lancet*, 337(8754), 1387–1393. https://doi.org/10.1016/0140-6736(91)92068-W
42. Martin, W., & Russell, M. J. (2003). On the origins of cells: A hypothesis for the evolutionary transitions from abiotic geochemistry to chemoautotrophic prokaryotes, and from prokaryotes to nucleated cells. *Philosophical Transactions of the Royal Society B*, 358(1429), 59–85. https://doi.org/10.1098/rstb.2002.1183
43. Sims, C. A. (2003). Implications of rational inattention. *Journal of Monetary Economics*, 50(3), 665–690. https://doi.org/10.1016/S0304-3932(03)00029-6
44. Tishby, N., Pereira, F. C., & Bialek, W. (1999/2000). The information bottleneck method. arXiv:physics/0004057.
45. Wächtershäuser, G. (1988). Before enzymes and templates: Theory of surface metabolism. *Microbiological Reviews*, 52(4), 452–484. https://doi.org/10.1128/mmbr.52.4.452-484.1988
46. Friston, K. (2010). The free-energy principle: a unified brain theory? *Nature Reviews Neuroscience*, 11, 127–138. https://doi.org/10.1038/nrn2787
47. LiangRuifeng (2026). *Structure Recursive Viability Dynamics* (SRVD) v1.5, five-volume combined edition, preprint; cited in this book at Volume I §1.2.1, Volume IV §2.1, and the statement of the division of labor in Chapter 11. Released jointly with this book. https://doi.org/10.5281/zenodo.24365889
