# Lightweight-Convolutional-Liquid-Neural-Network-for-Efficient-Classification-of-Bioacoustic-Signal

# Lightweight Convolutional Liquid Neural Network (Hybrid LNN)

## 📌 Overview
This repository contains the code and dataset used in my Master’s thesis:  
**"Lightweight Convolutional Liquid Neural Network for Efficient Classification of Bioacoustic Signal"** (2025, Lou Andrei Rabanzo).

The project introduces a **Hybrid Liquid Neural Network (Hybrid LNN)** that combines 1D convolutional feature extraction with liquid neurons for efficient bioacoustic signal classification.  
It is designed to run on **resource-constrained devices** while maintaining competitive accuracy compared to heavier spectrogram-based models.

---

## 📂 Contents
- `src/` → Implementation of baseline models (CNN, LSTM, RNN, LNN) and Hybrid LNN  
- `data/` → Dataset files (or instructions to download if hosted externally)  
- `notebooks/` → Jupyter notebooks for experiments and visualizations  
- `results/` → Evaluation metrics, confusion matrices, and plots  
- `README.md` → This document  

---

## ⚙️ Requirements
- Python 3.9+
- PyTorch
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- Librosa (for audio preprocessing)

You can install dependencies with:
```bash
pip install -r requirements.txt

▶️ How to Run

Clone the repository:

git clone https://github.com/USERNAME/thesis-project.git
cd thesis-project


Preprocess dataset:

python preprocess.py


Train the Hybrid LNN:

python train.py --model hybrid_lnn


Evaluate:

python evaluate.py --model hybrid_lnn

📊 Datasets

To Bee or Not to Bee dataset → used for binary classification (Bee vs. NoBee).

ASC24 dataset → used for multi-class classification (dog, cow, frog sounds).

If datasets are too large for GitHub, you can download them from [Google Drive/Zenodo link here].

📈 Results

Hybrid LNN (Proposed): 89.57% accuracy (Bee dataset) with only 2,460 parameters.

Outperforms raw-audio baselines (RNN, LNN) and approaches spectrogram-based CNN/LSTM performance with far fewer parameters.

Generalizes well to multi-class classification (ASC24 dataset): 85.38% accuracy across three animal sound categories.

📖 Citation

If you use this repository, please cite:

Lou Andrei Rabanzo. "Lightweight Convolutional Liquid Neural Network for Efficient Classification of Bioacoustic Signal." Master's Thesis, 2025.
Repository: https://github.com/USERNAME/thesis-project
