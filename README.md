# Ibom_Air-Airline_Operations_Analytics_Dashboard_2025
A production-grade, 16-page Power BI report delivering full-year operational intelligence across flight performance, route analytics, passenger traffic, fleet utilisation, fuel cost management, cargo operations, and revenue intelligence — built for airline leadership and commercial teams.

### Table of Contents

* Project Overview
* Business Problem
* Key Insights & Findings
* Dashboard Pages
* Data Model & DAX
* Technical Stack
* Repository Structure
* How to Use
* Author

### Project Overview
|Detail            |Info                                                      |
|------------------|----------------------------------------------------------|
|Tool              |Microsoft Power BI Desktop                                |
|Domain            |Aviation / Airline Operations                             |
|Year              |2025 (Full Year — Jan to Dec)                             |
|Report pages      |16 analytical views                                       |
|Aircraft types    |CRJ 900 · A220                                            |
|Routes covered    |20 origin-destination pairs                               |
|Currency          |Nigerian Naira (NGN)                                      |
|Data areas        |Operations · Commercial · Fleet · Fuel · Cargo · Revenue  |

### Business Problem
Airlines operate in one of the most data-intensive industries in the world — thousands of flights, millions of passengers, billions in fuel spend — yet operational data often sits in disconnected systems. Without a unified view, leadership cannot:

* Identify why flights are delayed and on which routes the problem is worst
* Know whether the fleet is being used efficiently or if aircraft are sitting idle
* Track how rising fuel prices are eating into ticket revenue in real time
* Understand which routes, cabin classes, and sales channels drive the most value
* Make proactive scheduling and procurement decisions backed by data

This dashboard was designed to close that gap — a single source of truth, no coding required, interactive for every level of the organisation.

### Key Insights & Findings
These are the headline findings surfaced by the dashboard — the kind of insight that drives real decisions:
1. Technical faults are the leading cause of delays — not weather or fuel
Out of 2,149 delayed flights across 2025, technical issues caused 550 incidents — the single largest category, more than weather (283) and Lagos station congestion (395) combined. The ABV–LOS and LOS–ABV trunk routes each recorded over 300 delay incidents individually, making them the highest-risk corridors for operational disruption.

_Implication: A targeted maintenance review on the CRJ 900 fleet — which handles the majority of high-frequency routes — could meaningfully reduce the delay count and improve the 81% OTP rate._


2. December OTP collapsed to 58% — the network's weakest month
While the annual OTP averaged 81%, December fell to 58% — the worst performance of the year by a wide margin. Schedule reliability in December also dropped to 68%. The combination of high cancellations (6 in December) and rising delays signals a systemic peak-season capacity or crew management challenge.

_Implication: Advance crewing plans, maintenance buffers, and slot management are needed before Q4 2026 to prevent a repeat._


3. The A220 is punching above its weight commercially
With only 2 aircraft in the fleet, the A220 generated ₦59bn in revenue — 43% of total revenue — while operating just 3,183 flights compared to the CRJ 900's 8,135. The A220 carried 363,730 passengers at higher per-passenger yields, and both aircraft (CDA and CDB) delivered near-equal contributions (51%/49%).

_Implication: Expanding the A220 fleet or deploying it more strategically on high-yield routes (ABV–LOS, LOS–PHC) could significantly improve revenue per available seat._


4. Class Y full-fare economy is the single biggest revenue driver
Class Y (unrestricted economy) generated ₦47.1bn — 32.6% of all ticket revenue despite not being the highest volume booking class. By contrast, Class B (the next revenue contributor at 19.4%, ₦28bn) shows that the top two classes alone account for over half of all ticket revenue.

_Implication: Fare class mix management is critical. Diluting Y-class inventory with discount classes costs disproportionately more than volume gains suggest._


5. Internet sales now account for 72% of all revenue
₦104.6bn was collected through the internet channel — 72.1% of total salespoint revenue. Nigerian airport stations contributed 11.9% (₦17.3bn), and travel agencies 7.8% (₦11.3bn). The mobile app, despite being a direct channel, generated only 1.2% (₦1.76bn).

_Implication: The mobile app is significantly underperforming relative to its strategic potential. A UX and marketing investment in the app could capture a meaningful share of the internet channel's volume at lower distribution cost._


6. ABV–LOS is the undisputed backbone of the network
The ABV–LOS / LOS–ABV route pair operated 2,778 flights across the year — 24.5% of all operated flights — and offered 334,000 seats, more than double the next largest route (LOS–QUO at 182K). It is the highest-volume, highest-capacity, and highest-delay route simultaneously.

_Implication: Any disruption on ABV–LOS has an outsized network effect. Operational resilience planning (spare aircraft positioning, crew standby) should be centred here first._


7. No-show rate of 7% represents recoverable revenue leakage
With 974,805 total bookings and only 905,079 passengers flown, approximately 69,726 booked seats went unflown — a 7% no-show rate. At an average ticket value, this represents hundreds of millions in revenue dilution that resale or overbooking strategy could partially recover.

_Implication: Reviewing the overbooking policy on high-demand routes and strengthening the ancillary penalties strategy (₦948M captured in 2025) could convert no-shows from a cost centre into a revenue buffer._

### Dashboard Pages
#### Page 1 — Operational Performance
Tracks the full operations lifecycle: scheduled flights, operated flights, cancellations, unscheduled (charter/ferry) activity, on-time performance, and schedule reliability — by month for all of 2025.
KPIValueScheduled Flights11,738Operated Flights11,318On-Time Performance (OTP)81%Schedule Reliability (SR)81%Cancelled Flights30Un-operated Flights390Non-Scheduled Flights45
Trend: OTP peaked at 94% in March and July, before declining sharply to 58% in December. The strongest operational months were Q2–Q3; Q4 showed consistent deterioration.

![Ibom Air Operational Performance Overview](images/Operational%Performance.PNG)
