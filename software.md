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
.badges-row {
  margin-top: 4px;
  margin-bottom: 10px;
}
.badges-row img {
  margin-right: 6px;
  display: inline-block;
}

/* NEW: jump menu for packages */
.software-toc {
  margin: 20px 0 10px;
  padding: 0;
  list-style: none;
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}
.software-toc li {
  margin: 0;
}
.software-toc a {
  font-size: 0.9rem;
  padding: 4px 10px;
  border-radius: 999px;
  border: 1px solid #ccc;
  text-decoration: none;
}
.software-toc a:hover {
  border-color: #6c4edb;
  color: #6c4edb;
}
</style>


<!-- Top Logos -->
<img class="software-logo" width="100" src="../assets/images/software/scROAD_database.png">
<img class="software-logo" width="100" src="../assets/images/software/ArchRtoSignac.png">
<img class="software-logo" width="75"  src="../assets/images/software/hdWGCNA.png">

<!-- <ul class="software-toc">
  <li><a href="#scroad">scROAD</a></li>
  <li><a href="#archrtosignac">ArchRtoSignac</a></li>
  <li><a href="#hdwgcna">hdWGCNA</a></li>
</ul> -->
<ul class="software-toc">
  <li><a href="#scroad" style="font-size: 0.8em;">scROAD</a></li>
  <li><a href="#archrtosignac" style="font-size: 0.8em;">ArchRtoSignac</a></li>
  <li><a href="#hdwgcna" style="font-size: 0.8em;">hdWGCNA</a></li>
</ul>

<h2>Developer</h2>

<!-- scROAD -->
<div class="section-block" id="scroad">
  <a href="https://swaruplab.bio.uci.edu/scROAD/">scROAD</a>

  <div class="badges-row">
    <img src="https://img.shields.io/badge/type-interactive%20database-blueviolet" alt="Interactive database">
    <img src="https://img.shields.io/badge/status-online-brightgreen" alt="Status online">
    <a class="badge-link" href="https://www.science.org/doi/10.1126/sciadv.ads7973" target="_blank" rel="noopener">
      <img src="https://img.shields.io/badge/publication-Science%20Advances-%2300A1D7" alt="Science Advances Publication">
    </a>
  </div>

  <p><strong>scROAD</strong> database offers comprehensive information on single-cell cCRE transcription factor occupancy data generated from snATAC-seq analysis of human postmortem prefrontal cortex (PFC) tissue. The data specifically focuses on Alzheimer's Disease and Pick's Disease.
  I developed this interactive database, <a href="https://github.com/rootze/scROAD" target="_blank">scROAD</a>, which integrates single-cell chromatin data processed with Signac, cis-regulatory links inferred by Cicero, and TF binding occupancy profiles generated using TOBIAS. We performed single cell co-accessibility analyses using <a href="https://cole-trapnell-lab.github.io/cicero-release/docs_m3/" target="_blank">Cicero</a> to construct putative cis-regulatory enhancer-promoter links. Additionally, with the help from <a href="https://github.com/loosolab/TOBIAS" target="_blank">TOBIAS</a> package, we can further explore transcription factor (TF) binding occupancy in ATAC-seq. This analysis allows us to detect differences in TF binding between disease and control samples, providing insights into how regulatory mechanisms are altered in specific cell types. By integrating TF binding data with co-accessibility analyses to create this scROAD interactive database, users can easily explore transcription factor binding activity and their implications in disease, providing a valuable resource for understanding gene regulation in neurodegeneration.
  For a more in-depth understanding of the database's purpose and contents, please refer to the <a href="https://www.science.org/doi/10.1126/sciadv.ads7973" target="_blank">Science Advances</a> paper.</p>
</div>


<!-- ArchRtoSignac -->
<div class="section-block" id="archrtosignac">
  <a href="https://github.com/swaruplabUCI/ArchRtoSignac">ArchRtoSignac</a>

  <div class="badges-row">
    <img src="https://img.shields.io/badge/version-1.0.5-red.svg" alt="Version">
    <a class="badge-link" href="https://github.com/swaruplabUCI/ArchRtoSignac/issues">
      <img src="https://img.shields.io/github/issues-raw/swaruplabUCI/ArchRtoSignac?label=open%20issues&color=yellow" alt="Open Issues">
    </a>
    <a class="badge-link" href="https://github.com/swaruplabUCI/ArchRtoSignac/issues?q=is%3Aissue+is%3Aclosed">
      <img src="https://img.shields.io/github/issues-closed-raw/swaruplabUCI/ArchRtoSignac?label=closed%20issues&color=green" alt="Closed Issues">
    </a>
    <a class="badge-link" href="https://www.sciencedirect.com/science/article/pii/S2666166722003719?via%3Dihub" target="_blank" rel="noopener">
      <img src="https://img.shields.io/badge/publication-STAR%20Protocols-%2300A1D7" alt="STAR Protocols Publication">
    </a>
  </div>

  <p><strong>ArchRtoSignac</strong> is an R package to convert an ArchRProject [<a href="https://www.archrproject.com/index.html" target="_blank">ArchR</a>] to a Signac SeuratObject [<a href="https://satijalab.org/signac/index.html" target="_blank">Signac</a>]. ArchR and Signac are both commonly used scATAC-seq analysis packages with comparable sets of features and are currently under development, which means they are likely to change over time. You can choose to use only one of these packages; however, you may want to use both packages for your analysis. For example, we use ArchR to generate a fixed-width peak matrix due to its computational advantage, and we use Signac for reference mapping to assist in cell-type annotation. Here we provide an option to help with the data formatting from an ArchRProject to a Signac SeuratObject: <strong>ArchRtoSignac</strong>, a wrapper function that allows easier implementation of both pipelines. In addition, conversion to a SeuratObject allows the use of other packages available through SeuratWrappers.</p>
</div>


<h2>
Contributor
</h2>

<!-- hdWGCNA -->
<div class="section-block" id="hdwgcna">
  <a href="https://github.com/smorabit/hdWGCNA">hdWGCNA</a>

  <div class="badges-row">
    <a class="badge-link" href="https://github.com/smorabit/hdWGCNA/tree/dev">
      <img src="https://img.shields.io/github/r-package/v/smorabit/hdWGCNA" alt="hdWGCNA Version">
    </a>
    <a class="badge-link" href="https://www.cell.com/cell-reports-methods/fulltext/S2667-2375(23)00127-3" target="_blank" rel="noopener">
      <img src="https://img.shields.io/badge/publication-Cell%20Rep%20Meth-%2300A1D7" alt="Cell Reports Methods Publication">
    </a>
  </div>

  <p><strong>hdWGCNA</strong> is an R package for performing weighted gene co-expression network analysis [<a href="https://doi.org/10.1186/1471-2105-9-559" target="_blank">WGCNA</a>] in high dimensional transcriptomics data such as single-cell RNA-seq or spatial transcriptomics. <strong>hdWGCNA</strong> is highly modular and can construct context-specific co-expression networks across cellular and spatial hierarchies. hdWGNCA identifies modules of highly co-expressed genes and provides context for these modules via statistical testing and biological knowledge sources. hdWGCNA uses datasets formatted as [<a href="https://satijalab.org/seurat/index.html" target="_blank">Seurat</a>] objects.</p>
</div>
