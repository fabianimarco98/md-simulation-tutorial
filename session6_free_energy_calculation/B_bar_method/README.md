# Part B: Bennett Acceptance Ratio (BAR) Method

This project covers the calculation of binding free energy for the 1CEA complex using a rigorous alchemical method, the Bennett Acceptance Ratio (BAR). This involved running separate simulations at 11 intermediate states (λ points) to compute the free energy difference.

---

## Workflow Overview

1.  **System Preparation:** A dual topology was prepared for the ligand to allow for its alchemical transformation (annihilation) in the binding pocket.
2.  **Lambda Simulations:** A series of 11 independent simulations were run, each at a different λ value (from 0 to 1), to sample the system at intermediate states between the fully interacting and non-interacting ligand.
3.  **Analysis with BAR:** The GROMACS `gmx bar` tool was used to analyze the simulation data from all λ windows and calculate the final ΔG_binding using the Bennett Acceptance Ratio estimator.

---

## Key Results

The BAR analysis yielded a final calculated binding free energy of **[Inserisci il tuo valore qui, es. -35.1 ± 0.8 kJ/mol]**. The plot below shows the derivative of the Hamiltonian with respect to lambda (dH/dλ) at each lambda point, which is used to compute the free energy.

![dH/dλ vs. Lambda Plot](./3_results/dhd_lambda.png)

The final log files from the `gmx bar` analysis are included in the `3_results` folder.

---

## Conclusion

This project demonstrates proficiency in performing rigorous alchemical free energy calculations, a state-of-the-art technique in computational drug design. It showcases the ability to set up, run, and analyze complex multi-simulation workflows to obtain accurate thermodynamic properties.
