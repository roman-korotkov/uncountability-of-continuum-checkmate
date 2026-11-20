# Uncountability of continuum, check

[![DOI](https://zenodo.org/badge/1465076094.svg)](https://doi.org/10.5281/zenodo.24390197)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

## Preface

This article is a culmination of the series Uncountability of Continuum. Its character remains deliberately investigational: rather than offering a finished, self-contained solution, it traces a path of inquiry and invites the reader to follow the same line of thought.

When I was around five or six, walking past my brother's room, I noticed something strange. The geometric pattern on the blanket he used to block out the light from the window was forming a shape completely different from the one I was used to seeing on it. I stared at it intently for hours until I learned to switch the pattern my brain perceived by sheer force of will. At that age, it felt like a mind-blowing discovery: we can perceive the world in completely different ways, and we have the power to influence that. Since then, I developed a habit of finding different perspectives on phenomena - the result of curiosity and deliberate searching sparked by that discovery, which somehow naturally stuck. As I grew older, I noticed a strange thing: the vast majority of people reduce their perception to a single possible perspective, without even suspecting that others exist. Even more than that, they are so attached to that reduction that when you try to show them an alternative picture, they take it as an argument, as an assault on the truth. This trait of human thinking became especially obvious, of course, once the war in Ukraine began. Yet I could never have imagined that this fascinating ability, nurtured by a childhood game, would lead me to understand one of the most controversial problems in mathematics - one that triggered a crisis in its foundations. It turned out that switching between perspectives is a fundamental capacity of human thinking that, unfortunately, fades with age. And it is precisely the inability - or lost ability - to switch between key perspectives of interacting with reality that causes a huge number of problems and paradoxes in mathematics.

Once I realized that there was an alternative perspective connected to Cantor's theorem, my main goal became to pin that picture down. With visual reductions, it is simple: for the most part, the brain does the heavy lifting itself; you just need to know how to guide it. With conceptual mental pictures, though, things are much harder. You can catch only a small fragment of an alternative pattern, which is fairly tough to hold in your head because the brain constantly and treacherously collapses back to its habitual interpretation. At that point, I had only read Cantor's works, and I was reading them through the lens of the modern interpretation - not even suspecting that Cantor himself intuitively knew how to switch between perspectives. Once I started digging into the history, it became clear why things ended up this way. Zermelo axiomatized only a fragment of Cantor's theory, not the whole thing. Von Neumann still grasped the full picture at Cantor's level: in his original system, which later became NBG, the entirety of Cantor's theory is covered, unlike in Zermelo's theory. As a result, a rather primitive mainstream picture took shape by working with a limited fragment of the theory and combining completely different perspectives, where the perspective shifts Cantor used become invisible.

Everything fell into place after that. Thousands of authors writing papers that refute Cantor's theorem aren't losing their minds - they simply haven't lost the childhood ability to switch perspectives. Seriously: did anyone really think there was some kind of mass psychosis where people started looking for an error not in Euclid's theorem and not in Euler's identity, but specifically in Cantor's theorem? The thing is, keeping this ability into adulthood really can look like a pathology. It is pretty resource-heavy for the brain, so evolutionarily this mode is usually limited to childhood, when a system of knowledge about the world is being formed. Later, the brain shifts into an operational mode and switches into the cognitive mode less and less. For example, a mom says, "I don't have ten arms," and a child innocently asks back, "Twenty?" Mom uses a contrary negation in operational mode, while the child takes it contradictorily in cognitive mode, ruling out only the specific option explicitly named. That's a feature of the inquiring brain: in that mode, it can easily create new abstractions and concepts. Cantor's theorem itself is fine - within modern axiomatic systems and the modern system of definitions, it is completely true. Yet the meaning Cantor put into it and the meaning the modern mainstream puts into it are fundamentally different. That's where the error comes from: the mainstream tries to imitate Cantor without understanding him. It's practically a cargo cult in the foundations of mathematics - repeating the arguments without grasping their meaning. As a result, a vicious circle arises in modern theory, only tied to a different theorem. That is, thousands of people intuitively sense the problem, but try to attack it head-on—where everything is clear and sound - while the theory's real Achilles' heel is somewhere else entirely.

In this article, we do not formulate the independence of the mainstream interpretation from the axiomatics as a theorem. Independence would mean that this interpretation is still admissible, and we are not taking that sin upon our conscience. Right now, it is almost impossible to assert this mistake outright, so we have to be careful about it. In the future, however, there will be no doubt about it - and that is where the checkmate comes from. As for Poincaré's famous remark, hopefully we will be able to cure this "disease" soon (though Poincaré likely hinted at mental disorder in Cantor, which is not the sense I mean here). In stronger theories, the modern interpretation is a definite formal error, softened only by censoring the fragment where it produces a contradiction. So the reason we cannot see it now is that we have cut out the part of the theory where it is obvious, while effectively operating within a relatively consistent fragment of an inconsistent theory interpretation.

## Abstract

The paper continues the critical analysis of the limits of applicability of Cantor's theorem on the uncountability of the continuum and the associated diagonal argument, begun in the earlier articles of the series. It is shown that the classical proof (including Hessenberg's generalization) is valid only within well-ordered structures under sufficiently strong assumptions regarding the universality and totality of infinity. Three fundamentally distinct algebraic structures for describing infinite sets are identified: the internal (cardinal), the hybrid (ordinal), and the external (indexical, associated with numerosities, surreal numbers, and grossone objects). The modern axiomatic interpretation (ZFC, NBG) conflates these structures, leading to a breakdown of isomorphism with Cantor's original constructions and to a persistent conditional consistency of the theory. Architectural shortcomings of modern axiomatic systems—related to points of discontinuity in predicative description at limit ordinals, the fallacy of reification, and the ambiguity of the membership relation—are demonstrated as the cause of this breakdown of isomorphism. It is shown that each algebraic structure requires its own balance of predicativity and impredicativity, and that conflating them under a single notion of bijection leads to the loss of ontological support for operations (in particular, Cantor's distinction between left and right addition and multiplication). A close connection between Russell's paradox and Cantor's theorem is revealed, pointing to a single structural conflict underlying both phenomena. The phenomenon of inexpressible objects, the role of impredicativity in the closure of algebraic structures, and connections to non-standard analysis, surreal numbers, and grossone objects are discussed. A fundamental incompatibility between the global closure of an algebra and the total ordering of its objects is established. Restoring Cantor's original ontology makes it possible to reconcile cardinal, ordinal, and indexical algebras, clarify the status of the continuum (as an object that is not a set in the strict sense), and outline a path toward resolving a number of paradoxes and methodological collisions in the foundations of mathematics.

## Repository Structure

```text
.
├── article_ru.tex      # Main LaTeX source file in Russian
├── article_ru.bib      # BibTeX bibliography
├── CITATION.cff        # Citation metadata for GitHub and Zenodo
├── LICENSE             # CC BY 4.0 license text
└── README.md           # Project overview and build instructions
```

## Compiling the Paper

To compile the PDF locally using `latexmk` (recommended, handles bibliography passes automatically):

```bash
latexmk -pdf article_ru.tex
```

Alternatively, run `pdflatex` and `bibtex` manually:

```bash
pdflatex article_ru.tex
bibtex article_ru
pdflatex article_ru.tex
pdflatex article_ru.tex
```

## How to Cite

If you reference this work, please cite it via Zenodo or use the following BibTeX entry:

```bibtex
@misc{korotkov2026continuumanother,
  author       = {Korotkov, Roman},
  title        = {Uncountability of continuum, checkmate},
  year         = {2026},
  publisher    = {Zenodo},
  version      = {v0.9.0},
  doi          = {10.5281/zenodo.24390197},
  url          = {https://doi.org/10.5281/zenodo.24390197}
}
```

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
