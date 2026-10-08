# Visualize Plastid Genome Structure

## Student Information

**Name:** Junavhel Jane B. Olaguir  
**Program/Course:** BS Biology  
**Section:** A  
**Subject:** Cell and Molecular Biology  

## 1. Selected Plant

**Scientific Name:** *Curcuma longa*  
**Common Name:** Turmeric  
**Family:** Zingiberaceae  

The same plastid genome selected in the previous plastid genome characterization activity was used in this activity to generate and examine a graphical representation of its genome structure.

## 2. NCBI Accession and Genome Information

- **NCBI Accession:** NC_042886.1
- **Genome Type:** Complete chloroplast genome
- **Plastid Genome Length:** 159,550 bp
- **Topology:** Circular
- **Database:** NCBI Reference Sequence (RefSeq)
- **Genome Record:** https://www.ncbi.nlm.nih.gov/nuccore/NC_042886.1

The annotated GenBank file used for visualization was:

`Curcuma_longa_NC_042886.1.gb`

The GenBank file was obtained from the NCBI record for *Curcuma longa* and contains the nucleotide sequence together with its gene annotations.

## 3. Software Used

**Software:** OGDRAW (OrganellarGenomeDRAW)

**OGDRAW website:**  
https://chlorobox.mpimp-golm.mpg.de/OGDraw.html

OGDRAW was used to convert the annotated GenBank file into a graphical map of the chloroplast genome. OGDRAW accepts annotated GenBank or EMBL/ENA files and generates graphical maps of organellar genomes, including plastid genomes.

## 4. OGDRAW Settings

The following settings were used to generate the *Curcuma longa* plastid genome map:

| Setting | Selected Option |

| Mode | Standard |

| Input file | `Curcuma_longa_NC_042886.1.gb` |

| Genome map | Circular |

| Sequence source | Plastid |

| Inverted repeat detection | Automatic |

| GC content graph | Enabled |

| Direction of transcription | Enabled |

| Full legend | Enabled |

| Intron-containing gene labels | Enabled |

| Output format | PNG |

| Gene categories | Major plastid gene groups and other available features |

The standard circular plastid map was generated using the annotated GenBank file. Automatic inverted-repeat detection was used to identify the IR regions. The GC content graph, transcription directions, full legend, and intron-containing gene labels were also enabled.

## 5. Plastid Genome Map

The resulting OGDRAW map of the *Curcuma longa* chloroplast genome is shown below.

![Plastid genome map](Lab_Plastid_Genome_Visualization/Figures/Curcuma_longa_plastid_map.png)

**Figure 1.** Circular plastid genome map of *Curcuma longa* generated using OGDRAW from the annotated GenBank accession NC_042886.1.

## 6. Main Structural Features Observed

The *Curcuma longa* chloroplast genome exhibits the typical quadripartite organization of an angiosperm plastid genome. The circular genome contains a **Large Single-Copy (LSC) region**, a **Small Single-Copy (SSC) region**, and two **Inverted Repeat regions (IRa and IRb)**.

The genome is **159,550 bp** long. The LSC region is approximately **87,058 bp**, the SSC region is approximately **18,542 bp**, and each inverted repeat is approximately **26,975 bp**. The overall organization can therefore be represented as:

**LSC – IR – SSC – IR**

The map displays numerous protein-coding genes, transfer RNA genes, and ribosomal RNA genes distributed around the genome. Genes located within the inverted-repeat regions can occur in duplicated copies because the two IR regions contain corresponding repeated sequences.

The map also displays the direction of transcription using gene arrows. The GC content graph provides a visual representation of nucleotide composition across different regions of the plastid genome. Intron-containing genes are additionally marked according to the selected OGDRAW settings.

## 7. Important Genome Features

The OGDRAW map allows the following features to be examined:

- Large Single-Copy (LSC) region
- Small Single-Copy (SSC) region
- Inverted Repeat A (IRa)
- Inverted Repeat B (IRb)
- Protein-coding genes
- tRNA genes
- rRNA genes
- Genes duplicated within the IR regions
- Direction of transcription
- Intron-containing genes
- GC content distribution

The visualization provides a clearer representation of plastid genome organization than viewing the raw nucleotide sequence or a long list of GenBank annotations.

## 8. Genome Visualization Workflow

The activity was performed using the following workflow:

1. The previously selected *Curcuma longa* plastid genome was retained for this activity.
2. The annotated GenBank file `Curcuma_longa_NC_042886.1.gb` was prepared.
3. OGDRAW was opened through the CHLOROBOX website.
4. The annotated GenBank file was uploaded.
5. Standard mode was selected.
6. Circular genome map and Plastid sequence source were selected.
7. Automatic inverted-repeat detection was enabled.
8. The GC content graph was enabled.
9. Direction of transcription was enabled.
10. The full legend was enabled.
11. Intron-containing gene labeling was enabled.
12. The map was generated and saved as a PNG file.
13. The final map was placed in the `figures` folder.

## 9. Answers to the Activity Questions

The detailed answers to the ten questions in Part E are provided in:

[**Lab_plastid_genome_answers.md**](Lab_Plastid_Genome_Visualization/Answers)

10. Conclusion
The OGDRAW visualization provides a graphical representation of the Curcuma longa chloroplast genome and makes its major structural features easier to identify and interpret. The map demonstrates the characteristic LSC–IR–SSC–IR organization and allows the distribution, orientation, and functional groups of plastid genes to be examined. The visualization also provides information about duplicated genes within the IR regions, intron-containing genes, and variation in GC content across the genome.
This activity connects the annotated GenBank sequence used in the previous plastid genome characterization activity with a visual representation of the same genome, providing a clearer understanding of plastid genome structure and gene organization.

## 11. Data Source

NCBI Accession: NC_042886.1
Organism: Curcuma longa
Database: NCBI Reference Sequence (RefSeq)
NCBI Record:
https://www.ncbi.nlm.nih.gov/nuccore/NC_042886.1

## 12. OGDRAW Reference

OGDRAW (OrganellarGenomeDRAW). CHLOROBOX, Max Planck Institute of Molecular Plant Physiology.
https://chlorobox.mpimp-golm.mpg.de/OGDraw.html
Greiner, S., Lehwark, P., & Bock, R. (2019). OrganellarGenomeDRAW (OGDRAW) version 1.3.1: expanded toolkit for the graphical visualization of organellar genomes. Nucleic Acids Research, 47, W59–W64.
