# mandalaR

Public-facing documentation for Mandala, an R mixed-model framework for plant
breeding and quantitative genetics.

This repository is intended for documentation, examples, rendered vignettes,
benchmark summaries, and roadmap material. The private development source code
for Mandala v2.0 is maintained separately.

## Documentation

Start here:

- [Mandala documentation home](index.html)
- [Introduction to Mandala](vignettes/01-introduction-to-mandala.html)
- [Single-Stage to Multi-Stage Trial Analysis](vignettes/02-single-stage-to-multi-stage-trial-analysis.html)
- [Genomic Prediction](vignettes/03-genomic-prediction.html)
- [Spatial Analysis](vignettes/04-spatial-analysis.html)
- [Advanced Variance Structures](vignettes/05-advanced-variance-structures.html)
- [Mandala Package Comparison](mandala_package_comparison.html)

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

