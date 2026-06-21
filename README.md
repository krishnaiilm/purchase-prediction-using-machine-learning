# 🏖️ Holiday Package Purchase Prediction

A machine learning classification project that predicts whether a customer is likely to purchase a holiday travel package based on demographic, travel, and behavioral attributes. The project follows an end-to-end machine learning pipeline, including data preprocessing, feature engineering, model development, hyperparameter tuning, and model evaluation.

---

## 📌 Problem Statement

Travel companies invest significant resources in marketing campaigns and customer outreach. Identifying customers who are more likely to purchase a holiday package can improve conversion rates and reduce marketing costs.

The objective of this project is to build a predictive machine learning model that helps travel companies target potential customers more effectively by forecasting purchase likelihood.

---

## 📂 Dataset

* Dataset: `Travel.csv`
* Target Variable: `ProdTaken`

  * `1` → Customer purchased the holiday package
  * `0` → Customer did not purchase the holiday package

### Key Features

| Feature                  | Description                     |
| ------------------------ | ------------------------------- |
| Age                      | Age of the customer             |
| MonthlyIncome            | Monthly income                  |
| TypeofContact            | Mode of customer contact        |
| DurationOfPitch          | Sales pitch duration            |
| NumberOfFollowups        | Number of follow-up calls       |
| PreferredPropertyStar    | Preferred hotel star rating     |
| NumberOfTrips            | Number of trips taken           |
| MaritalStatus            | Marital status                  |
| Gender                   | Gender of the customer          |
| NumberOfChildrenVisiting | Number of accompanying children |

---

## 🔧 Project Workflow

### Data Cleaning

* Handled missing values using median and mode imputation.
* Fixed inconsistent categorical labels.
* Removed unnecessary identifiers such as `CustomerID`.

### Feature Engineering

* Created a new feature called `TotalVisiting` by combining:

  * `NumberOfPersonVisiting`
  * `NumberOfChildrenVisiting`
* Improved representation of total travelers for better model learning.

### Data Preprocessing

* Performed an 80:20 Train-Test Split.
* Built a preprocessing pipeline using:

  * `OneHotEncoder` for categorical variables.
  * `StandardScaler` for numerical variables.
  * `ColumnTransformer` for efficient feature transformation.

### Model Development

Implemented and compared multiple machine learning algorithms:

* Logistic Regression
* Decision Tree Classifier
* Random Forest Classifier
* AdaBoost Classifier
* Gradient Boosting Classifier
* XGBoost Classifier

### Hyperparameter Tuning

* Applied `RandomizedSearchCV` to optimize:

  * Random Forest
  * XGBoost
* Improved model performance and generalization.

### Model Evaluation

Compared models using:

* Accuracy Score
* Precision Score
* Recall Score
* F1-Score
* ROC-AUC Score

### Model Selection

Selected the best-performing model based on overall predictive performance and robustness on unseen data.

---

## 📊 Machine Learning Algorithms Used

* Logistic Regression
* Decision Tree
* Random Forest
* AdaBoost
* Gradient Boosting
* XGBoost

---

## 📈 Model Performance

The performance of all machine learning models was evaluated and compared using multiple classification metrics.

| Metric  | Score |
| ------- | ----- |
| ROC-AUC | 0.83  |

The final model achieved a ROC-AUC score of **0.83**, demonstrating strong capability in distinguishing customers who are likely to purchase a holiday package from those who are not.

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost

### Development Environment

* Jupyter Notebook

---

## 🚀 How to Run

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/holiday-package-prediction.git
cd holiday-package-prediction
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run the Notebook

```bash
jupyter notebook Holiday_package_prediction.ipynb
```

---

## 📁 Repository Structure

```text
holiday-package-prediction/
│
├── Holiday_package_prediction.ipynb
├── Travel.csv
├── README.md
└── requirements.txt
```

---

## 🎯 Project Outcome

This project demonstrates how machine learning can be used to identify potential customers for targeted marketing campaigns. By comparing multiple classification algorithms and optimizing their performance, the solution helps improve customer acquisition strategies and business decision-making.

---

## 👨‍💻 Author

Krishna Kumar

B.Tech (Computer Science Engineering - AI & ML)

IILM University, Greater Noida

AI/ML Enthusiast | Aspiring Data Scientist

---

## ⭐ If you found this project useful, consider giving it a star on GitHub.
