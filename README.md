# RNA-Seq Analysis Project: Exploring the Impact of SNP Variants on Gene Expression

![Project Banner](https://via.placeholder.com/1200x300.png?text=RNA-Seq+Analysis+Project)

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Data Sources](#data-sources)
- [Installation](#installation)
- [Usage](#usage)
- [Workflow](#workflow)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

---

## Overview

This project involves the comprehensive analysis of RNA-Seq data from the 1000 Genomes Project. The primary objective is to explore the impact of Single Nucleotide Polymorphisms (SNPs) on gene expression levels across different populations. By leveraging tools such as `samtools`, `cufflinks`, and statistical methods like ANOVA, we aim to identify SNPs that significantly influence gene expression.

## Features

- **High-throughput RNA-Seq Data Analysis**: Efficiently processes RNA-Seq data using industry-standard tools.
- **Gene Expression Quantification**: Utilizes `cufflinks` for accurate transcript assembly and quantification.

- **Figure 1:** Differential gene expression analysis
![Data Visualization](Figures/Cufflinks.png)

- **Variant Impact Assessment**: Performs ANOVA to assess the impact of SNP variants (1/1, 1/0 or 0/1, 0/0) on gene expression.
  - **Homozygous Variants (1/1)**: Individuals who have two identical alleles for a particular SNP.
  - **Heterozygous Variants (1/0 or 0/1)**: Individuals who have two different alleles for a particular SNP.
  - **Homozygous Reference (0/0)**: Individuals who have two reference alleles, meaning they do not carry the variant.

- **Figure 2:** Homozygous Variants Vs. Heterozygous Variants Vs. Homozygous Reference
![Data Visualization](Figures/Homo-Hetro.png)

- **Significance Filtering**: Applies statistical thresholds to identify SNPs with significant effects.
- **Reproducibility**: Includes detailed instructions and scripts to replicate the analysis.

So here is the pipeline of the project:
- **Figure 3:** Project Pipeline

![Data Visualization](Figures/Pipeline.drawio.png)


And here is the pipeline of the processing of data:
- **Figure 4:** Data Processing Pipeline

![Data Visualization](Figures/Data_Diagram.drawio.png)


## Data Sources

1. **1000 Genomes Project**: 
   - The 1000 Genomes Project provides comprehensive genomic data for a wide range of human populations. This project uses the variant data from the 1000 Genomes Project to classify samples based on their SNP variants.
   - **Website**: [1000 Genomes Project](http://www.internationalgenome.org/)

2. **GEUVADIS Project**:
   - The GEUVADIS (Genetic European Variation in Health and Disease) project provides RNA-Seq data and corresponding genotype data for human populations. It is an essential resource for studying the relationship between genetic variation and gene expression. This project uses GEUVADIS RNA-Seq data for quantifying gene expression levels.
   - **Website**: [GEUVADIS Data Browser](https://www.ebi.ac.uk/Tools/geuvadis-das/)

3. **Annotation File**: 
   - To accurately quantify gene expression, the project utilizes an annotation file that provides detailed information on gene structures. The specific annotation file used is from Ensembl.
   - **Annotation File**: `Homo_sapiens.GRCh38.112.gtf.gz` from [Ensembl](https://www.ensembl.org)
   

## Installation

To replicate this project, you will need the following software and packages installed:

1. **Python 3.8+**
   - Install necessary Python packages:
     ```bash
     pip install pandas numpy scipy matplotlib seaborn
     ```

2. **samtools**
   - Installation guide: [samtools installation](http://www.htslib.org/download/)

3. **cufflinks**
   - Installation guide: [cufflinks installation](http://cole-trapnell-lab.github.io/cufflinks/install/)

4. **Jupyter Notebook** (optional, for interactive analysis)
   - Install Jupyter:
     ```bash
     pip install notebook
     ```

you can also find other requierement in this project in the requieremnt.txt file in repository.

## Acknowledgments
- Mahshid Khatami [linkedin](https://www.linkedin.com/in/mahshidkhatami-data-analyst)
