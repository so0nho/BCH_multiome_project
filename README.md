
# Project details
Cardiomyocytes are responsible for the contractile force and blodd pumping in the heart. Humans are born 
with a set number of cardiomyocytes and if injured, they are not able to regenerate and turn? into fibroblasts. 

Phenotypically mice hearts look the same between 4 month old injured hearts (4M-TAC) and aged hearts (24M and 28M). Both present
signs of hypertrophy, with aged samples having a higher immune cell activity and fibrosis. Younger samples (4M) usually show
hypertrophy in the left ventricle. 

Even though, the samples are phenotypically similar they differ in the underlying molecular mechanisms. 

In this project, we will compare healthy heart mice samples (4M-H) against 4M-TAC samples and aged samples.

## Additional ideas
1. HafPaf + HafRaf in addition to comparing 4M-H + 4M-TAC + 24M/28M. 

2. In diseased heart models, stress genes are turned on temporarily and then turn off. Aging models, however, exhibit 
prolonged stress signal activation. 

If we study the genes that are temporarily activated and identify the mechanisms by which those genes get turned off and apply
it to aging hearts, we can basically reverse aging in hearts. 
  
3. Do cross comparison of the current project between species (human data)

# Analysis steps
Preprocess steps:
- get data 
- clean up each dataset and assay 
  - filtering out low quality cells
  - *ATAC* keep standard chromosomes only
    - create a combined peak set 
  - merge then process atac data
  - *RNA* normalize, find variable features, scale, pca
    - umap only for visualization purposes
- integrate layers 
- wnn
- annotate clusters

Motif analysis:
  - 

**Next steps**
Compare the motifs to gene expression levels. 
  - Motifs that show a higher gene expression are the ones that are active. 

Clean out data more and remove clusters that show multiple markers. 
Run preprocess again to remove high mitochondrial percentage. 

