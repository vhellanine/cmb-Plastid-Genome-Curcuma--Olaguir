# cmb-Plastid-Genome-Curcuma--Olaguir

This repository contains the data, workflow, results, and documentation for a Cell and Molecular Biology laboratory activity on the characterization of a complete plastid genome. The selected genus is *Curcuma*, with *Curcuma longa* (turmeric) used as the representative species.

The activity includes retrieval of a complete chloroplast genome from NCBI, FASTA sequence analysis using Galaxy, examination of the annotated GenBank/RefSeq record, characterization of genome organization and gene content, comparison of plastid and mitochondrial genomes, and documentation of the complete workflow in GitHub.

# 1. Student Information

**Student:** Junavhel Jane B. Olaguir  
**Course:** Cell and Molecular Biology  
**Section:** A  
**Laboratory Activity:** Characterization of a Plastid Genome

# 2. Selected Genus and Species

**Chosen genus:** *Curcuma*  
**Selected species:** *Curcuma longa* L.  
**Common name:** Turmeric  
**Family:** Zingiberaceae  
**Organelle:** Chloroplast  
**Genome type:** Complete chloroplast/plastid genome

The genus *Curcuma* was selected after checking the class list to ensure that it had not already been selected by another student. *Curcuma longa* was then selected because a complete, annotated chloroplast genome is available in NCBI.

# 3. NCBI Data Source

**Database:** NCBI Nucleotide / RefSeq  
**Accession:** NC_042886.1  
**Organism:** *Curcuma longa* voucher wen13706  
**Description:** *Curcuma longa* voucher wen13706 chloroplast, complete genome  
**Genome topology:** Circular  
**Molecule type:** DNA

**NCBI record:**  
https://www.ncbi.nlm.nih.gov/nuccore/NC_042886.1

The NC_042886.1 record is identified by NCBI as a complete chloroplast genome. The GenBank annotation also identifies the record as a circular DNA molecule and states that the reference is full length.


# 4. Date the Genome Was Retrieved

**Date retrieved:** October 7, 2026

The complete chloroplast genome and its corresponding annotated GenBank record were retrieved from the NCBI Nucleotide database for the laboratory analysis.

# 5. Genome Size and Plastome Summary

## Verified GenBank/NCBI annotation

The uploaded NC_042886.1 GenBank record reports:

| Feature | Result |
| Organism | *Curcuma longa* |
| Accession/version | NC_042886.1 |
| Genome length | **159,550 bp** |
| Topology | **Circular** |
| GC content | **36.3%** (published characterization) |
| Genome type | Complete chloroplast genome |

The complete chloroplast genome is organized into the typical quadripartite structure consisting of a Large Single-Copy (LSC) region, a Small Single-Copy (SSC) region, and two Inverted Repeat (IR) regions.

For the NC_042886.1 plastome, the published characterization reports:

| Plastome region | Size |
| LSC | **87,058 bp** |
| SSC | **18,542 bp** |
| IRa | **26,975 bp** |
| IRb | **26,975 bp** |

The IR size is calculated from the complete genome length after subtracting the reported LSC and SSC sizes.

## Current Galaxy run

The current Galaxy FASTA-statistics screenshot produced the following values:

| Galaxy statistic | Current result |
| Genome length | **168,985 bp** |
| Number of sequence records | **1** |
| GC content | **36.82%** |
| A | 53,058 |
| T | 53,713 |
| C | 31,515 |
| G | 30,699 |
| N | 0 |
| Scaffold N50 | 168,985 bp |
| Scaffold L50 | 1 |

These Galaxy values are retained as the results of the current run, but they should **not be presented as the final statistics for NC_042886.1 until the FASTA/GenBank discrepancy is resolved**.

# 6. Evidence That the Sequence Is a Complete Plastid Genome

The selected record is appropriate for plastid-genome characterization because:

1. The NCBI record identifies it as a **chloroplast, complete genome**.
2. The GenBank LOCUS line identifies NC_042886 as a **159,550-bp circular DNA molecule**.
3. The record contains extensive annotated genomic features rather than only a single barcode marker.
4. The annotation contains protein-coding sequences, tRNA genes, and rRNA genes characteristic of a chloroplast genome.
5. The record is described as **full length** in the RefSeq comment.

