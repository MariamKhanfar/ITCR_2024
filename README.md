# README
#Generated from PHIND in the workshop

Acute Myeloid Leukemia Heatmap Analysis
Project Overview
This project performs a clustering heatmap analysis on acute myeloid leukemia (AML) RNA-seq data. It uses a dataset from Shih et al., 2017, pre-processed by refine.bio.

#Last Updated
October 2021

#Software Requirements
R (version used in the original analysis can be found in the session info at the end of the script)
Required R Packages
pheatmap
magrittr
readr
tibble
dplyr
Project Structure
data/: Contains the input data files
SRP070849/: Specific dataset directory
SRP070849.tsv: Gene expression matrix
metadata_SRP070849.tsv: Metadata file
plots/: Output directory for generated plots
results/: Output directory for analysis results
How to Run the Project
Ensure all required R packages are installed.
Set your working directory to the project root.
Run the R script or open the R Notebook in RStudio.
The script will automatically create necessary directories and download data if not present.
Project Goals
Import and preprocess AML RNA-seq data.
Select genes of interest based on variance.
Create an annotated heatmap of the selected genes.
Save the heatmap as a PNG file.
Key Steps
Set up analysis folders
Install and load required libraries
Import and set up data
Choose genes of interest (top 75% by variance)
Prepare metadata for annotation
Create and save an annotated heatmap
Output
results/top_90_var_genes.tsv: TSV file containing the top variable genes
plots/aml_heatmap.png: PNG file of the annotated heatmap
Future Improvements
Implement alternative gene selection methods (e.g., fold change, t-statistic)
Add more customization options for heatmap generation
Incorporate additional statistical analyses
Data Source
The dataset used in this analysis can be downloaded from refine.bio.

References
Shih, A. H., et al. (2017). Combination Targeted Therapy to Disrupt Aberrant Oncogenic Signaling and Reverse Epigenetic Dysfunction in IDH2- and TET2-Mutant Acute Myeloid Leukemia. Cancer Discovery, 7(5), 494-505.
