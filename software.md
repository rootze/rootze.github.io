---
title: Software
layout: page
---
<img width="100" src="../assets/images/software/scROAD_database.png">
<img width="100" src="../assets/images/software/ArchRtoSignac.png">
<img width="90" src="../assets/images/software/hdWGCNA.png">

<h2>
Developer
</h2>

<a href="https://github.com/swaruplabUCI/ArchRtoSignac">ArchRtoSignac</a>
<img src="https://img.shields.io/badge/version-1.0.5-red.svg">
<img src="https://img.shields.io/badge/Years%20Active-$(expr $(date +%Y) - 2021)-blueviolet">

**ArchRtoSignac** is an R package to convert an ArchRProject [(ArchR)](https://www.archrproject.com/index.html) to a Signac SeuratObject [(Signac)](https://satijalab.org/signac/index.html).
<br>
ArchR and Signac are both commonly used scATAC-seq analysis packages with comparable sets of features and are currently under development, which means they are likely to change over time. You can choose to use only one of these packages; however, you may want to use both packages for your analysis. For example, we use ArchR to generate a fixed-width peak matrix due to its computational advantage, and we use Signac for reference mapping to assist in cell-type annotation. Here we provide an option to help with the data formatting from an ArchRProject to a Signac SeuratObject: **ArchRtoSignac**, a wrapper function that allows easier implementation of both pipelines. In addition, conversion to a SeuratObject allows the use of other packages available through SeuratWrappers.


<h2>
Contributor
</h2>

<a href="https://bioconductor.org/packages/fishpond">fishpond</a>
<img src="https://bioconductor.org/shields/years-in-bioc/fishpond.svg">

* Nonparametric testing procedures for differential transcript and gene analysis
for a collection of experiment designs making use of inferential replicate counts.
Mainly developed by Dr. Michael Love, and in collaboration
with Dr. Joseph Ibrahim (UNC-CH), and Avi Srivastava and Dr. Rob Patro (UMD).

<a href="https://mikelove.github.io/mrlocus">MRLocus</a>
<img width="100" src="../assets/images/gh.png">

* Bayesian estimation of the gene-to-trait effect and credible interval from GWAS and eQTL
  summary statistics for a single loci where harbors multiple independent signals from both studies.
  Developed by Dr. Michael Love, and in collaboration with Dr. Nana Matoba, and Dr. Jason
  Stein (UNC-CH).
