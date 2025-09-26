# Breast Cancer Classification using Logistic Regression

This project demonstrates how to build a machine learning model to classify breast cancer tumors as either **malignant** or **benign**. It utilizes the **Logistic Regression** algorithm, a fundamental technique for binary classification tasks.

---

## 🛠️ Tools and Libraries Used
* **Python**
* **Pandas** for data loading and manipulation.
* **Scikit-learn** for:
    * Splitting the data (`train_test_split`)
    * Feature scaling (`StandardScaler`)
    * Building the model (`LogisticRegression`)
    * Evaluating performance (accuracy, precision, recall, F1-score, confusion matrix)
* **Matplotlib & Seaborn** for visualizing the confusion matrix.

---

## 📋 Project Workflow

1.  **Data Loading and Cleaning:**
    * The dataset (`data.csv`) was loaded into a pandas DataFrame.
    * The unnecessary `id` and `Unnamed: 32` columns were dropped to clean the data.

2.  **Data Preprocessing:**
    * The target variable, `diagnosis`, was **encoded** from categorical ('M'/'B') to numerical (`1`/`0`) for model compatibility.

3.  **Data Splitting and Scaling:**
    * The data was split into an **80% training set** and a **20% testing set**.
    * **Feature Scaling** was applied using `StandardScaler` on both the training and testing sets. This is a crucial step for logistic regression to ensure all features are on the same scale and contribute equally to the model's decision-making process.

4.  **Model Training:**
    * A **Logistic Regression** model was instantiated and trained on the scaled training data.

5.  **Model Evaluation:**
    * The trained model was used to make predictions on the scaled test data.
    * The model's performance was rigorously evaluated using several key classification metrics:
        * **Accuracy:** The overall percentage of correct predictions.
        * **Precision:** The accuracy of positive predictions.
        * **Recall:** The model's ability to find all actual positive cases.
        * **F1-Score:** A balanced measure of precision and recall.
    * A **Confusion Matrix** was generated to provide a detailed, visual breakdown of the model's predictive performance, showing the counts of true positives, true negatives, false positives, and false negatives.

---

## ✅ Results

The model achieved an outstanding **accuracy of 97%** on the test set, demonstrating its effectiveness in correctly classifying tumors. The high precision and recall scores further indicate that the model is both reliable and comprehensive in its predictions. The confusion matrix confirmed a very low number of misclassifications, making this a highly successful and robust classification model.
