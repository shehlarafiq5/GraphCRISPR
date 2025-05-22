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

GraphCRISPR/
├── Data/
│   ├── pos_dataset.csv         # Positive off-target samples
│   ├── neg_dataset.csv         # Negative off-target samples
│   └── README.md               # Description of data format
│
├── pretrained/
│   └── dna2vec.bin             # Pretrained DNA2Vec embeddings
│
├── graphcrispr/
│   ├── __init__.py
│   ├── models.py               # GCN/GAT model implementations
│   ├── data_utils.py           # Graph construction and preprocessing
│   ├── train.py                # Training pipeline
│   ├── evaluate.py             # Evaluation metrics and scripts
│   └── config.yaml             # Configuration file for experiments
│
├── requirements.txt
├── README.md                   # Project overview and usage guide
└── run_experiment.py           # Entry point to launch training/evaluation
🚀 Getting Started
1. Clone the repository
```sh
git clone https://github.com/your-username/GraphCRISPR.git
cd GraphCRISPR
```
2. Install dependencies
Create a virtual environment (optional):
```sh
python -m venv crispr-env
source crispr-env/bin/activate  # On Windows: crispr-env\Scripts\activate
```
Then install the requirements:
```sh
pip install -r requirements.txt
```
```sh
python graphcrispr.py 
```
📂 Datasets
The Data/ folder contains:

pos_dataset.csv: Positive off-target sgRNA-target pairs

neg_dataset.csv: Negative (non-target or safe) pairs

Each file includes:

sgRNA sequence

Target sequence

Additional context features (e.g., GC content, chromatin state)
