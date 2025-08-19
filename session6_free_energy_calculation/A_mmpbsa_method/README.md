# Part A: MM-PBSA Method

This project demonstrates the calculation of binding free energy for the 1CEA protein-ligand complex using the MM-PBSA method as implemented in the `gmx_MMPBSA` tool. The analysis was performed on the last 1 ns of the production trajectory from Session 3.

---

## Workflow Overview

1.  **Trajectory Preparation:** The last 1 ns of the protein-ligand trajectory was extracted and prepared for analysis, ensuring no periodic boundary condition artifacts.
2.  **Input File Creation:** An input file was created to define the parameters for the MM-PBSA calculation, specifying the protein and ligand groups and the computational model (e.g., Poisson-Boltzmann).
3.  **Calculation:** The `gmx_MMPBSA` script was executed to calculate the different energy components (molecular mechanics, polar and apolar solvation energies) and compute the final ΔG_binding.

---

## Key Results

The analysis yielded a final estimated binding free energy of [27.70 kcal/mol]**. The key energy components are summarized below:

![free gibbs energy of the complex](../results/free-energy-complex.png)

The final results files (`.dat` and `.csv`) containing the detailed energy breakdown are included in the `3_results` folder.

---

## Conclusion

This project provided hands-on experience with the MM-PBSA method, a computationally efficient technique for estimating binding affinities. It highlights the ability to use specialized post-processing tools to extract thermodynamic data from MD trajectories.
