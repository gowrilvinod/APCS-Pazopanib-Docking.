# APCS-Pazopanib-Docking.


This repository contains the molecular docking study of **Pazopanib** with a target protein structure, along with structural interaction analysis.

##  Repository Contents

- **1sac.pdb** – Original protein structure.
- **Pazopanib.pdb** – Ligand structure after preparation.
- **Conformer3D_COMPOUND_CID_10113978.sdf** – Ligand conformer from PubChem.
- **docked.sdf** – Docking output file.
- **docked1.png** – Visualization of docked complex.
- **COMPLEX_RENAMED_PROTEIN_PAZ_Z_0.png** – Interaction visualization image.
- **README.md** – This documentation.
- **.gitignore** – Git ignore file for unnecessary local files.

##  Methodology

1. **Protein Preparation**
   - Retrieved protein structure from the Protein Data Bank (PDB ID: 1SAC).
   - Removed water molecules and unwanted chains.
   - Added missing hydrogen atoms and optimized structure.

2. **Ligand Preparation**
   - Retrieved Pazopanib structure from PubChem (CID: 10113978).
   - Converted to `.pdb` format and energy-minimized.

3. **Docking**
   - Docking performed using **AutoDock Vina**.
   - Search grid defined around the active site.
   - Binding affinity calculated and best pose saved.

4. **Interaction Analysis**
   - PLIP used to identify protein-ligand interactions.
   - Hydrogen bonds, hydrophobic interactions, and other non-covalent interactions mapped.
   - Visualized using PyMOL and Discovery Studio Visualizer.

##  Results

### Binding Interactions
- **Ligand**: Pazopanib (PAZ)
- **Interacting Chains**: A, E
- **Key Residues**:
  - 68A VAL
  - 83A LYS
  - 88E PHE (multiple interactions)

### Hydrogen Bonds
| Residue | Distance H-A (Å) | Donor Angle (°) | Protein Donor? |
|---------|------------------|-----------------|----------------|
| 88E PHE | 2.97              | 153.33          | ✅ |
| 88E PHE | 3.33              | 100.02          | ❌ |



##  License
This project is released under the MIT License. See `LICENSE` file for details.
