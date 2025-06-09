# 📊 ADR Report Pattern Analysis

This project analyzes patterns in Adverse Drug Reaction (ADR) reports submitted over a specific time frame. By using statistical and visualization tools, we uncover insights into drug safety signals, reporting trends, and the distribution of ADRs by drug class, demographics, and geography.

---

## 🧠 Objective

To explore and visualize adverse drug reaction data in order to:
- Identify trends in ADR reporting
- Examine distribution by drug, age group, gender, and region
- Detect potential safety signals that may need further investigation

---

## 🗂️ Dataset

- Source: Public pharmacovigilance or FAERS dataset (can be anonymized or synthetic if required)
- Format: CSV
- Columns include:
  - Report ID
  - Patient Age, Gender
  - Suspected Drug
  - Reaction Description
  - Report Date
  - Outcome (e.g., hospitalization, recovery, death)
  - Country / Region

Note: A sample dataset is included in the /data folder.

---

## 🛠️ Tools & Libraries

- Python 3.9+
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- jupyter notebook

---

## 🔍 Key Steps

1. Data Cleaning:
   - Handling missing values
   - Standardizing drug names
   - Parsing dates

2. Exploratory Data Analysis (EDA):
   - ADR counts by year/month
   - ADRs by age group and gender
   - Top 10 drugs associated with ADRs
   - Geographical distribution of reports

3. Visualization:
   - Bar charts and heatmaps for frequency analysis
   - Line plots for time-series trends
   - Pie charts for outcome distributions

4. Statistical Insights:
   - Hypothesis testing (e.g., gender differences in ADR frequency)
   - Signal detection via proportion analysis

---

## 📈 Sample Visualizations

- 📌 ADR Trend Over Time
- 🧪 Top 10 Suspected Drugs
- 🗺️ Heatmap of ADRs by Country
- 🚻 Gender-wise ADR Distribution

(All charts available in the /outputs folder and notebooks)

---

## 📌 Findings (Example)

- A steady increase in ADR reporting over 5 years
- Female patients report slightly more ADRs compared to males
- Certain antibiotics and NSAIDs are repeatedly flagged
- Hospitalizations are most common in age groups over 60

(Findings will vary depending on dataset)

---

## 📎 Folder Structure

