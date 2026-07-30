# Python scripts used for data aggegation in the publication: 
# Functional metatranscriptomics of the rhizosphere: towards an understanding of metabolic processes of the microbial carbon pump
The scripts have been developed and executed as Jupyter notebooks on a high-performance computing cluster running AlmaLinux with glibc 2.34. A Conda environment with Python 3.11 and the required dependencies has been used. Because the scripts primarily parse, filter, merge, and aggregate text-based output files, they do not require specialized hardware and may also be executed on a standard workstation, depending on the size of the input files.

The summarize_kofamscan_add_megan_tax script uses RSEM isoform abundance files, kofamscan annotation files and MEGAN taxonomic assignment as input. Kofamscan results are further filtered with an evalue=1e-10. The output is Sample-by-KO abundance tables containing TPM and expected counts with taxonomic annotation. 

Similarly, the dbcansummarize_cazy_add_megan_taxa script uses RSEM isoform abundance files, results from dbcan/hmmsearch and MEGAN taxonomic assignment as input. HMMER hits are filtered using an E-value threshold of 1 × 10⁻¹⁰ and a minimum HMM coverage of 30% before functional annotations are merged. The output is Sample-by-CAZy abundance tables containing TPM and expected counts with taxonomic annotation.
