# Hackbio-Internship
This repository houses the tasks assigned to me for the duration of my internship at Hackbio
## Task 1
## Task 2
## Task 3
### Task Overview
In this task, we were expected to visualize and interpret a gene expression dataset to generate a heatmap and perform downstream functional enrichment analysis. The aim of this task was to help us understand and learn how to interpret patterns of gene expression and the biological significance of differentially expressed genes. The task involves data preprocessing, visualization, and interpretation of functional enrichment results.    
1. Download and use one of these datasets:
* https://raw.githubusercontent.com/HackBio-Internship/public_datasets/main/Cancer2024/glioblastoma.csv
* https://raw.githubusercontent.com/HackBio-Internship/public_datasets/main/Cancer2024/pregnancyLactationCells.csv
2. Generate a heatmap for the entire dataset. Use a diverging and sequential color palette to generate two color variants of the same heatmap. Think about the importance of color selection in the ease of interpreting plots. Write about this in your report. We recommend using the heatmap.2() function under gplots in R.
3. With the same heatmap, generate a variant of your heatmap where you
* Cluster your genes (rows) alone,
* Cluster your samples (col) alone;
* Cluster both genes and sample together;
4. Subset genes that are significantly upregulated. (Setup your own cut-offs for the fold change and P-values).
5. Subset genes that are significantly downregulated. (Setup your own cut-offs for the fold change and P-values).
6. Perform functional enrichment analysis with either ShinyGO, GOrilla or PANTHER.
7. Using the top 10 pathways, create a straightforward visualization (such as a lollipop plot, dot plot, lineplot or bubble plot) that displays the number of genes associated with each pathway. The plot should also reflect the significance of each pathway by scaling the points according to the negative log10 of the p-value.
8. Describe the top 3 enriched pathways according to biological process in your report
