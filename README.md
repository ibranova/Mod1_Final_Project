# Cafe Financial Analysis & Insights

## Project Overview
This project was conducted to help a small café owner better understand their sales trends. By analyzing transaction-level data, we aimed to identify peak sales times, best-selling items, and customer behavior across the week and year. The insights are intended to guide smarter inventory and marketing decisions. 

## 🧠 Business Problem & Stakeholder

The café owner wanted to answer several key questions:
- **What are the peak sales months?**
- **Are weekends busier than weekdays?**
- **Which products generate the most revenue?**
- **How reliable is the dataset?**
The primary stakeholder is the café owner, who can utilize these insights to enhance profitability and operational efficiency.

## 🧹 Data Cleaning Choices & Justification
- **Data Type Corrections:** Converted `Transaction Date` to datetime; `Price Per Unit`, `Quantity`, and `Total Spent` to numeric
- **Missing Data:** Used mapping dictionaries to infer missing item names and prices based on other columns; dropped rows with <5% missing values
- **Duplicates:** Checked for and found no duplicate rows
- **Dropped/Imputed Columns:** Replaced 'ERROR' and 'UNKNOWN' entries with `NaN`; inferred some missing values via formulas (e.g. Price = Total / Quantity)

## 🔍 Key Findings
- **Most sold item by quantity:** Sandwich
- **Highest revenue item:** Salad
- **Peak Month:** June
- **Busiest Day:** Thursday
- **Weekends showed higher average spending**
- **Feature Engineering:** Created `Month` and `Day Of The Week` columns for temporal analysis
- **Payement Methode:** Payment method was roughly equally distributed across categories, with roughly each method taking 33% of the total

## 🤔 Reflections
- **Challenges:** Ambiguous item-price mapping (e.g. $3 could be Cake or Juice, or $4 could be Smoothie or Sandwich)
- **Biases:** Imputations were based on assumptions; might not fully represent real-world behaviors
- **Next Time:** Add a unique transaction ID and explore customer loyalty patterns or time-of-day effects

## ✅ Takeaways & Recommendations

- Increase inventory of **Sandwiches** and **Salads**
- Focus staffing and marketing efforts on **weekends** and **Thursdays**
- Use **slow months** to experiment with discounts or new menu items
- Improve data entry to minimize 'ERROR'/'UNKNOWN' records in the future

## People who collaborated on this project 

- Ibrahima Diallo [LinkedIn](https://www.linkedin.com/in/ibranova/)
- Vincent Perez [LinkedIn](https://www.linkedin.com/in/thevinceperez/)

