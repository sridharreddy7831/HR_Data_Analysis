# HR Employee Attrition Analysis

## Project Overview

This project focuses on analyzing employee attrition data from a Human Resources dataset to identify key factors contributing to employees leaving the organization. Understanding these drivers is crucial for HR departments to develop effective retention strategies and improve overall employee satisfaction and stability.

## Dataset

The analysis is performed on the `HR-Employee-Attrition.csv` dataset. This dataset contains a variety of features including employee demographics, job role, salary, satisfaction levels, and work-life balance, along with an 'Attrition' column indicating whether an employee left the company.

## Project Goal

The primary goal of this project is to:
* Perform a thorough data analysis to uncover patterns and relationships within the HR data.
* Identify significant attributes correlated with employee attrition.
* Provide actionable insights that HR can use to reduce turnover.

## Analysis Steps Performed

The project follows a standard data analysis pipeline:

1.  **Data Collection & Initial Understanding:**
    * Loading the dataset into a Pandas DataFrame.
    * Initial inspection of data structure, column types, and basic statistics.
    * Checking for missing values and duplicate records.

2.  **Data Cleaning & Preprocessing:**
    * Converting the 'Attrition' column from categorical ('Yes'/'No') to numerical (1/0) for analytical purposes.
    * Renaming columns for clarity (e.g., 'EmployeeNumber' to 'EmployeeID').
    * Checking for unique values and standardizing text data (e.g., stripping whitespace).
    * Removing redundant columns (e.g., 'EmployeeCount' and 'StandardHours', which were constant).

3.  **Exploratory Data Analysis (EDA):**
    * **Overall Attrition Rate:** Calculating the company-wide attrition rate.
    * **Categorical Variable Analysis:** Analyzing attrition rates across various categorical features like Department, Job Role, Gender, Marital Status, Education Field, Business Travel, and Overtime.
    * **Numerical Variable Analysis:** Exploring the distribution and relationship of numerical features such as Age, Monthly Income, Years at Company, Total Working Years, Distance From Home, Job Satisfaction, Environment Satisfaction, Relationship Satisfaction, and Work-Life Balance with attrition using visualizations (KDE plots, Box plots).

## Key Insights from EDA (So Far)

Based on the Exploratory Data Analysis, some significant patterns and potential drivers of attrition have been identified:

* **Overall Attrition:** [Insert the overall attrition rate you calculated, e.g., "Approximately 16% of employees have attrited."]
* **Department:** The **Sales** and **Human Resources** departments tend to have higher attrition rates compared to Research & Development.
* **Job Role:** **Sales Representatives** and **Laboratory Technicians** show notably higher attrition.
* **Marital Status:** **Single** employees have a significantly higher attrition rate than Married or Divorced employees.
* **Education Field:** Employees with **Life Sciences** and **Technical Degree** backgrounds exhibit higher attrition compared to other fields.
* **Business Travel:** Employees who **Travel Frequently** show the highest attrition rates, followed by those who travel rarely, while Non-Travelers have the lowest attrition.
* **Overtime:** Employees who work **OverTime** have a substantially higher attrition rate than those who do not. This is a very strong indicator.
* **Age:** Younger employees (early career stage) show a higher tendency to attrite.
* **Monthly Income:** Employees with **lower monthly incomes** tend to have higher attrition. The median monthly income for attrited employees is noticeably lower than for non-attrited employees.
* **Years at Company & Total Working Years:** Employees with **fewer years at the company** and **fewer total working years** are more likely to attrite. This suggests issues with onboarding, early career development, or immediate role fit.
* **Satisfaction Levels:** Lower levels of **Job Satisfaction**, **Environment Satisfaction**, **Relationship Satisfaction**, and **Work-Life Balance** are generally associated with higher attrition.

## Technologies Used

* **Python:** Programming Language
* **Pandas:** Data manipulation and analysis
* **Matplotlib:** Data visualization
* **Seaborn:** Enhanced statistical data visualization
* **Jupyter Notebook:** Interactive computing environment for analysis and presentation

## How to Run the Analysis

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/sridharreddy7831/HR_Data_Analysis.git](https://github.com/sridharreddy7831/HR_Data_Analysis.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd HR_Data_Analysis
    ```
3.  **Ensure you have the necessary libraries installed:**
    ```bash
    pip install pandas matplotlib seaborn
    ```
4.  **Open the Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
5.  Open the `HR_Data_Analysis.ipynb` (or similar name) notebook and run the cells sequentially.

## Future Enhancements (Next Steps)

* **Further EDA:** Explore correlations between numerical features.
* **Feature Engineering:** Create new features that might be insightful.
* **Hypothesis Testing:** Statistically validate observed patterns.
* **Predictive Modeling:** Build machine learning models to predict attrition.
* **Dashboard Creation:** Visualize key insights in an interactive dashboard (e.g., using Power BI or Tableau).
* **Business Recommendations:** Translate findings into concrete, actionable strategies for HR.

---

Feel free to customize the "Key Insights" section with the specific values and more detailed observations you made during your EDA, as you have the exact output from your notebook.

Let me know if you'd like any adjustments or help with the next steps (SQL-like operations, Dashboarding, Business Insights)!