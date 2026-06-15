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

1. **Data Cleaning** — Handling inconsistent categories, missing values imputed using median/mode
2. **Exploratory Data Analysis (EDA)** — Distribution plots, correlation heatmap, category analysis
3. **Feature Engineering** — Label encoding for categorical variables
4. **Model Training** — Random Forest Classifier
5. **Evaluation** — ROC-AUC curve, classification report

---

## 📊 Model Performance

**Algorithm Used:** Random Forest Classifier

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
