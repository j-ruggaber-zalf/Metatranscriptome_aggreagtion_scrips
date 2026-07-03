# Python scripts used for data aggegation in the publication: 
# Functional metatranscriptomics of the rhizosphere: towards an understanding of metabolic processes of the microbial carbon pump
Scripts were run as Jupyter notebooks using Python3.6 on HPC running AlmaLinux (glibc 2.34). The script does not require specialized hardware as it is mostly parsing text and calculating TPM/RPKM.  

The parse cazy hmmr file uses hmmserach dbCAN files as input and calculates an intermediate lenght normalization, before TPM are RPKM are calculated de novo and parsed as tables.
The summarize_kofamscan_add_megan_tax uses RSEM isoforms, and results from kofamscan and adds the taxonomic best match fro MEGAN. TPM, RPK and RPKM are not calculated as they are provided from the input files already. 
