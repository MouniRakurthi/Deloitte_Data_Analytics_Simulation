# Deloitte_Data_Analytics_Simulation
Deloitte Australia Technology Virtual Experience (Forage) — Tableau dashboard for factory downtime analysis &amp; Excel gender pay equality classification.
 # Deloitte Australia – Technology Virtual Experience (Forage)

![Deloitte](https://img.shields.io/badge/Deloitte-Virtual%20Experience-86BC25?style=flat&logo=deloitte)
![Tableau](https://img.shields.io/badge/Tableau-Dashboard-E97627?style=flat)
![Excel](https://img.shields.io/badge/Excel-Data%20Analysis-217346?style=flat)

## Overview
This repository contains the work completed during the **Deloitte Australia Technology 
Virtual Experience** simulation on Forage. The simulation involved two analytical tasks 
for a fictional industrial client, **Daikibo Industrials**.

---

## Task 1: Data Analysis & Visualization (Tableau)

### Background
Daikibo operates 4 global factories with 9 machine types each, sending telemetry 
data every 10 minutes. One month of data (May 2021) was analysed to answer:
- Which factory had the most machine downtime?
- Which machine types broke down most in that location?

### Factories
| Factory | Location |
|---|---|
| Daikibo Factory Meiyo | Tokyo, Japan |
| Daikibo Factory Seiko | Osaka, Japan |
| Daikibo Berlin | Berlin, Germany |
| Daikibo Shenzhen | Shenzhen, China |

### Steps Performed
- Imported unified JSON telemetry data into Tableau
- Created a calculated field **"Unhealthy"** (value = 10 per unhealthy status = 10 mins downtime)
- Built a **"Down Time per Factory"** bar chart
- Built a **"Down Time per Device Type"** bar chart
- Created an interactive Dashboard with factory chart as a filter

### Key Finding
> 🏭 **Daikibo Factory Seiko (Osaka, Japan)** had the highest downtime with **480 unhealthy readings**



---

## Task 2: Forensic Technology – Gender Pay Equality (Excel)

### Background
Daikibo faced internal complaints about gender pay inequality. A forensic algorithm 
generated an **Equality Score** (-100 to +100, where 0 is ideal) for each job role 
across all factory locations.

### Task
Added an **Equality Class** column to classify each score:

| Equality Class | Score Range |
|---|---|
| Fair | -10 to +10 |
| Unfair | < -10 or > 10 |
| Highly Discriminative | < -20 or > 20 |

### Excel Formula Used
```excel
=IF(ABS(C2)<=10,"Fair",IF(ABS(C2)<=20,"Unfair","Highly Discriminative"))
```

---

## Tools & Skills
- **Tableau** — Data visualization, calculated fields, interactive dashboards
- **Microsoft Excel** — Conditional logic, data classification, formula design
- **Data Analysis** — Telemetry analysis, KPI identification, business reporting

---

## Certificate
Completed via [Forage](https://www.theforage.com/simulations/deloitte-au/data-analytics-s5zy/completed) — Deloitte Australia Technology 
Virtual Experience Program
