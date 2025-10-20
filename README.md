# Predicting and Visualizing the Structure of the Human Aquaporin-6 Tetramer
## Background information
From UniProt entry Q13520 for the Human Aquaporin-6: 
- Aquaporins form homotetrameric transmembrane channels, with each monomer independently mediating water transport across the plasma membrane along its osmotic gradient.
- Unlike classical aquaporins, AQP6 is an intracellular channel with selective anion permeability, particularly for nitrate, and exhibits very low water permeability.
- It may also facilitate the transport of gases, such as CO2 and NH4+.
## Workflow
### 1. Retrieve the structure of the human aquaporin-6 monomer (AFDB ID Q13520) from AlphaFold DB
The structure colored by the pLDDT value of each residue: \n
![Q13520_structure](https://github.com/rmvjh27/aquaporin6-structure/blob/a7bab4a7979c49d6d8cbb7c9622325d54f85816d/Aquaporin6%20monomer.png)

### 2. Visualize the amino acid residues with high AlphaMissense pathogenicity
E30, N82, P83, Q107, G110, E148, N196, F216, G223 \n
High AlphaMissense pathogenicity values of these residues indicate that any mutation that changes any of them into another amino acid residue is likely to be pathogenic. This means that these residues are likely to be important for the normal function of aquaporin-6.
The residues are colored in hot pink and shown as sticks, while the rest of the protein is colored green. \n
![highlight_res](https://github.com/rmvjh27/aquaporin6-structure/blob/main/Aquaporin6%20monomer-1.png)
![zoomed_res](https://github.com/rmvjh27/aquaporin6-structure/blob/main/Aquaporin6%20monomer-2.png)

