# Urban Crime Analytics Dashboard

> **A multi-page Looker analytics report analyzing 32,000 urban offense records (2017–2021) across temporal trends, incident types, geographic zones, and statistical validation.**

![Looker Live Dashboard](https://lookerstudio.google.com/u/0/reporting/3770a34c-1b0e-4913-a00b-f004392d1a91/page/p_w29d4zv4ad)

---

## Overview

This project delivers an end-to-end crime data analytics solution built in Power BI. The dashboard spans 8 interactive report pages and covers everything from high-level offense summaries to granular statistical correlation analysis — designed to support data-driven public safety decision-making.

**Dataset**: ~32,000 offense records | Jun 2017 – Aug 2021 | 8 City Zones | 78 Incident Types

---

## Dashboard Pages

| Page | Description |
|------|-------------|
| **Offenses Data Details** | Summary KPIs, monthly/daily/hourly trend lines with average benchmarks |
| **Incident Types** | Treemap, donut chart, and Sankey flows by incident type and zone |
| **Vehicle-Related Incidents** | 7% vehicle-related breakdown, hourly/monthly trends, zone treemaps |
| **Case Analysis By Zone** | Bubble chart (cases × incident types), monthly and hourly zone breakdowns |
| **Homicide & Rape Categories** | Monthly time-series, ranked tables by incident type and zone |
| **Other Category Analysis** | 72% share analysis, top incident types, zone-level breakdown |
| **Larceny Category Analysis** | 28% share analysis with Z1/Z8 as dominant larceny zones |
| **Hypothesis Testing & Correlation** | Chi-square tests, p-values, correlation matrix across all key variables |
| **Scatter Plots – Zone & Incident Types** | Z1/Z3/Z5 vs 23C/35A/13B scatter relationships |
| **Scatter Plots – Zone & Categories** | Z1/Z3/Z5 vs Larceny/Other/Vehicle scatter relationships |

---

## Key Findings

### Temporal Patterns
- **Peak crime hour**: 2 PM (2,550 cases) — strong afternoon concentration (12PM–3PM)
- **Lowest activity**: 3 AM (638 cases) — clear overnight trough
- **Yearly trend**: Declining from 8,234 (2019) → 4,375 (2021), with a sharp drop visible post-2020

### Category Breakdown
- **Larceny**: 8.8K cases (28%) — dominated by incident types 23C, 13B, 35A across zones Z1 and Z8
- **Other**: 22.9K cases (72%) — highest in Z3, Z5; 23C leads with 3,581 records
- **Vehicle-related**: Only 7% (2.4K) with a downward trend over the study period
- **Homicide**: 14 cases (0.04%); **Rape**: 230 cases (0.72%)

### Geographic Insights
- **Z3** has the strongest correlation with vehicle-related incidents and homicide
- **Z5** and larceny are closely correlated
- **Z1** consistently ranks highest in larceny cases (2,776 total)
- **23C** is the top incident type across every category analyzed

### Statistical Validation
All three chi-square hypothesis tests rejected the null hypothesis of variable independence:

| Test | χ² Statistic | p-value | df | Critical Value | Result |
|------|-------------|---------|-----|----------------|--------|
| 1 | 23.661 | 0.01% | 4 | 9.49 | Reject H₀ |
| 2 | 26.691 | 0.08% | 8 | 15.51 | Reject H₀ |
| 3 | 59.338 | <0.001% | 20 | 31.41 | Reject H₀ |

Correlation matrix highlights: Vehicle Related & Total Cases (0.97), Larceny & Vehicle Related (0.90), Z3 & Homicide (0.74).

---
<img width="1204" height="907" alt="Screenshot 2026-03-23 at 11 08 29 AM" src="https://github.com/user-attachments/assets/0362357d-2bed-4746-adad-76547a72d7d9" />
<img width="1212" height="921" alt="Screenshot 2026-03-23 at 11 09 50 AM" src="https://github.com/user-attachments/assets/e4dae826-01d8-40c0-9daa-4ad962db1826" />
<img width="1212" height="911" alt="Screenshot 2026-03-23 at 11 09 44 AM" src="https://github.com/user-attachments/assets/6b3b1400-1ae2-4fdc-a9de-564e8cbefd7e" />
<img width="1205" height="908" alt="Screenshot 2026-03-23 at 11 09 36 AM" src="https://github.com/user-attachments/assets/a364ee16-7a7e-48f4-a693-4bd1f2f3886d" />
<img width="1206" height="906" alt="Screenshot 2026-03-23 at 11 09 27 AM" src="https://github.com/user-attachments/assets/0862ce0d-904b-4404-8c72-1a9ec1bbaf86" />
<img width="1208" height="911" alt="Screenshot 2026-03-23 at 11 09 18 AM" src="https://github.com/user-attachments/assets/5e612f16-2011-4b47-ae92-c154413406eb" />
<img width="1206" height="906" alt="Screenshot 2026-03-23 at 11 09 08 AM" src="https://github.com/user-attachments/assets/3f424525-1275-4e01-b2ac-f56da89a9d35" />
<img width="1203" height="903" alt="Screenshot 2026-03-23 at 11 08 57 AM" src="https://github.com/user-attachments/assets/91c4c3bf-de01-496d-b4f1-cf7179435a1d" />
<img width="1203" height="903" alt="Screenshot 2026-03-23 at 11 08 47 AM" src="https://github.com/user-attachments/assets/df84b7f1-a23d-49af-8474-d9c0e49eaeca" />
<img width="1208" height="905" alt="Screenshot 2026-03-23 at 11 08 37 AM" src="https://github.com/user-attachments/assets/6f6908b0-c265-476a-837e-e945adc752d5" />



---
## Tech Stack

- **Power BI Desktop** — report development, visuals, filters
- **DAX** — KPI measures, rolling averages, YoY calculations
- **Power Query (M)** — data cleaning, type normalization
- **Statistics** — Chi-Square hypothesis testing, Pearson correlation matrix


---



