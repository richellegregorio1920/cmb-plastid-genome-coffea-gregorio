# Final Report

This section compiles the complete workflow, characterization, and comparative analysis of the *Coffea arabica* chloroplast genome for this lab activity.

---

## I. Choosing and Recording a Plant Genus

For this project, the genus *Coffea* was chosen after verifying that complete, high-quality chloroplast genome sequences are available in public databases. Specifically, *Coffea arabica* (arabica coffee) was selected as our target species because its fully annotated plastid genome provides an ideal dataset for studying angiosperm chloroplast structure, gene organization, and organelle evolution.

---

## II. Data Source and Genome Selection

The complete chloroplast genome sequence for *Coffea arabica* was retrieved directly from the NCBI RefSeq database. The record represents a full-length, annotated plastid genome, and both the FASTA sequence and complete GenBank annotation file were retained for downstream analysis.

| Information | Details |
| :--- | :--- |
| **Organism** | *Coffea arabica* (Family: Rubiaceae) |
| **Chosen Genus** | *Coffea* |
| **Database Source** | NCBI RefSeq / Nucleotide |
| **NCBI Accession/Version** | EF044213.1 |
| **Genome Type** | Chloroplast / plastid genome |
| **Genome Completeness** | Complete genome / full length |
| **Genome Length** | 155,189 bp |
| **Topology** | Circular |
| **Associated Publication** | The complete nucleotide sequence of the coffee (*Coffea arabica* L.) chloroplast genome |
| **Authors** | Samson, N., et al. |
| **FASTA File Retained** | `Coffea_arabica_EF044213.1.fasta` |
| **Annotated GenBank File Retained** | `Coffea_arabica_EF044213.1.gb.txt` |

---

## III. Files to Obtain

To complete the bioinformatics workflow, the core sequence files required for sequence statistics and feature annotation review were organized as follows:

| File Format | File / Source | Purpose |
| :--- | :--- | :--- |
| **Genome sequence (FASTA)** | `Coffea_arabica_EF044213.1.fasta` | Uploaded to UseGalaxy to verify sequence length, GC content, and continuity. |
| **Annotated genome (GenBank)** | `Coffea_arabica_EF044213.1.gb` | Used to inspect gene coordinates, functional groups, introns, and structural boundaries. |
| **Source record (NCBI RefSeq)** | EF044213.1 | Documented the official accession and biological background of the target sample. |

---

## IV. Galaxy Workflow and Sequence Statistics

After uploading the FASTA file to the UseGalaxy platform, the **FASTA Statistics** tool was run to confirm the basic compositional metrics of the *Coffea arabica* plastome.

### Galaxy FASTA Statistics
| Statistic | Result |
| :--- | :--- |
| **Genome length** | 155,189 bp |
| **Number of sequence records** | 1 (Single continuous contig) |
| **GC content** | 37.43% |
| **Number of gaps** | 0 |
| **Complete plastome represented by one sequence record?** | Yes |

The Galaxy output confirms that the *Coffea arabica* chloroplast genome is an intact, continuous sequence spanning exactly 155,189 base pairs with a GC content of 37.43% and zero internal gaps. This verifies that the dataset is pristine and fully ready for detailed annotation analysis.

