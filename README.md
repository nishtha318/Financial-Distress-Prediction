# Financial Distress Prediction Using Machine Learning

## 1. Project Overview

This project focuses on predicting corporate financial distress using machine learning and deep learning techniques. It uses financial indicators to classify companies as bankrupt or non-bankrupt.

The objective is to develop and evaluate predictive models that can identify potential financial distress and support data-driven financial risk assessment.

## 2. Project Objectives

- Analyze financial indicators associated with corporate bankruptcy.
- Perform exploratory data analysis and data preprocessing.
- Address class imbalance in the dataset.
- Apply feature selection to identify relevant financial variables.
- Implement and compare machine learning and deep learning models.
- Evaluate model performance using multiple classification metrics.

## 3. Dataset Description

The project uses a financial distress dataset containing company-level financial indicators.

| Attribute | Description |
|---|---|
| Total Records | 6,819 |
| Initial Features | 96 (including target variable) |
| Target Variable | `Bankrupt?` |
| Non-Bankrupt Companies | 6,599 |
| Bankrupt Companies | 220 |

### Class Distribution

- Non-Bankrupt: 96.77%
- Bankrupt: 3.23%

The dataset exhibits significant class imbalance, making minority-class identification an important aspect of the project.

## 4. Methodology

The project follows the following workflow:

1. **Data Collection and Loading:** Importing and examining the financial dataset.
2. **Exploratory Data Analysis:** Analyzing feature distributions, correlations, and class distribution.
3. **Data Preprocessing:** Removing constant features, checking missing values, and scaling numerical variables.
4. **Feature Selection:** Selecting 29 relevant features for model development.
5. **Model Development:** Training machine learning and deep learning models.
6. **Model Evaluation:** Comparing models using classification metrics and performance analysis.

## 5. Models Implemented

### Machine Learning Models
- Logistic Regression
- XGBoost Classifier

### Deep Learning Models
- Long Short-Term Memory (LSTM)
- Transformer-based Architecture

## 6. Model Evaluation

The models were evaluated using the following metrics:

- **Accuracy:** Measures the proportion of correctly classified observations.
- **Precision:** Measures how many predicted bankrupt companies were actually bankrupt.
- **Recall:** Measures how many actual bankrupt companies were correctly identified.
- **F1-Score:** Represents the harmonic mean of precision and recall.
- **ROC-AUC:** Measures the model's ability to distinguish between the two classes.
- **PR-AUC:** Evaluates precision-recall performance, particularly useful for imbalanced datasets.

### Performance Comparison

| Model | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 97.21% | 68.75% | 25.00% | 36.67% | 93.16% |
| XGBoost | 93.62% | 29.91% | 72.73% | 42.38% | 92.72% |
| LSTM | 81.82% | 13.04% | 81.82% | 22.50% | 89.87% |

### Results and Observations

- Logistic Regression achieved the highest accuracy of 97.21%.
- XGBoost achieved the highest F1-score of 42.38% among the three models and demonstrated a stronger balance between precision and recall.
- LSTM achieved a recall of 81.82%, identifying a larger proportion of actual bankrupt companies.
- The results highlight the importance of evaluating multiple metrics rather than relying exclusively on accuracy when working with imbalanced datasets.

## 7. Technologies and Tools

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Development Environment | Google Colab |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn, XGBoost |
| Deep Learning | TensorFlow / Keras |

## 8. Project Structure

```text
Financial-Distress-Prediction/
│
├── notebooks/
│   └── Financial_Distress_Prediction.ipynb
│
├── dataset/
│   └── data.csv
│
├── README.md
└── requirements.txt
```

*The structure above is a suggested organization. Update the filenames and folders to match the actual repository.*

## 9. Installation and Execution

Clone the repository:

```bash
git clone https://github.com/your-username/financial-distress-prediction.git
```

Navigate to the project directory:

```bash
cd financial-distress-prediction
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Open the Jupyter Notebook or upload it to Google Colab and execute the cells sequentially.

## 10. Future Scope

- Experiment with advanced ensemble learning techniques.
- Improve minority-class prediction through class imbalance handling.
- Perform systematic hyperparameter optimization.
- Incorporate explainable AI techniques such as SHAP.
- Explore additional financial indicators to improve predictive performance.
- Develop an interactive dashboard for financial distress prediction.

## 11. Conclusion

This project demonstrates the application of machine learning and deep learning techniques to corporate financial distress prediction. The comparative evaluation highlights the trade-offs between accuracy, precision, and recall when identifying financially distressed companies.

The findings emphasize the importance of selecting evaluation metrics that account for class imbalance and the practical objective of identifying potential bankruptcy cases.

## Disclaimer

This project is developed for academic and research purposes only. The predictions generated by the models should not be considered professional financial advice or used as the sole basis for financial decisions.
