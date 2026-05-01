# 🛡️ Insurance Data Analysis — Power BI Dashboard

A comprehensive Power BI report built to analyze insurance policy data, claims behavior, customer demographics, and customer feedback sentiment. Data was sourced, cleaned, and transformed using **SQL** and **Power Query Editor** before being modeled and visualized in Power BI.

---

## 🔗 Report Link 

``` 
# Main Power BI report Link:
(https://app.powerbi.com/reportEmbed?reportId=0cad6508-5a11-4ec3-9339-6d2fdf35080c&autoAuth=true&ctid=7158a9ab-ddfe-406f-9a9b-4e3d7d144024)
README.md 
```

---
---
## 🔗 Dashboard Report Link
```
# Main Dashboard Link:
(https://app.powerbi.com/groups/81569ce2-8245-4e06-9ec8-45ee4ff09b66/dashboards/ffc5eebe-bcad-436f-b189-b8635083aec5?experience=power-bi)


```
---


## 📊 Report Overview

The report is organized across **3 pages**, each targeting a different analytical focus:

### Page 1 — Claims & Policy Analysis
The core analytical dashboard. It includes:
- **KPI Cards** — Total Premium Amount, Total Coverage Amount, Total Claim Amount, and Customer Count
- **Ribbon Chart** — Number of Claims by Claim Status (Approved, Pending, Rejected)
- **Bar Chart** — Premium Amount broken down by Policy Type
- **Line Chart** — Claim Amount distribution across Age Groups
- **Donut Chart** — Active vs. Inactive policy holders
- **Matrix / Pivot Table** — Coverage Amount by Policy Type and Claim Status
- **Slicers** — Filter by Policy Number, Claim Number, and Customer ID

### Page 2 — Customer Detail Table
A detailed tabular view of individual customer records including Policy Number, Customer ID, Age, and other attributes. Includes a navigation action button for improved user experience.

### Page 3 — Customer Feedback & Sentiment
- **Word Cloud** — Visual representation of frequently occurring feedback keywords (Custom Visual)
- **Bar Chart** — Count of Customers by Feedback Rating
- **Table** — Customer-level breakdown showing Customer Name, Sentiment Score (out of 10), and Feedback text

---

## 🗄️ Data Sources & Fields

The primary dataset is **InsuranceData**, containing the following key fields:

| Field | Description |
|---|---|
| `PolicyNumber` | Unique identifier for each insurance policy |
| `CustomerID` | Unique identifier for each customer |
| `ClaimNumber` | Unique identifier per claim |
| `PolicyType` | Type of insurance policy (e.g., Health, Auto, Life) |
| `ClaimStatus` | Current status of the claim (Approved / Pending / Rejected) |
| `PremiumAmount` | Amount paid as premium |
| `CoverageAmount` | Total coverage value of the policy |
| `ClaimAmount` | Amount claimed by the customer |
| `Age` / `Age Group` | Customer age and derived age group |
| `Gender` | Customer gender |
| `Active/Inactive` | Policy status |

A secondary dataset (**Sheet1**) powers the Feedback page:

| Field | Description |
|---|---|
| `Customer Name` | Name of the customer |
| `Feedback` | Free-text customer feedback |
| `Rating` | Numeric rating given |
| `Sentiment Score (out of 10)` | Sentiment score derived from feedback |

---

## 🧹 Data Preparation

### SQL
Raw data was queried and pre-processed using SQL. This involved:
- Filtering out incomplete or invalid records
- Joining relevant tables to consolidate the dataset
- Aggregating and deriving fields where needed before loading into Power BI

### Power Query Editor
Further transformations were applied inside Power BI using Power Query:
- Data type corrections (dates, numbers, text)
- Null value handling and row filtering
- Creation of derived columns (e.g., **Age Group** from raw `Age`)
- Renaming and reordering columns for clarity
- Merging/appending queries as needed

---

## 🎨 Custom Visuals Used

| Visual | Purpose |
|---|---|
| **tCard** (Custom KPI Card) | Enhanced KPI display cards on Page 1 |
| **Insurance Data** | Provided the Insurance Data on Page 2 
| **Word Cloud** | Visualizing customer feedback frequency on Page 3 |

---

## 🚀 How to Use 

1. **Clone or download** this repository.
2. Download the [Report](https://app.powerbi.com/reportEmbed?reportId=0cad6508-5a11-4ec3-9339-6d2fdf35080c&autoAuth=true&ctid=7158a9ab-ddfe-406f-9a9b-4e3d7d144024) open in [Power BI Desktop](https://powerbi.microsoft.com/desktop/).
3. If prompted about data source credentials, update the connection to point to your local SQL database or file source.
4. Refresh the data using **Home → Refresh**.
5. Use the slicers on Page 1 to filter by Policy Number, Claim Number, or Customer ID.
6. Navigate between pages using the tabs at the bottom or the action button on Page 2.
7. To See the Dashboard Report, refer to this [Dashboard Report](https://app.powerbi.com/groups/81569ce2-8245-4e06-9ec8-45ee4ff09b66/dashboards/ffc5eebe-bcad-436f-b189-b8635083aec5?experience=power-bi)
Link
---

## 🛠️ Tools & Technologies

- **Power BI Desktop**
- **SQL** — Data extraction and pre-processing
- **Power Query (M Language)** — Data transformation inside Power BI
- **DAX** — Measures and calculated columns
- **Custom Visuals** — Word Cloud, tCard

---

## 📌 Key Insights This Dashboard Enables

- Monitor total premiums collected vs. claims paid out
- Identify which policy types drive the most premium revenue
- Track claim approval, rejection, and pending rates
- Understand which age groups file the highest claim amounts
- Assess the proportion of active vs. lapsed policies
- Analyze customer satisfaction through feedback sentiment scores

---
---
## Snapshot of Power BI Report
![Snapshot of Power BI Report](https://github.com/Dogra-458/Power-BI-Project--Insurance-Data-Analysis-/issues/1#issue-4365533311)
---

## 👤 Dogra-458

**[Sumit Kumar]**  
[Your GitHub Profile](https://github.com/yourusername) · [LinkedIn](https://www.linkedin.com/in/sumit-kumar-69b33423b)

---

