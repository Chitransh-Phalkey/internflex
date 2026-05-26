# 📊 Iris Flower - Supervised Classification Project

Is project mein humne machine learning ka use karke phoolon ke measurements (length/width) se unki species predict karna sikha hai.

## 1. Project Objective & Dataset
* **Objective:** Build a supervised classification model to predict the species of an Iris flower based on its physical measurements.
* **Dataset Used:** Iris Flower Dataset (150 rows, 5 columns).
* **Features ($X$):** Sepal length, Sepal width, Petal length, Petal width.
* **Target ($y$):** Flower Class (`Iris-setosa`, `Iris-versicolor`, `Iris-virginica`).

## 2. Data Preprocessing & Splitting
* **Missing Values:** Checked the dataset using `isnull().sum()`. Found 0 missing values; the data was completely clean.
* **Train/Test Split:** Split the dataset into an **80% Training set** (120 samples) to train the models and a **20% Testing set** (30 samples) to evaluate them. Stratification was used to keep the class distribution balanced.

## 3. Model Selection & Comparison
We trained and evaluated two distinct algorithms: **Logistic Regression** (Linear Baseline) and **Random Forest** (Ensemble Tree-based).

### Final Evaluation Metrics:

| Metric | Logistic Regression | Random Forest Classifier |
| :--- | :--- | :--- |
| **Accuracy** | 97% | 97% |
| **Precision** | 0.97 | 0.97 |
| **Recall** | 0.97 | 0.97 |
| **F1-Score** | 0.97 | 0.97 |
| **5-Fold CV Mean Accuracy** | 97% | 97% |

## 4. Key Insights & Conclusion
* Both models performed exceptionally well, achieving an identical **97% accuracy** on the unseen test data.
* The 5-Fold Cross-Validation confirmed that this high performance is stable and consistent across different subsets of data (97% mean accuracy).
* **Final Recommendation:** Since it is a small and linearly separable dataset, **Logistic Regression** is preferred for production due to its low computational cost and simplicity.
