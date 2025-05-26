# iInternship-Task1
Internship
  Task 1: Data Cleaning & Preprocessing

This task involves cleaning and preparing the Titanic dataset for machine learning. Below are the three key steps performed in this notebook.

---

  Task Steps

 1. **Handle Missing Values**
- **Age**: Replaced missing values with the **median**.
- **Embarked**: Filled missing values with the **most frequent category (mode)**.
- **Cabin**: Dropped due to a high percentage of missing data.

---

 2. **Convert Categorical Features to Numerical**
- **Sex**: Converted to numeric using **label encoding** (`male` → 0, `female` → 1).
- **Embarked**: Converted using **one-hot encoding** with `drop_first=True` to avoid multicollinearity.

---

 3. **Normalize Numerical Features and Remove Outliers**
- Used **boxplots** to visualize outliers in the `Fare` column.
- Removed values above the **99th percentile** to clean extreme outliers.
- Applied **StandardScaler** to scale `Age` and `Fare` columns for consistent feature ranges.

---
 🛠 Tools & Libraries

- **Python**
- **Pandas** for data manipulation
- **NumPy** for numerical operations
- **Matplotlib & Seaborn** for visualization
- **Scikit-learn** for scaling and preprocessing
