# Healthcare_US_analysis

# 🏥 Healthcare Data Analysis & Visualization

This project explores and analyzes a comprehensive patient-level healthcare dataset using Python and Power BI. It uncovers insights into patient demographics, treatment costs, medical outcomes, and institutional performance using both statistical techniques and interactive dashboards.

---

## 📊 Power BI Dashboard Overview

The Power BI dashboard includes interactive visuals for:

- Units admitted by age group and gender
- Billing amount trends by condition, hospital, and insurance provider
- Test results breakdown by gender and admission type
- Medication usage by condition and hospital
- Hospital locations plotted by latitude/longitude

👉 **Explore the Dashboard Screenshot or .pbix file in the repository**

---

## 📌 Key Findings & Insights

### ✅ 1. Patient Demographics Are Skewed Toward Middle-Aged Groups

- Majority of patients fall in the **30–59 age range**.
- **Gender is balanced**, but test outcomes vary by gender.
- **Blood types** are evenly distributed and not linked to outcomes.

📊 *Charts*: Age group bar chart, gender breakdown, blood type pie chart

---

### ✅ 2. Medical Conditions Do Not Drive Cost Differences

- **Billing amounts are flat** across all conditions.
- Mean, median, and IQR differ by **<1%**.
- Implies **flat-rate billing** or non-condition-based pricing.

📉 *Conclusion*: Medical condition **does not predict cost**.

---

### ✅ 3. Hospitals Show Small but Notable Cost Variation

- Mean billing ranges from **$25,000–$26,000**.
- Wide standard deviation (~$14k), outliers range from **$9 to $52,000**.
- Some hospitals show **more abnormal test results** than others.

📊 *Charts*: Boxplot of billing, stacked bar of test results per hospital

---

### ✅ 4. No Cost Difference Between Admission Types

- **ANOVA and t-tests show no significant cost differences** across Emergency, Elective, or Urgent admissions.
- Emergency stays tend to be **longer**, which weakly affects cost.

📉 *Test*:  
`t = -0.75, p = 0.4555` — no significant difference

---

### ✅ 5. Test Results Significantly Differ by Gender

- **Females: 60% abnormal**, others: 50% abnormal.
- Confirmed by **Chi-square** and **Logistic Regression**.

📉 *Statistical Results*:  
`Chi² = 645.68, p < 0.001` ✅  
**Conclusion**: Test outcomes are **not gender-neutral**

---

### ✅ 6. Most Common Medications Are Consistent Across Conditions

- Medications are **reliably matched to conditions**.
- Slight variations across hospitals hint at **protocol differences**.

📊 *Visuals*: Bar chart of top meds per condition, heatmap by hospital

---

### ✅ 7. Insurance Provider Slightly Affects Cost, Not Outcomes

- Billing differences across insurers are **~$1,000**.
- **Test results are similar** regardless of insurance.

📉 *Visuals*: Billing by insurance provider, test results stacked bar chart

---

### ✅ 8. Geographic Distribution Is Uniform — No Strong Regional Trends

- Hospital locations vary, but **no clear regional pattern** exists for cost or outcomes.
- No spatial clustering detected.

🗺️ *Visual*: Hospital map with outcomes and billing color-coded

---

## 🛠️ Tools & Technologies

- Python: `pandas`, `matplotlib`, `seaborn`, `statsmodels`
- Power BI: Interactive dashboards with filters, slicers, and custom tooltips
- Jupyter Notebook for EDA, visualizations, and statistical tests

---

## 📂 Repository Contents

- `notebooks`: Python analysis and EDA
- `dashboard`: Power BI `.pbix` file and screenshots
- `README.md`: Project overview and key results
- `report.pdf`: Academic report version of this analysis

---

## 📌 Conclusion

This project shows how well-structured healthcare datasets can be analyzed to generate meaningful insights for hospitals and decision-makers. Although treatment cost is surprisingly uniform across many variables, outcomes and protocols differ by gender and location — with real implications for healthcare equality and efficiency.

---

