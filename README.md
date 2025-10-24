# Optimization Project 2 — Marketing Budget Allocation

This repository contains all deliverables for the **Marketing Budget Allocation** project.  
The objective is to build and compare optimization models (linear and mixed-integer) to determine optimal marketing-budget allocations across multiple advertising media.

---

## Project Components

| Part | Summary of Requirements | Notebook / Code Link |
|------|--------------------------|----------------------|
| **1 – 3. Linear Programming Model (Formulation and Solution)** | Formulate and solve the initial marketing-budget allocation using `roi_company1.csv`. ROI is non-increasing, so the total return is concave. Define continuous tier variables, objective (maximize Σ ROI × Investment), and constraints: total budget ≤ 10 M$, per-platform ≤ 3 M$, Print + TV ≤ Facebook + Email, and Social ≥ 2×(SEO + AdWords). | [Open proj_2_1-3.ipynb in Colab](https://colab.research.google.com/github/AHMerrill/optimization-project-2/blob/main/proj_2_1-3.ipynb) |
| **4. Second ROI Data (Mixed Integer Formulation)** | Use `roi_company2.csv`, where ROI values are **not** non-increasing. Reformulate as a **mixed-integer program** with binary tier-activation variables to preserve correct piecewise behavior and re-solve under the same constraints. | _TBD (link to proj_2_4.ipynb or .py)_ |
| **5. Allocation Comparison and Objective Impact** | Compare allocations from Parts 3 and 4. Compute how much lower the total return becomes when each allocation is applied to the other ROI set. Discuss the managerial usefulness of the $3 M per-platform constraint. | _TBD (link to proj_2_5.ipynb)_ |
| **6. Minimum Spend Rule** | Introduce minimum-investment thresholds from `min_amount.csv`. Modify the mixed-integer model so each medium is either not invested in or invested at least its minimum amount. Solve again using `roi_company2.csv`. | _TBD (link to proj_2_6.ipynb)_ |
| **7. Reinvestment Over Time** | Allow reinvestment of **50 % of returns** each month: new budget = 10 M + 10 M × ROI × 0.5. Use `roi_monthly.csv` to find optimal allocations month-by-month while retaining previous constraints. | _TBD (link to proj_2_7.ipynb)_ |
| **8. Budget Stability Analysis** | Define stability: monthly change ≤ 1 M per platform. Check whether the allocation from Part 7 meets this criterion and, if not, describe how to model it with additional constraints. | _TBD (link to proj_2_8.ipynb)_ |
| **9. Final Report and Submission** | Compile a well-written PDF report summarizing all analyses, graphs, and code snippets. Ensure the first code cell in each notebook reads the appropriate CSV with `pd.read_csv()`. Code must be generalizable for grading on new data. | _Report PDF (TBD)_ |

---

## Deliverables
- One PDF report summarizing methodology, results, and graphs  
- One Python code file or .ipynb per part (Parts 1 – 8)  
- All CSV inputs referenced dynamically  

---

## Completed By
**Team Members:**  
- Hardy Smith
- Mihir Jeshurun Gandham
- Prisca Varner
- Zan Merrill  

**Course:** Optimization / Integer Programming — McCombs School of Business  
**Instructor:** Dan Mitchell

---

## Date
**Completed:** October 2025  

---

**Repository:** [AHMerrill/optimization-project-2](https://github.com/AHMerrill/optimization-project-2)
