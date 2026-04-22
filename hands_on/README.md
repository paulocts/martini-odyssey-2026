# 🧪 Hands-On Tutorials — MARTINI Odyssey Athens 2026

Welcome to the **hands-on section** of the MARTINI Odyssey school.  
This repository contains guided tutorials corresponding to each day of the event, as well as additional advanced material.

Each hands-on links to dedicated pages with step-by-step instructions. 

*Exercises require a pre-configured software environment (Python tools and external packages). Details are provided at the end of this page.*

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
- **Parametrization of a new Martini 3 small molecule model**  
  ↳ [Introduction to Parametrization — manual approach](https://cgmartini.nl/docs/tutorials/Martini3/Small_Molecule_Parametrization/)  
  ↳ [Small-molecule models with Auto-MartiniM3](https://github.com/M2BMI-Lab/Workshop-MartiniOdyssey/blob/main/Tutorial-Parametrization-AutoMartiniM3-MartiniOdyssey.md)  

- **Protein–ligand binding simulations**  
  ↳ [Binding of caffeine to Adenosine 2 receptor](https://github.com/M2BMI-Lab/Workshop-MartiniOdyssey/blob/main/Tutorial-Simulation-with-GPCR-AutoMartiniM3-MartiniOdyssey.md)  

- **CG Modeling of delivery systems**  
  ↳ [How to build a Lipid Nanoparticle CG models](https://zenodo.org/records/19632806)

---

# 🦠 Day 3 — Biological Applications

**Hands-on Session 3:**  
*Simulations of complex biological systems*

## Exercises

- **Visualisation of Martini models in VMD**
  ↳ [Using MartiniGlass](https://cgmartini.nl/docs/tutorials/Martini3/LipidsII/](https://martiniglass.readthedocs.io/en/latest/index.html)  

- **Modeling Complex lipid membranes**  
  ↳ [Using INSANE](https://cgmartini.nl/docs/tutorials/Martini3/LipidsII/)  
  ↳ [Using COBY](https://github.com/MikkelDA/COBY/tree/master/Tutorial)

- **Modeling Crowded  biological systems and Cellular models**  
  ↳ [Using Bentopy](https://cgmartini.nl/docs/tutorials/Martini3/Bentopy/)

---

# 🚀 Advanced Material

Additional tutorials for deeper exploration beyond the core sessions.

## Topics

- **More on Lipid Simulations and Protein-lipid interactios with Martini**  
  ↳ [Vesicles and Membranes in Complex Shapes (TS2CG2)](https://github.com/weria-pezeshkian/TS2CG-v2.0/wiki/Tutorial)  
  ↳ [Analysis of Protein-Lipid interactions - Introduction to Prolint2](https://cgmartini.nl/docs/tutorials/Martini3/ProLint/)  
  ↳ [Analysis of Protein-Lipid interactions - Jupyter notebooks](https://pylipid.readthedocs.io/en/master/tutorial.html)  
  ↳ [Analysis of Protein-Lipid interactions - Additional Tutorials](https://prolint2.readthedocs.io/en/latest/source/tutorials.html)  

- **More on Protein Martini Models**  
  ↳ [Evaluating the Quality of Protein Models](https://cgmartini.nl/docs/tutorials/Martini3/ProteinsI/Tut2.html)  
  ↳ [Intrinsically Disordered Regions in Proteins](https://cgmartini.nl/docs/tutorials/Martini3/ProteinsI/Tut3.html)  
  ↳ [Protein Complexes with Martini](https://cgmartini.nl/docs/tutorials/Martini3/ProteinsIIb/)  
  ↳ [Notes and Limitations](https://cgmartini.nl/docs/tutorials/Martini3/ProteinsI/Tut4.html)

- **Enhanced Sampling with Martini**  
  ↳ [Free Energy Techniques](https://cgmartini.nl/docs/tutorials/Martini3/Free_Energy_Techniques/)

  ---

# 💻 Computing Environment & Setup

The hands-on sessions will use a **remote Linux environment**, accessible from both the computer lab and your personal laptop.

---

## 🧭 Workflow Overview

```
Your Laptop / Lab PC (Windows + MobaXterm)
                │
                ▼
        Workshop Gateway
                │
                ▼
        Linux Workstations (GPU)
                │
        ┌───────┴────────┐
        ▼                ▼
  Run locally        ARIS HPC (GRNET)
 (interactive)       (large jobs)
```

---

## Login

1. Connect to the workshop gateway (use the IP provided to you):  
   `ssh -p 65022 workshop2026_1@XXXXXX`

2. From there, connect to ARIS HPC:  
   `ssh -i ~/.ssh/aris train01@login.aris.grnet.gr`

## Running jobs

- Navigate to the relevant tutorial folder  
- Preparation can be done on the local machines  
- Submit jobs to ARIS HPC using: `sbatch submit.sh` *(ask for help if you need guidance on the `submit.sh` format)*  

## 🧪 Software Environment

- GROMACS  
- Martini 3 tools  
- Python libraries for analysis  

A shared Python virtual environment (venv) will be provided on each workstation.  
This environment will be pre-configured and shared among participants on the same system.

For participants using their own laptops (Linux), a setup package is available:

- Download the setup package (you may need to adapt it): [installation.zip](./installation.zip)  
- Unzip and run: `./setup.sh`

Running the setup script will install the required dependencies locally if needed.

## Notes

- Each compute node has 20 cores (use fewer if needed, e.g. 16)  
- In principle, no installation is required on lab machines (except for specific tools indicated in certain exercises)  
- Only an SSH client is required for personal laptops  

---

Happy computing! 🚀



