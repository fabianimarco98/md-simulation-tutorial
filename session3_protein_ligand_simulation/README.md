# Session 3: Protein-Ligand MD Simulation

This project details the simulation of a protein-ligand complex. The primary goal was to learn how to handle non-standard residues (a small molecule ligand) by generating a custom topology and then analyzing the stability and dynamics of the complex.

---

## Workflow Overview

1.  **Ligand Parameterization:** The ligand topology was generated using the CGenFF server. The resulting CHARMM force field parameters (`.itp` and `.prm` files) were validated to ensure their quality.

2.  **System Preparation:** The protein topology was generated separately. The protein and ligand topologies were then combined in the main system topology file. The complex was solvated and neutralized with ions.

3.  **Minimization & Equilibration:** The standard energy minimization and NVT/NPT equilibration protocols were applied, with position restraints on both the protein and the ligand.

4.  **Production MD:** A 10 ns production simulation was run to observe the behavior of the ligand within the protein's binding pocket.

---

## Key Results & Analysis

### RMSD of Protein and Ligand

The RMSD of the protein backbone confirms the overall structural stability. The RMSD of the ligand (fitted on the protein backbone) was calculated to assess its stability within the binding site. The low and stable ligand RMSD suggests it remains bound in a consistent pose.

![Protein RMSD Plot](./3_results/protein_rmsd.png)
![Ligand RMSD Plot](./3_results/ligand_rmsd.png)

### Principal Component Analysis (PCA) & Free Energy Landscape

PCA was performed on the protein backbone atoms to identify the dominant collective motions during the simulation. The projection of the trajectory onto the first two principal components (PC1 and PC2) allows for the visualization of the system's free energy landscape. The landscape reveals a single, well-defined energy minimum, indicating that the complex is stable and does not undergo large conformational changes.

![Free Energy Landscape Plot](./3_results/pca_fel.png)

---

## Conclusion

This project successfully demonstrated the complete workflow for simulating a protein-ligand complex. Key skills acquired include ligand parameterization, combining topologies, and advanced analysis techniques like PCA, which are essential for studying molecular recognition and drug design.
