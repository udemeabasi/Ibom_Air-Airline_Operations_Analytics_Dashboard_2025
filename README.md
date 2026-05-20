# Ibom_Air-Airline_Operations_Analytics_Dashboard_2025
A production-grade, 16-page Power BI report delivering full-year operational intelligence across flight performance, route analytics, passenger traffic, fleet utilisation, fuel cost management, cargo operations, and revenue intelligence — built for airline leadership and commercial teams.

### Table of Contents

* Project Overview
* Business Problem
* Key Insights
* Dashboard Visuals & Deep Insights
    * Route Performance — Flights by Route
    * Route Performance — Flights by Day of Week
    * Capacity Utilisation
    * Load Factor by Origin & Destination
    * Fleet Availability
    * CRJ 900 Fleet Deep-Dive
    * A220 Fleet Deep-Dive
    * Fleet Cross-Tabular — Flights by Aircraft & Route
    * Fleet Cross-Tabular — Fleet Type by Route
    * Fleet Cross-Tabular — Monthly Aircraft Utilisation
    * Fleet Cross-Tabular — Aircraft Operating Days
    * Fuel Uplift Analysis
    * Fuel Breakdown — Cost vs Revenue
    * Fuellers Information
    * Aircraft & Fuel Utilisation
    * Cargo Operations
    * Flight Delays Analysis
* Data Model & DAX
* Technical Stack
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

### Dashboard Visuals & Deep Insights
#### Route Performance — Flights by Route

![Flights by Route](Images/Flights_by_Route.PNG)

Monthly flight frequency per origin-destination pair across all 20 routes for the full year, enabling scheduling teams to spot seasonality patterns, frequency gaps, and volume distribution.

#### Insights surfaced from this visual:

* ABV–LOS is the undisputed trunk route with 1,390 flights and near-uniform frequency of ~120 flights per month — the most consistent scheduling pattern in the network.
* February was the weakest month across all routes with the network dipping to just 774 total flights, roughly 24% below January's 1,020. Nearly every route shows its lowest monthly count in February, confirming a calendar-driven seasonality dip that should inform fleet maintenance scheduling.
* LOS–QUO (1,029 flights) and QUO–LOS (980 flights) are the second-busiest route pair, but the asymmetry — 49 more outbound flights from Lagos — hints at demand imbalance worth investigating for yield management.
* October is the standout peak month with 1,019 total flights, only narrowly behind January. The network operates near its structural capacity ceiling across Q3–Q4.
* ABV–CBQ (280) and CBQ–ABV (279) are the lowest-frequency routes, with volumes less than 20% of the trunk route. These are likely marginal routes that require close revenue-per-seat monitoring to justify continued scheduling.

#### Route Performance — Flights by Day of Week

![Flights by Day of Week](Images/Flights_by_Days_of_Week.PNG)

Cross-tab of all 20 routes vs. 7 days of the week, revealing which days carry the highest operational load and where scheduling asymmetries exist.

#### Insights surfaced from this visual:
* Wednesday is the network's peak day (1,644 flights), closely followed by Tuesday and Friday. This mid-week concentration is consistent with corporate travel patterns dominating the Ibom Air network.
* Saturday is the lightest day with just 1,583 flights — 61 fewer than Wednesday. For a leisure-heavy weekend, this suppression likely reflects conscious scheduling rather than low demand, presenting a potential upside if weekend load factors justify additional rotations.
* ABV–LOS and LOS–ABV show near-perfect daily balance (~196–201 flights per day), which is exceptional operational discipline — the kind of consistency that minimises rotational positioning costs.
* ABV–CBQ and CBQ–ABV display highly uneven day distribution: Monday and Wednesday see 48 flights each, while Tuesday drops to just 34 and Friday to 35. This pattern is irregular and may reflect aircraft positioning constraints at Calabar (CBQ).
* ABV–ENU / ENU–ABV pattern is inverted: Tuesday (47/47) and Thursday (45/46) are peak days, unlike the rest of the network. This suggests Enugu routes serve a different customer segment, possibly government or education-related travel.

#### Capacity Utilisation


Full-year comparison of seats available vs. bookings and passengers flown, with monthly load factor trends, capacity by aircraft, booked load factor trend, and available seats by route.

#### Insights surfaced from this visual:

* 80% flown load factor on 1.135 million available seats is a commercially healthy result, sitting above the typical industry breakeven threshold of ~75–77% for short-haul operations.
* Booked load factor of 86% vs. flown load factor of 80% confirms a 6-percentage-point leakage gap — the 7% no-show rate translates to approximately 69,726 seats paid for but not flown. At even a conservative average fare of ₦15,000, this is over ₦1bn in potential overbooking/yield recovery.
* CDB is the largest capacity contributor at 222K seats, edging CED (211K), CDA (200K), and CEE (199K). The near-equal distribution across these four tail numbers reflects a deliberate utilisation strategy rather than heavy reliance on any single aircraft.
* BWL (30K) and BXO (19K) are dramatically underutilised compared to peers. Both aircraft appear to have operated for only partial years — BWL until March and BXO until February based on the operating days data — which explains the low cumulative seat count.
* February capacity hit a 12-month low at 67K booked vs. 77K available — the widest gap between supply and bookings, confirming February as the softest demand month and the optimal window for heavy aircraft maintenance.
* ABV–LOS dominates route capacity at 334K seats — double the second-largest route (LOS–QUO at 182K). Any capacity disruption on ABV–LOS has an immediate and outsized network impact.

#### Load Factor by Origin & Destination


Full 12-month load factor percentages for every one of the 20 origin-destination pairs, with a network total row. This is the most granular demand intelligence view in the dashboard.

#### Insights surfaced from this visual:

