# Employee Attrition Prediction using Machine Learning

## 📌 Project Overview

Employee attrition is one of the biggest challenges faced by organizations. Losing experienced employees leads to increased recruitment costs, training expenses, and reduced productivity.

This project applies Machine Learning techniques to predict whether an employee is likely to leave the company based on HR-related factors such as job satisfaction, salary, work-life balance, overtime, years at the company, job role, and business travel.

The objective is to help HR departments identify employees at risk of leaving so that proactive retention strategies can be implemented.

---

## 🎯 Objectives

* Analyze employee attrition patterns.
* Clean and preprocess HR data.
* Perform Exploratory Data Analysis (EDA).
* Build multiple Machine Learning models.
* Compare model performance.
* Identify the most important factors influencing employee attrition.
* Generate business recommendations for HR teams.

---

## 📂 Dataset

**Dataset Name:** IBM HR Analytics Employee Attrition & Performance

* Total Records: **1470**
* Total Features: **35**
* Target Variable: **Attrition (Yes/No)**

The dataset contains employee information including:

* Age
* Department
* Job Role
* Monthly Income
* Overtime
* Business Travel
* Work-Life Balance
* Job Satisfaction
* Years at Company
* Performance Rating
* Education
* Marital Status
* and many more.

---

## 🛠 Technologies Used

* Python 3
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 📊 Exploratory Data Analysis (EDA)

The following analyses were performed:

* Employee Attrition Rate
* Attrition by Department
* Attrition by Job Role
* Monthly Income vs Attrition
* Work-Life Balance vs Attrition
* Years at Company vs Attrition

### Key Findings

* Approximately **16%** of employees left the company.
* The **Sales Department** had the highest attrition rate.
* **Sales Representatives** showed the highest employee turnover.
* Employees with lower salaries were more likely to leave.
* Overtime and frequent business travel significantly increased attrition risk.

---

## ⚙️ Data Preprocessing

The following preprocessing steps were completed:

* Checked for missing values.
* Removed unnecessary columns:

  * EmployeeNumber
  * EmployeeCount
  * Over18
  * StandardHours
* Converted Attrition from Yes/No to 1/0.
* Applied One-Hot Encoding to categorical variables.
* Standardized numerical features using StandardScaler.
* Split the dataset into training and testing sets (80:20).

---

## 🤖 Machine Learning Models

Three classification models were trained:

1. Logistic Regression
2. Random Forest Classifier
3. Gradient Boosting Classifier

To address class imbalance, class weights were used where applicable.

---

## 📈 Model Performance

| Model               | Precision | Recall | F1-Score |   ROC-AUC |
| ------------------- | --------: | -----: | -------: | --------: |
| Logistic Regression |     0.341 |  0.617 |    0.439 | **0.799** |
| Random Forest       |     0.571 |  0.085 |    0.148 |     0.772 |
| Gradient Boosting   |     0.588 |  0.213 |    0.313 |     0.794 |

### Best Model

**Logistic Regression**

Reasons:

* Highest ROC-AUC Score
* Highest Recall
* Highest F1-Score
* Easy to interpret for HR professionals

---

## 📉 Visualizations

The project includes the following visualizations:

* Attrition Rate by Department
* Attrition Rate by Job Role
* Monthly Income vs Attrition (Box Plot)
* Confusion Matrix
* Top 10 Feature Importance
* ROC Curve Comparison

---

## 💡 Business Insights

The analysis revealed several important findings:

* Sales employees have the highest attrition rate.
* Sales Representatives are the most likely to leave.
* Employees working overtime are at greater risk of attrition.
* Lower monthly income contributes to higher employee turnover.
* Frequent business travel is associated with increased attrition.

---

## ✅ HR Recommendations

* Focus retention programs on Sales Representatives and Laboratory Technicians.
* Reduce excessive overtime to improve work-life balance.
* Conduct regular employee engagement and career development discussions.
* Improve onboarding and mentoring for new employees.
* Monitor employees with frequent business travel.

---

## 📁 Project Structure

```
EmployeeAttrition/

│── analysis.ipynb
│── README.md
│── HR_Attrition.csv
│── summary.pdf
│
├── charts/
│   ├── department_attrition.png
│   ├── jobrole_attrition.png
│   ├── monthly_income_boxplot.png
│   ├── confusion_matrix.png
│   ├── top10_features.png
│   └── roc_curve.png
```

---

## 🚀 How to Run

1. Clone the repository

```bash
git clone https://github.com/yourusername/Employee-Attrition-Prediction.git
```

2. Navigate to the project folder

```bash
cd Employee-Attrition-Prediction
```

3. Install required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

4. Open the notebook

```bash
jupyter notebook analysis.ipynb
```

---

## 📌 Future Improvements

* Hyperparameter tuning using GridSearchCV.
* Handle class imbalance using SMOTE.
* Deploy the model using Flask or FastAPI.
* Build an interactive HR dashboard.
* Integrate real-time employee data for continuous prediction.

---

## 👨‍💻 Author

**Vishal Prajapati**

B.Tech Computer Science Engineering (AI & ML)

GitHub: https://github.com/CodeByVishal-0

LinkedIn: [www.linkedin.com/in/vishal-prajapati-725624286](http://www.linkedin.com/in/vishal-prajapati-725624286)

---

## ⭐ If you found this project useful, please consider giving it a star on GitHub.
