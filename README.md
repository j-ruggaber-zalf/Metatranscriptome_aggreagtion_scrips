# Python scripts used for data aggegation in the publication: 
# Functional metatranscriptomics of the rhizosphere: towards an understanding of metabolic processes of the microbial carbon pump
Scripts were run as Jupyter notebooks ona HPC running AlmaLinux (glibc 2.34). A conda environment with Python 3.11 installing the required packages was setup before runing the scripts as Jupyter notebooks. The script does not require specialized hardware as it is mostly parsing text from source files.  

The summarize_kofamscan_add_megan_tax uses RSEM isoforms, and results from kofamscan and adds the taxonomic best match from MEGAN. TPM, RPK, RPKM and counts are provided from the RSEM input files.
The summarize cazy---- likewise uses the RSEM isoforms and results from dbcan/hmmsearch and adds the best taxonomic match from MEGAN. Filtering of the hmm results with evalue of 1e-10 and hmmcovrage of 0.30 is done before parsing the results from the input files

