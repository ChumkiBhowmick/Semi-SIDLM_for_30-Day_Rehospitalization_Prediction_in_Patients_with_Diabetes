 SemiSIDLM for 30Day Readmission Prediction in Diabetic Patients

This repository contains the official implementation of the SemiSupervised Integrated Deep Learning Model (SemiSIDLM) for predicting 30day hospital readmission in diabetic patients, as described in the paper: "CrossPopulation Validation of SemiSIDLM for 30Day Rehospitalization Prediction in Patients with Diabetes".
 📌 Overview
This project implements and validates a hybrid deep learning model across three distinct cohorts:
 UC Irvine 130Hospital Dataset (US, development)
 Indian TertiaryCare Cohort (external validation 1)
 MMI4 ICU Dataset (external validation 2)
 🚀 Getting Started
 Prerequisites
 Python 3.8+
 Install dependencies: `pip install r requirements.txt`
 Data Access
The datasets used in this study are publicly available but have specific access requirements:
1. UC Irvine Dataset: Available at [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Diabetes+130US+hospitals+for+years+19992008)
2. MMI4 ICU Dataset: Available at [PhysioNet](https://physionet.org/content/mimiciv/2.2/)
3. Indian Cohort: The data cannot be shared publicly due to institutional ethics restrictions. Researchers may contact the corresponding author for inquiries.
Place the downloaded data in a `data/` folder following the structure in `data/README.md`.
 🧠 Model Architecture
The SemiSIDLM architecture consists of:
 Input layer with featureweighted enhancement
 Residual blocks with batch normalization
 Dropout regularization (30%)
 Semisupervised pseudolabeling with confidence thresholding
 Hybrid Random Forest probability augmentation
