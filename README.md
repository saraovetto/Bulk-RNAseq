# Bulk-RNAseq

I performed this analysis as a project for the Transcriptomics course delivered by Università statale di Milano as a part of the MSc in Bioinformatics for Computational Genomics.
The DE analysis has been performed with *edgeR*. The tissue samples are from GTEX, expression data from each replicate has been extracted using *recount3*.

### Description

The goal of the project was to discover differentially expressed genes across three different tissues (taken from GTEX): brain, liver and colon.
The replicates were selected according to three quality control parameters: RIN > 6, fraction of reads of rRNA < 0.1 and percentage of uniquely mapped reads > 85%. Normalization was performed with TMM (= trimmed mean of M values).

Differential expression results were obtained by employing a generalized linear model and designing a contrast matrix to detect the genes overexpressed in each tissue versus the other two. Then, a functional enrichment analysis was perfomed to identify the most relevant functional annotations (Gene Ontology) with [Enrichr](https://maayanlab.cloud/Enrichr/).
