# Call Centre Performance Analytics Dashboard

A Power BI dashboard project analyzing call centre operations to track agent performance, call resolution rates, customer satisfaction, and call volume trends. The dashboard provides management with real-time KPIs and breakdowns to identify operational bottlenecks and improve service quality.

**Author:** Ashwin Suryawanshi | **Tool:** Power BI Desktop

---

## Files in This Repository

| File | Description |
|------|-------------|
| `Call_Centre_Data_Analysis.pbix` | Power BI dashboard — 5 KPI cards, 5 charts, 2 slicers across 1 page |

---

## Tools & Technologies

- **Power BI Desktop** — KPI cards, column charts, bar charts, area chart, donut chart, pie chart, slicers
- **Data Sources:** Two connected tables — `Sheet1` (aggregated KPIs) and `Call Centre Data` (raw call records)

---

## Dataset

Two tables used in the model:

**Sheet1 — Aggregated KPI Table**

| Column | Description |
|--------|-------------|
| `Agent` | Call centre agent name |
| `Topic` | Call topic / category |
| `Resolution` | Whether the call was resolved (Yes/No) |
| `Total Calls` | Total number of calls |
| `Total Call Answered` | Count of answered calls |
| `Total Call Rejected` | Count of rejected/abandoned calls |
| `% Answered Calls` | Percentage of calls answered |
| `% Rejected Calls` | Percentage of calls rejected |

**Call Centre Data — Raw Records Table**

| Column | Description |
|--------|-------------|
| `Agent` | Agent handling the call |
| `Date` | Date of the call |
| `Total Calls` | Call volume metric |
| `Call Answered` | Answered call flag |
| `Call Rejected` | Rejected call flag |
| `Merged` | Combined performance metric |

---

## Dashboard — Page 1

### KPI Cards (5)

| Card | Metric |
|------|--------|
| Total Calls | Overall call volume |
| Total Answered Calls | Count of successfully answered calls |
| Total Rejected Calls | Count of rejected / missed calls |
| Total % Of Calls Answered | Answer rate (%) |
| Total % Of Calls Rejected | Rejection rate (%) |
| Total Agents | Number of agents in the dataset |
| Highest Calls Answered | Top-performing agent by calls answered |
| Avg Satisfaction Rate | Average customer satisfaction score |

### Charts (5)

| Visual | Type | X-Axis | Y-Axis | Insight |
|--------|------|--------|--------|---------|
| Calls by Resolution | Column Chart | Resolution (Yes/No) | Total Calls | Shows resolved vs unresolved call split |
| Calls by Topic | Clustered Bar Chart | Topic | Total Calls | Identifies highest-volume call categories |
| Agent Performance | Column Chart | Agent | Sum of Merged | Compares overall agent performance scores |
| Call Volume Over Time | Area Chart | Month → Day | Total Calls | Tracks daily and monthly call volume trends |
| Calls Answered by Agent | Donut Chart | Agent | Sum of Call Answered | Agent share of answered calls |
| Calls Rejected by Agent | Pie Chart | Agent | Sum of Call Rejected | Agent share of rejected/missed calls |

### Slicers (2)

| Slicer | Field | Purpose |
|--------|-------|---------|
| Month Slicer | Date → Month | Filter all visuals by month |
| Date Slicer | Date | Filter all visuals by specific date range |

---

## Key Insights Enabled by the Dashboard

- **Answer vs rejection rate** — headline KPIs immediately flag if the team is missing too many calls
- **Resolution breakdown** — column chart shows what proportion of answered calls are actually resolved
- **Topic analysis** — bar chart highlights which call topics drive the most volume, useful for staffing and training decisions
- **Agent performance** — column and pie/donut charts identify top and underperforming agents
- **Time trends** — area chart reveals peak call days and months for capacity planning
- **Date slicers** — allow managers to drill into specific months or date ranges for targeted analysis

---

## Business Recommendations this Dashboard Supports

1. **Staff scheduling** — use call volume trends (area chart) to align agent availability with peak demand periods
2. **Agent coaching** — agents with high rejection rates or low resolution scores (pie/donut + column charts) can be flagged for training
3. **Topic-based routing** — high-volume topics can inform IVR design and specialist team assignment
4. **SLA monitoring** — % answered and % rejected KPIs serve as live service level agreement trackers
5. **Customer satisfaction drivers** — Avg Satisfaction Rate card benchmarks overall service quality month-over-month

---

## Topics

`power-bi` `call-centre` `data-analysis` `kpi-dashboard` `agent-performance` `customer-service` `business-intelligence` `data-visualization`
