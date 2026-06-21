# 🏖️ Holiday Package Purchase Prediction

A machine learning project to predict whether a customer will purchase a holiday travel package, based on demographic and behavioral features.

---

## 📌 Problem Statement

A travel company wants to identify which customers are most likely to buy a newly launched holiday package. By predicting purchase likelihood, the company can target marketing efforts more efficiently and reduce sales costs.

---

## 📂 Dataset

- **File:** `Travel.csv`
- **Source:** Customer data from a travel company
- **Target Variable:** `ProdTaken` (1 = Package Purchased, 0 = Not Purchased)

**Key Features:**
| Feature | Description |
|---|---|
| Age | Age of the customer |
| MonthlyIncome | Monthly income of the customer |
| TypeofContact | How the customer was contacted |
| DurationOfPitch | Duration of the sales pitch (minutes) |
| NumberOfFollowups | Number of follow-up calls made |
| PreferredPropertyStar | Preferred hotel star rating |
| NumberOfTrips | Number of trips taken per year |
| NumberOfChildrenVisiting | Number of children accompanying |
| MaritalStatus | Marital status of the customer |
| Gender | Gender of the customer |

---

## 🔧 Project Workflow

1.Data Cleaning — fixed inconsistent labels, imputed missing values (median/mode), dropped CustomerID
2.Feature Engineering — combined NumberOfPersonVisiting + NumberOfChildrenVisiting into a single TotalVisiting feature
3.Preprocessing — train-test split (80/20), ColumnTransformer with OneHotEncoder + StandardScaler
4.Modeling — trained Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, AdaBoost, XGBoost
5.Tuning — RandomizedSearchCV on Random Forest and XGBoost
6.Evaluation — compared models on Accuracy, F1, Precision, Recall, ROC-AUC
---

## 📊 Model Performance

**Algorithm Used:** 
• Logistic Regression
• Decision Tree Classifier
• Random Forest Classifier
• AdaBoost Classifier
• Gradient Boosting Classifier
• XGBoost Classifier

| Metric | Score |
|---|---|
| ROC-AUC | **0.83** |

### ROC Curve

![ROC AUC Curve](images/auc.png)

The model achieves an AUC of **0.83**, indicating strong discriminatory ability between customers who will and won't purchase the holiday package.

---

## 🛠️ Tech Stack

- **Language:** Python 3
- **Libraries:** pandas, numpy, matplotlib, seaborn, plotly, scikit-learn
- **Environment:** Jupyter Notebook

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/holiday-package-prediction.git
   cd holiday-package-prediction
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebook:
   ```bash
   jupyter notebook notebooks/Holiday_package_prediction.ipynb
   ```

---

## 📁 Repository Structure

```
holiday-package-prediction/
│
├── data/
│   └── Travel.csv
├── notebooks/
│   └── Holiday_package_prediction.ipynb
├── images/
│   └── auc.png
├── README.md
└── requirements.txt
```

---

## 👨‍💻 Author

**Krishna**  
B.Tech Student | IILM University, Greater Noida  
Aspiring Data Scientist | ML Enthusiast

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
