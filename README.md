# AI-Driven Beneficiary Retention & Intervention System

<img width="1486" height="782" alt="image" src="https://github.com/user-attachments/assets/6f3907e5-e52d-4392-814f-e899cc9d742f" />

## 📌 Project Overview
**End-to-End Data Science Solution:** This project integrates a Python Machine Learning model (Logistic Regression) with SQL pipelines to predict beneficiary dropout risk and optimize a $626K program budget.

It features a **Dual-Layer Intelligence System**:
1.  **Strategic Executive View:** For high-level ROI monitoring and program health.
2.  **Operational Action Board:** Translates complex algorithms into a prioritized "hit list" for field officers to take immediate action.

### 🔗 Live Demo
* **View the Interactive Dashboard on Tableau Public:** **[https://public.tableau.com/app/profile/tinotenda.muchenje/viz/program-impact-analysis-dashboard/ImpactOverviewDashboard]**
---

## 📊 Dashboard Previews

### 1. The Strategic Executive View
*Designed for Directors to monitor high-level KPIs, budget utilization ($626K), and overall retention rates (94%).*

<img width="1486" height="782" alt="image" src="https://github.com/user-attachments/assets/b79d1f76-e072-41fe-8c2a-1b2c8be34a7d" />

### 2. The Operational Action Board
*Designed for Case Managers. Features a "Risk vs. Investment" scatter plot and a prioritized action list for 85 critical cases.*

<img width="1481" height="781" alt="image" src="https://github.com/user-attachments/assets/55745e8c-d9da-4535-a092-ad761d7a63fa" />

---

## 🛠️ Tech Stack
* **Python (Pandas, Scikit-Learn):** Data cleaning, feature engineering, and building the Logistic Regression prediction model.
* **SQL:** creating the "Master Analytics View" and joining prediction outputs with demographic data.
* **Tableau:** Advanced data visualization, parameter actions, and interactive dashboard design.
* **Figma:** UI/UX wireframing and layout design.

---

## ⚙️ Methodology: How It Works

### Step 1: Predictive Modeling (Python)
* Ingested raw attendance and demographic data.
* Engineered features including `Attendance_Rate`, `Vulnerability_Score`, and `Distance_to_Facility`.
* Trained a **Logistic Regression** model to generate a `Dropout_Risk_Probability` (0-100%) for every beneficiary.

### Step 2: Data Engineering (SQL)
* Created a robust data pipeline to join the static beneficiary profile data with the dynamic risk scores from the Python model.
* Structured the data into a flattened `view_master_analytics` table for optimal Tableau performance.

### Step 3: Visualization & Action (Tableau)
* **Strategic Layer:** visualized geographical hotspots and program flow using Sankey-style logic.
* **Operational Layer:** Implemented a **"Risk Quadrant" Scatter Plot** to identify high-cost, high-risk investments.
* **Action Logic:** Created dynamic filters to generate a "High Priority Hit List" for field officers.

---

## 🚀 Key Results & Impact
* **$28,000 Capital-at-Risk Identified:** Flagged specific investments currently tied to high-risk beneficiaries.
* **85 Critical Cases Flagged:** Generated an immediate intervention list for beneficiaries with >75% dropout probability.
* **Proactive Decision Making:** Transformed reactive reporting into a predictive tool, allowing the organization to intervene *before* a beneficiary drops out.

---

## 📂 Repository Structure
* `data/`: Contains dummy/anonymized datasets used for the project.
* `notebooks/`: Jupyter notebooks with the Python Logistic Regression model.
* `sql/`: SQL scripts used for data joining and view creation.
* `dashboards/`: Tableau packaged workbook files (.twbx).

---
