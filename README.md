# West Nile Virus Multi-Epitope Vaccine Design Workflow

This repository contains the in silico workflow and result files for designing a potential multi-epitope vaccine against West Nile Virus (WNV), based on immunoinformatics and structural bioinformatics methods.

---
**Note**: This project is finished in terms of execution, but not in terms of satisfaction.  
Some predicted results and design choices may not meet my standards, and I intend to revisit them with improved methods and insights.
Educational purposes. Not a finalized.

---
## 0. Select and Prepare Target Protein

- Retrieve protein sequence from **NCBI**
- Assess **antigenicity** using **VaxiJen v2.0**  

## 1. Epitope Prediction

- Predict **MHC Class I**, **MHC Class II**, and **B-cell epitopes** using **IEDB**
- Select **high-affinity**, **immunogenic** epitopes

## 2. Allergenicity and Toxicity Screening

Test selected epitopes using:
- **AllerTOP v2.0** for allergenicity
- **ToxinPred** for toxicity
  
## 3. Epitope Clustering

- Perform cluster analysis with **IEDB's Epitope Cluster Analysis Tool**

## 4. Population Coverage Analysis

- Use **IEDB Population Coverage Tool** to assess epitope relevance based on **geographic regions**
  
## 5. Vaccine Construct Design

- Link selected epitopes with **linkers** (e.g., `GPGPG`, `AAY`)
- Add an **adjuvant** at the N-terminus (`Human β-defensin-3`)
- Reassess **construct antigenicity** with **VaxiJen**

## 6. Structural Modeling and Docking

- Model 3D structure with **AlphaFold**
- Validate/refine using **MolProbity**
- Dock with innate immune receptor (**TLR4**) via **ClusPro**

## 7. Immune Simulation

- Simulate host immune response using **C-ImmSim**
- Evaluate:
  - **Cytokine levels**
  - **Memory formation**
  - **Immune profile dynamics**
 
---

## Tools & Servers Used

- NCBI
- IEDB
- VaxiJen
- ToxinPred
- AllerTOP
- PyMol
- AlphaFold
- MolProbity
- ClusPro
- C-IMMSIM
