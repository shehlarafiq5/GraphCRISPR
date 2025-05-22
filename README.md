# GraphCRISPR
# GraphCRISPR: Harnessing Graph Neural Networks for Off-Target Minimization in Genome Editing

> A novel GNN-based framework designed to minimize off-target effects in CRISPR/Cas9 genome editing by modeling DNA sequences and contextual features as graph representations.

## 📄 Overview

**GraphCRISPR** explores the use of Graph Neural Networks (GNNs) to predict and minimize off-target activity in CRISPR/Cas9 genome editing. By converting sgRNA and potential DNA target sites into graph structures, the model learns intricate dependencies that traditional sequence-based models may overlook.

This repository contains code, data processing scripts, and model implementations used in the associated paper:

**📘 Citation:**  
> _GraphCRISPR: Harnessing Graph Neural Networks for Off-Target Minimization in Genome Editing_  
> _Shehla Rafiq, Assif Assad, Tariq Ahmad Masoodi, Muzafar Ahmad Macha, Muzafar Rasool Bhat_  
> [Add journal name / preprint link if available]

---

## 🧬 Key Features

- 🔍 Graph representation of sgRNA and DNA sequences
- 🧠 GCN/GAT-based model for off-target prediction
- ⚖️ Handles sequence-structure relationships with higher accuracy
- 📊 Evaluation using Spearman correlation, AUC, and precision-recall
- 💾 Compatible with benchmark CRISPR datasets

---

## 🗂️ Repository Structure

