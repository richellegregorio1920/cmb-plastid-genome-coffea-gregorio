# cmb-plastid-genome-Coffea-Gregorio
*Coffea arabica* Complete Chloroplast Genome Characterization and Analysis using NCBI, GALAXY, and Github for documentations.

## Student Information
* **Student Name:** Richelle Gregorio
* **Course & Section:** Cell and Molecular Biology - Section B

## Chosen Genus & Selected Species
* **Chosen Genus:** *Coffea*
* **Selected Species:** *Coffea arabica* (Arabica coffee)
* **Family:** Rubiaceae

## NCBI Accession & Source Link
* **NCBI Accession / Version:** `EF044213.1`
* **Database Source:** NCBI RefSeq / Nucleotide
* **Source Link:** [NCBI EF044213.1 Record](https://www.ncbi.nlm.nih.gov/nuccore/EF044213.1)

## Genome Retrieval Date
* **Date Retrieved:** October 2026

## Genome Size & Summary
* **Genome Size:** 155,189 base pairs (a complete, circular ring of DNA)
* **GC Content:** 37.43%
* **Summary:** The coffee plant's chloroplast DNA is a single, continuous loop with no missing pieces. Like most plants, it is split into four main sections: two large identical copies and two smaller unique sections.

## How the Genome Was Downloaded and Uploaded to Galaxy
I first went to the NCBI database and downloaded the complete chloroplast DNA file (in FASTA format) and the detailed feature file (GenBank format) using the accession number `EF044213.1`. After that, I uploaded the FASTA file to the UseGalaxy website so I could check its size, GC percentage, and structure.

## Galaxy History & Tools Used
* **Galaxy History Name:** `Plastid_Coffea_Gregorio`
* **Galaxy History Link:** [https://usegalaxy.org/u/richelle_gregorio/h/plastid-coffea-gregorio](https://usegalaxy.org/u/richelle_gregorio/h/plastid-coffea-gregorio)
* **Tools Used:** FASTA Statistics (used to confirm total length, check for gaps, and verify GC content).

## Complete Analysis Directory & File Paths
You can find all parts of this project organized across the repository folders:
* **Main README:** Located in the root folder (`/README.md`).
* **Data Folder:** Located at `Data/` (contains raw FASTA and GenBank sequence files).
* **Figures Folder:** Located at `Figures/` (contains Galaxy statistics screenshots).
* **Report Folder:** Located at `Report/` (contains Final completed reports).
* **Results Folder:** Located at `Results/` (contains `genome_summary.md`, gene group lists, and comparisons).

## Concise Summary of Gene Content & Important Observations

The chloroplast genome of *Coffea arabica* contains approximately 130 total genes that work together to maintain vital cellular functions. This gene suite includes around 79 protein-coding genes responsible for building core photosynthetic machinery like photosystems, ATP synthase, and RuBisCO, alongside 29 transfer RNA genes and 4 unique ribosomal RNA genes that manage protein synthesis. Looking at its structure, the plastome exhibits a classic, stable quadripartite architecture divided into a large single-copy region, a small single-copy region, and two identical inverted repeat regions where key rRNA and tRNA genes appear in duplicate. Furthermore, the genome features conserved group II introns in specific genes like *trnK* and *rps16* to help with RNA processing, all while maintaining a compact, continuous structure with zero internal gaps.

## Data Sources & References
* Birky, C. W., Jr. (2001). The inheritance of genes in mitochondria and chloroplasts: Laws, mechanisms, and models. *Annual Review of Genetics*, 35, 125–148. https://doi.org/10.1146/annurev.genet.35.102401.090231
* National Center for Biotechnology Information. (n.d.). *Coffea arabica* chloroplast, complete genome (EF044213.1). NCBI Nucleotide. https://www.ncbi.nlm.nih.gov/nuccore/EF044213.1
* Ni, Y., et al. (2023). Genetic diversity of *Coffea arabica* L. mitochondrial genomes caused by repeat-mediated recombination and RNA editing. *Frontiers in Plant Science*, 14, 1261012. https://doi.org/10.3389/fpls.2023.1261012
* Park, J., Kim, Y., Xi, H., & Heo, K.-I. (2019). The complete chloroplast genome of coffee tree, *Coffea arabica* L. 'Blue Mountain' (Rubiaceae). *Mitochondrial DNA Part B*, 4(2), 2436–2437. https://doi.org/10.1080/23802359.2019.1624213
* Samson, N., et al. (2007). The complete nucleotide sequence of the coffee (*Coffea arabica* L.) chloroplast genome: organization and implications for biotechnology and phylogenetic relationships amongst angiosperms. *GenBank Accession EF044213.1*.
* Wicke, S., Schneeweiss, G. M., dePamphilis, C. W., Müller, K. F., & Quandt, D. (2011). The evolution of the plastid chromosome in land plants: Gene content, gene order, gene function. *Plant Molecular Biology*, 76, 273–297. https://doi.org/10.1007/s11103-011-9762-4

## How Another Student Can Repeat This Analysis
If you want to do this project yourself, just follow these simple steps:
1. **Get the Data:** Go to the NCBI website, look up the coffee chloroplast genome using code `EF044213.1`, and download both the FASTA file and the GenBank file into your `Data/` folder.
2. **Use Galaxy:** Log into UseGalaxy, create a history named `Plastid_Coffea_Gregorio`, upload your FASTA file, and run the **FASTA Statistics** tool to check the size and GC content.
3. **Review the Genes:** Open the GenBank file (`.gb`) to see what genes are inside and how they are arranged.
4. **Compare Organelles:** Read up on plant mitochondria (such as Ni et al., 2023) to see how plant power-plant DNA differs from chloroplast food-making DNA.
