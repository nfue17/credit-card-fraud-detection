# Credit Card Fraud Detection

This project focuses on detecting fraudulent credit card transactions using machine learning classification techniques. The dataset is highly imbalanced, making this a realistic and challenging problem in applied data science.

## Objective
The goal of this project is to build and evaluate a classification model that can accurately identify fraudulent transactions while minimizing false negatives (missed fraud cases).

## Dataset
The dataset used in this project is publicly available on Kaggle:

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

Due to licensing and size considerations, the dataset is not included in this repository.

## Tools & Technologies
- Python  
- Jupyter Notebook  
- pandas  
- numpy  
- matplotlib  
- scikit-learn  

## Project Workflow
1. Data loading and initial inspection  
2. Data cleaning and preprocessing  
3. Exploratory Data Analysis (EDA)  
4. Feature engineering (log transformation of transaction amount)  
5. Handling class imbalance using class weighting  
6. Model training using Logistic Regression  
7. Threshold tuning for classification  
8. Model evaluation using multiple metrics  

## Key Concepts
This project highlights important concepts in fraud detection:

- Imbalanced datasets  
- Classification modeling  
- Confusion matrix analysis  
- Precision and recall trade-off  
- F1-score evaluation  
- ROC curve and AUC  
- Threshold tuning  

## Model Evaluation

### ROC Curve

The model achieved an AUC score of approximately **0.97**, indicating a strong ability to distinguish between fraudulent and legitimate transactions.

![ROC Curve](images/roc_curve.png)

This demonstrates that the model performs very well in ranking transactions by their likelihood of being fraud.

### Interpretation

While the model achieves excellent discrimination performance (high AUC), practical fraud detection requires balancing recall and precision.

The model was optimized to increase recall (detect as many fraudulent transactions as possible), which led to a lower precision due to an increase in false positives.

This reflects a real-world trade-off in fraud detection systems, where missing fraudulent transactions is often more costly than incorrectly flagging legitimate ones.

## Results
- High recall for fraud detection (most fraudulent transactions are identified)  
- Lower precision due to false positives  
- Strong overall classification performance (AUC ≈ 0.97)  
- Demonstrates effective handling of imbalanced data  

## Repository Structure
- `credit_card_fraud_detection.ipynb` → main notebook  
- `README.md` → project documentation  
- `images/` → visualizations and plots  

## How to Run
1. Clone this repository  
2. Download the dataset from Kaggle  
3. Place the dataset in your working directory  
4. Install dependencies:
```bash
pip install pandas numpy matplotlib scikit-learn
