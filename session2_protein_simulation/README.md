# Session 2: A Simple Protein MD Simulation

This project covers the foundational workflow for a standard molecular dynamics simulation of **T4 Lysozyme (PDB ID: 177L)** in an aqueous solution. This specific crystal structure is one of 25 forms studied to understand protein flexibility and adaptability, making it an interesting case for a baseline dynamics study.

The primary goal was to practice the entire MD pipeline, from system preparation and equilibration to running a production simulation and analyzing the resulting trajectory.

---

## Workflow Overview

1.  **System Preparation:** The initial PDB structure (177L) was cleaned, and a topology was generated using the CHARMM27 force field. The protein was then solvated in a cubic box with TIP3P water and neutralized with ions.
2.  **Energy Minimization:** A steepest descent algorithm was used to relax the system and remove any steric clashes.
3.  **Equilibration:** The system was equilibrated in two phases:
    * **NVT (100 ps):** To stabilize the temperature of the system.
    * **NPT (100 ps):** To stabilize the pressure and ensure the correct density.
4.  **Production MD:** A 1 ns production simulation was run to generate the trajectory for analysis.

---

## Key Results & Analysis

### Root Mean Square Deviation (RMSD)

The RMSD of the protein backbone was calculated to assess structural stability. The plot below shows that the system reached equilibrium and remained stable throughout the simulation, fluctuating around 0.2 nm.

![RMSD Plot](./3_results/rmsd.png)

### Radius of Gyration (Rg)

The Radius of Gyration was calculated to assess the protein's compactness. The stable Rg value indicates that the protein maintained its folded state and did not undergo significant unfolding.

![Radius of Gyration Plot](./3_results/gyrate.png)

---

## Conclusion

This simulation successfully demonstrated the standard workflow for simulating a soluble protein. The analyses confirm that the protocol used resulted in a stable and well-behaved trajectory, providing a solid foundation for more complex simulations.

