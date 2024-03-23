# Ceratopipra_rubrocapilla_Phylogeography
 
# Dataset preparation
### Reference genome preparation
The pipeline for preparing the reference genome, including the step of scaffolding to pseudochromosome scale, is in `1_Datasets/1.0_Reference_genome`. The *Pipra* reference genome can be obtained from NCBI under accession number GCF_003945595.2. The version scaffolded to pseudochromosome scale is too large to be placed into the Github repository, but can be recreated with the instructions in the `.md` file or obtained from the Dryad repository.

### Raw data trimming
The pipeline for downloading, assessing, and trimming the raw data is in the file `1_Datasets/1.1aa_GBSDatasets.md`. The pipeline for downloading the data will be different, as the raw sequencing reads will be available from the NCBI SRA after publication. The trimming logs and QC data for the reads is in the folder `1_Datasets/1.1aa_GBSDatasets` (not on Dryad due to copyright of FastQC reports).

### mapping to reference genome
The file `1_Datasets/1.2a_mapping.md` contains the instructions for mapping the trimmed sequencing reads to the reference genome, as well as the pipeline for identifying whether a sample is dilpoid or hemizygous on the Z chromosome. Quality reports related to the mapping are in the folder `1_Datasets/1.2a_mapping`. The raw `.bam` files of sequence alignments are too large to be placed in the repository, but can be regenerated with the code in the markdown file.  

### Genotype calling  
The pipeline for calling and filtering genotypes is in the file `1_Datasets/1.3a_genotyping.md`. The filtered datasets are placed in the folder `1_Datasets/1.3a_genotyping` where space allows; some of the larger datasets with invariant sites are too large for the repository but can be regenerated from the instructions in the `.md` file.    

# Analyses

### Maximum likelihood nuclear tree

### SVDQuartets tree

### Splitstree network

### Maximum likelihood mitochondrial tree
The instructions for replicating the maximum likelihood tree from the mitochondrial data are in the file `2_Phylogeny/2.4aa_ML_mtDNAtree.md`; the input aligment and output tree are in the folder `2_Phylogeny/2.4aa_ML_mtDNAtree/datasets`

### Time-calibrated mitochondrial phylogeny
The instructions for replicating the time-calibrated tree from the mitochondrial data are in the file `2_Phylogeny/2.5aa_BEAST_mtDNAtree.md`; the input aligment and output tree are in the folder `2_Phylogeny/2.5aa_BEAST_mtDNAtree/datasets`

### PCoA Analysis
The code for replicating the PCoA analysis is in the R markdown file `3_Structure/3.1aa_PCoA.Rmd` which is also knit into `3_Structure/3.1aa_PCoA.html`. The output and input data for this analysis is in the foldder `3_Structure/3.1aa_PCA/Input_data`.

### STRUCTURE analysis.
Instructions for replicating the STRUCTURE analysis of *C. rubrocapilla* are in the file `3_Structure/3.2aa_STRUCTURE.md`, and the raw results are in the folder `3_Structure/3.2aa_STRUCTURE`. The input data for this analysis is `Ceratopipra_rubrocapilla.GBSPipfilbwa.allsites.filtered.thinned10k.forSVD.AC4.37_0.2_5_20.0.vcf.gz`, found in the folder `1_Datasets/1.3a_genotyping/filteredSNPs/thinned_datasets`.  

### map of genetic gradient  
Instructions for replicating the map illustrating the genetic gradient across *C. rubrocapilla* are in the file `3_Structure/3.5aa_gradients.md`. The input data for this analysis is `Ceratopipra_rubrocapilla.GBSPipfilbwa.allsites.filtered.genicintergenic.forSVD.AC0.37_0.2_5_20.0.vcf.gz`, found in the folder `1_Datasets/1.3a_genotyping/filteredSNPs`. The metadata file with the coordinates for each sample is in the folder `3_Structure/3.1aa_PCA`   

### pi, dxy, and Fst estimates
Instructions for replicating the estimates of pi, dxy, and Fst are in the file `3_Structure/3.3aa_pixy.md`, and the code for calculating the genome-wide averages is in the R markdown file `3_Structure/3.3aa_pixy.Rmd`. The raw output is in the folder `3_Structure/3.3aa_pixy`.  

### Tajima's D
Instructions for replicating the Tajima's D estimates are in the file `4_Demography/4.2_tajimasD.md` and the raw results are in the folder `4_Demography/4.2_tajimasD`.  The input dataset for Tajima's D is `Ceratopipra_rubrocapilla.GBSPipfilbwa.allsites.filtered.genicintergenic.forSVD.AC0.37_0.2_5_20.0.vcf.gz` which is in the folder `/1_Datasets/1.3a_genotyping/filteredSNPs`.  

### Introgression analyses
The folder `5_Introgression` contains the raw results and instructions for replicating the ABBA BABA tests. The input dataset for this analysis is `Ceratopipra_rubrocapilla_imeriout_m07.GBSPipfilbwa.allsites.filtered.genicintergenic.forSVD.49_0.2_5_20.vcf.gz`, found in the folder `1_Datasets/1.3a_genotyping/filteredSNPs`.  

### Demographic simulations

3_Structure/3.3aa_pixy.Rmd
3_Structure/3.2aa_STRUCTURE.Rmd