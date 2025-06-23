# ☕ ☕️ Cafe Financial Analysis & Insights

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
- **Missing Data:** Used mapping dictionaries and Excel filters to infer missing item names and prices based on other columns
- **Duplicates:** Checked for and found no duplicate rows
- **Dropped/Imputed Columns:** Replaced 'ERROR' and 'UNKNOWN' entries with `NaN`; inferred some missing values via formulas (e.g. Price = Total / Quantity)
- **Feature Engineering:** Created `Month` and `Day Of The Week` columns for further analysis


## 🔍 Key Findings
- **Most sold item by quantity:** Sandwich
- **Highest revenue item:** Salad
<img width="770" alt="Items" src="https://github.com/user-attachments/assets/801ca0ef-d359-403b-8f9d-008cc645b08c" />

- **Peak Month:**
- Maximum in June (7353.0), minimum in February (6644.0).
  
<img width="1013" alt="sales_by_month" src="https://github.com/user-attachments/assets/52039f56-be61-4d3e-86e8-4969174acc16" />

- **Busiest Day:** 
- Maximum sales on Thursday $12401.5, minimum - on Wednesday $11680.5. The difference is small, so the demand is stable.
  
<img width="866" alt="sales_by_day_of_week" src="https://github.com/user-attachments/assets/470467ef-6c29-4e40-ac69-05986afe4f24" />

- **Weekends showed higher average spending**
- **Payment Method:** Payment method was roughly equally distributed across categories, with each method taking roughly 33% of the total
- Payment method and ordering location do not affect the sales volume.
<img width="444" alt="payement_method" src="https://github.com/user-attachments/assets/2082a578-8a76-436f-b6a7-c102b2078ad1" />


## 🤔 Reflections
- **Challenges:** Ambiguous item-price mapping (e.g. $3 could be Cake or Juice, or $4 could be Smoothie or Sandwich)
- **Biases:** Imputations were based on assumptions; might not fully represent real-world behaviors
- **Next Time:** Add a unique transaction ID and explore customer loyalty patterns or time-of-day effects

## ✅ Takeaways & Recommendations

- Salads and Sandwiches and Smoothie generate the most revenue
- Increase inventory of **Sandwiches** and **Salads**
- Focus staffing and marketing efforts on **weekends** and **Thursdays**
- Use **slow months** to experiment with discounts or new menu items
- Potential to increase the average total spending by offering combos
- Consider promotions on days with slightly lower demand (e.g. Wednesday)
- Improve data entry to minimize 'ERROR'/'UNKNOWN' records in the future

## People who collaborated on this project 

- Ibrahima Diallo [LinkedIn](https://www.linkedin.com/in/ibranova/)
- Vincent Perez [LinkedIn](https://www.linkedin.com/in/thevinceperez/)

