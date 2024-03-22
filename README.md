# Ceratopipra_rubrocapilla_Phylogeography
 
The folder `1_Datasets` contains FastQC reports for the raw and trimmed sequencning data, as well as records of the logs produced by Trimmomatic during trimming of the sequencing reads.

# map of genetic gradient  
Instructions for replicating the map illustrating the genetic gradient across *C. rubrocapilla* are in the file `3_Structure/3.5aa_gradients.md`. The input data for this analysis is `Ceratopipra_rubrocapilla.GBSPipfilbwa.allsites.filtered.genicintergenic.forSVD.AC0.37_0.2_5_20.0.vcf.gz`, found in the folder `1_Datasets/1.3a_genotyping/filteredSNPs`.  

# pi, dxy, and Fst estimates
Instructions for replicating the estimates of pi, dxy, and Fst are in the file `3_Structure/3.3aa_pixy.md`, and the code for calculating the genome-wide averages is in the R markdown file `3_Structure/3.3aa_pixy.Rmd`.  

# Tajima's D
Instructions for replicating the Tajima's D estimates are in the file `4_Demography/4.2_tajimasD.md` and the raw results are in the folder `4_Demography/4.2_tajimasD`.  The input dataset for Tajima's D is `Ceratopipra_rubrocapilla.GBSPipfilbwa.allsites.filtered.genicintergenic.forSVD.AC0.37_0.2_5_20.0.vcf.gz` which is in the folder `/1_Datasets/1.3a_genotyping/filteredSNPs`.  

# Introgression analyses
The folder `5_Introgression` contains the raw results and instructions for replicating the ABBA BABA tests. The input dataset for this analysis is `Ceratopipra_rubrocapilla_imeriout_m07.GBSPipfilbwa.allsites.filtered.genicintergenic.forSVD.49_0.2_5_20.vcf.gz`, found in the folder `1_Datasets/1.3a_genotyping/filteredSNPs`.  