* ABV–LOS (88%) and LOS–ABV (88%) are the highest-performing routes by annual load factor, confirming that demand on the trunk route consistently fills capacity. These routes rarely dip below 80% even in weak months.
* LOS–PHC (80%), LOS–QUO (84%), and PHC–LOS (85%) are the next-strongest routes, all performing above the network average — the PHC corridor is clearly a commercially robust secondary hub.
* ACC–LOS (52%) and LOS–ACC (54%) are the weakest routes by a wide margin. The Accra route consistently underperforms — no month exceeds 68% on ACC–LOS, and the route dropped to 43% in March. This is a significant commercial red flag. The route is either incorrectly priced, poorly marketed, or structurally unable to compete on this international corridor.
* April was the strongest month across the network at 87% total load factor, coinciding with Easter travel peak. This is the highest single-month figure of the year.
* December declined to 80% — the second-weakest month (after January's 73%), confirming Q4 tail-off. Notably, LOS–PHC hit 95% in December while LOS–QUO hit 97%, suggesting domestic holiday travel concentrates on specific corridors rather than lifting the whole network.
* ABV–CBQ (68%) and CBQ–ABV (70%) are the lowest-performing domestic routes after Accra — worth scrutinising for frequency rationalisation.
* January is the weakest month at 73% total — an important planning baseline. Network-wide, only 2 routes exceeded 85% in January (CBQLOS at 90%, LOSABV at 85%), while several dropped to the 47–63% range.

#### Fleet Availability


Fleet count, serviceability split by aircraft type, flights and passengers by type, revenue contribution by type, monthly serviceable aircraft count, and individual aircraft operating days per month.

#### Insights surfaced from this visual:

* The A220 is the revenue efficiency champion. Two aircraft generating ₦59bn (43% of total revenue) while operating only 3,183 flights (28% of total) means the A220 earns significantly more per flight than the CRJ 900 — a powerful argument for fleet expansion.
* The CRJ 900 carries 60% of passengers (541,349) but generates only 57% of revenue (₦77bn), despite operating 72% of all flights (8,135). The revenue-per-passenger ratio strongly favours the A220.
* 8 out of 9 aircraft were serviceable throughout most of the year, with the combined serviceability dropping to 5 only in April and May — confirming a period of maintenance concentration that correlates with the April load factor dip.
* 365 distinct operating days confirms zero non-operating calendar days in 2025. The fleet never had a full day offline as a combined unit — a strong maintenance performance indicator.
* December shows only 1 A220 serviceable (CDA was offline) while CDB continued solo. This A220 capacity reduction in the peak December period partially explains why certain high-demand routes still underperformed despite compressed capacity.
* BWK entered service in July (first appearance in the monthly table), while BWL and BXO were retired or transferred by Q2. BXP entered mid-February. This significant fleet transition mid-year adds complexity to year-on-year comparisons.

#### CRJ 900 Fleet Deep-Dive


Revenue generated, passengers carried, flights operated, and revenue contribution percentage — broken down by each CRJ 900 tail number (CED, CEE, BXP, BWK, BWL, BXO).

#### Insights surfaced from this visual:

* CED is the top-performing CRJ 900 aircraft generating ₦23bn (30% of CRJ revenue) across 2,367 flights — the highest operated count in the entire fleet including A220s.
* CEE is a close second at ₦21bn (27%) with 2,236 flights. Together, CED and CEE account for 57% of CRJ revenue while operating 57% of CRJ flights — a near-perfect proportionality confirming consistent yield per flight.
* BXP (₦18bn, 24%, 1,922 flights) is the third-ranking CRJ and operated for 11 months (February–December), meaning its per-month performance is marginally below CED and CEE.
* BWK (₦11bn, 14%, 988 flights) operated only from July onwards (6 months) yet generated 14% of CRJ revenue — a higher revenue rate per flight (₦11.1M/flight) compared to CEE (₦9.4M/flight) and CED (₦9.7M/flight), suggesting BWK is deployed on more lucrative routes or time slots.
* BWL (₦3bn, 3%, 401 flights) and BXO (₦2bn, 2%, 221 flights) operated for only 3 months and 2 months respectively. These are transitional aircraft — their low contribution is a function of limited operating time, not poor per-flight economics.
* CRJ passenger distribution mirrors revenue distribution exactly: CED carries the most (160K), CEE second (151K), BXP third (126K) — reinforcing that revenue differences are driven by flight frequency rather than yield variation between aircraft.

#### A220 Fleet Deep-Dive


Revenue, passengers, flights, and contribution split between the two A220 tail numbers — CDB and CDA.

#### Insights surfaced from this visual:

* CDB slightly leads CDA across all metrics: ₦30bn vs ₦29bn revenue, 1,670 vs 1,513 flights, 190K vs 174K passengers, 51% vs 49% revenue share.
* The near 50/50 split is a deliberate operational decision — Ibom Air has balanced both A220s as evenly as possible across the year, minimising single-aircraft dependency risk on high-value routes.
* CDB's higher flight count (157 more flights than CDA) with proportionally higher revenue confirms similar yield per flight between the two aircraft — around ₦17.9M per flight for CDB vs ₦19.2M for CDA. Interestingly, CDA generates slightly more revenue per flight despite fewer total flights, suggesting CDA is scheduled on more premium or longer sectors.
* Combined A220 performance: ₦59bn from 3,183 flights = ₦18.5M average revenue per flight, compared to ₦9.5M per flight for the CRJ 900 fleet. The A220 generates nearly double the revenue per flight of the CRJ 900 — the single most important strategic insight in this dashboard for fleet planning.
* 363,730 passengers carried at an average of ~114 passengers per flight, versus 80 passengers per flight for the CRJ 900 — consistent with the A220's larger cabin configuration.
