# Part A: Simple Protein-Membrane System

This project demonstrates the setup and simulation of a transmembrane protein embedded in a simple, symmetric POPC lipid bilayer. The primary goal was to learn the standard workflow using CHARMM-GUI and understand the specific protocols required for membrane equilibration.

---

## Workflow Overview

1.  **System Building with CHARMM-GUI:** The entire system was constructed using the CHARMM-GUI web server. This tool automated the process of orienting the protein in the membrane and building the surrounding POPC bilayer, solvent, and ions.

2.  **Multi-step Equilibration:** CHARMM-GUI provides a robust, multi-step equilibration protocol designed to slowly relax the system. This involves a series of short simulations with gradually decreasing position restraints on the protein, lipids, and water.

3.  **Production MD:** Following equilibration, a 200 ns production simulation was run to observe the interactions between the protein and the lipid environment.

---

## Key Results & Analysis

### System Stability (RMSD)

The RMSD of the protein's backbone atoms was monitored to ensure its structural integrity. The stable RMSD indicates that the protein does not undergo significant conformational changes.

![Protein RMSD in Membrane](./3_results/protein_rmsd_membrane.png)

### Membrane Properties (Area per Lipid)

The area per lipid was calculated to confirm that the membrane itself was properly equilibrated. The convergence of this value to the expected experimental value for a POPC bilayer confirms the quality of the simulation.

![Area per Lipid Plot](./3_results/area_per_lipid.png)

---

## Conclusion

This project was a successful exercise in simulating a membrane protein system. It highlights proficiency with advanced system-building tools like CHARMM-GUI and an understanding of the specific analysis techniques associated with membrane simulations.

