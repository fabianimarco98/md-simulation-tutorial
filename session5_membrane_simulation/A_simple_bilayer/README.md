# Part A: Simple Lipid Bilayer Simulation

This project demonstrates the setup and simulation of a simple, symmetric POPC lipid bilayer patch (membrane only). The primary goal was to learn the standard workflow using CHARMM-GUI for building membranes and to understand the specific protocols and analyses required for lipid bilayer equilibration.

---

## Workflow Overview

1.  **System Building with CHARMM-GUI:** The system, a 100-lipid POPC bilayer, was constructed using the CHARMM-GUI web server. This tool automated the process of building the membrane patch, adding solvent, and ions.

2.  **Multi-step Equilibration:** CHARMM-GUI provides a robust, multi-step equilibration protocol designed to slowly relax the system. This involves a series of short simulations with gradually decreasing position restraints on the lipids and water.

3.  **Production MD:** Following equilibration, a 1 ns production simulation was run to analyze the properties of the equilibrated bilayer.

---

## Conclusion

This project was a successful exercise in building and simulating a pure lipid bilayer. It highlights proficiency with advanced system-building tools like CHARMM-GUI and an understanding of the specific analysis techniques associated with membrane simulations, such as calculating area per lipid and order parameters.
