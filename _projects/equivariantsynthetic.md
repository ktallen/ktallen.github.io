---
title: "Synthetic equivariant spectra for finite abelian groups and motivic homotopy theory"
collection: projects
draftlink: https://arxiv.org/abs/2510.20197
permalink: /projects/equivariantsynthetic
collaborators: Lucas Piessevaux
collaboratorlinks: https://lucas-piessevaux.github.io
# journalinfo: 
date: 2025-10-23
---
For any finite abelian group $$A$$, we introduce a category of *synthetic $A$-spectra*, which generalizes the category of even $$\mathrm{MU}$$-synthetic spectra introduced by Pstrągowski. For any prime $$p$$, we show that this category is $$p$$-complete equivalent to a cellular subcategory of the $$\mathbb{C}$$-motivic $$A$$-equivariant stable homotopy category, providing it with a purely topological model.

Nonequivariantly, the category of $\mathrm{MU}$-synthetic spectra serves as a categorification of the Adams-Novikov spectral sequence, or equivalently the even filtration over the sphere. We show that our category of synthetic $A$-spectra, and thus cellular $A$-equivariant $\mathbb{C}$-spectra, play an analogous role. I'll give a not-so-brief overview of our work here.

What are synthetic $A$-spectra?
---
We take inspiration from Pstrągowski's work on [synthetic spectra](https://arxiv.org/abs/1803.01804) and the [even filtration](https://arxiv.org/abs/2304.04685) in our definition of synthetic $A$-spectra. Let

$$
\mathrm{Pure}(A) \subset \mathrm{Sp}^A
$$ 

be the subcategory generated under extensions and retracts by $A / H_+ \otimes S^V$, where $H$ ranges over subgroups of $A$ and $V$ ranges over virtual complex representations. We define the category of *synthetic $A$-spectra*,

$$\mathrm{Syn}^A = \operatorname{Shv}_{\Sigma}\left(\mathrm{Pure}(A); \mathrm{Sp}\right),$$

to be the category of additive presheaves which take cofiber sequences in $\mathrm{Pure(A)}$ to fiber sequences of spectra. When $A$ is the trivial group, this recovers Pstrągowski's category of even $\mathrm{MU}$-synthetic spectra, motivating our terminology.

The homotopy of equivariant algebraic cobordism
---
*(Discussed in Sections 4 and 5 of v1)*

The main computational input into our results is a comparision of the homotopy groups of $$\mathrm{MGL}_A$$, the equivariant algebraic cobordism spectrum, to those of its topological analogue $$\mathrm{MU}_A$$. Among other things, we show that there is an isomorphism 

$$
\left(\pi^A_{*, *} \mathrm{MGL}\right)_{p}^{\wedge} \simeq \left(\pi_{*}^A \mathrm{MU}\right)_p^{\wedge}[\tau],
$$

