# Data-Driven-Career-Intelligence-and-Salary-Forecasting
Data Mining and Data Warehousing Project


Developed as part of the ICT 333: Data Mining and Data Warehousing course  
**Author:** J.A.D.V JAYASOORIYA

---

[Watch on Google Drive - Explanation Video](https://drive.google.com/drive/folders/1WVfBtlsq6iSWFUPNq-L4yQVLzErsPyhz?usp=sharing)

## Project Summary

This project combines Machine Learning and Business Intelligence to analyze the drivers of professional compensation in the tech industry. By processing over 137,000 records, the system identifies professional clusters and predicts market value based on experience, education, and technical skill density.

---

## Objectives

- Segment the Workforce: Use Unsupervised Learning (K-Means) to categorize professionals into distinct career tiers.
- Predict Compensation: Implement Regression models to forecast salary based on professional profiles.
- Interactive Visualization: Build a high-fidelity Power BI dashboard for real-time market benchmarking.

---

## Dataset

- **Source:** Kaggle – Superstore Sales Dataset [Download the original dataset](https://www.kaggle.com/datasets/nalisha/job-salary-prediction-dataset)

- **Records:** 137,677 Professional Records  
- **Features:** 10+ columns analyzed across four primary dimensions:
  - Professional: Job Title, Years of Experience, Education Level (Bachelor, Master, PhD).
  - Financial: Annual Salary (USD) — used as the primary target for predictive modeling.
  - Technical: Skills Count (numerical representation of technical breadth).
  - Geographic & Logistical: Country/Location, Remote Work Status (Remote, Hybrid, On-Site).

---
## Tools & Technologies

| Tool/Library       | Purpose                            |
|--------------------|------------------------------------|
| **Python (Colab)** | Primary environment for data engineering, mathematical modeling, and executing the ML pipeline   |
| **Pandas & NumPy** | Used for high-volume data manipulation, handling the 137k+ records, and performing statistical audits  |
| **Scikit-learn**   | Core ML library used for K-Means Clustering (segmentation) and Random Forest/Linear Regression (prediction) |
| **Power BI**       | Used to architect the final interactive dashboard, utilizing DAX for custom measures and AI visuals like the Decomposition Tree    |

---


## Project Highlights

### Key Findings (EDA)
- Salary Drivers: Years of experience and technical skill count are the strongest predictors of high compensation.
- Education Impact: Advanced degrees (Masters/PhD) act as a "Price Floor," significantly raising starting salaries.
- The Remote Factor: Remote roles in specialized tech fields now match or exceed on-site pay, showing a shift in global hiring.

### Workforce Segmentation (Clustering)
- Used **RFM (Recency, Frequency, Monetary)** features
- Applied **K-Means clustering** → 3 customer segments:
  - High-value, Mid-value, Low-value customers
- Method: Applied K-Means Clustering to group 137k+ records into 3 professional tiers:
  - Tier 0 (Junior): Entry-level with high growth potential.
  - Tier 1 (Mid-Level): The core market with stable, moderate pay.
  - Tier 2 (Senior Expert): High-value earners with the widest technical breadth.
 
### Predictive Modeling
- The Random Forest model was selected as the champion for its high accuracy in handling complex professional variables:

| Metric             | Linear Regression  |Random Forest (Champion)  |
|--------------------|--------------------|--------------------------|
| R²                 | 0.37               |  0.77                    |
| MAE                | 218.16             |  92.54                   |



### Dashboard Insights (Power BI)
- KPIs: Average Salary, Skill Density, and Regional Pay Benchmarks.
- Visuals: * Radar Charts: To compare "Skill Signatures" between tiers.
    - Decomposition Trees: For AI-driven root-cause analysis of high pay.
    - Global Maps: To identify high-paying geographic hotspots.

---
