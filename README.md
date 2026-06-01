# Healthcare Patient Wait List Analytics Dashboard

## 📊 Project Overview
This end-to-end Power BI business intelligence solution tracks, analyzes, and visualizes medical patient wait list data from 2018 to 2021. The dashboard translates complex hospital operational metrics into actionable insights, allowing healthcare administrators to monitor wait times, identify specialty bottlenecks, and optimize patient delivery systems across various case types.

---

## 🚀 Live Previews

### 1. Summary Insights View
Features high-level KPI cards for the latest month's wait list numbers, Prior Year (PY) comparisons, time-band trends, and age profile tracking.
![Summary Dashboard View](Screenshot%202026-06-01%20115811.png)

### 2. Granular Data Deep-Dive
An interactive, hierarchical matrix view detailing case types, specific age brackets, and performance breakdowns across clinical specialties.
![Detailed Matrix View](Screenshot%202026-06-01%20115816.png)

---

## 🛠️ Data Architecture & Technical Skills

### 1. Advanced DAX Calculations
As seen in the data schema, complex Data Analysis Expressions (DAX) were authored to handle dynamic calculations:
* **`Latest Month Wait List`**: Dynamically computes active patient queues for the most recent reporting period.
* **`PY Latest Month Wait List`**: Time intelligence measure calculating prior year benchmarks to analyze Year-over-Year (YoY) performance.
* **`Average Wait List` & `Median Wait List`**: Statistical distribution metrics configured alongside a custom calculation toggle.

### 2. Relational Data Modeling
* Engineered a star-schema model linking the central fact table (`All_Data`) with optimized dimension mapping tables (`Mapping_Specialty` and `Calculation Method`) to handle secure, performant filtering.

### 3. Dynamic UI/UX Layouts
* Integrated multi-tiered slice panels (Archive Date ranges, Case Types, Age Profiles, and Specialty Names) paired with page navigation elements to ensure an intuitive user experience.

---

## 💡 Key Business Insights Discovered
* **Trend Anomalies**: Pinpointed a sharp shifting spike in Outpatient waitlist volumes beginning in early 2020, providing data support for hospital capacity tracking.
* **Age Group Demographics**: Identified that the `18+ Months` wait band is disproportionately occupied by specific age demographics across segments like Otolaryngology (ENT) and Orthopaedics.
* **Specialty Bottlenecks**: Revealed that Ophthalmology and Paediatric Orthopaedics maintain uniquely high average/median wait lists compared to other clinical departments.

---

## 📂 How to Run the File
1. Download and install **Power BI Desktop**.
2. Clone this repository to your local machine using git:
```bash
   git clone [https://github.com/irfanhabeeb550/healthcare-waitlist-analytics.git](https://github.com/irfanhabeeb550/healthcare-waitlist-analytics.git)
