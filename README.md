# md-simulation-tutorial
# GROMACS Molecular Dynamics Workshop Projects

This repository contains a collection of projects completed during the **1st inSilicoSci GROMACS Workshop** (July-August 2025). Each project, corresponding to a workshop session, is self-contained in its own directory and demonstrates the application of MD simulations to progressively complex biomolecular systems.

The goal of this collection is to showcase my hands-on skills in using GROMACS, VMD, and other essential tools for computational biochemistry.

---

## Table of Contents

Below is a list of the projects included in this repository. Click on any project to view its detailed workflow, analysis, and results.

* ### [Session 2: A Simple Protein MD Simulation](./session2_protein_simulation/)
    * **Description:** A foundational simulation of a globular protein in an aqueous solution. This project covers the entire basic MD pipeline: system building, energy minimization, NVT/NPT equilibration, production run, and standard trajectory analysis (RMSD, Radius of Gyration).

* ### [Session 3: A Protein-Ligand Simulation](./session3_protein_ligand_simulation/)
    * **Description:** Simulation of a protein-ligand complex, focusing on ligand parameterization using the CGenFF server. The analysis includes assessing the stability of the ligand in the binding pocket and exploring the system's dynamics through Principal Component Analysis (PCA) and Free Energy Landscapes.

* ### [Session 4: Dealing with Metallic Ligands](./session4_metalloprotein_simulation/) --> **work in progress**
    * **Description:** An advanced project on handling non-standard residues, specifically a metal-coordinating ligand. This workflow utilizes AmberTools (MCPB.py) for parameter generation and Acpype for converting between AMBER and GROMACS formats.

* ### [Session 5: Bio-Membrane Simulations](./session5_membrane_simulation/)
    * **Description:** This project explores the setup and simulation of membrane proteins. It covers building lipid bilayers and embedding proteins using the CHARMM-GUI web server, a key tool for complex system preparation.

* ### [Session 6: Calculating Free Energy](./session6_free_energy_calculation/)
    * **Description:** Application of alchemical free energy methods. This project demonstrates the calculation of protein-ligand binding energy using the MM-PBSA method, a widely used technique for binding affinity estimation.

---

## Core Competencies and Tools

* **Simulation Engine:** GROMACS
* **System Building & Analysis:** VMD, CHARMM-GUI, AmberTools (MCPB.py), Acpype, gmx\_mmpbsa
* **Force Fields:** CHARMM36, CGenFF
* **Visualization & Plotting:** VMD, PyMOL, Matplotlib (Python)
