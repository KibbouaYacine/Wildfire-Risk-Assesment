# Wildfire Risk Prediction with LSTM and XAI


This repository contains the code and report for my Master's dissertation project: 
**Wildfire Risk Assessment Using Long Short-Term Memory (LSTM) and Explainable Artificial Intelligence (XAI): Case Study of the Mediterranean Basin (2006–2022).**

## Key Features:

**Data**: [Mesogeos](https://orionlab.space.noa.gr/mesogeos/), a multi-purpose dataset for data-driven wildfire modeling in the Mediterranean (meteorological, environmental, anthropogenic variables).

**Model**: Long Short-Term Memory (LSTM) neural network for temporal wildfire risk prediction.

**Performance**: 
  - The model caught 87.5% of the wildfires that actually occurred (Recall = 87.5%).
    
  - Overall reliability was very high: when the model flagged a potential fire, it was correct 89% of the time (Area under the Precision-Recall curve AUPRC = 89%)
    
**Explainability**: Integrated Gradients & Permutation Feature Importance to identify key predictors (Meteorological factors like temperature and moisture dynamics were the **dominant predictors**).

**Tools** : R (Tidyverse), Python (NumPy, Pandas, Matplotlib, Seaborn, Pytorch).

## Data Access

Due to file size constraints, the dataset used in this project is hosted on Google Drive.

📁 **Download the dataset here**: [Google Drive Link](https://drive.google.com/drive/folders/1dRyn7EAwG88f0QMKGz74rWY8krKH8VSV) (Negatives + Positives) 

  Positives: 30-day sequences (across 27 variables) that ended with a wildfire ignition on the final day of the window.
  
  Positives : 30-day sequences that did not result in a wildfire ignition at the end of the window. 
