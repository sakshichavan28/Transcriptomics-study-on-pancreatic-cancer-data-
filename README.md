# Cancer Nanopore Data Analysis

This repository contains a Jupyter Notebook for **processing and analysing Nanopore sequencing data**.

## Workflow

### 1. Data extraction

- Uses SRA accession `SRR25143528`.
- Downloads FASTQ reads using **`fastq-dump`**.

## Main Tools and Libraries

### Command-line / bioinformatics tools

- **SRA Toolkit / `fastq-dump`**
- **Cutadapt**
- **FastQC**
- **NanoQC**
- **minimap2**

## Purpose

The overall workflow demonstrates how **Nanopore sequencing reads** can be taken from SRA data through:

1. Preprocessing
2. Quality control
3. Reference alignment
4. Gene quantification
5. Expression-data processing
6. Functional enrichment analysis
