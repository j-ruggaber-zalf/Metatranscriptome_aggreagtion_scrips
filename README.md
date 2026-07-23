# Python scripts used for data aggegation in the publication: 
# Functional metatranscriptomics of the rhizosphere: towards an understanding of metabolic processes of the microbial carbon pump
The scripts were developed and executed as Jupyter notebooks on a HPC running AlmaLinux (glibc 2.34). A Conda environment with Python 3.11 installing the required dependencies was used. The scripts primarily perform parsing and aggregation of text-based output files and therefore do not require specialized hardware.

The summarize_kofamscan_add_megan_tax uses RSEM isoform abundance files, kofamscan annotation files and MEGAN taxonomic assignment as input. Kofamscan result are further filtered with a evalue=1e-10.  The output is Sample-by-KO abundance tables containing TPM, expected counts, RPK, and RPKM with taxonomic annotation. 

dbcansummarize_cazy_add_megan_taxa likewise uses RSEM isoform abundance files, results from dbcan/hmmsearch and and MEGAN taxonomic assignment as input. HMMER hits are filtered using an E-value threshold of 1 × 10⁻¹⁰ and a minimum HMM coverage of 30% before functional annotations are merged.  The output is Sample-by-CAZy abundance tables containing TPM and expected counts with taxonomic annotation.
