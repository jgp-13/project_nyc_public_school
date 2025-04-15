# 🧠 Analysis of SAT Scores in New York City Public Schools

This project presents a concise data-driven analysis of SAT score distributions across public secondary schools in New York City. It aims to highlight top-performing schools and uncover disparities in academic outcomes across different boroughs.

> **Note**: This analysis was conducted as part of a [DataCamp](https://www.datacamp.com/) project.

---

## 🧹 Data Preparation

To enable accurate analysis, the following data preparation steps were performed:

- A dataset containing SAT scores and school information was loaded.
- A composite variable `total_SAT` was engineered, representing the sum of:
  - `average_math`
  - `average_reading`
  - `average_writing`
- Values were rounded to two decimal places for clarity in reporting.

---

## 📊 Analytical Workflow

### 1. 📐 High-Scoring Schools in Mathematics
- Schools with an average SAT math score of **640 or above** (80% of the maximum score) were identified.
- Results were stored in `best_math_schools`, including:
  - `school_name`
  - `average_math`
- Sorted in descending order by math score to highlight excellence in mathematics.

### 2. 🏅 Top 10 Schools by Overall SAT Performance
- A total SAT score was calculated by **summing** the three subject areas.
- The top 10 schools were extracted and stored in `top_10_schools`, showing:
  - `school_name`
  - `total_SAT`

### 3. 🌆 Borough Variability in SAT Outcomes
- The standard deviation of total SAT scores was computed for each borough.
- The borough with the **widest variation in performance** was identified.
- Results were summarised in `largest_std_dev`, including:
  - `borough`
  - `num_schools`
  - `average_SAT`
  - `std_SAT`

---

## 📌 Summary of Insights

- A small number of schools consistently outperform in mathematics, scoring near the maximum.
- The top overall performers were identified based on combined SAT results.
- One borough demonstrated a significantly higher variation in SAT scores, suggesting disparities in educational quality and resource allocation.

---

This analysis serves as a foundation for deeper exploration into factors affecting academic outcomes and helps inform discussions around equity in education across New York City.
