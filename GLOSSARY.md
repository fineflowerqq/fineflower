# Glossary — SRVD v1.5

One line per term. Symbols follow the printed edition; the bracketed section refers to the PDF.

## Information family

| Symbol | Term | Definition |
|---|---|---|
| *I*_struct | Structural information | The ordered difference a structure carries in its own organization (lattice, DNA, wiring). |
| *I*_latent | Latent configurational information | Information present but not currently activated (dormant knowledge, uninvoked weights). |
| *I*_causal | Causal information | Information that actually changes the state of a decoder holder, measured against a control baseline. |
| *I*_net | Net effective causal information | The quantity written as *I* in every formula: the active, decoder-extracted information of a structure. |
| *I*⁺ / *I*⁻ / *I*⁰ | Information polarity | Sign assigned by the decoder: increases, decreases, or leaves unchanged the holder's viability. |
| η_D | Decoding efficiency | *I*_active = η_D · *I*_latent; low and roughly constant for physical decoders, learnable for cognitive ones. |
| 𝒵_e | Causal efficiency coefficient | *I*_causal / *E*_causal, in bit/J; a proportional proxy for *V*_c at fixed *T*. |

## Time family

| Symbol | Term | Definition |
|---|---|---|
| *T* | Persistence time | How long the structure remains identifiable as itself. |
| *T*_pred | Endogenous time horizon | The span over which a structure plans for future states; can collapse under stress. |
| *T*_min | Minimum time grain | Physical or computational resolution limit (Planck time, clock cycle, neural response). |

## Energy family

| Symbol | Term | Definition |
|---|---|---|
| *E*_eff | Effective thermodynamic cost | Total energy the structure spends to keep itself in existence. |
| *E*_struct | Structural energy | The standing cost of holding the structure's organization. |
| *E*_causal | Causal-processing energy | The energy spent running the decoder. |
| *E*_build | Construction cost | One-off energy paid at a topological transition. |

## Viability family

| Symbol | Term | Definition |
|---|---|---|
| *V* | Viability potential | Baseline *V* ≈ *I*·*T*/*E*; general power-law with exponents α, β, γ. |
| α, β, γ | ITE elasticity exponents | Response exponents of *V* to information, time and energy; to be measured, not assumed. |
| *V*_obj | Objective viability potential | The thermodynamically real value, *V*_s + *V*_c; cannot be deceived. |
| *V*^virt | Virtual viability potential | The structure's internal estimate of *V*_obj. |
| *V*^val | Value viability potential | The weighted mix the structure actually optimizes. |
| Δ_VV | Decoupling deviation | Difference between virtual and objective viability; the measure of self-deception. |
| χ | Self-referential coupling strength | How strongly the structure's own model feeds back into its dynamics. |
| χ_c | Saddle-node threshold | Bifurcation threshold of the reduced *I*–*V* subsystem, not a free model parameter. |

## Decoder and dynamics

| Symbol | Term | Definition |
|---|---|---|
| *D* | Decoder | Any mechanism with a self-maintained boundary that selectively extracts differences and updates its state. |
| *D*_phys | Physical decoder | Extracts information without an internal predictive model (ion channels, chemotaxis). |
| *D*_cog | Cognitive decoder | Physical decoder plus a predictive model of its own extraction (mammals, humans, embodied AI). |
| PS | Persistent structure | The unit of analysis: anything that maintains identity across time against entropy. |
| ℱ | Recursive unfolding | Adds information inside an existing topology; capacity-bounded. |
| 𝒯 | Topological transition | Changes the topology itself; pays *E*_build once and resets capacity. |

## Named regimes and concepts

| Term | Definition |
|---|---|
| Myopic runaway | A hypothesis: strong self-referential coupling inflates *V*^virt, hijacks *V*^val, collapses *T*_pred, and destroys objective stock. |
| Triple splitting | The division of *V* into objective, virtual and value components. |
| Fivefold recursion | The coupled co-evolution *I* → *V* → *T* → *E* → *D*. |
| Paradigm-breaking information | Information that opens a new causal dimension rather than adding content inside an existing one. |
| Cross-scale | Comparison of structures whose characteristic times and energies differ by many orders of magnitude. |
