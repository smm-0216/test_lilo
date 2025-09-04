# 🚖📊 Problem-Solving Challenge  

This repository contains the solutions to two technical challenge problems. The development was done in **Jupyter Notebooks** to make the exploration, analysis, and explanation of each step more transparent.  

---

## 📂 Repository Structure  

- `sum_numbers.ipynb` → Solution to **Problem 1** (Subset Sum / simplified Knapsack).  
- `taxis.ipynb` → Solution to **Problem 2** (Unit economics metric for NYC taxis).    
- `README.md` → Project documentation.  

---

## 📝 Problem Statements & Solutions  

### ⚡ Question #1: Subset Sum Problem  

**Summary:**  
Given a CSV file where each row contains one big number and up to 12 small numbers, the task is to find the combination of small numbers whose sum is as close as possible to the big number without exceeding it.  

**Implemented Solution:**  
- Notebook: `sum_numbers.ipynb`  
- Algorithm: a variation of the **Knapsack Problem (0/1)** optimized for this context.  
- Input: CSV rows in the format `[big_number, small_numbers...]`.  
- Output: For each row, the selected subset of small numbers and their sum.  

**Advantages:**  
- Efficiently handles multiple combinations.  
- Scales well.

**Limitations:**  
- Does not support negative numbers or decimals (requires preprocessing or transformations).  

---

### 🚕 Question #2: NYC Taxi Unit-Economics  

**Summary:**  
Taxi pricing often does not reflect the true cost of each trip. Using NYC Taxi Trip Data, the tasks are:  
1. Design and calculate a **unit-economic metric** (e.g., per mile or per minute).  
2. Analyze how this metric varies across different **Rate Codes**.  

**Implemented Solution:**  
- Notebook: `taxis.ipynb`  
- Methodology:  
  - Defined a metric based on **average cost per mile**.  
  - Processed multiple months of trip data (Parquet format).  
  - Produced tables and visualizations by Rate Code.  

**Advantages:**  
- Simple and intuitive metric, easy to compare across categories.  
- Highlights differences in effective pricing between Rate Codes.  

**Limitations:**  
- Only considers distance, not time or additional operational costs.  
- Results may be affected by outliers in the dataset.  

**Next Iteration Proposal:**  
- Extend the metric to a multivariable function including both **time and distance** (optimization).  
- Add sensitivity analysis to propose potential pricing adjustments.  

---

## ⚙️ Requirements  

- Python 3.10+  
- Jupyter Notebook  

Quick installation:  

```bash
pip install -r requirements.txt