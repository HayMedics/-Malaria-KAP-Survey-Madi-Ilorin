# Malaria Knowledge, Attitude & Preventive Practices (KAP) Survey
### Madi Community, Ilorin — Community Health Outreach (20 December 2025)

A data-driven public-health analysis of a malaria KAP survey conducted during a community health outreach in Madi Community, Ilorin, Nigeria.

**By HayMedics Academy**

---

## About This Project

I served as the **Project Manager** for this community health outreach. As a **data scientist**, I introduced a data-collection component that set this outreach apart from typical health drives — instead of only delivering services, we systematically captured community knowledge, attitudes, and behaviours around malaria so the impact could be measured and future interventions could be evidence-based.

This repository contains the full pipeline: raw data cleaning, statistical analysis, visualisation, and a professional consultant-style report.

---

## The Headline Finding: A Knowledge–Practice Gap

The community **knows** a lot about malaria and holds **positive attitudes** — but **protective behaviour is rare**.

| Domain | "Good" level |
|---|---|
| Knowledge | **86.9%** |
| Attitude | **76.2%** |
| Practice | **3.3%** |

- 93% know that mosquito nets prevent malaria — but only **28%** sleep under one every night.
- Only **19%** clear stagnant water around their homes.
- **46%** buy drugs from a chemist as their first response to fever, instead of getting tested.

Statistical tests showed education level did **not** significantly predict good practice (χ² tests, p > 0.05), meaning the barrier is not awareness — it is converting knowledge into action.

---

## Repository Contents

| File | Description |
|---|---|
| `malaria_clean.csv` | Cleaned dataset (122 respondents, ready for analysis) |
| `Malaria_KAP_Cleaned.xlsx` | Cleaned data + a one-page summary sheet |
| `Malaria_KAP_Report.docx` | Full biostatistical & public-health report with figures |
| `README.md` | This file |

> _Outreach photos and supporting documents will be added to the `/media` and `/docs` folders._

---

## Data Cleaning Highlights

Real-world survey data is messy. Key fixes performed:

- **Age:** Over half of respondents entered their *birth year* (e.g. 1980, 2007) instead of their age. These were converted to true ages and impossible values removed.
- **Text fields:** Stripped trailing spaces, standardised casing, and merged typos (e.g. "Hair deesser" / "Hair dersser" → "Hair dresser").
- **Junk column:** Removed an empty trailing column carrying no information.
- **Optional test field:** Recoded blank RDT results as "Not Tested" rather than missing.

---

## Methods

- **Design:** Cross-sectional KAP survey via Google Forms
- **Sample:** 122 community members
- **Scoring:** Knowledge (5 items), Attitude (4 items), Practice (3 items); Bloom's cut-offs (Good ≥ 80%, Moderate 60–79%, Poor < 60%)
- **Analysis:** Descriptive statistics, chi-square tests of association, Spearman correlation

**Tools:** Python (pandas, scipy, matplotlib)

---

## Recommendations (from the report)

1. Pair net distribution with hang-up demonstrations and follow-up reminders.
2. Run community clean-up campaigns targeting stagnant water.
3. Discourage chemist self-medication; promote test-before-treat.
4. Deliver interventions across all education levels — no group is protected by education alone.
5. Repeat the survey in wet season to measure behaviour during peak transmission.

---

## Outreach Photos
![Outreach](media/Photo from Abu Talha(HayMedics).jpg)
![Outreach](media/Photo from Abu Talha(HayMedics)(1).jpg)
![Outreach](media/Photo from Abu Talha(HayMedics)(2).jpg)



---
## Author

**Awal Abdulrahman**
Project Manager for the Madi Community Health Outreach.

---

*Survey responses were anonymous and collected for research purposes only.*
