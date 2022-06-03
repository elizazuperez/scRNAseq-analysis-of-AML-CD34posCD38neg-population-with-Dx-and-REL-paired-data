# Supp files from Full data integration 

## `Normal ORA`: **Supp. files 3** 

This directory contains the **Supp files 3**, consisting of:
* `cluster markers.xlsx`: An excel spreadsheet with the DEG of each cluster (logFC > 0.25, p.adjust < 0.05, expressed in at least 15% of the cells in the specific cluster and in the rest of cells), the output from *FindAllMarkers* function from Seurat.
* `enrichment normal.xlsx`: An excel spreadsheet with the ORA results in GO, KEGG and REACTOME, output from *compareCluster* by clusterProfiler package. The input for this function is a list of the top 100 genes DE from each cluster from `cluster markers.xlsx`.
* `enrichment normal.pdf`: A pdf of three pages. On each, a dotplot of the 5 most differentially enriched gene sets on each data base. 


## `Dx REL conserved markers ORA`: **Supp. files 4** 
Using *FindConservedMakers* from Seurat, the 100 most DEG both in Dx condition and REL condition for each cluster has been obtained and used for the ORA.
This directory contains the **Supp files 4**, consisting of:
* `Conserved_enrichment_ALL.xlsx`: An excel spreadsheet with the ORA results in GO, KEGG and REACTOME, output from *compareCluster* by clusterProfiler package. The input for this function is a list of the top 100 genes DE from each cluster from `cluster markers.xlsx`.
* `enrichment_conserved_ALL.pdf`: A pdf of three pages. On each, a dotplot of the 5 most differentially enriched gene sets on each data


## `Signatures`: **Supp. files 5** 
Using *AddModuleScore* from Seurat, based on the results avaliable in Supp Files 4, 7 signatures were analyzed:
1. The Reactome pathway **G0 and early G1**,
2. The WikiPathways **Aerobic Glycolysis**,
3. The Reactome pathway **Glycolysis**, 
4. The GO term **G0 to G1 transition**, 
5. The KEGG pathway **Drug Metabolism - Other Enzymes** (*KEGG: Drug Metabolism* in the plot), 
6. The GO term **DNA Damage Response Signal Transduction by P53 Class Mediator Resulting in Cell Cycle Arrest** (*GO: p53 DNA dam. resp.* in the plot)
7. The Reactome pathway **TP53 Regulates Transcription of Genes Involved in G1 Cell Cycle Arrest** (*PA: TP53 G1 arrest* in the plot)  


This directory contains the **Supp files 5**, consisting of:
* `UMAP_signatures_selected.pdf`: a UMAP plot for each of the signatures.



## `Dx vs REL ORA`: **Supp. files 6** 
One of the problems arisen in this project: the ORA performed (REL vs ORA) in all cells in the data and the performed within all the selected clusters (clusters 5, 7, 10, 12) have similar results.  
* `Enrichment allDX vs allREL.xlsx`: Dx vs REL ORA result in all cells of the data
* `Cluster X allDx vs allREL.xlsx`: ORA results in the three databases in X cluster comparing REL vs Dx cells
* `Cluster X allDx vs allREL.pdf`: Dotplots of the 5 most enriched terms from the analysis of the previous file
