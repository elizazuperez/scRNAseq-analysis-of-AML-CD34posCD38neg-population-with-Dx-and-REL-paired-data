## `Normal ORA`: **Supp. files 3** 

This directory contains the **Supp files 3**, consisting of:
* `cluster markers.xlsx`: An excel spreadsheet with the DEG of each cluster (logFC > 0.25, p.adjust < 0.05, expressed in at least 15% of the cells in the specific cluster and in the rest of cells), the output from *FindAllMarkers* function from Seurat.
* `enrichment normal.xlsx`: An excel spreadsheet with the ORA results in GO, KEGG and REACTOME, output from *compareCluster* by clusterProfiler package. The input for this function is a list of the top 100 genes DE from each cluster from `cluster markers.xlsx`.
* `enrichment normal.pdf`: A pdf of three pages. On each, a dotplot of the 5 most differentially enriched gene sets on each data base. 
