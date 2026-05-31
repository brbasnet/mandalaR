# Public Example Datasets

This folder contains the small public datasets used in the Mandala vignettes.
They are included so that readers can reproduce the examples without requiring
access to the private development repository.

## Files

| File | Records | Description | Used In |
|---|---:|---|---|
| `fullrep_MET_n1000.csv` | 1000 | Full-replicated multi-environment trial example with genotype, environment, replication, row-column layout, and trait columns. | Introduction, single-stage to multi-stage analysis, genomic prediction, advanced variance structures |
| `sparse_prep_MET_n1000.csv` | 1000 | Sparse/partially replicated multi-environment trial example with incomplete genotype sharing across environments and row-column layout. | Introduction |
| `augmented_single_n200.csv` | 200 | Single-site augmented/spatial field-trial example with row-column layout and trait columns. | Spatial analysis |
| `sim_GRM_1000.rds` | 1000 x 1000 | Genomic relationship matrix for the public example genotype set. | Genomic prediction |

## Common Columns

The CSV files include core design and trait columns:

- `geno`: genotype identifier
- `env`: combined environment identifier
- `loc`: location
- `year`: year
- `rep`: replication
- `block`: block label
- `row`, `col`: field coordinates
- `yield`, `disease`, `height`, `heading`: simulated trait values
- `yld`: analysis response used in most examples
- `family`, `sire`, `dam`: pedigree-style grouping columns

## Example

```r
df <- read.csv("data/fullrep_MET_n1000.csv", stringsAsFactors = FALSE)

for (v in c("geno", "env", "loc", "year", "rep", "block", "row", "col")) {
  df[[v]] <- factor(df[[v]])
}

df$yld <- as.numeric(df$yld)
```

