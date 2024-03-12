# Med263 - Final Project
In this tutorial 

## Background
### Introduction
Single cell RNA sequencing (scRNA-seq) is a powerful technology in which RNA transcripts from individual cells are quantified in an isoform aware manner. In the biomedical field, scRNA-seq is used for several applications, including validating genetic hits in GWAS studies by cell-type specific eQTL mapping1. CITE-seq is a modified version of scRNA-seq that includes measuring RNA abundances, as well as surface protein quantification by tagging cells with oligo-conjugated antibodies before sequencing. In this tutorial, we will explore how to impute protein expression values into scRNA-seq data from the same sample type through joint embedding and integration. Furthermore, we will conduct an analysis on the joint data to find which proteins and genes are expressed in each cell type.
### Project Aim
We are putting a spin on a standard scRNA-seq analysis tutorial by incorporating joint integration and an introduction to CITE-seq data. The use of multimodal data integration has shown benefits in biomedical research, including one study we found, where the authors used an approach to find genes to prioritize in diseases that have no clear candidate genes by using integrated protein and gene expression data3. They found that the integrated approach produced better results than either independently, and applied this to find genes of interest in Alzheimer’s disease. 

This tutorial can serve as a pipeline that students can follow in their own biomedical research. As single cell sequencing becomes more prevalent, researchers may often find themselves with data collected through multiple single cell modalities across hundreds of individuals. This data needs to be integrated in a way where meaningful analyses can be performed downstream. 



## Installation and Data Files
### Software Installation
Software installs
Ths project is done in Jupyter Notebook. We started with the med263_jupyter environment we previously made in class, and installed additional packages using the following commands.

pip install pandas==2.1.1 <br>
pip install git+https://github.com/maximilian-heeg/UCell.git <br>
pip install scanpy <br>
pip install numpy <br>
pip install scvi-tools <br>
pip install scrublet <br>
pip install --upgrade setuptools <br>
pip install mygene <br>

If running in the jupyter notebook cell, add ! in front. This is also included in our notebook. 

The test if they were successfully installed, run the following block in the notebook:
![packageAssertion](https://github.com/jennydongwx/JointRNAProteinAnalysis/assets/59887313/d6b5437f-7ffe-41a8-8f72-8ff4de042b29)


### Data 
While we address the preprocessing and integration in the tutorial, we have provided the already integrated data as a starting point for following along. 

These data frames are too large to be uploaded on GitHub so they can be accessed here: 

scRNA: https://drive.google.com/file/d/1L-cGY75HJoPmiDF7q5hRjXMas3YbNUmD/view?usp=share_link
Cite Seq: https://drive.google.com/file/d/1kksWD7atJlxbrOMJYYkKyY1RM59QZ2Ej/view?usp=share_link

You will need to be on a UCSD account to access. 


