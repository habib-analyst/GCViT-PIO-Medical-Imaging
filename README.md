# GCViT–PIO Medical Imaging

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://github.com/habib-analyst/GCViT-PIO-Medical-Imaging)
[![GitHub stars](https://img.shields.io/github/stars/habib-analyst/GCViT-PIO-Medical-Imaging.svg)](https://github.com/habib-analyst/GCViT-PIO-Medical-Imaging)

A hybrid Global Context Vision Transformer (GCViT) + Perceiver IO framework for multi-disease medical image classification — brain MRI, chest X-rays, and dermatology images in one pipeline.

## Quickstart

```bash
git clone https://github.com/habib-analyst/GCViT-PIO-Medical-Imaging
cd GCViT-PIO-Medical-Imaging
pip install tensorflow keras numpy matplotlib scikit-learn
```

Open `GCVIT_PIO_Habib_Ur_Rehman.ipynb` and run it top to bottom. The notebook is self-contained: data preprocessing, the GCViT backbone, the Perceiver IO fusion block, training (early stopping + LR scheduling), and evaluation with confusion matrices and visualizations.

Input format: RGB images at 224×224, multi-class or binary labels, in train/val/test splits; normalization and augmentation are handled inside the notebook.

## Results (as reported in the paper)

Test metrics from the published work (accuracy / precision / recall / F1):

| Domain | Accuracy | Precision | Recall | F1 |
|---|---|---|---|---|
| Neuro (stroke/Alzheimer's MRI) | 1.00 | 1.00 | 1.00 | 1.00 |
| Skin (melanoma/tinea) | 0.95 | 0.95 | 0.95 | 0.95 |
| Lung (pneumonia/lung cancer) | 1.00 | 1.00 | 1.00 | 1.00 |

25,000 Kaggle images total (10k neuro MRI, 10k dermoscopic, 5k chest X-ray/CT), 70/15/15 split, standard config (224×224×3 input, batch 32, LR 1e-4, 5–20 epochs).

## How it works

1. **GCViT backbone** — multi-scale hierarchical patch embedding with a hybrid CNN+Transformer stem extracts global-context features.
2. **Perceiver IO fusion** — latent cross-attention fuses the multi-scale features efficiently.
3. **Classification head** — fully connected layers with dropout and softmax for multi-class diagnosis.

## Citation

```bibtex
@article{rehman2025gcvitpio,
  author  = {Habib Ur Rehman et al.},
  title   = {AI-Driven Multi-Disease Classification: {GCViT} \& {Perceiver IO} Synergistic Framework Revolutionizing Multi-Domain Medical Diagnosis Through Advanced Hybrid Neural Architecture},
  journal = {The Journal of Supercomputing},
  publisher = {Springer},
  year    = {2025},
  note    = {Accepted; DOI pending}
}
```

## License

For research and educational use. © 2026 Habib Ur Rehman

---
Built by [Habib Ur Rehman](https://github.com/habib-analyst) · ML/AI Engineer & healthcare-AI researcher ·
[LinkedIn](https://www.linkedin.com/in/hur-dev) · [habib.top](https://habib.top)
