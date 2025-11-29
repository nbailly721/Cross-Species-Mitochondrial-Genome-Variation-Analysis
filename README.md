                                                                  ######Variation of Genome Length and GC Content Across Species######

**Description**

This project examines mitochondrial genome length and GC content across multiple species by combining shell-based sequence processing with R-based exploratory analysis and visualization. The workflow downloads raw mitochondrial genomes, computes genome length and GC composition, and compares these metrics across species.

**Workflow Overview**

     1. Genome Download and Processing (Shell Script)

Download mitochondrial genome FASTA files from NCBI using wget.

Calculate total genome length and GC content using standard Linux tools (grep, awk, tr).

Output summary statistics for each species to mt_stats.tsv.

     2. Genome Statistics Analysis (R Script)

Load genome statistics from mt_stats.tsv.

Explore variation in genome size and GC content across species.

Generate visualizations including bar plots for genome length and GC content and a scatter plot showing their relationship.

**Datasets Used**

Mitochondrial genome FASTA files for:
Human, Mouse, Cattle, Gorilla
(Downloaded directly from NCBI via shell script.)

**Packages / Tools Used**

Shell / Command-Line Tools

wget – Download mitochondrial genome sequences

grep, awk, tr – Process FASTA files and calculate statistics

R Environment

tidyverse – Data manipulation and visualization

**Key Results**

Quantified species-specific differences in mitochondrial genome length and GC content.

Visual comparisons of genome size and GC composition across species.

Scatter plot illustrating the relationship between genome length and GC content.

**Files in This Repository**

variation_genome_gc_download.sh – Shell script for downloading genomes and computing statistics

variation_genome_gc_analysis.R – R script for data loading, exploration, and visualization

**Important Notes**

Genome sequences are sourced directly from NCBI.

Workflow can be extended to additional species or other genomic features.

The shell script must be run first to generate mt_stats.tsv, which is then used as input for the R analysis.

Resulting figures are not included in the repository; they are produced by running both scripts.
