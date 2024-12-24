# Protein Modeling using ColabFold 

In this Repo I demonstrate and use the latest and in Protein Modeling made available through [ColabFold](https://github.com/sokrypton/ColabFold) notebooks.
For large number proteins sets I remind using nf-core [proteinfold](https://github.com/nf-core/proteinfold/tree/1.0.0), more massive parallel processing of protein structures.

ColabFold is a community implementation of a Colab for running AlphaFold2. It offers many more adjustable parameters than AlphaFold2 Colab, such as the depth of the MSA and the number of recycles. Furthermore, ColabFold uses quick MSA preparation via the MMseqs2 server. You can also use a custom MSA as input and supply templates (Mirdita et al, 2022).



# Projects and Select Outputs

Brief Dataset & Project Description:
Amino acid sequences for D. melanogaster were sourced from uniprot.org. Sequences for C. quinquefasciatus, A.aegypti, A. albopictus, and A. gambiae receptors were sourced from Vectorbase18 T.ambionenisis sequences were acquired from the supplementary of its primary study. B.dorasalis and B. minax sequences were acquired using provided accession number from the NCBI database. Olfactory receptors for A. aegypti, A. albopictus, and C. quinquefasciatus were identified from Vectorbase by searching for all genes with an associated description of Interpro IPR004117 (Olfactory receptor, insect) or PFAM: PF02949(7tm Odorant receptor). The amino acid of each receptor was then used to generate Protein models using ColabFold v1.5.1 :Alphafold2 using MMseq2 online server. The best-ranked model was selected for downstream clustering and comparison.

