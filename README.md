# RNA-seq Analysis Reports

This repository contains R Markdown (`.Rmd`) files and corresponding rendered HTML reports for processing and analyzing RNA-seq data. The workflow includes generating a count matrix from Salmon quantification and performing a complete differential expression analysis pipeline.

## Contents

| File Name                         | Description                                   |
|----------------------------------|-----------------------------------------------|
| `countMatrix_from_salmon.Rmd`    | Script to import and process Salmon quantification files into a combined gene-level count matrix |
| `countMatrix_from_salmon.html`   | Rendered HTML report of the count matrix generation |
| `rnaseq_analysis_workflow.Rmd`   | Full RNA-seq differential expression workflow using DESeq2 and visualization |
| `rnaseq_analysis_workflow.html`  | Rendered HTML report for the RNA-seq workflow |

## Workflow Overview

1. Import Salmon quantifications using `tximport`
2. Build gene-level count matrix
3. Normalize and transform data (VST or rlog)
4. Perform differential expression analysis with `DESeq2`
5. Generate quality control and visualization plots (PCA, heatmaps, volcano plots)
6. Output annotated result tables
