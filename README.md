# 🛳️ Titanic Survival Prediction

This project analyzes the Titanic passenger dataset to identify key factors influencing survival and builds a predictive model to estimate the chances of survival for future passengers.

## 📌 Project Goals
- Perform data cleaning and preprocessing
- Conduct exploratory data analysis (EDA) to extract insights
- Visualize key patterns using Seaborn and Matplotlib
- Build and evaluate basic predictive models

---

## 📂 Dataset
The dataset is available on [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic/data)

**Features include:**
- Passenger demographics (Age, Sex, Class, etc.)
- Travel details (Fare, Cabin, Embarked, etc.)
- Survival outcome (`Survived` - 0 = No, 1 = Yes)

---

## 🔧 Steps Performed

### 1. Data Cleaning
- Imputed missing values (`Age`, `Embarked`)
- Dropped columns with excessive missing data (`Cabin`)
- Converted categorical data (`Sex`, `Embarked`) to numerical
- Removed irrelevant columns (`Name`, `Ticket`, `PassengerId`)

### 2. Exploratory Data Analysis (EDA)
- Visualized survival rates by `Sex`, `Pclass`, `Age`, `Fare`, and `Family Size`
- Used Seaborn and Matplotlib for visual analysis
- Identified strong survival trends across gender and class

### 3. Feature Engineering
- Created new feature: `FamilySize = SibSp + Parch + 1`
- Binned age and fare for better interpretability

### 4. Model Building
- Logistic Regression: Baseline model (~78% accuracy)
- Random Forest Classifier: Improved model (~81% accuracy)
- Train/test split with standard scaling
- Evaluated models using accuracy and confusion matrix

---

## 📊 Key Insights
- **Females** had much higher survival rates (~74%)
- **1st class passengers** were more likely to survive
- Children and those with smaller family sizes had higher chances
- Higher ticket fare positively correlated with survival

---

## 💡 Tech Stack
- Python
- Jupyter Notebook
- pandas, numpy
- matplotlib, seaborn
- scikit-learn

---


