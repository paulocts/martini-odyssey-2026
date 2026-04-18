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
  ↳ [Analysis of Protein-Lipid interactions - Jupyter notebooks](https://pylipid.readthedocs.io/en/master/tutorial.html)  
  ↳ [Analysis of Protein-Lipid interactions - Tutorials](https://prolint2.readthedocs.io/en/latest/source/tutorials.html)  

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

## 🖥️ Accessing the System

### Step 1 — SSH Client

- Lab PCs: MobaXterm already available ✅  
- Personal laptops:
  - Windows → install MobaXterm  
  - Mac/Linux → use terminal  

---

### Step 2 — Connect to Workshop Gateway

```bash
ssh -p 65022 workshop2026_1@88.197.83.25
```

---

### Step 3 — Connect to ARIS HPC

From the gateway:

```bash
ssh -i ~/.ssh/aris train01@login.aris.grnet.gr
```

---

## ⚙️ Running Jobs

### Navigate to your working directory

```bash
cd TEST
```

### Submit a job

```bash
sbatch submit.sh
```

---

## 🧮 Where to Run Your Work

### Local Workstations

- Linux systems with GPUs  
- Best for:
  - Setup  
  - Testing  
  - Short runs  

---

### ARIS HPC

- For larger simulations  
- Uses SLURM scheduler (`sbatch`)

---

## 📂 File Transfer

### Using MobaXterm

- Drag & drop files (SFTP interface)

### Using command line

```bash
scp file train01@login.aris.grnet.gr:/path/
```

---

## 🧪 Software Environment

- GROMACS  
- Martini 3 tools  
- Python libraries for analysis  

A setup script may be provided if needed.

---

## 💡 Notes

- Each compute node has **20 cores**
- For stability, use fewer cores when needed (e.g. **16 cores** in systems that are not so big)

- You can run simulations:
  - On local workstations (interactive)
  - On ARIS HPC (recommended for larger jobs)

- No software installation is required on your laptop (except SSH client)

---

Happy computing! 🚀



