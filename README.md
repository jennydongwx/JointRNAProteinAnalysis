# Med263 - Final Project
In this tutorial 

## Background
### Introduction
Single cell RNA sequencing (scRNA-seq) is a powerful technology in which RNA transcripts from individual cells are quantified in an isoform aware manner. In the biomedical field, scRNA-seq is used for several applications, including validating genetic hits in GWAS studies by cell-type specific eQTL mapping1. CITE-seq is a modified version of scRNA-seq that includes measuring RNA abundances, as well as surface protein quantification by tagging cells with oligo-conjugated antibodies before sequencing. In this tutorial, we will explore how to impute protein expression values into scRNA-seq data from the same sample type through joint embedding and integration. Furthermore, we will conduct an analysis on the joint data to find which proteins and genes are expressed in each cell type.
### Project Aim
We are putting a spin on a standard scRNA-seq analysis tutorial by incorporating joint integration and an introduction to CITE-seq data. The use of multimodal data integration has shown benefits in biomedical research, including one study we found, where the authors used an approach to find genes to prioritize in diseases that have no clear candidate genes by using integrated protein and gene expression data3. They found that the integrated approach produced better results than either independently, and applied this to find genes of interest in Alzheimer’s disease. 

This tutorial can serve as a pipeline that students can follow in their own biomedical research. As single cell sequencing becomes more prevalent, researchers may often find themselves with data collected through multiple single cell modalities across hundreds of individuals. This data needs to be integrated in a way where meaningful analyses can be performed downstream. 


