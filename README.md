# 🧠 Slice-Aware Vision Transformer for MRI-Based Alzheimer's Staging

This project implements a **Slice-Aware Vision Transformer (SE-ViT)** to classify Alzheimer's Disease progression using 3D MRI data. We introduce a novel combination of Squeeze-and-Excitation (SE) modules and Vision Transformers to rank the most informative axial slices and perform binary, multi-class, and hierarchical classification.

> 🔗 **GitHub Link :** [https://github.com/yourusername/se-vit-alzheimers](https://github.com/UmairAmir/Alzheimer-Detection-23-)

---

## 📂 Project Files

This repository contains the following Jupyter Notebooks, each corresponding to a key experiment:

| Notebook                                | Description                                                                 |
|----------------------------------------|-----------------------------------------------------------------------------|
| `Baseline.ipynb`                       | Implements a baseline binary ViT using a pre-trained Hugging Face model.   |
| `firstImprovement.ipynb`              | Adds SE module to rank MRI slices and train a custom SE-ViT binary model.  |
| `SecondImprovement_Experiment1.ipynb` | Extends SE-ViT for direct 4-class staging using a single-head softmax.     |
| `SecondImprovement_Experiment2.ipynb` | Implements a hierarchical SE-ViT model with binary + 3-class classification.|
| `VitTransformer.ipynb`                | Contains modular ViT and SE module code used across experiments.           |

---

## 🧪 Overview

- **Dataset:** OASIS-2 (Open Access Series of Imaging Studies)
- **Input:** Preprocessed 3D T1-weighted MRIs (skull stripped, normalized)
- **Objective:** Classify Alzheimer’s progression across 4 stages using MRI scans
- **Best Model:** Hierarchical SE-ViT (74% accuracy, 0.72 F1 score)

---

## 🚀 How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/se-vit-alzheimers.git
   cd se-vit-alzheimers