### Galaxy Workflow Screenshot
![Figure 1. UseGalaxy FASTA Statistics Output](https://raw.githubusercontent.com/richellegregorio1920/cmb-plastid-genome-coffea-gregorio/main/Figures/Galaxy_Fasta_Statistics_Coffea_arabica.png)  
*Figure 1. Overview of the UseGalaxy workflow history (`Plastid_Coffea_Gregorio`) showing the FASTA statistics results for the Coffea arabica nucleotide dataset (Accession: EF044213.1).*

### Galaxy History Details
* **History Name:** `Plastid_Coffea_Gregorio`
* **Tool Used:** FASTA Statistics
* **Galaxy History Link:** [https://usegalaxy.org/u/richelle_gregorio/h/plastid-coffea-gregorio](https://usegalaxy.org/u/richelle_gregorio/h/plastid-coffea-gregorio)

---

## V. Required Plastid Genome Characterization

Synthesizing data from the GenBank annotation file and our Galaxy statistics, the *Coffea arabica* plastome exhibits the classic circular, quadripartite architecture typical of land plant chloroplasts.

| Characteristic | Result |
| :--- | :--- |
| **Chosen genus & species** | *Coffea arabica* (Rubiaceae) |
| **NCBI accession** | EF044213.1 |
| **Genome size & GC content** | 155,189 bp; 37.43% GC |
| **Topology & Regions** | Circular; structured into Large Single-Copy (LSC), Small Single-Copy (SSC), and two Inverted Repeats (IR) |
| **Annotated gene content** | ~130 total gene entries, including ~79 protein-coding CDS, ~29 tRNAs, and 4 unique rRNAs |
| **Introns & Duplications** | Group II introns present in select genes (*trnK*, *rps16*); standard gene duplications located within the IR boundaries |
| **Structural status** | Stable, compact asterid chloroplast architecture |

---

## VI. Gene Groups Identified

The annotated genome contains a robust suite of genes categorized into major functional machinery:

* **Photosystem I (*psa*):** *psaA*, *psbB*-related core complexes, *psaC*, *psaI*, *psaJ*
* **Photosystem II (*psb*):** *psbA* (D1 protein), *psbB*, *psbC*, *psbD*, and associated reaction center subunits (*psbE* through *psbZ*)
* **ATP Synthase (*atp*):** *atpA*, *atpB*, *atpE*, *atpF*, *atpH*, *atpI*
* **Cytochrome b6/f (*pet*):** *petA*, *petB*, *petD*, *petG*, *petL*, *petN*
* **Carbon Fixation:** *rbcL* (RuBisCO large subunit)
* **Transcription & Translation:** Plastid RNA polymerase subunits (*rpoA*, *rpoB*, *rpoC1*, *rpoC2*), large ribosomal proteins (*rpl* series), and small ribosomal proteins (*rps* series)
* **RNAs:** Ribosomal RNAs (*rrn16*, *rrn23*, *rrn4.5*, *rrn5*) and various transfer RNAs (*trn*)

---

## VII. Questions & Answers

#### VII.1. Give the full scientific name, family, NCBI accession/version, database source, and complete plastid-genome size of your selected organism. 
* The selected organism is *Coffea arabica* (family Rubiaceae). Its complete chloroplast genome was obtained from the NCBI RefSeq/Nucleotide database under accession number EF044213.1, with a total length of 155,189 bp.

#### VII.2. What evidence shows that the sequence is a complete plastid/chloroplast genome rather than a barcode marker, genome fragment, or nuclear sequence?
* The NCBI record explicitly labels the entry as a complete chloroplast genome and designates the organelle source as plastid. Furthermore, its full-length circular topology and comprehensive coverage of photosynthetic and housekeeping gene suites confirm it is a whole plastome rather than a partial fragment or nuclear contaminant.

#### VII.3. Describe the overall organization of the plastid genome. Does it contain the common LSC-IR-SSC-IR arrangement? Give the sizes of these regions when available.
* Yes, the genome follows the standard angiosperm quadripartite structure consisting of a Large Single-Copy (LSC) region, a Small Single-Copy (SSC) region, and two symmetric Inverted Repeat (IR) regions.

#### VII.4. Summarize the annotated gene content: total genes, protein-coding genes, tRNA genes, rRNA genes, and pseudogenes. Explain why genes located in the inverted-repeat regions may appear in two copies. 
* The annotation features ~130 total genes (~79 protein-coding CDS, ~29 tRNAs, and 4 unique rRNAs). Genes located in the IRa and IRb segments appear in duplicate because the duplication of these large repeat blocks inherently copies any resident genes.

#### VII.5. Choose at least eight protein-coding plastid genes from different functional groups. List each gene and briefly explain its biological function.
* *psaA* – Core Photosystem I protein driving electron transport.  
* *psbA* – Photosystem II D1 reaction center protein.  
* *atpB* – Subunit of ATP synthase for cellular energy generation.  
* *petA* – Cytochrome f component of the cytochrome b6/f complex.  
* *rbcL* – RuBisCO large subunit responsible for carbon fixation.  
* *rpoB* – Subunit of plastid-encoded RNA polymerase.  
* *rpl2* – Structural protein of the large ribosomal subunit.  
* *rps16* – Structural protein of the small ribosomal subunit.

#### VII.6. Identify important RNA and RNA-processing features. Include the rRNA genes, examples of tRNA genes, and at least two genes with introns if present in your genome.
* The genome encodes standard rRNAs (*rrn16*, *rrn23*, *rrn4.5*, *rrn5*) and diverse tRNAs (such as *trnH-GUG*, *trnK-UUU*, and *trnL-UAA*). Introns are reliably found in genes like *trnK* and *rps16*.

#### VII.7. Describe any pseudogenes, gene losses, duplications, rearrangements, or other unusual features reported for your plastid genome.
* No pseudogenes are explicitly annotated in the reference file. The *Coffea arabica* plastome maintains a highly conserved, stable architecture typical of asterid lineages.

#### VII.8. What is the GC content of your plastid genome? Based on your Galaxy results and annotation, describe two other notable sequence or structural observations.
* The GC content is 37.43%. Key structural observations include its single continuous contig representation and the clear preservation of the quadripartite LSC/SSC/IR layout.

#### VII.9. Compare plastid and mitochondrial genomes.
* Both are semi-autonomous cytoplasmic organelle genomes containing multiple cellular copies and coding for core translation machinery (Birky, 2001). However, while plastid genomes are compact, circularly mapped, and dedicated primarily to photosynthesis (Park et al., 2019; Wicke et al., 2011), plant mitochondrial genomes are vastly larger, structurally multipartite, highly prone to repeat-mediated recombination, and centered around cellular respiration (Ni et al., 2023; Smith & Keeling, 2015).

#### VII.10. Explain the practical value of plastid genomes in research. Include advantages, limitations, and examples of research questions.
* Plastid genomes are exceptionally useful for phylogenetics, molecular barcoding, and maternal lineage tracing due to their conserved structure and haploid, maternal inheritance (Birky, 2001; Wicke et al., 2011). However, they only represent uniparental chloroplast evolution and cannot capture nuclear genomic complexity.  
***Plastid research question example:*** How do maternal lineages vary across wild and cultivated *Coffea arabica* populations?  
***Nuclear research question example:*** Which nuclear alleles control complex agronomic traits like disease resistance and cup quality?

----

## VIII. Plastid vs. Mitochondrial Genome Comparison

Both plastid and mitochondrial genomes are semi-autonomous cytoplasmic organelle genomes that exist in multiple cellular copies and encode their own translation machinery (Birky, 2001). However, they exhibit differences in their structure, function, and evolutionary dynamics.

| Feature | Plastid Genome (*Coffea arabica*) | Mitochondrial Genome (*Coffea arabica*) |
| :--- | :--- | :--- |
| **Cellular location** | Localized within chloroplasts in the plant cell cytoplasm (Wicke et al., 2011). | Localized within plant mitochondria, frequently incorporating migrated chloroplast sequences (Ni et al., 2023). |
| **Main biological functions** | Dedicated to photosynthesis, carbon fixation, and plastid gene expression (Park et al., 2019; Wicke et al., 2011). | Dedicated to cellular respiration, oxidative phosphorylation, ATP production, and high-frequency RNA editing (Ni et al., 2023) |
| **Typical genome organization** | Compact circular molecule featuring the classic quadripartite structure (LSC, SSC, and two IRs) (Park et al., 2019). | Complex multichromosomal architecture (e.g., multiple chromosomes) with multi-conformation fluidity (Ni et al., 2023) |
| **Relative genome size** | Compact and relatively small, measuring ~155,189 bp (Park et al., 2019). | Significantly larger, spanning over 1 million base pairs across multiple configurations (Ni et al., 2023). |
| **Gene content** | ~130–131 total genes focused on photosynthesis, tRNAs, and rRNAs (Park et al., 2019). | Core respiration genes (*atp*, *cox*, *nad*), rRNAs, tRNAs, and integrated chloroplast DNA fragments (Ni et al., 2023). |
| **Copy number** | High polyploidy per plant cell across multiple chloroplast copies (Birky, 2001). | Multiple copies per mitochondrion and cell, varying across tissue types (Birky, 2001; Ni et al., 2023). |
| **Inheritance** | Typically maternally inherited in angiosperms (Birky, 2001). | Maternally inherited, though shaped by dynamic intracellular DNA transfer (Birky, 2001; Ni et al., 2023). |
| **Recombination / structural change** | Highly conserved structure with stable gene order (Park et al., 2019; Wicke et al., 2011). | Highly dynamic with frequent repeat-mediated recombination and structural restructuring (Ni et al., 2023; Sakamoto et al., 2020). |
| **Mutation / substitution pattern** | Moderate, stable substitution rates typical of asterid plastomes (Park et al., 2019). | Low synonymous substitution rates paired with high structural plasticity and extensive C-to-U RNA editing (Ni et al., 2023; Sakamoto et al., 2020). |
| **Research applications** | Species identification, maternal barcoding, and comparative phylogenetics (Park et al., 2019; Wicke et al., 2011). | Investigating cytoplasmic male sterility, cp-to-mitochondrial gene migration, and recombination (Ni et al., 2023; Smith & Keeling, 2015). |

---

## IX. References

* Birky, C. W., Jr. (2001). The inheritance of genes in mitochondria and chloroplasts: Laws, mechanisms, and models. *Annual Review of Genetics*, 35, 125–148. https://doi.org/10.1146/annurev.genet.35.102401.090231
* National Center for Biotechnology Information. (n.d.). *Coffea arabica* chloroplast, complete genome (EF044213.1). NCBI Nucleotide. https://www.ncbi.nlm.nih.gov/nuccore/EF044213.1
* Ni, Y., et al. (2023). Genetic diversity of *Coffea arabica* L. mitochondrial genomes caused by repeat-mediated recombination and RNA editing. *Frontiers in Plant Science*, 14, 1261012. https://doi.org/10.3389/fpls.2023.1261012
* Park, J., Kim, Y., Xi, H., & Heo, K.-I. (2019). The complete chloroplast genome of coffee tree, *Coffea arabica* L. 'Blue Mountain' (Rubiaceae). *Mitochondrial DNA Part B*, 4(2), 2436–2437. https://doi.org/10.1080/23802359.2019.1624213
* Samson, N., et al. (2007). The complete nucleotide sequence of the coffee (*Coffea arabica* L.) chloroplast genome: organization and implications for biotechnology and phylogenetic relationships amongst angiosperms. *GenBank Accession EF044213.1*.
* Sakamoto, W., Takami, T., & Beppu, T. (2020). DNA repair and the stability of the plant mitochondrial genome. *International Journal of Molecular Sciences*, 21(2), 328. https://doi.org/10.3390/ijms21020328
* Smith, D. R., & Keeling, P. J. (2015). Mitochondrial and plastid genome architecture: Reoccurring themes, but significant differences at the extremes. *Proceedings of the National Academy of Sciences*, 112(33), 10177–10184. https://doi.org/10.1073/pnas.1422049112
* Wicke, S., Schneeweiss, G. M., dePamphilis, C. W., Müller, K. F., & Quandt, D. (2011). The evolution of the plastid chromosome in land plants: Gene content, gene order, gene function. *Plant Molecular Biology*, 76, 273–297. https://doi.org/10.1007/s11103-011-9762-4

