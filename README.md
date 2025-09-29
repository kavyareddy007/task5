# Titanic Dataset - Exploratory Data Analysis (EDA)

## Project Overview
This project performs **Exploratory Data Analysis (EDA)** on the Titanic dataset to identify key factors that influenced passenger survival.  
It is based on the classic Kaggle Titanic dataset (`train.csv`, `test.csv`, and `gender_submission.csv`).  

The analysis is implemented in **Python (Jupyter Notebook)** with visualizations, a **PowerPoint presentation**, and a **PDF report**.

---

## Dataset
The dataset comes from Kaggle’s Titanic competition and contains the following files:

- `train.csv` → Training dataset (891 passengers with labels).  
- `test.csv` → Test dataset (no survival labels).  
- `gender_submission.csv` → Sample submission file.  

Key features:
- **Survived**: Survival status (0 = No, 1 = Yes)  
- **Pclass**: Ticket class (1st, 2nd, 3rd)  
- **Sex, Age, SibSp, Parch, Fare, Cabin, Embarked**  

---

## Steps Performed
1. **Data Loading & Cleaning**  
   - Filled missing values (Age → median, Embarked → mode, Fare → median).  
   - Dropped/simplified Cabin due to many missing values.  

2. **Feature Engineering**  
   - Created new features (Title, FamilySize, IsAlone, Age/Fare bins).  

3. **Exploratory Data Analysis (EDA)**  
   - Survival distribution.  
   - Survival by Sex, Passenger Class, and their interaction.  
   - Age and Fare distributions.  
   - Correlation heatmap of numerical features.  

4. **Visualization**  
   - Countplots, barplots, histograms, boxplots, and heatmaps generated with `matplotlib` and `seaborn`.  

---

## Key Findings
- Only **38% survived** (62% died).  
- **Women (74%)** and **children** had higher survival rates.  
- **1st class passengers (63%)** survived more than 3rd class (24%).  
- **Wealth (Fare)** positively correlated with survival.  
- Strongest interaction: **1st-class women (97% survived)** vs **3rd-class men (14% survived)**.  
  

---

## 📦 Requirements
- Python 3.8+  
- Libraries:  
  ```bash
  pip install pandas numpy matplotlib seaborn python-pptx
