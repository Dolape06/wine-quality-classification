# Wine Quality Classification Model

## Problem Statement & Project Impact

### The Problem: Subjective Wine Quality Evaluation
In the wine industry, quality assessment is traditionally performed by human experts through sensory analysis. While effective, this process is **subjective**, **costly**, and **difficult to scale** consistently across large production volumes. Variability in expert judgment can lead to inconsistent quality ratings and inefficient production decisions. This creates a **market information asymmetry** where producers lack a standardized, objective chemical benchmark for their products.

### The Solution: Objective Quality Prediction Using Machine Learning
This project implements a **Machine Learning classification model** to predict red wine quality using physicochemical properties from the `winequality-red.csv` dataset. By analyzing features such as alcohol content, acidity levels, and sulphates, the model provides a **data-driven and reproducible approach** to wine quality assessment, supporting more consistent quality control and transparent market valuation.

## Technical Methodology

* **Imbalanced Learning**: Utilized **SMOTE** (Synthetic Minority Over-sampling Technique) to address the minority class of high-quality wines, ensuring the model identifies "Premium" samples effectively.
* **Robust Preprocessing**: Employed **RobustScaler** to mitigate the influence of outliers in the chemical measurements.
* **Ensemble Architecture**: Trained a **Random Forest Classifier** to capture complex, non-linear interactions between chemical properties.
* **Model Validation**: Analyzed performance through **Learning Curves** to confirm the model's ability to generalize to unseen data.

## Dataset Overview
The dataset contains physicochemical measurements of red wine samples with the following key features:

* **quality (Target)**: Quality score assigned by wine experts.
* **alcohol**: Alcohol percentage by volume.
* **volatile acidity**: Acetic acid concentration.
* **fixed acidity**: Tartaric acid content.
* **citric acid**: Citric acid concentration.
* **sulphates**: Sulphate concentration contributing to preservation and taste.

## Key Insights

* **Alcohol Impact**: Higher alcohol content is strongly associated with higher quality scores.
* **Acidity Control**: Elevated volatile acidity negatively affects wine quality.
* **Feasibility**: Physicochemical features alone are sufficient to build effective quality classification models, reducing the reliance on expensive sensory analysis.
* **Robustness**: The use of scaling and over-sampling techniques ensures the model remains stable across different chemical profiles.

## Tech Stack
* **Language**: Python
* **Libraries**: Scikit-learn, Imbalanced-learn (SMOTE), Pandas, NumPy
* **Visualization**: Matplotlib, Seaborn
