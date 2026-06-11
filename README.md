# Healthcare Patient Care & Satisfaction Analysis (Tableau)

## 📌 Executive Project Overview
This project delivers an interactive, enterprise-grade healthcare business intelligence solution that processes over 2,200 unique patient visit records across 8 specialized clinical departments. The analytical objective was to evaluate operational latencies, diagnose bottlenecks in patient triaging workflows, and uncover systemic correlations between pre-consultation wait times, facility conditions, and underlying customer satisfaction scores. 

By structuring a multi-table relational model and translating metrics into an intuitive, high-fidelity dark-themed executive canvas, this solution provides clinic stakeholders with the targeted clarity needed to optimize scheduling buffers and improve patient care retention.

---

## 🛠️ Data Architecture & Tech Stack
The dataset is engineered utilizing a normalized relational star-schema structure to enforce strict data integrity and high-performance querying:

* **Fact Table:** `Patient_Visits` (Tracks transactional logs, metrics for wait times, consultation durations, and raw survey score integers).
* **Dimension Tables:** * `Departments` (Maps IDs to specialties including Cardiology, Pediatrics, General Medicine, and Neurology).
  * `Branches` (Segments facility operations by geographic UAE regional locations).
  * `VisitType` (Distinguishes service channels between Walk-in, Scheduled Appointments, and Emergencies).

**Technologies Used:**
* **Tableau Desktop:** Data modeling, calculated field design, and custom dashboard UX interface styling.
* **Advanced Microsoft Excel:** Initial multi-table structural data profiling, sorting, and integrity verification.

---

## 📈 Core Healthcare Performance Benchmarks (KPIs)
Through precise backend data aggregations, the following foundational organization-wide baselines were established:
* **Total Monitored Patient Visits:** 2,200 records
* **Average Patient Wait Time:** 62.35 Minutes *(Primary target identified for operational triaging updates)*
* **Average Physician Consultation Duration:** 27.48 Minutes
* **Overall Patient Care Satisfaction Index:** 2.72 / 5.00

---

## 🎯 Strategic Business Diagnostics & Deep Dives

### 1. The Pre-Consultation Latency Mismatch
A critical operational imbalance is isolated where pre-consultation patient wait times ($62.35 \text{ mins}$) drastically outpace actual face-to-face physician interaction time ($27.48 \text{ mins}$). This severe delta indicates a friction point inside front-desk registration, patient check-in queues, or pre-consultation nurse triaging workflows rather than medical staffing shortages.

### 2. Departmental Wait Time Outliers
When evaluating performance across specific specialties, **Neurology** and **Cardiology** exhibit the highest systemic wait variances. Conversely, departments processing static check-ups show stable care throughput, proving that unmanaged walk-in distributions are creating severe downstream resource bottlenecks.

### 3. Satisfaction vs. Facility Cleanliness Matrix
By mapping `Staff_Behavior_Rating` and `Facility_Cleanliness_Rating` concurrently across all 8 medical specialties using specialized cross-tabulations, clear performance outliers are visible. This isolation enables hospital management to execute highly targeted quality assurance training and site maintenance interventions instead of costly, blanket facility updates.

---

## 🖥️ Dashboard Interface & UX Design
The interactive Tableau workspace features a clean dark layout optimizing readability, unified KPI metric blocks, cross-departmental breakdown heatmaps, and dynamic time-slot filters to easily track changes from morning to evening shifts.

<img width="1858" height="847" alt="image" src="https://github.com/user-attachments/assets/89cdb6e7-cf30-4c8c-b3fb-38d2921804b8" />


---

## 📂 Repository Structure
```directory
├── Data/
│   ├── Patient_Visits.csv
│   ├── Departments.csv
│   ├── Branches.csv
│   └── VisitType.csv
├── Visualizations/
│   └── healthcare_patient_satisfaction.twb
└── README.md
