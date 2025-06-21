# ova_resolve
Spatial Transcriptomics Analysis of Ovarian Follicle Atresia
This repository contains computational code and scripts for the spatial transcriptomics analysis of ovarian tissue. This study investigates the poorly understood process of ovarian follicle atresia, a complex degeneration critical to female fertility. We specifically utilized spatial transcriptomics to explore the progression of follicular atresia by focusing on changes of steroidogenesis within granulosa and theca cells, and the dynamics of key signaling pathways, including WNT, TGFβ/BMP, Notch, and Hedgehog. Our analysis aims to provide novel insights into the spatial and molecular mechanisms driving this crucial biological process.
Analysis Methodology
Our analysis workflow is primarily implemented in Python and leverages the results provided by Resolve company's platform.
1.Data Preprocessing and anndata Construction:
•	Based on the raw data provided by Resolve, cell segmentation and transcript assignment for the ovarian samples were conducted on their dedicated analysis platform (https://my.resolvebiosciences.com/filemanager). 
•	Our Python scripts are primarily responsible for constructing the anndata data structure based on these processed results.
2.Downstream Analysis:
We utilized the scanpy package for a series of downstream analyses, including: Dimensionality Reduction: Such as UMAP, used for visualizing the structure of cell populations.
Clustering: To identify cell populations with similar gene expression patterns.
3.Visualization:
The matplotlib package was used to visualize the analysis results, specifically: Mapping the identified cell clusters and gene expression levels onto the original tissue samples.
