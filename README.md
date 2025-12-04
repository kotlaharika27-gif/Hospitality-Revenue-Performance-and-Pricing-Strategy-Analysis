# Hospitality-Revenue-Performance-and-Pricing-Strategy-Analysis
This end-to-end Power BI data analytics solution for Atli Grands generates critical revenue insights by analyzing key hospitality KPIs (RevPar, ADR, Occupancy Percentage), identifying the existing flat pricing strategy, and recommending a shift toward dynamic pricing to maximize revenue opportunities

## Problem Statement and Goals
The core goal was to build an analytical dashboard that moves beyond simple reporting to facilitate Level 1 and Level 2 analysis. This capability allows stakeholders to identify problems at a high level (Level 1) and then "peel the onion" to drill down into the root cause—identifying which city, channel, property, or room type is underperforming (Level 2)

## Key Performance Indicators (KPIs)
The sources identify the following Key Performance Indicators (KPIs) that are central to analyzing the hotel's revenue performance and pricing strategy
###  RevPar (Revenue Per Available Room):
Calculated as total revenue divided by the total rooms available to sell, or alternatively, ADR multiplied by occupancy
###  Occupancy Percentage:
The simple calculation of the number of rooms sold or utilized by customers divided by the number of available rooms. It is defined as total successful bookings divided by total capacity.
### ADR (Average Daily Rate):
This metric represents the average rate at which rooms were sold (Total Revenue / Utilized Room Nights)
### Realization Percentage: 
This KPI is calculated as Utilized Room Nights (UR) divided by Booked Room Nights (BRN) and indicates the actual revenue realized against the total bookings received.
###  Revenue:
The overall income generated
### DSRN (Daily Sellable Room Nights): 
This metric helps monitor any specific issues, such as room blocking or maintenance issues, by looking at the rooms available to sell on a daily basis
### Average Rating:
While not listed among the "top metrics" for the top-level dashboard, it is included in the property-level deep dive view
## Dash board
<img width="1228" height="738" alt="Dashboard" src="https://github.com/user-attachments/assets/bb454907-14a8-464f-99a8-94131229543e" />

##  Methodology and Technical Stack
1. Requirement Gathering: Stakeholder interviews established the need for key metrics (RevPar, ADR, Realization) and required data splits (e.g., weekday vs. weekend).
2. Data Acquisition and Transformation: Data mimicking real-life scenarios (including bookings, capacity, and hotel details) was imported, and transformation steps were performed in Power Query.
3. Data Modeling: Relationships between fact and dimension tables were established using a star schema. Custom calculated columns were added using DAX to redefine the business logic, specifically determining that weekends are Friday and Saturday for this industry.
4. Dashboarding: The final output is a Power BI dashboard featuring key visuals, filters (by city, room type, date), and trend analysis (week-on-week change and trend lines visible via tooltips)

##  Key Insights and Business Recommendations
Here are the key insights and business recommendations from the project in a simple, short, and understandable way:
1. Fixed Pricing Exposed: The analysis clearly showed that Atli Grands is using a flat pricing strategy across the weeks, as evidenced by the constant Average Daily Rate (ADR) line despite fluctuating occupancy.
2. Major Revenue Opportunity: The single biggest takeaway is the potential to maximize revenue by moving away from flat pricing and implementing dynamic pricing or at least differential weekday/weekend pricing.
3. Rating and Service Issues: There is a strong correlation between hotels with low occupancy/high cancellation rates and low average ratings (e.g., Atli Grands Bangalore). This points to a need for service improvement and accurate online content.
4. Channel Strategy: While the hotel should not undercut competitor pricing directly, they should use their own channels (website) to offer promotions and value-adds (like discount coupons or complimentary extras) to boost direct bookings and optimizatio

5. ##  Technical Stack
1.  Visualization & Analysis: Power BI Desktop
2. Data Transformation: Power Query
3. Calculations: DAX (Data Analysis Expressions)
