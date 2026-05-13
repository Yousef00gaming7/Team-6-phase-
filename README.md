# Team-6-phase-
# Explainable AI for Diabetes Prediction Using Machine Learning Models

## Project Overview

This project presents a comprehensive Explainable Artificial Intelligence (XAI) framework for diabetes prediction using the BRFSS 2015 Diabetes Health Indicators dataset.

The project focuses on developing accurate and interpretable machine learning models capable of predicting diabetes risk while providing transparent explanations for model predictions using multiple Explainable AI techniques.

The primary goal of this work is not only to maximize predictive performance but also to improve trust, transparency, and interpretability in healthcare-oriented AI systems.

---

# Dataset

Dataset Used:

* BRFSS 2015 Diabetes Health Indicators Dataset

Dataset Characteristics:

* Approximately 253,000 healthcare records
* 21 health-related features
* Binary classification target:

  * 0 → Non-diabetic
  * 1 → Diabetic / Prediabetic

Examples of Features:

* BMI
* HighBP
* GenHlth
* HighChol
* Age
* PhysHlth
* MentHlth
* Income

---

# Data Preprocessing

Several preprocessing steps were applied to improve data quality and model performance:

* Missing value handling using median imputation
* Duplicate removal
* StandardScaler normalization
* Train-test split
* Class balancing using SMOTE
* Feature selection using Correlation Analysis and Chi-Square Selection

Selected Features:

* GenHlth
* HighBP
* BMI
* DiffWalk
* HighChol
* Age
* HeartDiseaseorAttack
* PhysHlth
* MentHlth
* Income

---

# Implemented Machine Learning Models

The project includes multiple machine learning and deep learning models:

| Model                 | Description                                        |
| --------------------- | -------------------------------------------------- |
| Logistic Regression   | Linear baseline classification model               |
| Decision Tree         | Tree-based interpretable classification model      |
| AdaBoost              | Ensemble boosting model using weak learners        |
| Gradient Boosting     | Sequential ensemble boosting model                 |
| XGBoost               | Advanced gradient boosting framework               |
| CatBoost              | Robust boosting model for complex feature learning |
| LightGBM              | Efficient large-scale boosting model               |
| Extra Trees           | Randomized ensemble tree model                     |
| Neural Networks (MLP) | Deep learning classification model                 |

---

# Explainable AI Techniques

Several Explainable AI techniques were applied to analyze model behavior and improve transparency.

| Technique                                | Purpose                                        |
| ---------------------------------------- | ---------------------------------------------- |
| SHAP                                     | Global and local feature contribution analysis |
| LIME                                     | Local patient-level prediction explanation     |
| PDP (Partial Dependence Plot)            | Feature behavior visualization                 |
| ICE (Individual Conditional Expectation) | Individual feature effect analysis             |
| Permutation Importance                   | Feature contribution evaluation                |
| Feature Importance                       | Global feature ranking                         |

---

# Main Results

## Logistic Regression

* Accuracy: 0.72
* Recall: 0.75
* F1-score: 0.45

Key Findings:

* Stable and balanced performance
* Strong interpretability
* Smooth linear feature behavior

---

## Decision Tree

* Accuracy: 0.70
* Recall: 0.72
* F1-score: 0.42

Key Findings:

* High interpretability
* Easy-to-understand decision structure
* Strong nonlinear rule learning

---

## AdaBoost

* Accuracy: 0.72
* Recall: 0.74
* F1-score: 0.44

Key Findings:

* Improved diabetic case detection
* Better balance after threshold tuning
* Strong sensitivity to healthcare risk factors

---

## Gradient Boosting

Key Findings:

* Stable nonlinear learning
* Improved feature interaction handling
* Strong robustness

---

## XGBoost

* Accuracy: ~0.85
* AUC: ~0.81

Key Findings:

* Highest predictive performance
* Strong nonlinear learning capability
* More difficult interpretability

---

## CatBoost

* Accuracy: ~0.85
* AUC: ~0.81

Key Findings:

* Strong robustness
* Effective boosting behavior
* Stable healthcare predictions

---

## LightGBM

Key Findings:

* Fastest training performance
* Efficient memory usage
* Strong scalability

---

## Extra Trees

* Accuracy: ~0.80
* AUC: ~0.71

Key Findings:

* Reduced overfitting
* Stable ensemble predictions
* Good nonlinear learning capability

---

## Neural Networks (MLP)

Key Findings:

* Strong nonlinear learning capability
* Complex healthcare relationship modeling
* Improved transparency using XAI methods

---

# Explainability Insights

Across nearly all implemented models and XAI techniques, the following features consistently appeared as the strongest diabetes predictors:

* BMI
* General Health (GenHlth)
* High Blood Pressure (HighBP)
* Age
* High Cholesterol (HighChol)

These findings strongly align with established clinical knowledge and demonstrate that the models learned meaningful healthcare-related relationships.

---

# Key Observations

* Accuracy alone was insufficient for healthcare evaluation.
* Recall was considered more important because missing diabetic patients carries serious medical risks.
* Boosting models achieved the highest predictive accuracy.
* Simpler models provided stronger interpretability.
* Explainable AI techniques significantly improved model transparency and trustworthiness.

---

# Project Structure

```text
Project/
│
├── EDA/
├── Models/
│   ├── Logistic_Regression.ipynb
│   ├── Decision_Tree.ipynb
│   ├── AdaBoost.ipynb
│   ├── Gradient_Boosting.ipynb
│   ├── XGBoost.ipynb
│   ├── CatBoost.ipynb
│   ├── LightGBM.ipynb
│   ├── Extra_Trees.ipynb
│   └── Neural_Networks.ipynb
│
├── Reports/
├── Presentation/
├── References/
└── README.md
```

---

# Team Members

* Yousef Elrefaey
* Ahmed Mokhtar
* Farida Ehab
* Abdallah Saed

---

# Future Work

Potential future improvements include:

* Advanced deep learning explainability methods
* Larger healthcare datasets
* Real-time healthcare deployment
* Fairness and bias analysis
* Clinical decision-support integration

---

# Conclusion

This project demonstrates that combining Machine Learning with Explainable AI can produce reliable, transparent, and clinically meaningful healthcare prediction systems.

The integration of multiple XAI techniques significantly improved model interpretability and trustworthiness while maintaining strong predictive performance for diabetes risk prediction.
