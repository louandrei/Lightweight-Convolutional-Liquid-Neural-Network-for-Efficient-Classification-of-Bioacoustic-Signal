# 🐝 Hybrid Liquid Neural Network for Bee/NoBee Classification

![Python](https://img.shields.io/badge/python-3.9+-blue.svg)
![PyTorch](https://img.shields.io/badge/framework-PyTorch-red)
![License](https://img.shields.io/badge/license-MIT-green.svg)

---

## 📌 Overview
This repository contains the implementation of the **Hybrid Liquid Neural Network (Hybrid LNN)** used in my Master's thesis:  
**"Lightweight Convolutional Liquid Neural Network for Efficient Classification of Bioacoustic Signal"** (2025, Lou Andrei Rabanzo).

The Hybrid LNN combines **1D convolutional feature extraction** with **liquid neurons** to efficiently classify **bee vs. no-bee audio recordings** directly from raw waveforms.  
It achieves competitive performance with **very low parameter count (2,460)**, making it suitable for deployment on **resource-constrained devices**.

---

## 📂 Contents
- `hybrid_lnn_binary.py` → Implementation of Hybrid LNN for bee/no-bee classification  
- `requirements.txt` → Dependencies  
- `README.md` → This document  
- `LICENSE` → License file  

---

## ⚙️ Requirements
- Python 3.9+
- PyTorch
- torchaudio
- scikit-learn
- matplotlib
- numpy
- torchsummary (optional, for model summary)

## Install everything with:
```bash
pip install -r requirements.txt

---

