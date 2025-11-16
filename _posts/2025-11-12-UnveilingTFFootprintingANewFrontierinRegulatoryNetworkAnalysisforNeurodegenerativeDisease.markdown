---
title: "Unveiling TF Footprinting in Neurodegeneration"
layout: post
date: 2025-11-12 22:44
hidden: false
image: /assets/images/TF_Footprinting_Scenario.png
headerImage: false
tag:
- ATAC
- Footprinting
- Neurodegeneration
- scROAD
- TOBIAS
star: true
category: blog
author: zechuan
description: How TF footprinting improves regulatory network analysis in Alzheimer's and Pick's disease
---

## Introduction

Understanding transcription factor (TF) binding is essential for unraveling the complex regulatory networks that drive gene expression. Single-cell chromatin accessibility data (scATAC-seq) offers unprecedented opportunities to examine these regulatory landscapes. However, many existing approaches struggle to distinguish **functional TF binding** from **non-functional motifs**.

In this post, we explore how *TF footprinting* provides a more accurate way to identify true TF binding events—especially important for studying neurodegenerative diseases such as **Alzheimer’s Disease (AD)** and **Pick’s Disease (PiD)**.

---

## Challenges in Current Methods

Widely used tools like **SCENIC** ([Aibar et al., 2017](https://doi.org/10.1038/nmeth.4463)) and **SCENIC+** ([Bravo González-Blas et al., 2023](https://doi.org/10.1038/s41592-023-01938-4)) infer regulatory networks using:

* Motif enrichment  
* Promoter-associated co-expression  
* Enhancer–gene links from scATAC + scRNA integration  

But these methods have key limitations:

1. They infer TF activity *indirectly* through motif overrepresentation  
2. They cannot reliably distinguish **functional enhancer–TF interactions** from **inactive motifs**

A recent AD multi-omic study ([Mathys et al., 2024](https://doi.org/10.1038/s41586-024-07606-7)) used SCENIC for TF regulator identification but still relied heavily on motif enrichment—leaving ambiguity about true TF occupancy.

---

## Limitations of Using Open Chromatin as a Regulatory Marker

A major misconception in the field is that:

### **Open chromatin = active regulation**  
→ **Not always true.**

Recent works challenge this assumption:

* **Chromatin relaxation** is a hallmark of neurodegeneration  
  - [Xiong et al., 2023](https://doi.org/10.1016/j.cell.2023.08.040)  
  - [Frost et al., 2014](https://doi.org/10.1038/nn.3639)

* **80% of TF motifs lack measurable footprints**  
  - [Baek et al., 2017](https://doi.org/10.1016/j.celrep.2017.05.003)

These findings show that many accessible regions:

* Are *not* bound by TFs  
* Reflect global chromatin decompaction  
* Are easily misinterpreted as regulatory by motif-based methods  

---

## Open Chromatin Scenarios

![TF Footprinting Scenario](https://raw.githubusercontent.com/rootze/scROAD/main/images/TF_Footprinting_Scenario.png){: class="bigger-image" }

<figcaption class="caption">
**Figure 1.** Open chromatin with (left) and without (right) true TF binding. Many disease-associated accessible regions fall into the *non-functional* category (chromatin relaxation).
</figcaption>

---

## A Functional TF Footprinting Approach

To overcome these limitations, we implemented **TF footprinting + motif-flanking accessibility** using **TOBIAS** ([Bentsen et al., 2020](https://doi.org/10.1038/s41467-020-18035-1)) on single-cell ATAC data.

This approach enables:

### **1. Direct measurement of TF occupancy**
Rather than inferring activity through motifs, TOBIAS quantifies actual binding events.

### **2. Distinguishing functional enhancers from non-functional motifs**
By analyzing:

* Footprint depth  
* Flanking accessibility  
* Binding site depletion patterns  

### **3. Condition-specific comparison**
TOBIAS allows differential TF occupancy between:

* Disease vs. control  
* Cell types  
* Brain regions  

### **4. Improved network reconstruction**
Integrating snATAC + snRNA with true TF binding improves GRN accuracy over purely motif-based frameworks like SCENIC or HOMER.

---

## Implications for Neurodegenerative Disease Research

Applying TF footprinting to AD and PiD data reveals:

* True disease-associated TF binding events  
* Functional enhancer dysregulation  
* Misleading “relaxed” chromatin not involved in regulation  
* Candidate TFs and enhancers for therapeutic exploration  

This method also clarifies how:

* Chromatin accessibility changes  
* TF binding  
* Gene expression  
* Cellular vulnerability  

interact during neurodegeneration.

---

## Conclusion

TF footprinting represents a major advancement over motif-only regulatory network methods such as SCENIC and SCENIC+. By directly identifying TF binding events, we gain a more accurate and meaningful understanding of gene regulatory dysfunction in AD, PiD, and other neurodegenerative disorders.

This approach, powered by tools like **TOBIAS**, improves:

* Regulatory network accuracy  
* Enhancer–TF mapping  
* Disease mechanism interpretation  
* Target discovery opportunities  

Footprinting brings us closer to understanding the *true* regulatory events driving disease.

---

## References

1. Aibar et al., *SCENIC: single-cell regulatory network inference and clustering.* Nat Methods (2017).  
   DOI: https://doi.org/10.1038/nmeth.4463

2. Bravo González-Blas et al., *SCENIC+: single-cell multiomic inference of enhancers and GRNs.* Nat Methods (2023).  
   DOI: https://doi.org/10.1038/s41592-023-01938-4

3. Mathys et al., *Single-cell multiregion dissection of Alzheimer's disease.* Nature (2024).  
   DOI: https://doi.org/10.1038/s41586-024-07606-7

4. Xiong et al., *Epigenomic dissection of Alzheimer's disease.* Cell (2023).  
   DOI: https://doi.org/10.1016/j.cell.2023.08.040

5. Frost et al., *Tau promotes neurodegeneration through global chromatin relaxation.* Nat Neurosci (2014).  
   DOI: https://doi.org/10.1038/nn.3639

6. Baek et al., *Bivariate genomic footprinting detects changes in transcription factor activity.* Cell Reports (2017).  
   DOI: https://doi.org/10.1016/j.celrep.2017.05.003

7. Bentsen et al., *ATAC-seq footprinting reveals TF binding kinetics.* Nat Commun (2020).  
   DOI: https://doi.org/10.1038/s41467-020-18035-1
