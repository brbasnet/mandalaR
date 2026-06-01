# mandalaR

Comprehensive documentation for **Mandala**, an R mixed-model framework for
plant breeding and quantitative genetics.

## About Mandala

Mandala is being developed as a breeder-oriented statistical framework for
analyzing plant breeding experiments. Its primary focus is mixed-model analysis
of field trials, multi-environment trials, genomic prediction, spatial models,
and prediction of genetic values from complex breeding data.

Mandala is written for the R ecosystem with a deliberately small dependency
footprint. The package aims to keep the user-facing workflow transparent and
portable while using established mixed-model methodology, including REML,
mixed-model equations, AI-REML updates, sparse matrix computation, and
prediction from fitted linear mixed models.

The goal is to provide practical R syntax for common breeding workflows while
retaining access to modern variance structures and efficient sparse mixed-model
computation.

## Statistical Scope

Mandala currently emphasizes:

- single-site and multi-environment trial analysis
- genotype BLUPs and genotype BLUEs
- genomic relationship models and GBLUP
- sparse and partially replicated MET designs
- spatial row-column and residual covariance models
- single-stage and two-stage analysis workflows
- factor-analytic and other advanced variance structures

Multivariate modeling is under development, but is not the main focus of the
current public documentation.

## Current Development Status

Mandala is an active development package. The current implementation includes
an MME-based AI-REML engine, selected prediction standard errors for large
models, selected fixed-effect tests, genomic prediction utilities, spatial
diagnostics, and stage-wise analysis tools.

The package is still being refined for public release. Documentation in this
repository should therefore be viewed as a development preview rather than a
final release manual.

Installation instructions will be added when a public binary or approved
distribution channel is available.

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

## Public Example Data

The small datasets used in the vignettes are included in the `data/` folder so
that examples can be reproduced by users and learners.

- [fullrep_MET_n1000.csv](https://brbasnet.github.io/mandalaR/data/fullrep_MET_n1000.csv): full-replicated MET example
- [sparse_prep_MET_n1000.csv](https://brbasnet.github.io/mandalaR/data/sparse_prep_MET_n1000.csv): sparse/partially replicated MET example
- [augmented_single_n200.csv](https://brbasnet.github.io/mandalaR/data/augmented_single_n200.csv): augmented single-site spatial example
- [sim_GRM_1000.rds](https://brbasnet.github.io/mandalaR/data/sim_GRM_1000.rds): genomic relationship matrix
- [Dataset notes](https://brbasnet.github.io/mandalaR/data/)

## Repository Scope

This repository is intended for public documentation and communication. It may
include:

- rendered vignettes
- public examples
- documentation pages
- benchmark summaries
- package-positioning material
- roadmap notes

It should not include:

- unreleased implementation scripts
- internal development archives

Additional project information will be shared through
[Listo Agriculture](https://listoagriculture.com/).

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
