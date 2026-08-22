# *Trypanosoma cruzi* Cardiomyocyte Transcriptomics

<br>

Bulk RNA-seq analysis of human cardiomyocytes infected with *Trypanosoma cruzi*, using the publicly available dataset **GSE223600**.
<br>

## 🧬 Objective

To characterize transcriptional changes in human cardiomyocytes following *T. cruzi* infection and identify differentially expressed genes and biological processes associated with the infection.
<br>

## 📊 Dataset

The analysis uses RNA-seq count data from the **GSE223600** dataset available through the NCBI Gene Expression Omnibus (GEO).

Six samples were analyzed:

* 3 control samples — 0 h post-infection (0 hpi)
* 3 infected samples — 24 h post-infection (24 hpi)

The primary comparison was:

**24 hpi vs. 0 hpi**

## 🔬 Analysis workflow

```text
GEO dataset
     ↓
Raw count files
     ↓
Count matrix construction
     ↓
Sample metadata
     ↓
Low-count filtering
     ↓
DESeq2 normalization & differential expression
     ↓
PCA & sample correlation
     ↓
Differential expression visualization
     ↓
Gene annotation
     ↓
GO enrichment analysis
     ↓
Targeted analysis of hypoxia-related genes
```

## 🧪 Methods & Tools

### Differential expression

* R
* DESeq2
* Adjusted *p*-value < 0.05
* |log2 fold change| > 1

### Visualization

* ggplot2
* EnhancedVolcano
* pheatmap
* gplots
* ggrepel

### Functional analysis

* clusterProfiler
* enrichplot
* org.Hs.eg.db
* Gene Ontology (GO) enrichment

### Data acquisition

* GEOquery


## 📚 Data source

NCBI Gene Expression Omnibus (GEO):

**GSE223600**

---

*This repository contains an independent analysis of publicly available RNA-seq data and is intended for research and educational purposes.*