Therefore, NC_042886.1 represents a complete chloroplast genome rather than an isolated barcode gene, genome fragment, or raw sequencing-read dataset.

# 7. Galaxy Analysis

## Galaxy History

**History name:** `Plastid_Curcuma_Olaguir`

## Input dataset

**Dataset:** `Curcuma_longa_NC_042886.1.fasta`

The chloroplast genome sequence was downloaded from NCBI in FASTA format and uploaded to the student's own Galaxy account. Galaxy recognized the sequence as a FASTA dataset.

## Galaxy tool used

**Tool:** FASTA Statistics / `gfastats`

The tool was used to obtain basic sequence statistics, including sequence length, number of sequence records, nucleotide composition, GC content, N50, and L50.

The current Galaxy run showed one sequence record and therefore an N50 equal to the sequence length and an L50 of 1.

A screenshot of the Galaxy history, uploaded sequence, and successful FASTA-statistics output is stored in the `figures/` directory.

# 8. Plastid Genome Organization and Annotated Gene Content

The annotated GenBank record for NC_042886.1 contains the following feature counts:

| Annotated feature | Number |
| **Gene features** | **133** |
| **CDS features** | **86** |
| **tRNA features** | **38** |
| **rRNA features** | **8** |
| **Pseudogene features** | **1** |

The 133 gene features include duplicated genes associated with the inverted-repeat regions and one annotated *ycf1* pseudogene. The 86 CDS features represent the annotated protein-coding sequences; the 38 tRNA and 8 rRNA features complete the annotated gene-feature count.

## Pseudogene

One *ycf1* gene feature is explicitly annotated as a **pseudogene**. A second *ycf1* copy is annotated as a CDS, illustrating the presence of an IR-associated duplicated region with one copy affected by pseudogenization.

## Duplicated protein-coding genes

The following protein-coding genes occur in two annotated copies:

- *rps7*
- *rps12*
- *rps19*
- *rpl2*
- *rpl23*
- *ndhB*
- *ycf2*

## Duplicated tRNA genes

The following tRNA genes occur in duplicated copies:

- *trnH-GUG*
- *trnL-CAA*
- *trnV-GAC*
- *trnI-GAU*
- *trnA-UGC*
- *trnR-ACG*
- *trnN-GUU*

The annotation contains three copies of *trnM-CAU*.

## rRNA genes

Eight rRNA features are annotated, representing two copies each of the four major chloroplast rRNA types:

- 16S rRNA
- 23S rRNA
- 4.5S rRNA
- 5S rRNA

This duplication is consistent with their occurrence within the inverted-repeat regions.

# 9. Important Genes, Introns, and Structural Observations

## Selected protein-coding genes and functions

At least eight protein-coding genes from different functional groups were identified from the annotation:

| Gene | Functional group | Biological function |
| *psbA* | Photosystem II | Encodes the Photosystem II D1 reaction-center protein |
| *psaA* | Photosystem I | Encodes a major Photosystem I reaction-center protein |
| *atpA* | ATP synthase | Encodes the CF1 alpha subunit of chloroplast ATP synthase |
| *rbcL* | Carbon fixation | Encodes the large subunit of RuBisCO |
| *rpoC2* | Transcription | Encodes the beta-prime subunit of the plastid-encoded RNA polymerase |
| *rpl2* | Translation | Encodes ribosomal protein L2 |
| *matK* | RNA processing | Encodes maturase K, associated with intron processing |
| *clpP* | Protein turnover | Encodes the proteolytic subunit of the chloroplast Clp protease |

## Intron-containing genes

The GenBank annotation contains split features consistent with intron-containing genes. The following 18 distinct genes have multi-part annotated features:

**Protein-coding genes:**
- *atpF*
- *clpP*
- *ndhA*
- *ndhB*
- *petB*
- *petD*
- *rpl16*
- *rpl2*
- *rpoC1*
- *rps12*
- *rps16*
- *ycf3*

**tRNA genes:**
- *trnA-UGC*
- *trnG-GCC*
- *trnI-GAU*
- *trnK-UUU*
- *trnL-UAA*
- *trnV-UAC*

The *ycf3* and *clpP* genes contain two introns, while the other listed intron-containing genes contain one intron or have split annotations associated with their genomic structure.

## Important structural observations

