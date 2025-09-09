# 🐝 Lightweight Convolutional Liquid Neural Network (Hybrid LNN)

![Python](https://img.shields.io/badge/python-3.9+-blue.svg)
![PyTorch](https://img.shields.io/badge/framework-PyTorch-red)
![License](https://img.shields.io/badge/license-MIT-green.svg)

---

## 📌 Overview
This repository contains the source code and dataset used in my Master’s thesis:  
**"Lightweight Convolutional Liquid Neural Network for Efficient Classification of Bioacoustic Signal"** (2025, Lou Andrei Rabanzo).

The project introduces a **Hybrid Liquid Neural Network (Hybrid LNN)** that combines **1D convolutional feature extraction** with **liquid neurons** for efficient bioacoustic signal classification.  
It is designed to run on **resource-constrained devices** while maintaining competitive accuracy compared to heavier spectrogram-based models.

---

## 📂 Contents
- `src/` → Baseline models (CNN, LSTM, RNN, LNN) + Hybrid LNN implementation  
- `data/` → Dataset files or download instructions  
- `notebooks/` → Jupyter notebooks for training/evaluation  
- `results/` → Metrics, plots, and confusion matrices  
- `README.md` → This document  

---

## ⚙️ Requirements
- Python 3.9+
- PyTorch
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Librosa (for audio preprocessing)

Install dependencies:
```bash
pip install -r requirements.txt
