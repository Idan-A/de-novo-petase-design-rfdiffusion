# De Novo PETase Design via Generative AI (RFdiffusion)

[![University](https://img.shields.io/badge/University-Politecnico_di_Milano-003366.svg)](https://www.polimi.it/)
[![Framework](https://img.shields.io/badge/Pipeline-RFdiffusion_%7C_ProteinMPNN_%7C_AlphaFold2-orange.svg)]()
[![Focus](https://img.shields.io/badge/Target-PETase_C09_%2F_PDB_8CMV-green.svg)]()

> **Master's Thesis Project** | *Politecnico di Milano*  
> **Topic:** In silico enzyme engineering for plastic degradation (polyethylene terephthalate - PET) under acidic conditions.

---

## 📌 Executive Summary

Plastic pollution caused by **polyethylene terephthalate (PET)** is a major global environmental challenge. Biocatalytic recycling using PETase enzymes provides a sustainable solution, but industrial deployment is limited by **poor thermal stability and low acid resistance** during degradation.

This project validates the use of generative AI (**RFdiffusion**) for the *de novo* design of PETase variants with enhanced acid resistance and improved polymer interaction. Using the high-performing variant **C09 (PDB: 8CMV)** as a structural scaffold, we engineered new scaffolds aimed at:
1. **Lowering the $pKa$** of the catalytic histidine (evaluated via **PropKa**) to improve activity in acidic environments.
2. **Maximizing binding free energy and contact surface area** with the PET substrate (evaluated via **YASARA molecular docking**).

---

## 🛠 Computational Pipeline & Methodology

The project was executed through an end-to-end *in silico* pipeline:

```text
  [ RFdiffusion ] ──► [ ProteinMPNN ] ──► [ AlphaFold2 ] ──► [ Multi-Parametric Screening ]
(Backbone Generation)   (Sequence Design)    (Structure Validation)  (RMSD, pKa, Docking & Binding)
