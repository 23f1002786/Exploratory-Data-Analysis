# 🛳 Titanic Survival Prediction – Exploratory Data Analysis (EDA)

## 🎯 Objective

This project explores the **Titanic dataset** from Kaggle to identify factors influencing passenger survival. The aim is to perform comprehensive **Exploratory Data Analysis (EDA)** that uncovers meaningful patterns and supports predictive modeling.

---

## 🧹 Data Cleaning & Preparation

* Handled missing values in `Age`, `Embarked`, and `Cabin`.
* Converted categorical variables (e.g., `Sex`, `Embarked`, `Pclass`) into numeric or encoded formats.
* Detected and treated outliers in `Fare` and `Age`.
* Created derived features for deeper insights:

  * `FamilySize = SibSp + Parch + 1`
  * `IsAlone` (binary feature based on family size)
  * Extracted `Title` from passenger names

---

## 📊 Exploratory Data Analysis

### Key Relationships Studied

* **Class vs Survival:** First-class passengers had the highest survival rates.
* **Sex vs Survival:** Females were far more likely to survive than males.
* **Age vs Survival:** Younger passengers, especially children, showed higher survival rates.
* **SibSp & Parch vs Survival:** Passengers traveling alone were less likely to survive.
* **Embarked vs Survival:** Those who boarded at Cherbourg (C) had higher survival probabilities.
* **Age vs Class:** First-class passengers were generally older, while lower classes had more young passengers.

### Additional Insights

* Combined feature interactions like `Pclass + Sex` and `FamilySize + Survival` provided deeper patterns.
* Explored fare distributions and class-based differences in survival.

---

## 🖼 Visualization Approach

* Created **multiple grouped bar charts** using Matplotlib subplots for compact comparison.
* Used Seaborn for **countplots, boxplots, and KDE plots** to visualize survival trends across features.
* Heatmaps and correlation plots were employed to study relationships among numerical variables.

---

## 📈 Results & Findings

* **Strong predictors of survival:** `Sex`, `Pclass`, `Fare`, and `Family-related features`.
* Family size and passenger class played significant roles in determining survival odds.
* Clear demographic and social stratifications influenced the survival chances.

---

## 🚀 Next Steps

* Feature scaling and encoding for model input.
* Train models like **Logistic Regression, Random Forest, and XGBoost**.
* Optimize model performance via cross-validation and hyperparameter tuning.

---

## 🧰 Tools & Libraries

* **Python** (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
* **Jupyter Notebook** for analysis and visualization

---

## 💡 Key Takeaway

The EDA provides strong evidence that **socioeconomic status, gender, and family composition** were critical in determining survival. These insights lay the groundwork for effective predictive modeling in the next phase.