where $$\tau$$ is a class in bidegree $$(0, -1)$$. This is accomplished using the fact that $$\pi_{*, *}^A \mathrm{MGL}$$ for different $A$ assemble into a *global group law*; these are algebraic objects introduced by Hausmann, which he uses to great effect to show that [$\pi_*^A \mathrm{MU}$ is isomorphic to the equivariant Lazard ring](https://arxiv.org/abs/1912.07583). We show a regularity result for the Euler classes in this global group law; this allows for a quite streamlined approach to describing the bigraded homotopy groups of $\mathrm{MGL}_A$.  

An equivariant Chow $t$-structure
---
*(Discussed in Sections 6, 7 and 8 of v1.)*

We can leverage the computational results mentioned above to prove structural results about $A$-equivariant $\mathbb{C}$-motivic homotopy theory, culminating in our $p$-complete topological reconstruction result. Let the category of *cellular $A$-equivariant $\mathbb{C}$-motivic spectra*, 

$$\mathrm{SH}^A(\mathbb{C})^{\mathrm{cell}} \subset \mathrm{SH}^A(\mathbb{C})$$

be the subcategory generated under colimits and desuspensions by $A / H_+ \otimes \mathrm{Th}(V)$, where $H$ are subgroups and $\mathrm{Th}(V)$ are motivic Thom spaces of virtual complex representations $V$ (viewed as a vector bundle over the point). For example, if $\epsilon$ is the one-dimensional complex trivial representation, then $\mathrm{Th}(\epsilon) \simeq \mathbb{P}^1$. Inspired by [Pstrągowski](https://arxiv.org/abs/1803.01804) and [Pstrągowski-Haine](https://arxiv.org/abs/2309.15072), we show that this subcategory can be recovered as sheaves on a smaller subcategory. Specifically, we have an equivalence 

$$\mathrm{SH}^A(\mathbb{C})^{\mathrm{cell}} \simeq \mathrm{Shv}_{\Sigma}(\mathrm{Pure}_{\mathbb{C}}(A); \mathrm{Sp}),$$ 

where $$\mathrm{Pure}_{\mathbb{C}}(A)$$ is the subcategory generated under extensions and retracts by the motives $A / H_+ \otimes \mathrm{Th}(V)$. 

Knowing that it is category of sheaves of spectra endows $\mathrm{SH}^A(\mathbb{C})^{\mathrm{cell}}$ with a canonical $t$-structure, which we call the *Chow $t$-structure* following [Bachmann-Kong-Wang-Xu](https://arxiv.org/abs/2012.02687). The heart of this $t$-structure provides the first evidence that $\mathrm{SH}^A(\mathbb{C})^{\mathrm{cell}}$ encodes the equivariant Adams-Novikov spectral sequence; we have an equivalance 

$$\mathrm{SH}^A(\mathbb{C})^{\mathrm{cell}}_{c = 0} \simeq \mathrm{coMod} \left(\underline{\pi}_{\star}^A \mathrm{MU}^{\otimes 2}\right),$$

where the right-hand side denotes comodules over the Hopf algebroid (in complex representation graded Mackey functors) $$(\underline{\pi}_{\star}^A \mathrm{MU}, \underline{\pi}_{\star}^A \mathrm{MU}^{\otimes 2}).$$ 

A close analysis of this $t$-structure, combined with the computational results from above and an equivariant motivic Adams-Novikov spectral sequence, show us that Betti realization induces an equivalence 

$$\left(\mathrm{SH}^A(\mathbb{C})^{\mathrm{cell}}\right)^{\wedge}_p \simeq \left(\mathrm{Syn}^A\right)^{\wedge}_p$$ 

for each prime $p$. 

Equivariant lifts of $\tau$ and an equivariant even filtration
---
*(Discussed in Sections 9 and 10 of v1.)*

Our proof that $\mathrm{Syn}^A$ recovers motivic homotopy theory relies on carefully understanding the map $\tau: S^{2} \to (\mathbb{P}^1)^{\wedge}_p$, which appears in homotopy of $\mathrm{MGL}_A$ above. As in the nonequivariant case, $\tau$ can be constructed quite formally in $\mathrm{Syn}^A$. However, a new feature of the equivariant setting is that we can construct *more* maps like $\tau$; for any complex $A$-representation $V$, we have a map 

$$\tau_V: S^V \to \mathrm{Th}(V).$$

Under our equivalence, this gives some new maps in equivariant motivic homotopy theory. In the case of $C_2$, [Heller-Voineagu-Østvær](https://arxiv.org/pdf/2202.12366) have detected a similar map $\tau_{\sigma}$ on homology, and Jeremiah Heller has informed me of a geometric construction of it similar in spirit to that of the nonequivariant $\tau$. My guess is that this is a desuspension of $\tau_\lambda$, where $\lambda$ is the complex sign representation; we'll explore this further in future work. For other groups and representations, however, we know of no other such maps, and it is perhaps surprising that we don't need to know of them before proving our equivalence.

The maps $\tau_V$ let us construct an equivariant version of Pstrągowski's [perfect even filtration](https://arxiv.org/abs/2304.04685). We can construct a symmetric monoidal functor from 

$$\mathrm{Syn}^A \to \operatorname{Fil}_{\mathrm{RU}(A)}\left(\mathrm{Sp}^A\right) := \operatorname{Fun}(\mathrm{RU}(A)^{\mathrm{op}}, \mathrm{Sp}^A),$$ 

where $\mathrm{RU}(A)$ is the poset of (isomorphism classes of) virtual complex $A$-representations. We can precompose this with an equivariant version of the synthetic analogue $\nu: \mathrm{Sp}^A \to \mathrm{Syn}^A$ to obtain our even filtration

$$\operatorname{fil}^{\mathrm{ev}}_*: \mathrm{Sp}^A \to \operatorname{Fil}_{\mathrm{RU}(A)}\left(\mathrm{Sp}^A\right).$$ 

We show that our category of synthetic $A$-spectra is described as modules over the even filtration of the sphere; we have an equivalence 

$$\mathrm{Syn}^A \simeq \operatorname{Mod}\left(\operatorname{Fil}_{\mathrm{RU}(A)}\left(\mathrm{Sp}^A\right); \operatorname{fil}^{\mathrm{ev}}_{\star} \left(\mathbb{S}^0_A\right)\right).$$

We then identify $\operatorname{fil}^{\mathrm{ev}}_{\star} \left(\mathbb{S}^0_A\right)$ -- and thus the unit in $\mathrm{SH}^A(\mathbb{C})$ -- to an enrichment of the Adams-Novikov spectral sequence. We have 

$$\operatorname{fil}^{\mathrm{ev}}_{\star} \left(\mathbb{S}^0_A\right) \simeq \operatorname{Tot}_{\bullet} \tau_{\geq \star} \mathrm{MU}_A^{\otimes \bullet + 1},$$ 

where $\tau_{\geq V} X := \Sigma^{V} \tau_{\geq 0} \Sigma^{-V} X.$ When we restrict to trivial representations, this gives (a decalage of) the Adams-Novikov filtration, much like the nonequivariant case. The extra representation filtration shows us that the equivariant motivic unit contains more information than just this; exactly what this is will be explored in forthcoming work.

*Last updated November 4, 2025.*
