# Wildfire Risk Prediction with LSTM and XAI


This repository contains the code and report for my Master's dissertation project: 
**Wildfire Risk Assessment Using Long Short-Term Memory (LSTM) and Explainable Artificial Intelligence (XAI): Case Study of the Mediterranean Basin (2006–2022).**

---

## 🔑 Key Features:

**Data**: [Mesogeos](https://orionlab.space.noa.gr/mesogeos/), a multi-purpose dataset for data-driven wildfire modeling in the Mediterranean (meteorological, environmental, anthropogenic variables).

**Model**: Long Short-Term Memory (LSTM) neural network for binary wildfire risk prediction, classifying whether a wildfire will ignite at the end of a 30-day observation window.

**Performance**: 
  - At the chosen decision threshold = 0.24, the model caught 87.5% of wildfires (**Recall = 87.5%**).

  - At this threshold, when the model predicted a fire, it was correct 75.8% of the time (**Precision = 75.8%**).

  - Overall, the model achieved an **Area Under the Precision–Recall Curve (AUPRC) of 89%**, showing a strong balance between detecting wildfires and avoiding false alarms across all thresholds.
    
**Explainability**: Integrated Gradients & Permutation Feature Importance to identify key predictors (Meteorological factors like temperature and moisture dynamics were the **dominant predictors**).

**Tools**:
  - R (Tidyverse)
  - Python (NumPy, Pandas, Matplotlib, Seaborn, Pytorch, Captum).

---

## 📂 Data Access

Due to file size constraints, the dataset used in this project is hosted on Google Drive.

📁 **Download the dataset here**: [Google Drive Link](https://drive.google.com/drive/folders/1dRyn7EAwG88f0QMKGz74rWY8krKH8VSV) (Negatives + Positives) 

  Positives: 30-day sequences (across 27 variables) that ended with a wildfire ignition on the final day of the window.
  
  Negatives: 30-day sequences that did not result in a wildfire ignition at the end of the window. 

---

  ## 📖 Full Report
All **plots, results, and interpretations** are included in my dissertation in the [`report/`](report/) folder.  
- Chapter 3 covers how the dataset was explored and prepared, how the LSTM model was trained and evaluated, and how explainability methods were applied.  
