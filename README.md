# 🏥 Hospital Diabetic Patient Readmission Analysis — 

An Excel-based **Exploratory Data Analysis (EDA)** dashboard examining **66,587 diabetic hospital patient records** to identify readmission risk factors, clinical patterns, and resource utilization. Built as a structured multi-level assessment project, progressing from foundational to advanced analytics.

---

## 📊 Dashboard at a Glance

| Metric | Value |
|---|---|
| Total Patients | 66,587 |
| Total Readmitted | 30,764 |
| Overall Readmission Rate | **46.2%** |
| Mean Hospital Stay | 4.40 days |
| Mean Medications per Patient | 16.0 |

---

## 📁 Workbook Structure

The file is organized into **4 sheets**, each representing a deeper level of analysis:

```
Hospital_Diabetic_Patient_Readmission_Analysis__EDA___Multi-Level_.xlsx
│
├── 📊 Summary           → Executive KPI overview + key findings snapshot
│
├── Basic Level          → Readmission by age group; avg stay by medical specialty
│
├── Medium Level         → Comorbidity analysis; discharge disposition;
│                          race × gender × age demographics;
│                          chi-squared medication effectiveness test
│
└── Advanced Level       → Readmission distribution; K-means cluster analysis;
                           resource utilization by readmission type;
                           race × readmission breakdown;
                           estimated savings from avoided readmissions
```

---

## 📈 Key Findings

**Age** — Patients aged 70–80 have the highest readmission rate at **48%**, while children under 10 have the lowest at **22%**.

**Weight** — Underweight patients (BMI [0–25)) show a striking **80.8% readmission rate** — nearly double the overall average — pointing to critical nutritional risk.

**Comorbidity** — A comorbidity score of 8 correlates with the highest readmission rate (**53.2%**) and an average stay of **4.7 days**. Risk rises clearly with score.

**Medication Changes** — Patients whose medications were adjusted during hospitalization had a **48.6%** readmission rate vs **44.1%** for those on stable regimens.

**Lab Procedures** — Higher lab procedure counts consistently correlate with increased readmission likelihood, reaching up to **49%** in the highest bins.

**Correlations** — Medications and hospital stay show a moderate positive relationship (Pearson r = 0.466). Outpatient visits and readmission show only a weak link (r = 0.082).

**Race** — African American patients have the highest mean readmission score (0.80), followed by Caucasian (0.75) and Hispanic (0.72).

### Patient Clusters (K-Means, 4 Groups)

| Cluster | Readmit Rate | Avg Stay | Profile |
|---|---|---|---|
| 0 | 0% | 3.98 days | Low-risk, minimal utilization |
| 1 | 100% | 5.01 days | High-risk, high medication load |
| 2 | 50% | 7.12 days | Complex, long-stay cases |
| 3 | 20% | 2.57 days | Short stay, lower risk |

### Resource Utilization: Readmitted <30 Days vs Not Readmitted

| Resource | Not Readmitted | Readmitted <30 Days |
|---|---|---|
| Hospital Stay | 3.8 days | 5.5 days |
| Lab Procedures | 42.5 | 48.0 |
| Medications | 15.0 | 19.5 |
| Emergency Visits | 0.1 | 0.4 |

### Estimated Savings from Avoiding Readmissions
If preventable readmissions were eliminated, estimated resource savings include **~2,356 hospital days**, **~7,623 lab procedures**, **~6,237 medication administrations**, **~1,802 inpatient visits**, and **~416 emergency visits**.

---

## 💡 Recommendations

1. **Launch targeted discharge programs for elderly patients (70–80)** — With a 48% readmission rate, this group needs structured follow-ups: post-discharge calls, home care referrals, and medication counseling.

2. **Mandatory nutrition screening for underweight patients** — An 80.8% readmission rate demands action. Dietitian assessments and nutrition plans should be required before discharge for this group.

3. **Risk-flag patients with comorbidity score ≥ 8** — At 53.2% readmission, these patients should trigger extended monitoring protocols and specialist review before leaving hospital.

4. **Pharmacist-led medication reconciliation post-discharge** — The gap between medication-changed (48.6%) and stable (44.1%) patients suggests that transitions in medication regimens need closer supervision and patient education.

5. **Investigate and support Cluster 1 patients** — This segment shows a 100% readmission rate with heavy medication use. Case management or chronic disease management enrollment could break the cycle.

6. **Develop a composite risk score for early intervention** — Age, weight class, comorbidity score, medication change status, and lab procedure volume are all predictive. Combining them into a triage score could help staff prioritize at-risk patients before discharge.

7. **Address racial disparities in readmission outcomes** — African American patients have the highest mean readmission score. Culturally tailored care pathways and access barrier investigations are warranted.

---

