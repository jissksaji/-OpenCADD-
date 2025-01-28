

# Drug Discovery Pipeline

This repository contains a **drug discovery pipeline** that utilizes **Cheminformatics, Machine Learning, and Deep Learning** techniques for predicting active drug-like molecules targeting **EGFR inhibitors**.

## 🚀 Features

- **Molecular Fingerprints** (MACCS & Morgan)
- **Lipinski’s Rule of 5 Filtering**
- **Random Forest & Neural Network (PyTorch) Classifiers**
- **Stratified K-Fold Cross-Validation**
- **ROC Curve Analysis**
- **Molecular Clustering using Butina Algorithm**
- **Final Compound Selection & Visualization**
- **Docking with AutoDock Vina**
- **Off-target Prediction using SwissTargetPrediction**

---

## 📥 Installation & Setup

### 1️⃣ **Clone the Repository**

```bash
git clone https://github.com/jissksaji/OpenCADD.git
cd OpenCADD
```

### 2️⃣ **Create and Activate Conda Environment**

```bash
conda env create -f environment.yml
conda activate drug_pipeline
```

### 3️⃣ **Run the Pipeline**

```bash
jupyter-notebook cadd_pytorch.ipynb
```

This will **train the models, evaluate performance, and generate final predictions.**

---

## 📑 Overview

This pipeline identifies potential **EGFR inhibitors** by applying **machine learning-based screening** followed by **docking and off-target analysis**. The workflow starts with **compound filtering** based on pIC50 values, separating actives and inactives. MACCS and Morgan fingerprints are used to train **Random Forest and Neural Network models**, with **Random Forest outperforming PyTorch’s neural network**. The final model undergoes **Stratified K-Fold cross-validation**, ensuring robustness.

Filtered compounds are **clustered using Butina**, selecting diverse candidates. The **Lipinski rule of 5** ensures drug-like properties. Finally, **AutoDock Vina** performs docking, selecting the top **three compounds** based on binding affinity. Off-target interactions are predicted via **SwissTargetPrediction**, ensuring selectivity. The original report (without PyTorch implementation) is available in the `final_report` folder.

---

Special thanks to **[VolkamerLab](https://volkamerlab.org/)**&#x20;



