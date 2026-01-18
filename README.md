# DT/AI VR Training — Survey Data Analysis (2024 vs 2025)

This repository contains the code used to analyze post-experience survey data from two cohorts who completed a semiconductor virtual simulation experience:

- **2024 cohort:** VR-only simulation (n = 29)
- **2025 cohort:** AI-enhanced VR simulation with an AI tutoring agent (n = 37)

The analysis supports the manuscript’s Results and Discussion section, including:
1) descriptive summaries of learner perceptions, 
2) the engagement–interest relationship within the 2025 cohort, and  
3) a standardized (within-cohort) comparison of engagement–interest trends across 2024 and 2025.

---

## What the analysis does

### 1) Data cleaning and preparation
- Loads survey exports (CSV) for each cohort.
- Ensures consistent Likert-scale coding (1–5).
- Handles missing values and basic sanity checks.

### 2) Descriptive statistics 
For the **2025 AI-enhanced cohort**, the script computes and visualizes:
- mean and standard deviation for core survey items related to AI-in-VR instructional value
- distribution summaries (% ratings ≥ 4, % = 5, % ≤ 2)

### 3) Engagement → future interest 
For **2025**, the analysis:
- bins learners by self-reported engagement level
- plots mean future interest by engagement bin with **standard error** bars
- runs regression modeling to quantify the strength of association between engagement and future interest

### 4) Cross-cohort standardized comparison 
The analysis avoids direct comparison of raw Likert values and instead:
- standardizes interest within each cohort (z-scoring or mean-centering)
- fits standardized regressions within each cohort
- compares effect sizes and overall engagement–interest patterns across years

---

