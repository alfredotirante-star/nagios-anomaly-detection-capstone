# Nagios Network Anomaly Detection (Capstone Project)
AI-based network anomaly detection using supervised and unsupervised machine learning

## Overview
This project applies machine learning techniques to automatically detect anomalous network traffic using Nagios-style monitoring data. Both supervised and unsupervised models are evaluated to support proactive and scalable network monitoring.

## Models Implemented
- Logistic Regression (supervised baseline)
- Isolation Forest (unsupervised anomaly detection)
- Random Forest (final supervised model)

## Dataset
The dataset is a synthetic Nagios-style network monitoring dataset containing metrics such as traffic volume, latency, packet loss, service state, and host identifiers. Anomalies represent approximately 7.5% of total records.

## Methodology
- Data preprocessing and feature engineering
- Exploratory data analysis (EDA)
- Train/test split for generalization
- Model evaluation using accuracy, precision, recall, F1-score, and confusion matrices

## How to Run the Notebook

When executed, the notebook will prompt the user to select a CSV file containing the network monitoring data.

The data loader supports:
1. Google Colab file upload (if running in Colab)
2. A graphical file picker (if supported by the environment)
3. A command-line path prompt as a fallback

Once a valid CSV file is selected, the notebook proceeds automatically with preprocessing, modeling, and evaluation.


## Key Findings
- Supervised models achieved perfect performance due to the synthetic and highly separable nature of the dataset
- Isolation Forest demonstrated higher false positives, consistent with unsupervised detection behavior
- Random Forest was selected as the final model due to stability and recall

## Project Structure

- `notebooks/` – Jupyter notebook containing the full analysis pipeline
- `data/` – Synthetic Nagios-style network monitoring dataset
- `src/` – Supporting scripts (minimal, for structure compliance)
- `models/` – Documentation of evaluated machine learning models

## Notes
This project uses synthetic data for academic purposes. Real-world deployment would require validation using live network logs.
