# 📊 ADR Report Pattern Analysis

This project analyzes patterns in Adverse Drug Reaction (ADR) reports submitted over a specific time frame. By using statistical and visualization tools, we uncover insights into drug safety signals, reporting trends, and the distribution of ADRs by drug class, demographics, and geography.

---


- [Objective](#objective)
- [Dataset](#dataset)
- [Tools and Libraries](#tools-and-libraries)
- [Key Steps](#key-steps)
- [Sample Visualizations](#sample-visualizations)
- [Findings](#findings)
- [Folder Structure](#folder-structure)

---

## Objective

To explore and visualize adverse drug reaction data in order to:
- Identify trends in ADR reporting
- Examine distribution by drug, age group, gender, and region
- Detect potential safety signals that may need further investigation

---

## Dataset

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

## Tools and Libraries

- Python 3.9+
- pandas
- numpy
- matplotlib
- seaborn
- plotly
- jupyter notebook

---

## Key Steps

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

## Sample Visualizations

- 📌 ADR Trend Over Time
 ![Top Drugs](outputs/adr_reports_per_year.png)

- 🧪 Top 10 Suspected Drugs
![Top Drugs](outputs/top_10_suspected_drugs.png)

- 🗺️ Heatmap of ADRs by Country
![Heat Map](outputs/improved_adr_heatmap_country_year.png)

- 🚻 Gender-wise ADR Distribution
![Gender-wise ADR Distribution](outputs/gender_distribution.png)

- 🚻 Outcome distribution
![outcome_distribution_pie](outputs/outcome_distribution_pie.png)

---

## Findings

- A steady increase in ADR reporting till 2023 and slightly decrease in 2024
- Male patients report slightly more ADRs compared to Females
- Certain antibiotics and NSAIDs are repeatedly flagged



---

## Folder Structure
Folder Structure

ADR-Report-Analysis/

├── data/

│ └── sample_adr_data.csv

├── notebooks/

│ └── adr_analysis.ipynb

├── scripts/

│ └── clean_data.py

├── outputs/

│ └── adr_trend_plot.png

│ └── drug_top10_bar.png

│ └── heatmap_region.png

├── README.md

└── requirements.txt

---

🚀 Getting Started

To run this project locally:

Clone this repository:

git clone https://github.com/SudiptaGhosh2025/ADR-Report-Analysis.git

Install dependencies:

pip install -r requirements.txt

Launch Jupyter Notebook:

jupyter notebook notebooks/adr_analysis.ipynb

---

🧾 License

This project is licensed under the MIT License – see the LICENSE file for details.

---

📬 Contact

Sudipta Ghosh | Pharmacovigilance Associate | Data Analyst

LinkedIn: https://www.linkedin.com/in/sudipta-ghosh-36a94aab/

Email: sudipta.ghoshdata@gmail.com