1. The genome has a **circular topology**.
2. The plastome has the typical **LSC–IR–SSC–IR** organization.
3. Several genes occur in duplicated copies because of the two inverted-repeat regions.
4. *rps12* shows a trans-spliced organization, with its exons distributed between the LSC and IR regions.
5. One *ycf1* copy is annotated as a pseudogene.
6. The annotation contains numerous intron-containing genes, including *clpP* and *ycf3*, which have two introns.

# 10. Plastid vs. Mitochondrial Genome Comparison

| Feature | Plastid genome | Mitochondrial genome |
| Cellular location | Plastids, especially chloroplasts in photosynthetic plant cells | Mitochondria |
| Main biological functions | Photosynthesis, carbon fixation, plastid gene expression, and related metabolic functions | Cellular respiration, oxidative phosphorylation, and mitochondrial gene expression |
| Typical genome organization | Usually compact; many angiosperm plastomes have LSC, SSC, and two IR regions | Plant mitochondrial genomes are generally more structurally variable and may contain complex arrangements |
| Relative genome size | Usually around 100–200 kb in many land plants | Plant mitochondrial genomes are often considerably larger and more variable in size |
| Gene content | Includes photosynthesis, transcription, translation, and RNA-processing genes | Primarily contains genes associated with respiration, oxidative phosphorylation, and mitochondrial functions |
| Copy number | Multiple plastid genome copies can occur within plastids/cells | Multiple mitochondrial genome copies can occur within mitochondria/cells |
| Inheritance | Often maternal in angiosperms, but inheritance varies among lineages | Often maternal in angiosperms, with lineage-dependent variation |
| Recombination / structural change | Generally more structurally conserved, although rearrangements can occur | Often exhibits greater structural variation and recombination |
| Mutation / substitution pattern | Useful for phylogenetic, phylogeographic, and species-level analyses | Shows different evolutionary patterns and can be useful for mitochondrial inheritance and evolutionary studies |
| Common research applications | Plant identification, phylogenetics, phylogeography, genome evolution, DNA barcoding, and plastid engineering | Mitochondrial evolution, cytoplasmic inheritance, respiration, cytoplasmic male sterility, and organelle genetics |

# Data Sources

1. **National Center for Biotechnology Information (NCBI) Nucleotide / RefSeq**  
   *Curcuma longa* voucher wen13706 chloroplast, complete genome. Accession **NC_042886.1**.

2. **Galaxy Project**  
   Galaxy FASTA Statistics / `gfastats` was used to obtain basic sequence statistics from the uploaded FASTA dataset.

3. **Cell and Molecular Biology Laboratory Manual**  
   *Characterization of a Plastid Genome*. The manual provided the required NCBI retrieval, Galaxy workflow, plastid-genome characterization, plastid-versus-mitochondrial comparison, and GitHub documentation requirements.

# Conclusion

The complete chloroplast genome of *Curcuma longa* was selected for characterization using NCBI and Galaxy. The verified NC_042886.1 GenBank record is a circular, complete chloroplast genome of **159,550 bp** containing **133 annotated gene features, 86 CDS features, 38 tRNA features, and 8 rRNA features**, with one *ycf1* pseudogene.

The annotation also demonstrates duplicated genes associated with the inverted-repeat regions and multiple intron-containing genes, including *clpP* and *ycf3*. These features illustrate the compact yet structurally complex organization of an angiosperm plastid genome.

Before final submission, the FASTA used in Galaxy should be verified against NC_042886.1 so that the Galaxy sequence statistics and GenBank annotation describe exactly the same genome.

# References

Windsor, A. M., Ott, B. M., Zhang, N., Wen, J., Hsu, E., & Handy, S. M. (2019). Full chloroplast genome sequence of the economically important dietary supplement and spice *Curcuma longa*. *Microbiology Resource Announcements, 8*(32), e00576-19.

National Center for Biotechnology Information. *Curcuma longa* voucher wen13706 chloroplast, complete genome. RefSeq accession **NC_042886.1**.

Li, D.-M., et al. (2019). Characterization and phylogenetic analysis of the complete chloroplast genome of *Curcuma longa* (Zingiberaceae). *Mitochondrial DNA Part B, 4*(2), 2974–2975.

Galaxy Training Network. FASTA Statistics / sequence statistics documentation.

Cell and Molecular Biology Laboratory Manual. (2026). *Characterization of a Plastid Genome*.
