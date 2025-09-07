# Black Friday Sales EDA

This repository contains an **Exploratory Data Analysis (EDA)** on the **Black Friday Sales dataset**. The analysis aims to understand customer behavior, spending patterns, and key trends in sales, along with feature engineering and visualizations.

---

## Dataset

- **Source:** Black Friday dataset (train.csv)
- **Columns included:**
  - `User_ID`: Unique identifier of the customer
  - `Product_ID`: Product identifier
  - `Gender`: Gender of the customer
  - `Age`: Age group of the customer
  - `Occupation`: Occupation code of the customer
  - `City_Category`: Category of the city (A, B, C)
  - `Stay_In_Current_City_Years`: Number of years the customer has stayed in the current city
  - `Marital_Status`: Marital status of the customer
  - `Product_Category_1,2,3`: Product categories
  - `Purchase`: Purchase amount

---

## Project Structure

.
├── data/ # Dataset files
│ └── train.csv
├── notebooks/ # Jupyter notebook for analysis
│ └── BlackFriday_EDA.ipynb
├── plots/ # Folder containing saved plots
│ ├── univariate/
│ ├── bivariate/
│ ├── multivariate/
│ └── heatmaps/
└── README.md

---

## Libraries Used

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`

---

## Steps Performed in the EDA

1. **Data Cleaning**
   - Dropped irrelevant columns (e.g., `Product_ID`)
   - Handled missing values in `Product_Category_2` and `Product_Category_3`
   - Converted `Age` and `Stay_In_Current_City_Years` into numerical format

2. **Feature Engineering**
   - Created `Age_Group` (Teen, Young Adult, Adult, Senior)
   - Calculated `Avg_Purchase_Per_Customer`

3. **Univariate Analysis**
   - Distribution of Purchase Amount
   - Distribution of Age Groups
   - Insights from histograms and pie charts

4. **Bivariate Analysis**
   - Purchase vs Gender
   - Purchase vs Age Group
   - Purchase vs Occupation
   - Purchase distribution across Age Groups

5. **Multivariate Analysis**
   - Purchase vs Age, Gender, City Category
   - Correlation heatmap of numerical features

6. **Visualizations**
   - All plots saved in the `plots` folder for reference

---

## Key Insights

- Adults are the most frequent buyers; Teens are the least.
- Men purchase slightly more than women on average.
- City Category C customers tend to spend more on average.
- Most purchases fall between **₹5,000 - ₹10,000**.
- No significant impact of Occupation or Age Group on purchase amount.
