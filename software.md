---
title: Software
layout: page
---

<style>
.badge-link {
  text-decoration: none !important;
}
.badge-link img {
  display: inline-block;
  margin-right: 4px;
}
.software-logo {
  margin-right: 12px;
}
.section-block {
  margin-top: 20px;
  margin-bottom: 10px;
}
</style>

<!-- Top Logos -->
<img class="software-logo" width="100" src="../assets/images/software/scROAD_database.png">
<img class="software-logo" width="100" src="../assets/images/software/ArchRtoSignac.png">
<img class="software-logo" width="75"  src="../assets/images/software/hdWGCNA.png">

<h2>Developer</h2>

<!-- scROAD -->
<div class="section-block">
  <a href="https://swaruplab.bio.uci.edu/scROAD/">scROAD</a>
  <img src="https://img.shields.io/badge/type-interactive%20database-blueviolet" alt="Interactive database">
  <img src="https://img.shields.io/badge/status-online-brightgreen" alt="Status online">

  <p><strong>scROAD</strong> database offers comprehensive information on single-cell cCRE transcription factor occupancy data generated from snATAC-seq analysis of human postmortem prefrontal cortex (PFC) tissue. The data specifically focuses on Alzheimer's Disease and Pick's Disease. For a more in-depth understanding of the database's purpose and contents, please refer to the following publication.  
  The full study is available in
  <a href="https://www.science.org/doi/10.1126/sciadv.ads7973" target="_blank">Science Advances</a>.
  </p>
</div>


<!-- ArchRtoSignac -->
<div class="section-block">
  <a href="https://github.com/swaruplabUCI/ArchRtoSignac">ArchRtoSignac</a>

  <img src="https://img.shields.io/badge/version-1.0.5-red.svg" alt="Version">

  <a class="badge-link" href="https://github.com/swaruplabUCI/ArchRtoSignac/issues">
    <img src="https://img.shields.io/github/issues-raw/swaruplabUCI/ArchRtoSignac?label=open%20issues&color=yellow" alt="Open Issues">
  </a>

  <a class="badge-link" href="https://github.com/swaruplabUCI/ArchRtoSignac/issues?q=is%3Aissue+is%3Aclosed">
    <img src="https://img.shields.io/github/issues-closed-raw/swaruplabUCI/ArchRtoSignac?label=closed%20issues&color=green" alt="Closed Issues">
  </a>

  <p><strong>ArchRtoSignac</strong> is an R package to convert an ArchRProject [(ArchR)](https://www.archrproject.com/index.html) to a Signac SeuratObject [(Signac)](https://satijalab.org/signac/index.html). ArchR and Signac are both commonly used scATAC-seq analysis packages with comparable sets of features and are currently under development, which means they are likely to change over time. You can choose to use only one of these packages; however, you may want to use both packages for your analysis. For example, we use ArchR to generate a fixed-width peak matrix due to its computational advantage, and we use Signac for reference mapping to assist in cell-type annotation. Here we provide an option to help with the data formatting from an ArchRProject to a Signac SeuratObject: **ArchRtoSignac**, a wrapper function that allows easier implementation of both pipelines. In addition, conversion to a SeuratObject allows the use of other packages available through SeuratWrappers.</p>
</div>


<h2>
Contributor
</h2>

<!-- hdWGCNA -->
<div class="section-block">
  <a href="https://github.com/smorabit/hdWGCNA">hdWGCNA</a>
  <a href="https://github.com/smorabit/hdWGCNA/tree/dev">
    <img src="https://img.shields.io/github/r-package/v/smorabit/hdWGCNA" alt="hdWGCNA Version">
  </a>

  <p><strong>hdWGCNA</strong> performs high-dimensional weighted gene co-expression network analysis (WGCNA) for single-cell or spatial transcriptomics data.  
  It constructs multi-resolution, context-specific co-expression modules and integrates seamlessly with Seurat workflows.</p>
</div>


<a href="https://github.com/smorabit/hdWGCNA">hdWGCNA</a>
<a href="https://github.com/smorabit/hdWGCNA/tree/dev">
  <img src="https://img.shields.io/github/r-package/v/smorabit/hdWGCNA" alt="hdWGCNA Version">
</a>

<!-- **hdWGCNA** is an R package for performing weighted gene co-expression network analysis [(WGCNA)](https://doi.org/10.1186/1471-2105-9-559) in high dimensional transcriptomics data such as single-cell RNA-seq or spatial transcriptomics.
<br>
* **hdWGCNA** is highly modular and can construct context-specific co-expression networks across cellular and spatial hierarchies. hdWGNCA identifies modules of highly co-expressed genes and provides context for these modules via statistical testing and biological knowledge sources. hdWGCNA uses datasets formatted as [Seurat](https://satijalab.org/seurat/index.html) objects. Check out the [hdWGCNA in single-cell data tutorial](https://smorabit.github.io/hdWGCNA/articles/basic_tutorial.html) or the [hdWGCNA in spatial transcriptomics data tutorial](https://smorabit.github.io/hdWGCNA/articles/ST_basics.html) to get started. -->


<a href="https://mikelove.github.io/mrlocus">MRLocus</a>
<img width="100" src="../assets/images/gh.png">

* Bayesian estimation of the gene-to-trait effect and credible interval from GWAS and eQTL
  summary statistics for a single loci where harbors multiple independent signals from both studies.
  Developed by Dr. Michael Love, and in collaboration with Dr. Nana Matoba, and Dr. Jason
  Stein (UNC-CH).
