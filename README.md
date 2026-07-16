# Titanic Dataset Analysis with Python

## Project Overview
This project was completed as part of the **BCS 404: Introduction to Data Science with Python** Mid-Semester Examination for the **2025/2026 Second Semester**.

The objective is to perform a complete data science workflow on the **Titanic Dataset**, including:

- Data acquisition
- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Statistical analysis
- Machine Learning using Logistic Regression
- Performance evaluation
- Discussion and conclusions

---

## Student Information

| Item | Details |
|------|---------|
| **Student Name** | Buabeng Otoo Derrick |
| **Index Number** | 01259610B |
| **Course** | BCS 404 – Introduction to Data Science with Python |
| **Academic Year** | 2025/2026 Second Semester |
| **Lecturer** | Dr. Joseph Dadzie |

---

# Project Structure

```
Titanic-DataScience-Midsem/
│
├── train.csv
├── titanic_cleaned.csv
├── Titanic_Analysis.py
├── README.md
└── 
```

---

# Dataset

Dataset Used:

**Titanic Passenger Dataset**

The dataset contains passenger information including:

- Passenger ID
- Survival Status
- Passenger Class
- Name
- Sex
- Age
- Siblings/Spouses
- Parents/Children
- Ticket
- Fare
- Cabin
- Embarked Port

Target Variable:

```
Survived
```

- 0 → Did Not Survive
- 1 → Survived

---

# Technologies Used

- Python 3
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# Required Libraries

```python
pandas
numpy
matplotlib
seaborn
scikit-learn
```

Install them using:

```bash
pip install -r requirements.txt
```

or

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

# Project Workflow

## Task 1 – Data Acquisition

The dataset is loaded using Pandas.

Activities include:

- Loading CSV file
- Viewing first five rows
- Displaying dataset dimensions
- Checking data types
- Inspecting dataset information

---

## Task 2 – Data Cleaning

Cleaning operations performed include:

### Missing Values

- Removed **Cabin** column due to excessive missing values.
- Filled missing **Age** values using median grouped by passenger class.
- Filled missing **Embarked** values using the mode.

### Duplicate Detection

- Checked for duplicate records.
- Removed duplicates if present.

### Final Verification

- Confirmed there are no remaining missing values.

---

## Task 3 – Exploratory Data Analysis (EDA)

Visualizations created include:

- Histogram of passenger ages
- Passenger class distribution
- Age boxplot by passenger class
- Scatter plot of Age vs Fare
- Correlation heatmap
- Pairplot of numerical variables

Each visualization includes interpretation of the observed patterns.

---

## Task 4 – Statistical Analysis

Performed statistical analysis including:

- Descriptive statistics
- Frequency distributions
- Correlation matrix
- Strongest positive correlation
- Strongest negative correlation
- Discussion of key statistical findings

Major findings include:

- Women had significantly higher survival rates.
- First-class passengers survived more frequently.
- Family size influenced survival probability.

---

## Task 5 – Machine Learning

A Logistic Regression classifier was developed to predict passenger survival.

### Selected Features

- Passenger Class
- Sex
- Age
- SibSp
- Parch
- Fare
- Embarked

### Data Preparation

- Label Encoding
- Train-Test Split (80% Training, 20% Testing)

### Model

```
Logistic Regression
```

### Performance Metrics

- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1-Score
- Classification Report

---

## Task 6 – Discussion and Conclusion

The project concludes that:

- Gender is the strongest predictor of survival.
- Passenger class significantly affects survival.
- Fare and socio-economic status are important factors.
- Logistic Regression achieved good predictive performance.
- More advanced models could improve prediction accuracy.

---

# Output

The project generates:

- Cleaned Titanic dataset
- Statistical summaries
- Data visualizations
- Correlation analysis
- Logistic Regression model
- Performance evaluation metrics

The cleaned dataset is saved as:

```
titanic_cleaned.csv
```

---

# How to Run

1. Clone or download this repository.

2. Install required libraries.

```bash
pip install -r requirements.txt
```

3. Place the Titanic dataset inside the project folder.

4. Run the Python script.

```bash
python Titanic_Analysis.py
```

---

# Machine Learning Summary

| Item | Description |
|------|-------------|
| Algorithm | Logistic Regression |
| Problem Type | Binary Classification |
| Target Variable | Survived |
| Train/Test Split | 80% / 20% |
| Evaluation Metrics | Accuracy, Precision, Recall, F1-Score, Confusion Matrix |

---

# Learning Outcomes

This project demonstrates practical skills in:

- Data acquisition
- Data cleaning
- Exploratory Data Analysis
- Statistical analysis
- Data visualization
- Feature engineering
- Classification modeling
- Model evaluation
- Data interpretation

---

# Future Improvements

Possible enhancements include:

- Random Forest Classifier
- Decision Tree Classifier
- Support Vector Machine (SVM)
- XGBoost
- Hyperparameter tuning
- Cross-validation
- Feature engineering
- Interactive dashboards using Plotly or Streamlit

---

# Author

**Buabeng Otoo Derrick**

Computer Science Student

BCS 404 – Introduction to Data Science with Python

Academic Year: 2025/2026 Second Semester

---

# Acknowledgements

Special thanks to:

- **Dr. Joseph Dadzie** for guidance throughout the course.
- The Titanic dataset providers.
- The Python open-source community.
- Scikit-learn, Pandas, Matplotlib, and Seaborn developers.

---

# License

This project was developed solely for academic purposes as part of the BCS 404 Mid-Semester Examination.

© 2026 Buabeng Otoo Derrick. All rights reserved.