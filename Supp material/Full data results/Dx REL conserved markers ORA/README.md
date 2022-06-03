## `Dx REL conserved markers ORA`: **Supp. files 4** 
Using *FindConservedMakers* from Seurat, the 100 most DEG both in Dx condition and REL condition for each cluster has been obtained and used for the ORA.
This directory contains the **Supp files 4**, consisting of:
* `Conserved_enrichment_ALL.xlsx`: An excel spreadsheet with the ORA results in GO, KEGG and REACTOME, output from *compareCluster* by clusterProfiler package. The input for this function is a list of the top 100 genes DE from each cluster from `cluster markers.xlsx`.
* `enrichment_conserved_ALL.pdf`: A pdf of three pages. On each, a dotplot of the 5 most differentially enriched gene sets on each data
