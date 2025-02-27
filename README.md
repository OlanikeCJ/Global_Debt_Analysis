
# **Global Debt Analysis (1950 - 2022)**

![Dashboard](https://github.com/OlanikeCJ/Global_Debt_Analysis/blob/main/Images_global_debt/global_debt_dashboard.png?raw=true)

## **Project Description**

The **Global Debt Database (GDD)** is an extensive dataset compiled from various sources to provide insights into the total gross debt of the **nonfinancial sector** (both private and public) across **190 countries**, covering advanced economies, emerging markets, and low-income countries.

- **Data Range:** 1950 - 2022
  
- **Debt Categories:**
  - Government Debt
  - Corporate Debt
  - Household Debt
  - External Debt
    
- **Key Indicators:** Country name, debt type, and annual debt percentages

This dataset allows for an in-depth examination of **global debt trends**, relationships between economic indicators, and financial dynamics over the last seven decades.

---

## Data Cleaning & Transformation

To prepare the dataset for analysis, I performed the following steps:

1. **Pre-Merging Processing:**

   - Unpivoted columns to structure the data properly.

   - Changed data types for consistency.

   - Rounded off debt figures (I used Decimal data type instead of Fixed, which might have impacted precision slightly).

   - Extracted the Year column from the Date column.


2. **Merged Queries:** I combined all five datasets into one **(global\_debt dataset)** using the **Merge Queries as New** feature in Power Query.
   

3. **Post-Merging Processing:**

   - Added a Conditional Column to categorize debt types.

   - Loaded the cleaned dataset into the Power BI model.

4. **Created a Calendar Table** using DAX with a **Year column** and established a **One-to-Many Relationship** with the Year column in the global debt dataset.

5. **Calculations:** Follow [DAX](https://github.com/OlanikeCJ/Global_Debt_Analysis/commit/6263a3b3a4826e79c392809097271b551e9891b7) to view calculations used in this dataset.

## **Insights & Visualizations**

### **1. Global Debt by Category**

> **Insight:** Non-financial corporate debt leads with **67.43%**, followed by **private debt** and **general government debt**.


### **2. Global Debt Trends Over Time**

> **Insight:**

  > - From **1950 - 1959**, global debt averaged **30-32%**.

  > - Between **1960 - 1970**, it **declined to 27-29%**.

  > - From **1976 onward**, debt levels **began rising**, reaching **57.4% by 1993**.

  > - After stabilizing around **57-58% until 2014**, debt increased to **70.62% in 2020**.

  > - In **2021 and 2022**, debt slightly declined to **66-68%**.


### **3. Global Debt Distribution by Category**

> **Insight:** Private debt dominates at **34.8%**, followed closely by General Government Debt at **30.8%**.


### **4. YOY Debt % Change**

> **Insight:** "The chart displays the yearly percentage change in global debt. It highlights periods of rapid debt growth and decline, offering insights into economic shifts and financial stability over time. 


### **5. Global Debt by Country**

> **Insight:** **Cyprus has the highest debt (141.05%)**, while **Brunei Darussalam has the lowest (1.88%)**.

---


**Feel free to explore the dataset and share any insights!** 



