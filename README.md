# OneHealth-AMR
Integrated AMR surveillance platform for livestock pathogens under One Health framework

# OneHealth-AMR
### Integrated Genomic Surveillance & Network Modeling 
### for AMR in Livestock Pathogens

**Independent Research Project | March 2026**  
**Author:** H.S. Prithvi  
MSc Bioinformatics · JSS Academy of Higher Education & Research, Mysuru  
GitHub: HSPrithvi23 | Platform: BI23

> This is an independent, novel research project. Core pipeline 
> code is kept private. This repository showcases methodology, results, and findings.

## Overview
A full-stack bioinformatics surveillance platform for AMR monitoring 
in *E. coli* and *S. enterica* under a One Health framework-integrating network science, machine learning, deep learning and phylogenetics in a single deployable Streamlit tool.

Directly relevant to: Epidemiological Surveillance of AMR in 
livestock and poultry pathogens under One Health approach.

## Key Results

| Module | Result |
|--------|--------|
| Dataset | 11,436 genomes · 87 antibiotics |
| Co-resistance Network | 67 nodes · 446 edges |
| ML Prediction (RF + XGBoost) | AUC 0.876 |
| Deep Learning (LSTM) | Temporal resistance patterns |
| Anomaly Detection | 5% outbreak-flagged isolates |
| Phylogenetic Analysis | 4 organisms · 4 host species |

## Pipeline Architecture
```
Raw AMR Data (BV-BRC/NCBI)
        ↓
AMR Matrix Construction
        ↓
Co-resistance Network (NetworkX)
        ↓
ML Prediction (RF + XGBoost + SHAP)
        ↓
Deep Learning (LSTM + Autoencoder)
        ↓
Phylogenetic Analysis (zoonotic host coloring)
        ↓
Streamlit Surveillance Dashboard
```
## Results

### AMR Resistance Heatmap
*E. coli & S. enterica across 87 antibiotics* [Heatmap]

### Co-Resistance Network
*67 antibiotic nodes · 446 co-resistance edges*
*Node size = connectivity · Color = drug class* [amr_Network]

### ML Prediction — ROC & Confusion Matrix
*Random Forest AUC 0.874 · XGBoost AUC 0.876*[ML]

### SHAP Feature Importance
*Antibiotic identity is the strongest predictor* [SHAP]

### Phylogenetic Tree — Zoonotic Perspective
*Colored by host species — poultry/livestock/sheep/goat* [Phylo]

### Resistance Profile by Organism [Organism]

### Antibiotic Resistance Frequency [Frequency]

## Key Findings

**Network Analysis:**
Ampicillin, ciprofloxacin, tetracycline and 
trimethoprim/sulfamethoxazole identified as co-resistance 
hubs — antibiotics most likely to fail simultaneously 
in livestock settings.

**ML Prediction:**
Antibiotic identity is the strongest predictor of resistance 
phenotype (SHAP analysis), followed by organism species — 
biologically consistent with known AMR mechanisms.

**Phylogenetics:**
C. jejuni shows longest evolutionary branches (poultry-specific). 
E. coli and S. enterica cluster closely — indicating higher 
cross-species AMR transfer risk relevant to zoonotic 
transmission surveillance.

**Anomaly Detection:**
Autoencoder flagged 5% of isolates with unusual resistance 
profiles — potential outbreak strains or horizontal gene 
transfer events.

## Data Source
- BV-BRC (Bacterial and Viral Bioinformatics Resource Center)
- NCBI Genome Database.
## Tech Stack
Python · Pandas · NetworkX · Scikit-learn · XGBoost · 
SHAP · TensorFlow/Keras · Biopython · Streamlit · Plotly

## Note on Code Availability
This is an independent research project. The full pipeline code is kept private to protect the novel methodology. 
For collaboration or academic enquiries, contact via 
GitHub or LinkedIn.

---

## Relevance to One Health AMR Research
Built in direct alignment with the epidemiological surveillance 
framework for AMR in sheep, goats and poultry under One Health 
approach — covering network modeling, ML-based risk prediction, 
and zoonotic transmission analysis.
