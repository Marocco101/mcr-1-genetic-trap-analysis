# Unintended Consequences of Antibiotic Stewardship: How Antibiotic Substitution Stabilizes MDR Persistence in French Livestock Ecosystems

## Project Overview
This repository includes the pilot analysis for my PhD research (expected to start in Autumn 2027), focusing on the "Ecoantibio Paradox" in France. 

### The Problem: The Ecoantibio Paradox
Despite a reduction in colistin use in the French bovine sector, phenotypic resistance has increased since 2019. This suggests that usage reduction alone is insufficient to eliminate colistin-resistant reservoirs. 

### My Hypothesis: The Genetic Trap
I hypothesize an evolutionary "plasmid-to-chromosome transition" driven by the substitution of colistin with Category D antibiotics (trimethoprim-sulfonamides). 
* **Mechanism**: Co-selection with sulfonamide resistance genes ($sul1/dfrA$) physically captures and maintains the $mcr-1$ transposon. 
* **Stabilization**: Insertion Sequence ($ISApl1$) decay locks the resistance gene into the chromosome, neutralizing fitness costs. 

### 2026 Mini-Project Objectives
1. ## Current Progress: Pilot Analysis of PRJNA1166088

I have identified a key dataset (BioProject: PRJNA1166088) containing 127 isolates from French cattle (Haenni et al., 2017). This dataset serves as a representative sample for **Phase 2 (Stabilization)** of my research hypothesis.

### Technical Workflow for 2026 Pilot Study
To validate the "Genetic Trap" mechanism, I am implementing a two-step bioinformatic pipeline. I will begin with high-confidence screening using established tools before moving into advanced structural characterization.

### Step 1: Initial Screening
First of all, I will utilize the following tools to establish a genetic baseline for the 127 isolates (PRJNA1166088):

* **ResFinder**: To identify acquired AMR genes, specifically $mcr-1$, $sul1/2$, and $dfrA$.
* **MyDbFinder**: To perform targeted screening using a custom database. This will be used to detect the $ISApl1$ sequence and specific "trap" architectures (e.g., $mcr-1$ - $sul$ - $dfr$ clusters) to quantify IS decay.

### Step 2: Advanced Structural Analysis 
Building on the results from Step 1, I will apply new tools to characterize the physical stabilization of these genes:

* **Abricate**: To perform rapid, large-scale screening and cross-validation against multiple databases (CARD, VFDB).
* **IntegronFinder**: To define the architecture of Class 1 integrons and determine if $mcr-1$ is physically "captured" within these elements. 
* **PlasmidFinder**: To identify plasmid incompatibility groups (e.g., IncHI2) and evaluate the transition from plasmid-borne to chromosomal integration. 
