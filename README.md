# 🚖 Uber Trip Analysis | Power BI Dashboard

> **A comprehensive operational and demand intelligence report analyzing 103,700+ Uber trips across New York City in June 2024 — uncovering booking patterns, vehicle performance, location hotspots, and time-based demand to support smarter driver allocation and revenue optimization.**

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Business Problem](#-business-problem)
- [Dashboard Pages](#-dashboard-pages)
- [Key Metrics Summary](#-key-metrics-summary)
- [Key Insights & Findings](#-key-insights--findings)
- [Vehicle Type Analysis](#-vehicle-type-analysis)
- [Location Intelligence](#-location-intelligence)
- [Time & Demand Analysis](#-time--demand-analysis)
- [Payment Behaviour](#-payment-behaviour)
- [Business Recommendations](#-business-recommendations)
- [Tools & Technologies](#-tools--technologies)
- [Data Model & DAX](#-data-model--dax)
- [How to Use This Dashboard](#-how-to-use-this-dashboard)
- [Author](#-author)

---

## 📖 Project Overview

This Power BI project delivers a full operational analysis of Uber trip data covering the entire month of June 2024 across New York City. The report is structured across three pages — **Overview Analysis**, **Time Analysis**, and **Details** — giving stakeholders a complete picture of booking volume, revenue distribution, vehicle preferences, and hourly demand patterns.

The goal was to go beyond surface-level trip counts and answer real operational questions:
- When and where is demand highest?
- Which vehicle types are generating the most revenue?
- Are there underserved locations or time windows with unmet demand?
- How are customers paying — and what does that mean for operations?

---

## 🧩 Business Problem

Ride-hailing operations generate enormous amounts of transactional data every day, but without structured analysis, that data sits unused. Operations managers, fleet coordinators, and business analysts need answers to questions like:

- **Where should drivers be positioned** to capture peak demand?
- **Which vehicle categories** are most profitable and most requested?
- **What time of day and day of week** drives the most bookings?
- **Are there demand dips** that could be addressed with targeted incentives?

This report was built to answer exactly those questions — transforming raw trip data into a strategic operations tool.

---

## 📊 Dashboard Pages

### Page 1 — Overview Analysis
The executive summary page. Displays top-level KPIs, vehicle type performance, payment method split, day vs. night trip distribution, and location analysis including the most frequent pickup and drop-off points.

### Page 2 — Time Analysis
A deep-dive into demand timing. Features an hourly booking curve, a day-of-week comparison chart, and a full booking heatmap showing the intersection of hour and day — making peak demand windows immediately visible.

### Page 3 — Details
A transaction-level table showing individual trips with Trip ID, pickup date, vehicle type, payment method, passenger count, distance, booking amount, and location — enabling granular drill-down for operational review.

---

## 📈 Key Metrics Summary

| Metric | Value |
|---|---|
| 💰 Total Booking Amount | $1,600,000 |
| 🚗 Total Bookings | 103,700 |
| 📍 Total Trip Distance | 349,000 miles |
| 💵 Average Booking Amount | $15.00 |
| 🛣️ Average Trip Distance | 3 miles |
| ⏱️ Average Trip Time | 16 minutes |
| 📅 Period Covered | June 1 – June 30, 2024 |

---

## 🔍 Key Insights & Findings

### 1. Revenue is Evenly Distributed Across Premium Tiers — But UberX Dominates Volume
Despite all vehicle types averaging the same $15 booking amount, UberX accounts for **37.4% of all bookings** (38,744 trips) and **36.5% of total revenue** ($583,880). This is not just the most popular tier — it is the operational backbone of the entire network.

### 2. Weekend Demand is Significantly Higher Than Weekdays
The time analysis reveals a clear weekly demand pattern. Saturday and Sunday consistently record the highest booking volumes — with Sunday peaking at over **19,000 bookings** compared to Thursday's low of approximately **10,000 bookings**. This is a 90% swing in demand between the weakest and strongest days of the week.

### 3. Midday is the Revenue Sweet Spot
Bookings begin climbing sharply from 6:00 AM, reach their peak between **10:00 AM and 6:00 PM**, and decline into late evening. The 12:00 PM hour on Sundays alone records **1,424 bookings** — the single highest hour-day combination in the entire dataset.

### 4. Thursday Midnight is a Hidden Late-Night Demand Spike
While most weekday midnight hours see under 200 bookings, Thursday at hour 0 (midnight) records **312 bookings** — the highest late-night figure of the week. This is a consistently underserved window where driver availability often drops below demand.

### 5. Penn Station is the Undisputed Demand Hub
Penn Station/Madison Square West is the single most frequent pickup location with **4,500 bookings**, tied with Upper East Side North as a drop-off destination. Transit hub proximity is a clear and consistent demand driver.

### 6. Day Trips Dominate but Night Trips Represent a Third of All Revenue
65.28% of all trips (67,700) are classified as day trips. Night trips account for **34.72% (36,000 trips)** — a significant segment that requires dedicated driver availability planning, particularly on Thursday and Friday evenings.

---

## 🚗 Vehicle Type Analysis

| Vehicle | Total Bookings | Total Revenue | Trip Distance | Avg. Booking |
|---|---|---|---|---|
| UberX | 38,744 | $583,880 | 131,496 miles | $15 |
| Uber Comfort | 17,078 | $253,995 | 56,790 miles | $15 |
| Uber Black | 16,710 | $250,192 | 56,149 miles | $15 |
| UberXL | 16,698 | $249,424 | 55,721 miles | $15 |
| Uber Green | 14,498 | $216,181 | 48,778 miles | $15 |

**Key Takeaways:**
- UberX commands more bookings than the next two vehicle types **combined**
- Uber Comfort ($253,995) narrowly edges out Uber Black ($250,192) — indicating strong demand for comfort-tier rides at non-premium pricing
- Uber Green, the eco-friendly option, is the least booked — suggesting either limited driver availability or lower consumer awareness
- UberX is the **most preferred vehicle at the top location** (Penn Station) with 7,700 bookings — more than double the next preference

---

## 📍 Location Intelligence

### Top 5 Pickup Locations by Booking Volume

| Location | Total Bookings |
|---|---|
| Penn Station / Madison Sq West | 4,500 |
| Upper East Side North | 4,500 |
| Upper East Side (South) | 4,100 |
| Lenox Hill East | 4,000 |
| Upper West Side | 3,800 |

### Most Frequent Pickup Point
> 📍 **Penn Station / Madison Square West** — 4,500 bookings

### Most Frequent Drop-off Point
> 📍 **Upper East Side North**

### Farthest Trip Recorded
> 🛣️ **116,924 miles** — an exceptional outlier requiring data validation

**Location Insight:** The top 5 pickup locations are all concentrated in **Midtown Manhattan and the Upper East Side** — high-density residential and transit areas. These zones should be treated as priority deployment areas during peak hours.

---

## ⏰ Time & Demand Analysis

### Hourly Demand Pattern
Demand follows a classic urban mobility curve:

| Time Window | Pattern |
|---|---|
| 12:00 AM – 5:00 AM | Low demand (38–312 bookings/hour) |
| 6:00 AM – 8:00 AM | Sharp morning ramp-up |
| 9:00 AM – 6:00 PM | Peak demand window |
| 6:00 PM – 9:00 PM | Evening plateau |
| 9:00 PM – 12:00 AM | Gradual decline |

### Highest Demand by Hour & Day (Top 5)

| Day | Hour | Bookings |
|---|---|---|
| Sunday | 12 PM | 1,424 |
| Saturday | 12 PM | 1,269 |
| Sunday | 11 AM | 1,293 |
| Saturday | 11 AM | 1,217 |
| Sunday | 10 AM | 1,216 |

### Day of Week Ranking (Highest to Lowest Bookings)
1. 🥇 Sunday
2. 🥈 Saturday
3. 🥉 Monday
4. Tuesday
5. Wednesday
6. Friday
7. Thursday ← Lowest weekday volume but highest late-night spike

---

## 💳 Payment Behaviour

| Payment Method | Bookings | Share |
|---|---|---|
| Uber Pay | 69,500 | 67.03% |
| Cash | 33,400 | 32.23% |
| Amazon Pay | 600 | 0.56% |
| Google Pay | — | ~0.18% |

**Payment Insight:**
- Uber Pay dominates at 67% — indicating strong platform loyalty and digital payment adoption
- Cash at 32% is **significantly higher than industry norms** for app-based ride-hailing — this increases operational complexity, reduces real-time revenue tracking accuracy, and introduces potential reconciliation challenges
- Amazon Pay and Google Pay are negligible — resources spent maintaining these integrations may not justify the return

---

## 💡 Business Recommendations

### 1. 🎯 Deploy More Drivers Around Penn Station on Thursday Evenings
Penn Station records the highest pickup volume overall, and Thursday midnight shows a surprising demand spike of 312 bookings. Increasing driver incentives in this area on Thursday evenings from 10 PM to 2 AM could capture significant unmet demand.

### 2. 📅 Implement Weekend Surge Incentives Starting Saturday Morning
Weekend demand is nearly double weekday demand. Proactively incentivizing driver availability from Friday evening through Sunday evening — particularly for UberX and Uber Comfort — would prevent surge pricing from pushing customers toward competitors.

### 3. 🟢 Investigate and Promote Uber Green Availability
Uber Green is the lowest-booked vehicle type with 14,498 trips and $216,181 revenue — approximately 43% fewer bookings than UberX. With growing sustainability awareness, a targeted marketing push and driver acquisition campaign for Uber Green could unlock an underserved customer segment.

### 4. 💸 Reduce Cash Dependency Through Digital Payment Incentives
Cash transactions at 32% create reconciliation risk and reduce operational visibility. Offering small discounts or reward points for Uber Pay transactions could shift 10–15% of cash users to digital — improving revenue tracking and reducing cash-handling costs.

### 5. 📊 Investigate the 116,924-Mile Outlier Trip
The farthest trip recorded at 116,924 miles is statistically impossible for a June 2024 New York trip and is almost certainly a data entry error or GPS anomaly. This should be flagged, investigated, and either corrected or excluded to prevent it from distorting any distance-based analytics.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Power BI Desktop** | Dashboard development and visualization |
| **DAX** | KPI calculations, time intelligence, conditional measures |
| **Power Query (M)** | Data cleaning, transformation, and loading |
| **Microsoft Excel** | Initial data exploration and validation |

---

## 📐 Data Model & DAX

### Key DAX Measures Used

```dax
-- Total Booking Amount
Total Booking Amount = SUM(Uber[Total Booking Amount])

-- Average Booking Amount
Avg Booking Amount = AVERAGE(Uber[Total Booking Amount])

-- Total Trip Distance
Total Trip Distance = SUM(Uber[Trip Distance])

-- Night Trip Bookings
Night Trip Bookings = 
CALCULATE(COUNT(Uber[Trip ID]), Uber[Trip Type] = "NightTrip")

-- Night Trip %
Night Trip % = 
DIVIDE([Night Trip Bookings], [Total Bookings], 0)

-- Top Location by Bookings
Top Location = 
TOPN(1, VALUES(Uber[Location]), [Total Bookings], DESC)
```

### Data Cleaning Steps (Power Query)
- Removed null and blank rows from Trip ID and Pickup Date columns
- Standardized vehicle type naming conventions
- Created a calculated Trip Type column (Day/Night) based on pickup hour
- Flagged outlier distance records (>1,000 miles) for review
- Validated payment method categories for consistency

---

## 📂 How to Use This Dashboard

1. **Clone or download** this repository
2. Open the `.pbix` file in **Power BI Desktop**
3. Use the **Date slicer** (top right) to filter by specific date ranges within June 2024
4. Use the **City slicer** to filter by city if multi-city data is added in future
5. Navigate between **Overview Analysis**, **Time Analysis**, and **Details** pages using the left navigation panel
6. Click any **vehicle type, location, or payment method** to cross-filter all visuals on the page
7. Use the **Details page** for transaction-level investigation of specific trips

---

## 👤 Author

**Faleye Olumide David**
Data Analyst | Power BI Developer | Business Intelligence Analyst

📍 Nigeria
🔗 [LinkedIn](https://www.linkedin.com/in/olumide-david-79b17726a/)
🌐 Portfolio: *datascienceportfol.io* (coming soon)
