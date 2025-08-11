# June 2025 Totilpay Data Report

**Totilpay data: potential and current insights**  
By: Courtney Ignace, August 2025, For Fresh Truck

---

## Overview
Using the Totilpay data from June 2025 alongside market location data we can sort and view transaction data based on market locations and draw insights into how our customers pay with their EBT cards.  
This report is intended to present the potential uses of Totilpay data through analysis as well as present the analysis that has already been performed.

At this point in analysis we can:
- Advocate for different types of card-holder education based on error codes.
- Estimate SNAP utilization by market and by card.

With more dedicated time and larger datasets, we can further explore the potential insights this data may hold.

---

## Methodology
- **PostGreSQL** – data cleaning  
- **Google Sheets** – data cleaning and analysis  
- **Tableau** – analysis and visualization  

---

## Tableau Insight
The first table in Tableau plots the count of `Response Text` instances by market.  

**Example insights:**
- **Insufficient Funds** – Highest need for advocacy: MEM, Elm Hill, Hyde Park, Neponset.  
- **Invalid PIN – Retry** – Highest need: Elm Hill, MEM, Charlestown.  
- **Restricted Card** – Highest need: Franklin Field BHA, West Broadway, Elm Hill, Neponset.  

Full `Response Text Data Dictionary` [here](https://docs.google.com/spreadsheets/d/1ei-4zdohkVW0ffRwH0YIHNC3LV_x4xSjjLNlpnjjxPQ/edit?usp=sharing).

---

## Response Text Dictionary & Recommendations

### Card Not Found
- **Meaning:** Card is no longer active — DTA does not recognize it.  
- **Solution:** Ask customer if they have a newer card or still receive benefits. Dispose of inactive card.

### Insufficient Funds
- **Meaning:** Card balance is less than total amount charged.  
- **Solution:** Encourage customers to check their SNAP balance before shopping and communicate that SNAP balance with the cashier before they swipe.

### Invalid PIN Entry
- **Meaning:** Wrong PIN entered — common when using another family member’s card or due to physical/visual impairments.  
- **Solution:** Confirm PIN before checkout, offer to assist entry, and provide secure PIN reminders.

### PIN Tries Exceeded
- **Meaning:** More than three incorrect PIN attempts — card is locked.  
- **Solution:** Closely monitor PIN entries, communicate importance of correct entry the first time.

### Restricted Card
- **Meaning:** Card is locked in the DTAConnect App.  
- **Solution:** Instruct customers to unlock card before shopping.

---

## Spreadsheet Analysis

### 1. Count of Unique Cards by Market
- Model built to verify uniqueness of card numbers per market.  
- Initial estimates (June 2025):  
  - SNAP money used: **$7,388 – $7,584.15**  
  - Unique cards: **2,305 – 2,395**  
- More statistical validation needed.

### 2. Extra Swipes per Market
Helps identify:
1. Markets with customers having low balances.
2. Populations using full HIP/SNAP allowance monthly.

### 3. Repeat Customers Across Markets
Using last 4 digits of card numbers to infer repeat visits.  
- Potential for **cohort analysis** to identify retention vs. new customers per market.  
- Requires probability modeling and year-long dataset.

---

## Current & Potential Insights
- **SUM** of SNAP used by market and overall.  
- **COUNT** of unique cards per market and overall.  
- **COUNT** of repeat vs. new customers per market.  
- **Returning customers** after X+ month gap.  
- **Effectiveness** of partner promotions by market.  
- **Reassess** Square transaction counts vs. Totilpay data.  
- Potential **HIP vs. SNAP** sales breakdown.

---

## Moving Forward
- Need **5 dedicated hours/week** for analysis (currently only 2).  
- Requesting Thursdays 9am–12pm for focused work.  
- Require monthly Totilpay reports from Operations Manager.  

---

**Table of Contents**
1. Totilpay data: potential and current insights  
2. Overview  
3. Methodology  
4. Cleaning  
5. Response Text Dictionary & Recommendations  
6. Spreadsheet Analysis  
7. Moving Forward  
