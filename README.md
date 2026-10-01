# Titanic Power BI Analysis 🚢📊

A Power BI data analysis project based on the Titanic dataset.

## 📌 Project Overview

This project analyzes Titanic passenger data using **Microsoft Power BI**.

The dashboard provides insights into passenger demographics, survival, passenger class, age groups, and fare distribution.

### Key Questions

- How many passengers were on the Titanic?
- How many passengers survived?
- What was the survival rate?
- How did survival vary by gender?
- How did passenger class affect survival?
- What was the average fare?
- What were the minimum and maximum fares?
- How were passengers distributed across different age groups?

## 🛠️ Tools & Technologies

- Microsoft Power BI
- Power Query
- DAX
- Data Cleaning
- Data Analysis
- Data Visualization
- Titanic Dataset

## 📊 Key KPIs

The dashboard includes the following KPIs:

- **Total Passengers**
- **Total Survivors**
- **Survival Rate**
- **Average Fare**
- **Maximum Fare**
- **Minimum Fare**

## 📈 Dashboard Visualizations

The dashboard contains visualizations for:

- Survival Status
- Survival by Gender
- Survival by Passenger Class
- Passenger Distribution by Age Group
- Fare Analysis
- Passenger Class Distribution
- Passenger Demographics

Interactive filters and slicers are used to explore the data.

## 🧹 Data Cleaning

The dataset was cleaned and prepared before creating the dashboard.

### Data preparation steps:

1. Handling missing values
2. Checking and correcting data types
3. Creating calculated columns
4. Creating age groups
5. Creating survival-related fields
6. Creating DAX measures
7. Building KPIs
8. Creating interactive visualizations

## 🧮 DAX Measures

### Total Passengers

```DAX
Total Passengers = COUNTROWS(Titanic)
```

### Total Survivors

```DAX
Total Survivors =
CALCULATE(
    COUNTROWS(Titanic),
    Titanic[Survived] = 1
)
```

### Survival Rate

```DAX
Survival Rate =
DIVIDE(
    [Total Survivors],
    [Total Passengers],
    0
)
```

### Average Fare

```DAX
Average Fare = AVERAGE(Titanic[Fare])
```

### Maximum Fare

```DAX
Maximum Fare = MAX(Titanic[Fare])
```

### Minimum Fare

```DAX
Minimum Fare = MIN(Titanic[Fare])
```

## 📁 Project Structure

```text
Titanic-PowerBI-Analysis/
│
├── Titanic_PowerBI_Analysis.pbix
├── README.md
└── .gitignore
```

## 🚀 How to Use

1. Download or clone this repository.
2. Install **Microsoft Power BI Desktop**.
3. Open `Titanic_PowerBI_Analysis.pbix`.
4. Refresh the data if required.
5. Explore the dashboard using the available filters and visuals.

## 🎯 Project Objective

The objective of this project is to demonstrate practical skills in:

- Data Cleaning
- Data Analysis
- Power Query
- DAX
- KPI Creation
- Power BI Dashboard Development
- Data Visualization
- Interactive Reporting

## 👨‍💻 Author

**Atharva Kadu**

BSc Computer Science | Data Science & Data Analytics

## ⭐ Project

If you find this project useful, consider giving the repository a ⭐.
