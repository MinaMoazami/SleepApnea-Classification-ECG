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

## 📁 Repository Contents

- `notebooks/`: Jupyter Notebooks for data preprocessing, feature extraction, and model training
- `thesis/`: Final PDF of the thesis
- `data/`: Instructions for dataset access (MIT-BIH, NCHSDB, CFS)
- `models/`: Optionally include saved models or logs here

## 🧪 Datasets

The following public datasets are used:
- [MIT-BIH Polysomnographic Database](https://physionet.org/content/slpdb/1.0.0/)
- [Nationwide Children’s Hospital Sleep DataBank (NCHSDB)](https://physionet.org/content/nch-sleep/3.1.0/)
- [Cleveland Family Study (CFS)](https://sleepdata.org/datasets/cfs)

> Due to licensing, raw data is not included. Please refer to the links above.

## 📦 Requirements

Install required libraries via:

```bash
pip install -r requirements.txt

