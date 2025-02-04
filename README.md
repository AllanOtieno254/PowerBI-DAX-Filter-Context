# 📊 DAX Filter Context in Power BI
![YTD Sales](https://github.com/user-attachments/assets/5f4de99e-1284-454f-8252-5a3b8f75f0c7)

## 🔍 Overview
This repository contains a Power BI project that explores **DAX Filter Context**, a crucial concept in DAX calculations. The project focuses on **Bank Loan Analysis**, demonstrating how different filter contexts affect DAX formulas.

### 🏆 Key Objectives:
- Understand how **row, column, and visual-level filters** interact.
- Analyze **DAX functions like CALCULATE, FILTER, ALL, and REMOVEFILTERS**.
- Demonstrate real-world **Bank Loan Analysis** using Power BI.

---


### 🛠️ DAX Functions Used
1️⃣ CALCULATE
Modifies filter context for an expression.

### DAX
Copy
Edit
Total Sales = CALCULATE(SUM(Sales[Amount]), Sales[Region] = "East")
### 2️⃣ FILTER
Creates a table based on conditions.

DAX
Copy
Edit
FilteredData = FILTER(Sales, Sales[Amount] > 1000)
### 3️⃣ ALL
Ignores existing filters.

DAX
Copy
Edit
Total Sales (All Regions) = CALCULATE(SUM(Sales[Amount]), ALL(Sales[Region]))
### 4️⃣ REMOVEFILTERS
Removes all filters from a table or column.

DAX
Copy
Edit
Total Sales Without Filters = CALCULATE(SUM(Sales[Amount]), REMOVEFILTERS(Sales))
![duplicate sales by country](https://github.com/user-attachments/assets/f3fcd202-5e67-4380-b748-d4638389ff01)
![Sales by country](https://github.com/user-attachments/assets/5c69cff8-db77-418a-8061-0889478992b8)


## 🚀 Getting Started

### 📥 Clone the repository:
```sh
git clone https://github.com/your-username/DAX-Filter-Context.git
