# Transcriptomics-study-on-pancreatic-cancer-data- README

## Overview

This notebook provides a stepwise workflow for analyzing Nanopore sequencing data from cancer samples. The analysis includes data extraction, preprocessing, alignment, variant calling, and differential expression analysis.

## Steps

### 1. Data Extraction

- Define the SRA accession number and specify the local output path.
- Download FASTQ files using `fastq-dump` from NCBI SRA.

### 2. Preprocessing

- Reduce file size for efficient processing.
- Perform trimming to remove adapter sequences and low-quality reads.
- Use tools like porechop for quality control.

### 3. Alignment and Mapping

- Align reads to the reference genome using `Minimap2` or another suitable aligner.
- Convert SAM to BAM format and sort the alignments using `samtools`.

### 4. Variant Calling

- Use `bcftools` to identify variants (SNPs and indels).
- Filter and annotate variants using `bcftools`.

### 5. Differential Expression Analysis

- Use `featureCounts`, `HTSeq`, or `nanocount` to quantify gene expression.
- Normalize read counts using `DESeq2` (R).
- Identify differentially expressed genes (DEGs) and visualize results with volcano plots.

**For my own understanding, I did DiffEx analysis as mentioned below:**

1. **Quantification:** Quantify genes or transcripts using tools such as HTSeq or featureCounts.
2. **Differential Expression Analysis:** Identify significantly expressed genes using DESeq2 or edgeR.
3. **Pathway Enrichment Analysis:** Conduct functional analysis of differentially expressed genes.

### 6. Results Interpretation

- Generate expression heatmaps and PCA plots to observe clustering.
- Analyze significant DEGs to gain biological insights into cancer progression.

## Requirements

- Python 3.x, R with DESeq2/edgeR
- `fastq-dump`, `fastp`, nanoqc ,`Minimap2`, `samtools`, `bcftools`, `featureCounts`

## Usage

Run each cell sequentially in the notebook. Modify paths and parameters as needed.

## Output

- Trimmed and aligned sequencing data.
- Variant calling results (VCF files).
- Differential expression results and visualizations.
- Pathway enrichment results and visualizations



