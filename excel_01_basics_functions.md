# Date: May 28, 2026
# Excel Topic Names — Basics and Functions

---

## What I Learned Today
 I learnt how to navigate in the excel worksheets, got to know about how data is entered , sorted and filtered.

---

## Concepts Covered

### Excel Basics
**What is a Cell:**
Each box in Excel is called a cell.
Address = column letter + row number. Example: A1, B3, D12

**What is a Worksheet:**
The full grid of rows and columns inside Excel.

---

### Basic Functions

| Function | Formula          |  What It Does      | SQL Equivalent |
|----------|------------------|--------------------|----------------|
| SUM      | =SUM(D2:D13)     | Adds all values    |     SUM()      |
| AVERAGE  | =AVERAGE(D2:D13) | Calculates average |     AVG()      |
| COUNT    | =COUNT(D2:D13)   | Counts rows        |     COUNT()    |
| MAX      | =MAX(D2:D13)     | Finds highest value|     MAX()      |
| MIN      | =MIN(D2:D13)     | Finds lowest value |     MIN()      |

**My result from practice data:**
- Total Sales: 58950
- Average Sales: 4912.5
- Count: 12
- Highest Sale: 12000
- Lowest Sale: 800

---

### Sorting
Arranges rows by a column value.
Steps: Data tab → Sort → choose column → Largest to Smallest → OK

SQL equivalent:
ORDER BY sales DESC

---

### Filtering
Shows only rows matching a condition.
Steps: Data tab → Filter → click dropdown arrow → select value → OK

SQL equivalent:
WHERE category = 'Technology'

---

### IF Formula
Checks a condition and returns different values.

Syntax:
=IF(condition, value_if_true, value_if_false)

My example:
=IF(D2>5000,"High","Low")

SQL equivalent:
CASE WHEN sales > 5000 THEN 'High' ELSE 'Low' END

---

## SQL vs Excel Comparison Table

|           SQL         |              Excel                |
|-----------------------|-----------------------------------|
| SELECT SUM(sales)     | =SUM(D2:D13)                      |
| SELECT AVG(sales)     | =AVERAGE(D2:D13)                  |
| ORDER BY sales DESC   | Data → Sort → Largest to Smallest |
| WHERE category='Tech' | Data → Filter → select category   |
| CASE WHEN sales>5000  | =IF(D2>5000,"High","Low")         |

---

## What Confused Me Today
Didn't got that much of confusion.

---

## Practice File
See: 
practice: excel_01_basics_functions.xlsx
Screenshots: excel_functions.png and excel_if_formula.png

---

## Tomorrow's Topics
- Pivot Tables
- VLOOKUP