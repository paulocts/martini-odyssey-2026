# 🧪 Hands-On Tutorials — MARTINI Odyssey Athens 2026

Welcome to the **hands-on section** of the MARTINI Odyssey school.  
This repository contains guided tutorials corresponding to each day of the event, as well as additional advanced material.

Each hands-on links to dedicated pages with step-by-step instructions.

---

# 🧩 Day 1 — Fundamentals

**Hands-on Session 1:**  
*Basics of Martini (membranes and proteins)*

## Exercises

- **Introduction to Martini & MD Simulations**  
  ↳ [Membrane Self-Assembly](https://cgmartini.nl/docs/tutorials/Martini3/LipidsI/)

- **Martini Protein Model**  
  ↳ [Introduction](https://cgmartini.nl/docs/tutorials/Martini3/ProteinsI/)  
  ↳ [Using Martinize2](https://cgmartini.nl/docs/tutorials/Martini3/ProteinsI/Tut1.html)

- **Peptides and Lipids**  
  ↳ [Transmembrane Peptide Simulations](https://cgmartini.nl/docs/tutorials/Martini3/ProteinsIIa/)

---

# 💊 Day 2 — Pharmaceutical Applications

**Hands-on Session 2:**  
*Parametrization of small-molecules, protein-ligand binding, liposomes and LNPs*

## Exercises

- [Tutorial]

---

# 🧬 Day 3 — Biological Applications

**Hands-on Session 3:**  
*Simulations of membrane proteins and complex biological systems*

## Exercises

- [Tutorial]

---

# 🚀 Advanced Material

Additional tutorials for deeper exploration beyond the core sessions.

## Topics

- **More on Lipid Simulations with Martini**  
  ↳ [Vesicles and Membranes in Complex Shapes (TS2CG2)](https://github.com/weria-pezeshkian/TS2CG-v2.0/wiki/Tutorial)  
  ↳ [Complex Lipid Membranes with INSANE](https://cgmartini.nl/docs/tutorials/Martini3/LipidsII/)  
  ↳ [Complex Lipid Membranes with COBY](https://github.com/MikkelDA/COBY/tree/master/Tutorial)

- **More on Protein Martini Models**  
  ↳ [Evaluating the Quality of Protein Models](https://cgmartini.nl/docs/tutorials/Martini3/ProteinsI/Tut2.html)  
  ↳ [Intrinsically Disordered Regions in Proteins](https://cgmartini.nl/docs/tutorials/Martini3/ProteinsI/Tut3.html)  
  ↳ [Protein Complexes with Martini](https://cgmartini.nl/docs/tutorials/Martini3/ProteinsIIb/)  
  ↳ [Notes and Limitations](https://cgmartini.nl/docs/tutorials/Martini3/ProteinsI/Tut4.html)

- **Enhanced Sampling with Martini**  
  ↳ [Free Energy Techniques](https://cgmartini.nl/docs/tutorials/Martini3/Free_Energy_Techniques/)

  ---

  # 💻 Computing Environment (HPC Access)

All hands-on exercises can be run on the ARIS HPC system during the workshop.

Access credentials will be provided to participants during the event.

## Login

1. Connect to the workshop gateway:  
   `ssh -p 65022 workshop2026_1@88.197.83.25`

2. From there, connect to ARIS:  
   `ssh -i .ssh/aris train01@login.aris.grnet.gr`

## Running jobs

- Navigate to the relevant tutorial folder (e.g. `TEST`)  
- Submit jobs using: `sbatch submit_sample.sh`

## Notes

- Each node has 20 cores, but for some systems, jobs should be configured to less cores (e.g. **16 cores**)  



