# West Nile Virus Multi-Epitope Vaccine Design Workflow

This repository contains the in silico workflow and result files for designing a potential multi-epitope vaccine against West Nile Virus (WNV), based on immunoinformatics and structural bioinformatics methods.

---

## Workflow Overview

### 1. **Protein Retrieval**
- envelope [E] protein, partial [West Nile virus].fasta: Main target sequence retrieved from NCBI.

### 2. **Epitope Prediction**
- **MHC-I Binding**:
  Predicted CD8+ T-cell epitopes.
- **MHC-II Binding**:
  Predicted CD4+ T-cell epitopes.
- **B-cell Epitopes**:
  Linear B-cell epitopes.

### 3. **Filtering and Validation**
- **Allergenicity**: 'Allergenicity Prediction/' – Tools used: AllergenFP, AllerTOP.
- **Toxicity**: 'Toxicity Prediction/' – Tool: ToxinPred.
- **Antigenicity**: 'Antigenicity score' - Tool: VaxiJen.

### 4. **Epitope Clustering**
- 'Epitope Clustering Results/': Clustering overlapping epitopes to select conserved regions.

### 5. **Population Coverage**
- 'Population Coverage Calculation Result/': Estimation using IEDB population coverage tool.

### 6. **Vaccine Construct Design**
- 'vaccine/': Multi-epitope construct, with linkers and adjuvant added.
- 'fold_west_nile_virus_vaccine/': PDB of final construct.

### 7. **Structural Modeling**
- 'ClusPro/', 'C-IMMMSIM/', 'Advanced Structural Analysis/': Protein structure prediction, molecular docking, and immune simulation results.

---

## Tools & Servers Used

- NCBI
- IEDB (MHC-I, MHC-II, B-cell, population coverage)
- VaxiJen
- ToxinPred
- AllerTOP
- AlphaFold
- ClusPro
- C-IMMSIM
