# Protein Modeling using ColabFold 

In this Repo I demonstrate and use the latest and in Protein Modeling made available through [ColabFold](https://github.com/sokrypton/ColabFold) notebooks.
For large number proteins sets I recommend using nf-core [proteinfold](https://github.com/nf-core/proteinfold/tree/1.0.0), more massive parallel processing of protein structures.

ColabFold is a community implementation of a Colab for running AlphaFold2. It offers many more adjustable parameters than AlphaFold2 Colab, such as the depth of the MSA and the number of recycles. Furthermore, ColabFold uses quick MSA preparation via the MMseqs2 server. You can also use a custom MSA as input and supply templates (Mirdita et al, 2022).



# Projects and Select Outputs:

## Brief Dataset & Project Description:

Amongst Dipterans, sequence alignment comparisons of olfactory receptors largely falls into the “twilight zone” in which sequence similarity is such that it can be difficult to distinguish between protein pairs of similar and non-similar structure [40–42]. Recent, cryo-electron microscopy studies of the Machilis hrabei Or5 found that the transmembrane region of the protein’s s2-s6 helixes formed a simple binding pocket which recognized odor-ligands using weak intermolecular interactions [43]. This would suggest that the ligand preference is largely determined by the pocket’s geometric shape formed by relationships of multiple helices. Three-dimensional structural comparison should provide insight on possible similarity of pocket formations independent of specific interacting residues. We therefore generated Alphafold2 predicted protein structure to allow for 3D structural comparison of our 24 candidates against the 15 known 1-octen-3-ol dipteran receptors using LGA for protein comparisons 

<img width="813" alt="Screenshot 2024-12-24 at 12 29 21 AM" src="https://github.com/user-attachments/assets/58a8854d-4a4a-4674-9225-e395fed03af7" />

Fig. Structural comparative analysis of candidate receptors with known 1-octen-3-ol receptors.
A. Heatmap of structure similarity score (LGA_S) values of candidate receptors superimposed onto known dipteran 1-octen-3-ol receptors generated using LGA program. Species shorthand: Ae. aegypti (AaOr), Ae. albopictus, (AalOr), An. gambiae (AgOr), C. quinquesfasciatus (CqOr), T. amboinensis (TaOr), B. dorsalis (BdorOr), B. minax (BminOr), D. melanogaster (DmelOr). B. Visualization of Alphafold2 generated 3D protein structures models of AaOr88 (orange) superimposed onto AalOr88 (green) along with corresponding structure similarly score. C. Rainbow palette of AaOr88 showing predicted binding pocket formed by its transmembrane helices, general area of pocket formed indicated by black dash-lined and transmembrane domains labeled S0 (purple) ‐ S7b (red).


## Brief Dataset & Project Description:

A total of 456 receptors were modeled using google colab. Amino acid sequences for D. melanogaster were sourced from uniprot.org. Sequences for C. quinquefasciatus, A.aegypti, A. albopictus, and A. gambiae receptors were sourced from Vectorbase. T.ambionenisis sequences were acquired from the supplementary of its primary study. B.dorasalis and B. minax sequences were acquired using provided accession number from the NCBI database. Olfactory receptors for A. aegypti, A. albopictus, and C. quinquefasciatus were identified from Vectorbase by searching for all genes with an associated description of Interpro IPR004117 (Olfactory receptor, insect) or PFAM: PF02949(7tm Odorant receptor). The amino acid of each receptor was then used to generate Protein models using ColabFold v1.5.1 :Alphafold2 using MMseq2 online server. The best-ranked model made by ColabFold were selected for downstream clustering and comparison.

<img width="598" alt="Screenshot 2024-12-24 at 2 30 25 AM" src="https://github.com/user-attachments/assets/ce29276f-ddff-41d9-afca-3f461d3c0262" />

Fig. Structural Heatmap of pairwise comparison of 209,764 protein pairs. Heatmap plots computed structural similarity score (LGA_S) consisting of 209,764 protein pairs comparisons of orphan mosquito receptors and all dipteran deorphanized receptors. Hierarchical clustering analysis uses average link clustering with maximum distance. 

