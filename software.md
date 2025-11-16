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
  <a href="https://www.science.org/doi/10.1126/sciadv.ads7973" target="_blank" rel="noopener">
    <img src="https://img.shields.io/badge/publication-Science%20Advances-%23008CFF" alt="Science Advances Publication">
  </a>

  <p><strong>scROAD</strong> database offers comprehensive information on single-cell cCRE transcription factor occupancy data generated from snATAC-seq analysis of human postmortem prefrontal cortex (PFC) tissue. The data specifically focuses on Alzheimer's Disease and Pick's Disease. For a more in-depth understanding of the database's purpose and contents, please refer to the following publication.  
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
  <a href="https://www.sciencedirect.com/science/article/pii/S2666166722003719?via%3Dihub" target="_blank" rel="noopener">
    <img src="https://img.shields.io/badge/publication-STAR%20Protocols-%237000FF" alt="STAR Protocols Publication">
  </a>

  <p><strong>ArchRtoSignac</strong> is an R package to convert an ArchRProject [<a href="https://www.archrproject.com/index.html" target="_blank">ArchR</a>] to a Signac SeuratObject [<a href="https://satijalab.org/signac/index.html" target="_blank">Signac</a>]. ArchR and Signac are both commonly used scATAC-seq analysis packages with comparable sets of features and are currently under development, which means they are likely to change over time. You can choose to use only one of these packages; however, you may want to use both packages for your analysis. For example, we use ArchR to generate a fixed-width peak matrix due to its computational advantage, and we use Signac for reference mapping to assist in cell-type annotation. Here we provide an option to help with the data formatting from an ArchRProject to a Signac SeuratObject: <strong>ArchRtoSignac</strong>, a wrapper function that allows easier implementation of both pipelines. In addition, conversion to a SeuratObject allows the use of other packages available through SeuratWrappers.</p>
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
  <a href="https://www.cell.com/cell-reports-methods/fulltext/S2667-2375(23)00127-3" target="_blank" rel="noopener">
    <img src="https://img.shields.io/badge/publication-Cell%20Rep%20Meth-%2300A1D7" alt="Cell Reports Methods Publication">
  </a>

  <p><strong>hdWGCNA</strong> is an R package for performing weighted gene co-expression network analysis [<a href="https://doi.org/10.1186/1471-2105-9-559" target="_blank">WGCNA</a>] in high dimensional transcriptomics data such as single-cell RNA-seq or spatial transcriptomics. <strong>hdWGCNA</strong> is highly modular and can construct context-specific co-expression networks across cellular and spatial hierarchies. hdWGNCA identifies modules of highly co-expressed genes and provides context for these modules via statistical testing and biological knowledge sources. hdWGCNA uses datasets formatted as [<a href="https://satijalab.org/seurat/index.html" target="_blank">Seurat</a>] objects.</p>
</div>
