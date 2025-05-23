# A direct readout mechanism defines the sequence selectivity of human de novo DNA methyltransferases

The preprint describing our work: [![DOI:10.1101/2024.02.07.579311](http://img.shields.io/badge/DOI-10.1101/2024.02.07.579311-B31B1B.svg)](https://www.biorxiv.org/content/10.1101/2024.02.07.579311v2)

In mammals, de novo DNA methylation is essential to embryonic development, reprogramming, and gene regulation. The de novo DNA methylation is directed by DNMT3A and DNMT3B enzymes and mainly exerted on CpG islands. Over their enzymatic domains, DNMT3A/B proteins share over 90% of sequence similarity. Even so, DNMT3A predominantly methylates the first cytosine in the CGC and CGT motifs, while DNMT3B prefers the CGG and CGA sequences. To elucidate the mechanistic basis of these selective methylation profiles, we performed extensive molecular dynamics simulations of DNMT3A/B enzymes bound to all possible CGX[C/G/T/A] motifs. For each complex, we performed 2 µs long molecular dynamics (MD) simulations under AMBER parmbsc1 force-field. Afterwards, we calculated the differential base-specific hydrogen bonding profiles of the systems.

To perform a comparative analysis of our simulation sets, we present an interaction dynamics framework (IDF), concentrating on the differential analysis of base-specific hydrogen bonding patterns, which we expect to hold the specific partner selective signals **(Figure 1)**.

<img width="850" alt="IDF" src="https://github.com/aysebercin/DNM3AB_specificity/assets/46375571/61797317-28a1-4362-9174-93185f77bdc3">

**Figure 1:** An interaction Dynamics Framework (IDF) to identify DNMT3 selectivity. IDF aims to evaluate intermolecular interactions between protein and DNA, in terms of base-specific hydrogen bonds. Global interaction analysis of base-specific hydrogen bonds show the probability distributions of the number of h-bonds formed in each conformation generated during MD. Residue level flanking nucleotide – amino acid interactions show the mean hydrogen bonding capacity between observed amino acid-nucleotide pairs. Atom level flanking nucleotide – amino acid interactions plotted as frequency bar graphs.

## Repository Structure

The repository is organized into the following main folders:

***1.	Analysis_scripts:*** This folder contains two subfolders:
-	***IDF:*** includes analysis scripts and input datas of Interaction Dynamics Framework in the order **(i)** probability distribution analysis, **(ii)** residue level interaction intensity analysis and **(iii)** atom level cumulative h-bond analysis. Jupyter notebooks in each folder can be used directly.
-	***supplementary_analysis:*** includes supplementary analysis scripts and input datas as **(i)** DNA major groove width and base-pair step parameters analysis, **(ii)** cumulative ionic interaction analysis, and **(iii)** cumulative atom-atom interactions of each replica simulations. Jupyter notebooks in each folder can be used directly.

***2.	Gromacs_parameter_files:*** includes .mdp files that defines simulation parameters for each energy minimization step and production run of our MD simulations.

***3. Movies:*** includes movies of MD simulation trajectories of DNMT3A-CGC (cognate) and DNMT3B-CGG (cognate) complexes.
 	
***4.	Starting_structures:*** includes the initial structures of our DNMT3A/B – CGC/G/T/A complexes for MD simulations.

Our MD conformers are deposited at [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.12545441.svg)](https://doi.org/10.5281/zenodo.12545441)

### ***Important Note:***
At the beginning of the study, we started residue numbering from 1 to allow for direct sequence-based comparison between DNMT3A and DNMT3B constructs. For clarity and consistency with external references, we later adjusted the numbering to match UniProt annotations by adding 629 for DNMT3A and 570 for DNMT3B, and we use these UniProt-based residue numbers throughout the manuscript.

## Contact

If you have any questions related to our repository, please contact us:

- Ayşe Berçin Barlas: aysebercin.barlas@ibg.edu.tr
- Ezgi Karaca: ezgi.karaca@ibg.edu.tr


