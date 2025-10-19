# Lightweight Convolutional Liquid Neural Network for Efficient Classification of Bioacoustic Signals

![Python](https://img.shields.io/badge/python-3.9+-blue.svg)
![PyTorch](https://img.shields.io/badge/framework-PyTorch-red)
![License](https://img.shields.io/badge/license-MIT-green.svg)

---

## 📌 Overview
This repository contains the implementation of the **Hybrid Liquid Neural Network (Hybrid LNN)** used in my Master's thesis:  
**"Lightweight Convolutional Liquid Neural Network for Efficient Classification of Bioacoustic Signal"** (2025, Lou Andrei Rabanzo).

The Hybrid LNN combines **1D convolutional feature extraction** with **liquid neurons** to efficiently classify **bee vs. no-bee audio recordings** directly from raw waveforms.  
It achieves competitive performance with **very low parameter count (~3000)**, making it suitable for deployment on **resource-constrained devices**.

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

### Install everything with:

```bash
pip install -r requirements.txt
```
---

## ▶️ How to Run

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/USERNAME/thesis-hybrid-lnn.git
    cd thesis-hybrid-lnn
    ```

2.  **Update the dataset path in `hybrid_lnn_binary.py`:**

    ```python
    DATASET_PATH = "path/to/your/wav/files"
    ```

    The code expects `.wav` audio files named with keywords like **QueenBee** or **No_QueenBee** for automatic labeling.

3.  **Run the script:**

    ```bash
    python hybrid_lnn_binary.py
    ```

This will train and evaluate the Hybrid LNN using **5-fold cross-validation** and output metrics.

---


## 📊 Dataset

The model was evaluated on the ["To Bee or Not to Bee" dataset](https://www.kaggle.com/datasets/chrisfilo/to-bee-or-no-to-bee) and https://www.kaggle.com/datasets/haithammoh/sounds-of-animals

> Note: Dataset files are not included in this repository due to size. Please download and place them in your chosen `DATASET_PATH`.

---

## 📈 Results

* **Cross-validation accuracy:** ~85.19%
* **Cross-validation F1-score:** ~83.98%
* **Test accuracy:** ~89.57%
* **Test F1-score:** ~89.58%

The Hybrid LNN approaches CNN/LSTM performance while being >10x smaller in parameters.

---

## 📖 Citation

If you use this repository, please cite:

Lou Andrei Rabanzo. "Lightweight Convolutional Liquid Neural Network for Efficient Classification of Bioacoustic Signal." Master's Thesis, 2025.

Repository: https://github.com/louandrei/Lightweight-Convolutional-Liquid-Neural-Network-for-Efficient-Classification-of-Bioacoustic-Signal
