# CIRBP-Bowhead-Whale-MD 🐋💻

**In Silico Thermodynamic Validation of Bowhead Whale CIRBP (Cold-Inducible RNA-Binding Protein) for Human Applications at 310K.**

This repository contains the structural data and molecular dynamics validation for the *Balaena mysticetus* (Bowhead Whale) variant of the CIRBP protein, engineered to test its thermodynamic stability at human body temperature (37ºC / 310K).

### Context
A 2025 *Nature* paper (Firsanov et al.) demonstrated that the Bowhead Whale's high resistance to cancer and extreme longevity is partially mediated by CIRBP, which drives Liquid-Liquid Phase Separation (LLPS) for efficient DNA Double-Strand Break (DSB) repair. However, the whale's core temperature is ~33.8ºC. To repurpose this mechanism for human longevity, we must validate if the protein maintains its required structural entropy at 37ºC.

### In Silico Mutagenesis
The human canonical AlphaFold model (Q14011) was modified using UCSF ChimeraX. The 5 specific C-terminal mutations unique to the Bowhead Whale were introduced:
* N126S
* S148G
* G150S
* Y151C
* S152G

### Molecular Dynamics (MD) Simulation
* **Engine:** OpenMM
* **Force Field:** AMBER ff19SB
* **Solvation:** TIP3P water box (1.0 nm clearance)
* **Ions:** 0.15 M NaCl (physiological)
* **Ensemble:** NPT (310K, 1 bar)
* **Production:** 2 ns

### Results
The C-terminal of CIRBP is an Intrinsically Disordered Region (IDR) necessary for LLPS. The RMSD trajectory (~14 Å) confirms that the whale variant maintains a high-entropy disordered state at 310K without unnatural aggregation, preserving the biophysical prerequisites for phase separation in a human thermal environment.

*(Veja o gráfico de RMSD nos arquivos do repositório)*

### Files
* `cirbp_baleia_minimizada.pdb` - The energy-minimized structure of the chimeric protein.
* `rmsd_baleia.png` - The RMSD trajectory plot.

---
**Full Preprint & Discussion:** [COLE AQUI O LINK DO SEU POST DO RESEARCHHUB]
