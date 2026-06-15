EHB420E — Artificial Neural Networks Term Project.

This project compares **gradient boosting (XGBoost)** and **1D Convolutional Neural Networks** on two input representations (summary statistics vs. time-series MFCC) for identifying spoken language and accent (Arabic, English, French) from short audio clips.

## Key Result
The decisive factor is not the use of deep learning itself, but preserving the **temporal structure** of the input. A time-series 1D-CNN reached **93.67%** accuracy, outperforming an XGBoost baseline (89.00%) and a summary-feature CNN (86.50%).

## Dataset
Mozilla Common Voice — 1000 clips each for Arabic, English, and French (3000 total).

## Models
- **Model 1:** XGBoost on 54-dim summary features (baseline)
- **Model 2:** 1D-CNN on the same summary features
- **Model 3:** Time-series 1D-CNN on 216×13 MFCC sequences (proposed)

## Repository Contents
- `notebook.ipynb` — full pipeline (data, feature extraction, training, demo)
- `report/` — project report (LaTeX source and figures)
- `presentation.pptx` — project presentation

## Authors
- Yunus Gökdemir (040220060)
- Delfin Özdemir (040210087)

## Note
You need your own Mozilla Data Collective API key to run the data download.
