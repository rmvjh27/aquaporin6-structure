# Predicting and Visualizing the Structure of the Human Aquaporin-6 Tetramer
## Background information
From UniProt entry Q13520 for the Human Aquaporin-6: 
- Aquaporins form homotetrameric transmembrane channels, with each monomer independently mediating water transport across the plasma membrane along its osmotic gradient.
- Unlike classical aquaporins, AQP6 is an intracellular channel with selective anion permeability, particularly for nitrate, and exhibits very low water permeability.
- It may also facilitate the transport of gases, such as CO2 and NH4+.
### Data and tools used:
- Human aquaporin-6 sequence (UniProt ID Q13520)
- AlphaFold-predicted structure of the human aquaporin-6 monomer (AFDB ID Q13520)
- PyMOL 3.1
- ColabFold
## Workflow
### 1. Retrieve the structure of the human aquaporin-6 monomer from AlphaFold DB
The structure colored by the pLDDT value of each residue:

![Q13520_structure](https://github.com/rmvjh27/aquaporin6-structure/blob/a7bab4a7979c49d6d8cbb7c9622325d54f85816d/Aquaporin6%20monomer.png)

The structure colored with a blue-to-red spectrum, with blue denoting the N-terminus and red denoting the C-terminus:

![NtoCcolored](https://github.com/rmvjh27/aquaporin6-structure/blob/main/Aquaporin6%20monomer-3.png)

### 2. Visualize the amino acid residues with high AlphaMissense pathogenicity
The residues are as follows: E30, N82, P83, Q107, G110, E148, N196, F216, G223

High AlphaMissense pathogenicity values of these residues indicate that any mutation that changes any of them into another amino acid residue is likely to be pathogenic. This means that these residues are likely to be important for the normal function of aquaporin-6.
The residues are colored in hot pink and shown as sticks, while the rest of the protein is colored green.

![highlight_res](https://github.com/rmvjh27/aquaporin6-structure/blob/main/Aquaporin6%20monomer-1.png)
![zoomed_res](https://github.com/rmvjh27/aquaporin6-structure/blob/main/Aquaporin6%20monomer-2.png)

### 3. Predict the structure of the aquaporin-6 tetramer
The aquaporin-6 sequence obtained from UniProt was entered into [ColabFold](https://colab.research.google.com/github/sokrypton/ColabFold/blob/main/AlphaFold2.ipynb) four times, each instance of the sequence separated with a colon sign (:) to produce a tetramer.
Sequence coverage and pLDDT (predicted local distance difference test) of the generated tetramer:
