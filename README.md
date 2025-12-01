#  Credit Banking Analysis Project

This project contains a complete analysis of credit banking data using Python and Jupyter Notebook. The goal is to perform detailed data cleaning, transformation, aggregation, and financial calculations using real-world banking datasets such as **Credit banking data**, **spend data**, and **repayment data**.

The notebook covers **20 structured tasks**, including data loading, grouping, merging, date/time processing, visual analysis, and profit/penalty calculations.



## Technologies Used

* Python
* Jupyter Notebook
* pandas
* NumPy
* Matplotlib / Seaborn


## Dataset Description

The project works with 3 datasets:

* **Credit Banking_Project1.csv** → Customer info (age, segment, etc.)
* **spend.csv** → Monthly spending transactions
* **repayment.csv** → Customer repayment data

Each dataset is cleaned and transformed before performing analysis.

---

#  **TASKS COMPLETED IN THIS PROJECT**

Below is the exact set of problems solved in the notebook.

---

## 🔹 **1. Data Loading and Basic Operations**

1. Loaded `Credit Banking_Project1.csv` and displayed first 5 rows.
2. Loaded `spend.csv` and `repayment.csv`, renamed columns, and displayed first 10 rows.
3. Calculated mean age of customers **over 18**, and replaced any age below 18 with this mean.

---

## 🔹 **2. Grouping and Aggregation**

4. Calculated **total spending amount per customer**.
5. Calculated total repayment per customer and displayed **top 5 customers**.
6. Merged total spending and total repayment into a **single dataframe**.

---

## 🔹 **3. Conditional Filtering & Calculations**

7. Filtered customers who **repaid more than they spent** and calculated their **surplus**.
8. For those customers, calculated **return with 2% bonus** on surplus.

---

## 🔹 **4. Date & Time Operations**

9. Converted the 'Month' column of `spend` to datetime, extracted month+year.
10. Grouped spend data by **Customer + Month-Year** to compute **monthly spending**.

---

## 🔹 **5. Sorting & Ranking**

11. Displayed **top 10 customers** by total spending.
12. Grouped customers by **segment** and calculated total spending sorted descending.

---

## 🔹 **6. Merging and Joining**

13. Merged segment information with spending to analyze **segment-level patterns**.
14. Merged age-group information with spending and calculated **total spending per age group**.

---

## 🔹 **7. Mapping & Categorization**

15. Created a dictionary mapping spending types (e.g., "FOOD", "AIR TICKET") to categories like "Needs", "Travel", etc.
16. Added a new **Category** column to spend data and calculated total spending by category.



# Key Outputs

* Total spending per customer
* Total repayment per customer
* Surplus and return
* Monthly spending trends
* Category-wise spending
* Segment-wise spending
* Age-group spending
* Difference and penalty calculations
* Monthly profit summary

