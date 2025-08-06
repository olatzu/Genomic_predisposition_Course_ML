# Genomic Disorder Prediction (XGBoost) — Course ML Project

Kaggle: https://www.kaggle.com/code/brsdincer/genomes-and-genetics-disorder-prediction-ii/
This project aims to develop a **multi-class classifier** using XGBoost to predict various **genetic disorders** based on patient clinical, demographic, and family inheritance features. 
The model was trained and evaluated with a focus on high recall and interpretability to support safe and transparent use in medical contexts.

---

## Project Components

- **Notebook**: [`notebooks/genomic_model.ipynb`](notebooks/genomic_model.ipynb)  
  Contains all code, data preprocessing, modeling, and evaluation steps with clear comments.

- **Dataset Description** : "datasheet"
  Explains dataset origin, features, ethical considerations, and preprocessing details.

- **Model Card**: "model_card"
  Describes the chosen model architecture, intended use, metrics, limitations, and ethical implications.


---

##  Dataset: "train.csv"

The dataset was collected and curated by the author for this course project. 
It’s inspired by the Kaggle "Genomes and Genetics Disorder Prediction II" dataset and methodology :contentReference[oaicite:1]{index=1}. 
The dataset includes multiple encoded genetic inheritance features, clinical variables, and a multi-class label for genetic disorder types.



---

## Non-Technical Summary

This model predicts the likelihood of genetic disorders using patient age, genetic inheritance indicators (`Genes_Mother_Side`, `Inherited_Father`), and clinical features. 
I trained an XGBoost classifier—chosen for its performance on imbalanced, multi-class data and its interpretability via SHAP explanations. 
I used **SMOTENC** to balance classes without losing categorical feature information and applied feature scaling for preprocessing consistency. 
Evaluation prioritized **macro F1-score** and **class-wise recall** to reduce false negatives. 
SHAP-based analysis confirmed key genetic interactions. The model is designed for clinical support, not diagnosis, and emphasizes transparency and fair performance.

---

## 🛠️ How to Run This Project

1. **Clone the repository**  
   ```bash
   git clone https://github.com/olatzu/Genomic_predisposition_Course_ML.git
   cd Genomic_predisposition_Course_ML
