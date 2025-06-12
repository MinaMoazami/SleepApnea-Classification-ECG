# Sleep Apnea Classification using Deep Learning on ECG Signals

This repository contains the implementation and results of my Master's thesis:
**"Sleep Apnea Classification using Deep Learning Algorithm"**  
submitted to the Faculty of Electrical Engineering, K. N. Toosi University of Technology, Winter 2023.

## 📘 Thesis Overview

Sleep apnea is a prevalent disorder with serious health implications. This work proposes a deep learning approach to classify:
- Obstructive Sleep Apnea (OSA)
- Central Sleep Apnea (CSA)
- Mixed Sleep Apnea (MSA)
- Normal Breathing

The model is trained solely on ECG signals using HRV and EDR features with an LSTM-based neural network.

📄 Full thesis available in [`thesis/MinaMoazami_Thesis.pdf`](thesis/MinaMoazami_Thesis.pdf)

---

## 🧪 Datasets

The following public datasets are used:
- [MIT-BIH Polysomnographic Database](https://physionet.org/content/slpdb/1.0.0/)
- [Nationwide Children’s Hospital Sleep DataBank (NCHSDB)](https://physionet.org/content/nch-sleep/3.1.0/)
- [Cleveland Family Study (CFS)](https://sleepdata.org/datasets/cfs)

> Due to licensing, raw data is not included. Please refer to the links above.

---

## 🔬 Method

This study uses publicly available polysomnography datasets to extract single-lead ECG signals. The methodology includes:

- **Signal Processing:** Extracting HRV (Heart Rate Variability) and EDR (ECG-Derived Respiration) features from filtered ECG signals using NeuroKit2.
- **Segmentation:** Dividing signals into 60-second non-overlapping epochs with corresponding apnea labels.
- **Feature Engineering:** Time-domain, frequency-domain, and non-linear HRV features were combined with EDR patterns.
- **Modeling:** A stacked LSTM (Long Short-Term Memory) model was designed to learn temporal dynamics and classify each epoch into:
  - Normal Breathing
  - Obstructive Sleep Apnea (OSA)
  - Central Sleep Apnea (CSA)
  - Mixed Sleep Apnea (MSA)

---

## 📊 Results

The proposed model achieved high performance on multi-class classification tasks using ECG data alone:

| Metric     | Value    |
|------------|----------|
| Precision  | 0.721    |
| Recall     | 0.709    |
| F1 Score   | 0.699    |
| AUC (avg.) | 0.894    |

Class-wise performance showed that the model performs best for distinguishing **Normal** and **OSA** events, with slightly lower precision on **MSA** due to class imbalance.

---

## 📁 Repository Contents

- `notebooks/`: Jupyter Notebooks for data preprocessing, feature extraction, and model training
- `thesis/`: Final PDF of the thesis
- `models/`: Optionally include saved models or logs here

---

## 📦 Requirements

Install required libraries via:

```bash
pip install -r requirements.txt

