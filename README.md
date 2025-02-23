# Titanic Survival Analysis - Power BI Dashboard

## 📌 Project Overview
This project analyzes Titanic survival rates using **Power BI**. The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/brendan45774/test-file) and contains passenger details such as age, sex, ticket class, and survival status. The objective is to uncover insights about survival probabilities based on these factors.

## 📊 Dataset Description
The dataset includes the following features:
- **PassengerId**: Unique identifier for each passenger.
- **Survived**: 1 = Survived, 0 = Did not survive.
- **Pclass**: Ticket class (1st, 2nd, 3rd).
- **Name**: Passenger’s name.
- **Sex**: Gender of the passenger.
- **Age**: Passenger’s age (missing values replaced with -1).
- **SibSp**: Number of siblings/spouses aboard.
- **Parch**: Number of parents/children aboard.
- **Ticket**: Ticket number.
- **Fare**: Ticket fare.
- **Cabin**: Cabin number (many missing values).
- **Embarked**: Port of embarkation (C, Q, S).

## 🔧 Data Preprocessing Steps
- Created a **Survived_category** column (`Yes/No` based on survival status).
- Filled missing Age values with **-1**.
- Created an **Age_category** column:
  - `0 <= Age < 21` → "Teen"
  - `21 <= Age < 41` → "Young Adult"
  - `41 <= Age < 61` → "Adult"
  - `Age >= 61` → "Old"
  - `Age = -1` → "Null"

## 📈 Power BI Visualizations
### **1. Survival Status by Sex (Stacked Bar Chart)**
- **Observation**: Males had a lower survival rate compared to females.
![image](https://github.com/user-attachments/assets/e95660ce-5fd7-41fc-8694-9f611af2d5df)


### **2. Survival Status by Ticket Class (Pie Chart)**
- **Observation**: First-class passengers had the highest survival rate, while third-class passengers had the lowest.
![image](https://github.com/user-attachments/assets/e5d472c9-8e1f-4866-9a55-bdeaaddc926a)


### **3. Survival Status by Age Category (Clustered Column Chart)**
- **Observation**:
  - Young adults had the highest mortality rate.
  - Older individuals had the lowest survival and non-survival counts.
![image](https://github.com/user-attachments/assets/a8030363-f323-443e-9c04-c67043c433f7)


## 🚀 How to Use This Project
1. Download the Power BI file (`Titanic_Analysis_Report.pbix`).
2. Open it in **Power BI Desktop**.
3. Explore the visualizations and insights.

## 📌 Future Enhancements
- **Add more advanced visualizations**, such as heatmaps and trend analysis.
- **Integrate SQL queries** for additional filtering and data processing.
- **Enhance interactivity** by using slicers and drill-throughs in Power BI.
- **Perform hypothesis testing** to validate statistical significance of observations.

## 📄 License
This project is open-source and free to use for educational purposes.
