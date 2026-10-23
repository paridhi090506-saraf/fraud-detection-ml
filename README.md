# fraud-detection-ml
Fraud detection using machine learning, data preprocessing, and model evaluation.
# Fraud Detection Using Machine Learning

##  About the Project

Fraudulent transactions are a major challenge in digital payments and financial systems. Detecting these transactions accurately is important for reducing financial losses while avoiding unnecessary alerts on legitimate transactions.

This project applies machine learning classification techniques to identify potentially fraudulent transactions. It explores different classification models, compares their performance, and investigates how changing the prediction threshold can affect fraud detection.

The project is implemented in Python using a Jupyter Notebook.

##  Project Objectives

- Analyze transaction data to understand its features and patterns.
- Prepare the dataset for machine learning.
- Train multiple classification algorithms for fraud detection.
- Compare models using appropriate evaluation metrics.
- Study the effect of decision thresholds on fraud predictions.
- Understand the balance between identifying fraudulent transactions and minimizing false positives.

##  Machine Learning Approach

The project explores four classification algorithms:

### 1. Logistic Regression
A baseline classification algorithm that estimates the probability of a transaction belonging to the fraudulent class.

### 2. Decision Tree
A tree-based model that learns decision rules from the input features to classify transactions.

### 3. Random Forest
An ensemble learning algorithm that combines predictions from multiple decision trees to improve classification performance.

### 4. XGBoost
A gradient-boosting algorithm that builds decision trees sequentially, with each new tree helping improve the overall model.

Comparing these approaches helps examine the differences between linear classification, individual decision trees, bagging-based ensembles, and gradient boosting.

##  Project Workflow

The notebook follows a machine learning workflow consisting of the following stages:

1. **Data Loading:** Load the transaction dataset into Python for analysis.
2. **Exploratory Data Analysis:** Examine the dataset's structure, features, and distributions.
3. **Data Preprocessing:** Prepare the data for model training and prediction.
4. **Train-Test Split:** Separate the data into training and testing subsets to evaluate model performance on unseen examples.
5. **Model Training:** Train the selected classification algorithms.
6. **Prediction:** Generate class predictions and, where supported, predicted probabilities.
7. **Model Evaluation:** Compare classification performance using relevant evaluation metrics.
8. **Threshold Analysis:** Investigate how changing the decision threshold affects the classification of fraudulent transactions.

##  Evaluation and Threshold Analysis

Fraud detection is a classification problem in which accuracy alone may not provide a complete picture of model performance, particularly when fraudulent transactions are much less common than legitimate ones.

The project considers evaluation measures such as:

- **Precision:** The proportion of transactions predicted as fraudulent that are actually fraudulent.
- **Recall:** The proportion of actual fraudulent transactions correctly identified by the model.
- **F1-Score:** The harmonic mean of precision and recall.
- **Confusion Matrix:** A breakdown of correct and incorrect predictions for each class.
- **ROC-AUC:** A measure of how well a model distinguishes between the two classes across different classification thresholds, when applicable.

### Why Decision Thresholds Matter

A classification model that produces probabilities typically uses a threshold to convert those probabilities into class predictions.

Changing this threshold can affect the number of fraudulent transactions detected and the number of legitimate transactions incorrectly flagged.

- A lower threshold may identify more fraudulent transactions but can also increase false positives.
- A higher threshold may reduce false positives but can cause more fraudulent transactions to go undetected.

Threshold analysis helps explore this trade-off and highlights why the choice of threshold matters in practical fraud detection systems.

##  Technologies Used

- **Programming Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn, XGBoost
- **Development Environment:** Jupyter Notebook

##  Repository Structure

```text
fraud-detection-ml/
├── fraudDetectionML.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

### Dataset Instructions

The dataset is not included in this repository because of its large file size.

##  Author

**Paridhi Saraf**  
B.Tech, Computer Science and Engineering  
Birla Institute of Technology, Mesra

