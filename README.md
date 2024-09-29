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
## Task 4
### Task Overview
In this task, we were asked to identify potential cancer biomarkers from a given dataset using differential expression and machine learning models. This project will require creative thinking and collaboration, leveraging the strengths of both fields.
Form a team; 3 ML engineers and 5 biomarker developers
Pick any cancer type/subtype and download from TCGA.
Clean and preprocess the data (primarily biomarker team)
Handle missing values, normalize gene expression data.
Reduce the data to a maximum of 20 samples for the primary and 20 for the recurring tumor types. Please provide annotation for your data. (Feel free to pick other sample classification/categories you are interested in)
From here, the biomarker developer shares the dataset with machine learning engineer
Biomarker Discovery Specialist would:
Conduct differential expression analysis
Conduct functional enrichment analysis
ML Engineer would:
Prepare the data for ML
Perform feature selection
Conduct kNN or random forest classification
Final Report
Submit you complete code from data collection, ML and differential expression analysis to final figures
Write a comprehensive report that includes:
Introduction to the selected cancer
Description of the dataset and preprocessing steps.
Detailed methodology for biomarker discovery and machine learning analysis.
Results and interpretations of the identified biomarkers and model performance.
Visualizations that effectively communicate your findings.
Conclusion and future directions for research.
## Task 5
### Task Overview
In this task, we were asked reproduce the unsupervised clustering of gliomas (n = 516 LGG) based on methylation levels to classify the six IDH statuses as reported in a specified paper. You (the data scientist) will employ the K-Nearest Neighbors (KNN) method for the classification. The goal is to demonstrate your ability to perform unsupervised clustering using methylation data and to evaluate the clustering performance. While the biomarker hunter will develop expression biomarkers that can distinguish any 2 IDH classes.
:- You can also get the dataset for LGG from XENA Browser.
Steps
Keep your team from last week
Read the paper: https://www.cell.com/cell/fulltext/S0092-8674(15)01692-X 
Carefully read the paper that reports the clustering of gliomas using methylation levels to classify the six IDH statuses.
Understand the methodology and the specific findings related to unsupervised clustering and the use of methylation data.
Obtain the dataset
You can compile from the TCGA (more up to date) using TCGABiolinks in R or the XENA Browser link above
Ensure you have IDH status for each sample. You can get this only from the TCGA
Data Preprocessing
Clean and preprocess according to your pipeline and needs.
For ML engineers, feature selection is important
For Biomarker-Devs, normalization is important
Implement the same pipeline as last week
For ML, perform kNN and random forest
For BDevs, perform DEA
Generate final report
Introduction to gliomas, IDH status, and the significance of methylation levels.
Description of the dataset and preprocessing steps.
Methodology for implementing and applying the KNN algorithm.
Results of the kNN, including visualizations and evaluation metrics as presented in the paper.
Comparison with the findings reported in the target paper. (Do you think we need more clusters based on newer datasets)
Conclusion and insights gained from the analysis.
