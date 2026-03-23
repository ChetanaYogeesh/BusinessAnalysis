# 📞 Call Details Record — Telecom Analytics Looker Dashboard

> A comprehensive call data record (CDR) analytics platform for investigating mobile activity patterns across cell towers, geographic regions, and network contacts.

![Call Details Record — Telecom Analytics Dashboard](https://lookerstudio.google.com/reporting/a592fc9d-d083-42fc-b6ae-8f2b629d9df2/page/BIGgD)

---

## 📊 Overview

This dashboard provides end-to-end visibility into call detail records sourced from mobile network data. It is designed for **forensic telecom analysis**, **network monitoring**, and **investigative reporting** — enabling analysts to explore call patterns, dropped calls, SMSC messaging, geographic movement, and contact networks from a single interface.

The dataset covers activity from **Aug 26–29, 2021** across three tower cities: **San Francisco**, **Oakland**, and **Emeryville**.

---

## 🗂️ Dashboard Pages

### 1. 📋 Call Details Record
High-level summary of all call activity.

| Metric | Value |
|---|---|
| Total Activities | 352 |
| Call Directions | 3 |
| Tower Cities | 3 |
| Called Numbers | 40 |
| Total Call Volume | 260 |
| Incoming Call Volume | 100 |
| Outgoing Call Volume | 157 |
| Total Call Duration | 407.45 min |

**Visualizations:**
- Call volume by city per day (San Francisco, Oakland, Emeryville)
- Call direction breakdown (Outgoing 44.6%, Incoming 29.3%, SMSC 26.1%)
- Completion status (Completed Successfully 89.8%)
- Incoming & Outgoing calls by day
- MOC, MTC, and SMSC activity by day
- Bubble charts: Incoming & Outgoing calls — cell tower by city

---

### 2. ⏱️ Call Duration & Volume Metrics
Hourly and daily breakdown of call volumes and durations.

| Metric | Value |
|---|---|
| Avg Call Duration | 1.9 min |
| Longest Call | 43.17 min |
| Shortest Call | 0.02 min |

**Visualizations:**
- Hourly call volume + duration combo chart (Aug 26–29)
- Call volume and duration by day of week (two views)

**Key Insight:** Activity peaks on **Friday (71 calls, 72.75 min)** and **Saturday (78 calls, 74.92 min)**, with near-zero activity Mon–Thu.

---

### 3. 📉 Dropped Calls Metrics
Analysis of abnormal call completions and dropped call patterns.

| Metric | Value |
|---|---|
| Calls Completed | 224 |
| Calls Dropped | 36 |
| Avg Call Frequency | 0.64 min |

**Visualizations:**
- Hourly outgoing vs. incoming dropped calls timeline
- Dropped calls by called number (incoming vs. outgoing breakdown)

**Key Insight:** Number `14158887755` accounts for **25 outgoing dropped calls**, a significant anomaly worth investigation.

---

### 4. 📲 SMSC Metrics
Short Message Service Center (SMSC) message analysis.

| Metric | Value |
|---|---|
| Total SMSC Messages | 50 |

**Visualizations:**
- Hourly SMSC activity timeline
- Sankey diagram: sender (`16504838989`) → recipients
- SMSC sent by day of week (peaks Sunday: 41, Friday: 27)

---

### 5. 🗺️ Geography Metrics — Travel Analysis
Address-level call activity mapped to specific locations and times.

**Visualizations:**
- Detailed table: Date / Hour / Address / Calls / Duration / Tower Distance (Miles)

**Addresses observed:**
- `3067 Turk Blvd` — frequent nighttime outgoing calls
- `1358 S Van Ness Ave` — morning incoming calls with high durations
- `900 Corbett Ave` — mid-day activity
- `1418 Shrader St`, `2198 Fell St`, `248 9th St`, `1 Whiting Way`

---

### 6. 📡 Geography Metrics — Cell Tower Analysis
Call volumes by city and hour aggregated across the full activity window.

**Visualizations:**
- Aggregate hourly outgoing + incoming by hour of day
- Incoming calls by city over time (SF, Oakland, Emeryville)
- Outgoing calls by city over time

**Key Insight:** **10 PM** is the highest-activity hour with 31 outgoing calls. Emeryville activity is concentrated in the **Aug 28 morning window**.

---

### 7. 🤝 Network Metrics — Frequent Contacts
Contact frequency table and Sankey flow diagrams.

**Top Contacts:**

| Number | Incoming | Outgoing |
|---|---|---|
| 14151110505 | 17 | 10 |
| 16505551212 | 12 | 6 |
| 14157774455 | 7 | 0 |
| 15101112020 | 7 | 5 |
| 15105558686 | 5 | 1 |

**Visualizations:**
- Incoming & Outgoing call Sankey diagrams from `16504838989`
<img width="1205" height="905" alt="Screenshot 2026-03-23 at 11 00 32 AM" src="https://github.com/user-attachments/assets/008e4a96-4390-4a2e-89a6-16487b366096" />
<img width="1204" height="902" alt="Screenshot 2026-03-23 at 11 00 25 AM" src="https://github.com/user-attachments/assets/559244fd-6ed7-4736-84f3-5e3a4dfa1233" />
<img width="1209" height="908" alt="Screenshot 2026-03-23 at 11 00 18 AM" src="https://github.com/user-attachments/assets/a8bd2962-d667-4f2d-b76d-c9f76d38215b" />
<img width="1204" height="905" alt="Screenshot 2026-03-23 at 11 00 10 AM" src="https://github.com/user-attachments/assets/6546e5c5-74dc-47d1-88f1-c1dba7a13f52" />
<img width="1205" height="906" alt="Screenshot 2026-03-23 at 11 00 00 AM" src="https://github.com/user-attachments/assets/971a58de-07af-4f26-b8e7-ffdff07584a8" />
<img width="1204" height="904" alt="Screenshot 2026-03-23 at 10 59 46 AM" src="https://github.com/user-attachments/assets/02380bc0-fd13-420a-bb0d-730648402cc1" />
<img width="1207" height="908" alt="Screenshot 2026-03-23 at 10 59 36 AM" src="https://github.com/user-attachments/assets/6f59bc96-c32c-46f9-8c58-817f9055a125" />
<img width="1216" height="912" alt="Screenshot 2026-03-23 at 10 59 26 AM" src="https://github.com/user-attachments/assets/2462063f-89ed-4594-bcc0-dca202541fda" />
<img width="1215" height="917" alt="Screenshot 2026-03-23 at 10 43 36 AM" src="https://github.com/user-attachments/assets/00d5892c-5881-44e3-97e7-909dc0d94b9e" />

---

### 8. 📅 Network Metrics — Call Patterns
Date × contact matrix showing incoming/outgoing call counts per day.

**Notable Pattern:** Number `14158887755` shows 36 outgoing calls on Aug 27 and 46 on Aug 28 — a highly concentrated burst of activity.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| BI Platform | Looker  |
| Data Source | CDR CSV / Database |
| Geolocation | Cell tower coordinates + address lookup |
| Visualization | Bar charts, pie charts, bubble charts, Sankey diagrams, heatmaps |

---
