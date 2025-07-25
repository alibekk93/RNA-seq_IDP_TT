
# Thermus thermophilus Gene Expression and IDP Analysis

![Progress](https://img.shields.io/badge/Progress-40%25-yellow)

---

## Project Overview

This project investigates the relationship between **intrinsically disordered protein (IDP) levels** and **gene expression** in the thermophilic bacterium *Thermus thermophilus*. The workflow leverages publicly available transcriptomics data to:

- Download and preprocess gene expression data from GEO (GSE33985)
- Map microarray probe IDs to gene ORFs using platform annotation (GPL4902)
- Integrate gene expression data with predicted IDP scores
- Lay groundwork for analyzing proteome adaptability and gene regulation in thermophiles

---

## Current Status

- [x] Downloaded and parsed *T. thermophilus* microarray expression data (GSE33985)
- [x] Filtered and combined expression data for wild type samples
- [x] Downloaded and parsed microarray platform annotation (GPL4902)
- [x] Mapped probe-level expression data to gene-level ORFs
- [x] Performed initial data quality visualizations (scatterplots, correlation heatmaps)

### To-Do

- [ ] Integrate IDP prediction data for *T. thermophilus* protein sequences
- [ ] Data normalization across samples and probe handling
- [ ] Aggregate probe-level expression to gene-level (handling multiples)
- [ ] Extensive data quality assessment (missing values, outliers, batch effects)
- [ ] Advanced exploratory data analysis:
  - [ ] Visualize expression distributions (histograms, density plots) per sample
  - [ ] PCA/t-SNE for sample clustering and batch effect detection
  - [ ] Identify and visualize highly variable or highly expressed genes
  - [ ] Examine and report sample replicability and technical/biological consistency
  - [ ] Assess mapping/annotation completeness and coverage
- [ ] Merge expression with IDP disorder scores by gene
- [ ] Statistical analysis of expression–IDP correlation (Pearson/Spearman, significance, visualization)
- [ ] Differential or functional enrichment analyses for high/low disorder genes
- [ ] Interpret biological implications and discuss results
- [ ] Expand markdown documentation and add explanatory figures
- [ ] Improve automation, error handling, and reproducibility in workflows

---

## Repository Structure

```
/data/                   # Raw and processed GEO data files
/notebooks/              # Jupyter notebooks for data processing and analysis
/scripts/                # Python scripts for downloading, parsing, and analysis
/results/                # Output: figures, final datasets, and summaries
README.md                # Project overview and instructions
```

---

## Getting Started

### Requirements

- Python 3.7+
- Packages: `GEOparse`, `pandas`, `matplotlib`, `seaborn` (install via pip)

### Usage

1. Run the main notebook `RNA_seq_T_thermophilus.ipynb` to download and process expression and annotation data.
2. Adjust filtering as needed for your own sample selection.
3. Integrate with your predicted IDP scores for full analysis (pending).
4. Use or expand visualizations and analysis cells for your research.

---

## Next Steps

See the **To-Do** checklist above for all remaining analysis and interpretation tasks.

---

*Project is under active development. Community feedback and collaboration are welcome!*
