# West Nile Virus Multi-Epitope Vaccine Design Workflow

This repository contains the in silico workflow and result files for designing a potential multi-epitope vaccine against West Nile Virus (WNV), based on immunoinformatics and structural bioinformatics methods.

---

## Workflow Overview

### 0. **Protein Retrieval**
- envelope [E] protein, partial [West Nile virus].fasta: Main target sequence retrieved from NCBI.
- Antigenicity: 'VaxiJen': Antigenicity score

### 1. **Epitope Prediction**
- **MHC-I Binding**:
  Predicted CD8+ T-cell epitopes.
- **MHC-II Binding**:
  Predicted CD4+ T-cell epitopes.
- **B-cell Epitopes**:
  Linear B-cell epitopes.

### 2. **Filtering and Validation**
- **Allergenicity**: 'Allergenicity Prediction/' – Tools used: AllergenFP, AllerTOP.
- **Toxicity**: 'Toxicity Prediction/' – Tool: ToxinPred.
- 
### 3. **Epitope Clustering**
- 'Epitope Clustering Results/': Clustering overlapping epitopes to select conserved regions.

### 4. **Population Coverage**
- 'Population Coverage Calculation Result/': Estimation using IEDB population coverage tool.

### 5. **Vaccine Construct Design**
- 'vaccine/': Multi-epitope construct, with linkers and adjuvant added.

### 6. **Structural Modeling**
- 'fold_west_nile_virus_vaccine/': Protein structural prediction.
- 'ClusPro/': Molecular docking.

### 7. **Immune simulation**
- 'C-IMMMSIM/': Immune simulation results.

---

## Tools & Servers Used

- NCBI
- IEDB
- VaxiJen
- ToxinPred
- AllerTOP
- AlphaFold
- ClusPro
- C-IMMSIM
