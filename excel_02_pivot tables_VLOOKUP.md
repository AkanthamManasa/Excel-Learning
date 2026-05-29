# Date: May 29, 2026
# Excel Topic Names — Pivot Tables and VLOOKUP


---

## What I Learned Today
(2-3 lines in your own words)

---

## Pivot Tables

### What is a Pivot Table
Summarises large data by grouping instantly.
Exactly like SQL GROUP BY.

### How to Create
Insert tab → PivotTable → OK →
Drag fields into Rows, Columns, Values boxes

### 3 Pivot Tables I Built
1. Sales and Profit by Category
   → Category in Rows, Sales + Profit in Values

2. Sales by Region
   → Region in Rows, Sales + Quantity in Values

3. Category by Region cross-tab
   → Category in Rows, Region in Columns, Sales in Values

### SQL vs Pivot Table
| SQL | Excel Pivot Table |
|---|---|
| GROUP BY category | Category in Rows box |
| SUM(sales) | Sales in Values box |
| GROUP BY category, region | Category in Rows + Region in Columns |

---

## VLOOKUP

### What it does
Searches for a value in a column.
Returns matching data from another column.
Like SQL JOIN — connects two tables.

### Syntax
=VLOOKUP(find_this, look_in_this_range, return_column_number, FALSE)

### My Example
=VLOOKUP(B2,$J$2:$K$4,2,FALSE)
Finds category name → returns its tax rate

### What $ Signs Do
Locks the lookup table range when copying formula down.
Without $ the range shifts and gives wrong results.

---

### SQL Equivalent
SELECT o.category, t.tax_rate
FROM orders AS o
INNER JOIN tax_table AS t
ON o.category = t.category

---

## What Confused Me Today
(write honestly)

---

## How I Solved It

---

## Practice File
See: excel_01_basics_functions.xlsx
See: pivot_table_01.png
See: vlookup_01.png


---

## Next Excel Topic
mini project using pivot table and charts,Conditional formatting, more chart types