# mandalaR

Public-facing documentation for Mandala, an R mixed-model framework for plant
breeding and quantitative genetics.

This repository is intended for documentation, examples, rendered vignettes,
benchmark summaries, and roadmap material. The private development source code
for Mandala v2.0 is maintained separately.

## Documentation

Rendered documentation should be viewed through the GitHub Pages site:

<https://brbasnet.github.io/mandalaR/>

Direct links:

- [Mandala documentation home](https://brbasnet.github.io/mandalaR/)
- [Introduction to Mandala](https://brbasnet.github.io/mandalaR/vignettes/01-introduction-to-mandala.html)
- [Single-Stage to Multi-Stage Trial Analysis](https://brbasnet.github.io/mandalaR/vignettes/02-single-stage-to-multi-stage-trial-analysis.html)
- [Genomic Prediction](https://brbasnet.github.io/mandalaR/vignettes/03-genomic-prediction.html)
- [Spatial Analysis](https://brbasnet.github.io/mandalaR/vignettes/04-spatial-analysis.html)
- [Advanced Variance Structures](https://brbasnet.github.io/mandalaR/vignettes/05-advanced-variance-structures.html)
- [Mandala Package Comparison](https://brbasnet.github.io/mandalaR/mandala_package_comparison.html)

Note: clicking `.html` files inside the GitHub repository file browser shows
the HTML source code. Use the GitHub Pages links above to view rendered pages.

## Repository Scope

This repository should include:

- rendered vignettes
- public examples
- documentation pages
- benchmark summaries
- package-positioning material
- roadmap notes

This repository should not include:

- private Mandala source code
- unreleased implementation scripts
- private benchmark data
- internal development archives

## Local Preview

Open the documentation home page directly:

```sh
open index.html
```

Or serve locally:

```sh
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```
