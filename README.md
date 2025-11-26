# GCViT–PIO Medical Imaging Framework

Advanced hybrid deep learning architecture combining Global Context Vision Transformer (GCViT) and Perceiver IO for high-accuracy medical image classification.

## ✅ Publication

This work has been accepted in *The Journal of Supercomputing (Springer)*:

Habib Ur Rehman, "AI-Driven Multi-Disease Classification: GCViT & Perceiver IO Synergistic Framework Revolutionizing Multi-Domain Medical Diagnosis Through Advanced Hybrid Neural Architecture", The Journal of Supercomputing (Springer), 2025.  
(DOI will be added after publication.)

This repository contains the full implementation and experiments corresponding to the accepted paper.

---

## 📋 Project Overview

This project presents a hybrid GCViT–PIO model combining:

1. **GCViT for Global Context Feature Extraction**  
2. **Perceiver IO for Cross-Attention Fusion**  
3. **Classification Head for Multi-Class Medical Diagnosis**

The notebook demonstrates:

- Data preprocessing  
- GCViT backbone  
- Perceiver IO fusion  
- Model training  
- Evaluation and visualization  

Supported domains:

- Brain MRI  
- Chest X-rays  
- Dermatology images  

---

## 🏗️ Architecture

### 1. Global Context Vision Transformer (GCViT)
- Multi-scale hierarchical patch embedding  
- Global feature extraction  
- Hybrid CNN + Transformer stem  
- Long-range dependency modeling  

### 2. Perceiver IO Module
- Latent cross-attention  
- Efficient feature fusion  
- Scales well to high-dimensional data  

### 3. Classification Head
- Fully connected layers  
- Dropout regularization  
- Softmax output  

---

## 📁 Project Structure

```
GCViT-PIO-Medical-Imaging/
├── GCVIT_PIO_Habib_Ur_Rehman.ipynb
└── README.md
---

## 🚀 Quick Start

### Installation

```bash
pip install tensorflow keras numpy matplotlib scikit-learn
```
### Running

Open and run: GCVIT_PIO_Habib_Ur_Rehman.ipynb

## 📊 Model Performance

The GCViT–PIO architecture demonstrates:

- Superior accuracy over CNN and baseline ViT  
- Higher robustness on small medical datasets  
- Better global feature understanding  
- Lower false-positive rates  
- Strong generalization across imaging domains  

### Built-in Training Optimizations:

- Early Stopping  
- Learning Rate Scheduling  
- Dropout Regularization  
- Cross-Attention Fusion  
- Augmentation Pipeline  

---

## 🔧 Configuration

Standard configuration for GCViT–PIO:

- **Input Size:** 224×224×3  
- **Patch Size:** Multi-scale GCViT embedding  
- **Backbone:** GCViT Hierarchical Transformer  
- **Fusion:** Perceiver IO latent cross-attention  
- **Batch Size:** 32  
- **Learning Rate:** 1e-4  
- **Epochs:** 5–20  

---

## 📈 Training Pipeline

- Data Loading  
- Preprocessing (normalize, resize, augment)  
- Patch & feature extraction using GCViT  
- Cross-attention fusion using Perceiver IO  
- Train classification head  
- Evaluate (accuracy, loss)  
- Plot confusion matrix  
- Visualize curves  

---

## 💾 Model Outputs

- Accuracy & loss curves  
- Confusion matrix  
- Predictions  
- Classification scores  
- Visual interpretations  

---

## 🌟 Highlights

- First hybrid GCViT + Perceiver IO for medical imaging  
- Strong global context & long-range learning  
- Publication-grade results  
- Fully reproducible notebook  
- Works across multiple medical imaging tasks  

---

## 🎯 Key Features

- Clean, portable code  
- Modular architecture  
- Notebook-based implementation  
- Stable performance  
- Reproducible experiments  
- Research-grade pipeline  

---

## 📝 Dataset Format

- **Images:** RGB, 224×224  
- **Labels:** Multi-class / binary  
- **Splits:** Train, Val, Test  
- **Preprocessing:** Normalization + Augmentation  

Data preparation is fully included in the notebook.

---

## 🔍 Utility Modules (Inside Notebook)

- Data preprocessing cells  
- GCViT block  
- Perceiver IO block  
- Training loop  
- Evaluation pipeline  
- Visualization utilities  

---

## 📄 License

This project is for research and educational use.  
All rights reserved by the author.

---

## ✨ Author Information

Created as a research project:  
**Hybrid Global Context Vision Transformer + Perceiver IO for Medical Imaging**

**Author:** Habib Ur Rehman  
**Email:** habib.research.ai@gmail.com  
**GitHub:** https://github.com/habib-analyst
---

**Done.**
