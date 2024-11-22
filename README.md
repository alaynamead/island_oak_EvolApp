# Island Oak landscape genomics analysis
Code from "Comparison of conservation strategies for California Channel Island Oak *(Quercus tomentella)* using climate suitability predicted from genomic data"

Rmarkdown files with outputs (including plots) are available as supplementary information for the manuscript and at Dryad. Input data used in scripts are also available at Dryad.

Scripts are listed below in the order that they should be run.

## simple_pca_with_vegan.Rmd

PCA of genomic data using the R package vegan. 

## redundancy_analysis_SNPs.Rmd

Redundancy analysis (RDA) used to identify candidate SNPs associated with climate. Also includes SNP imputation. Based on code from [Brenna R. Forester](https://popgen.nescent.org/2018-03-27_RDA_GEA.html).

## read_and_plot_fast-wcfst.Rmd

 Heatmaps and tables of F<sub>ST</sub> for among individuals on each island, and among indidivuals on each island grouped by their species ancestry. F<sub>ST</sub> values were produced by [fast-wcfst](https://codeberg.org/fontenot/fast-wcfst).

## gradient_forest_candidate_SNPs.Rmd

Gradient Forest analysis on candidate SNPs identified from the redundancy analysis. Includes maps of genomic turnover across the landscape, calculation of genomic offset and climate suitability, identification of the pairs of seed sources and planting sites that minimize genomic offset, and comparison of the three conservation strategies. This script includes candidate SNPs identified from four Channel Islands (Santa Rosa, Santa Cruz, Catalina, and San Clemente), excluding individuals from Anacapa and Guadalupe.

## gradient_forest_candidate_SNPs_Guadalupe.Rmd

Same analysis as above, but using the candidate SNPs identified only from Guadalupe Island.





