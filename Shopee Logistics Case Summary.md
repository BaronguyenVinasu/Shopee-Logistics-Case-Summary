
# Shopee Logistics Case Challenge – Summary Report

---

## Executive Summary
In response to Shopee's logistical growth plan to double monthly order volume to 200 million while cutting late deliveries from 18% to 10%, this report analyzes operational performance across third-party logistics (3PLs) using four core evaluations: cost, timeliness, route complexity, and service level adherence. Recommendations are also proposed to support Shopee's scalability and reliability goals.

---

## Question 1: 3PL Fee & Lead Time Analysis

### Objective:
Compare estimated shipping fees and lead times of 3PLs across different delivery routes.

### Key Insights:
- **Shipping Carrier D** has the **lowest average shipping fee (1,794)** and **highest on-time delivery performance** (e.g., 97.63% on intra-city routes).
- **Shipping Carrier B** is the most expensive overall (avg. 1,822) and performs worse in timeliness.
- **Cross region tỉnh** and **special same region** routes have the highest fees and tend to be more delayed.
- Lead times increase significantly when one or both ends are in rural areas (up to 120 hours SLA).

### Visuals:
- Bar chart comparing estimated shipping fee per route per 3PL.
- SLA table used to benchmark delivery performance.

---

## Question 2: % Late Delivery per 3PL per Route

### Objective:
Determine late delivery patterns across 3PLs and route types.

### Key Insights:
- **Shipping Carrier D** is the most reliable: e.g., **only 2.37% late** on special same region routes.
- **Carrier B and E** consistently underperform across most routes.
- **Intra-city routes** show best overall performance across all 3PLs, while **cross-region** has the highest delay rates.

---

## Question 3: Route Mapping & Estimated Shipping Fee Calculation

### Objective:
Classify orders by route type using seller/buyer region and calculate estimated shipping fees by weight.

### Method:
- Use Area mapping (Table 1) + Route logic (Table 2) + Fee matrix (Table 3)
- Routes include: intra-city, intra-region, cross-region, special same region, etc.
- Fees increase by weight brackets and distance complexity

### Example:
> An order from Hồ Chí Minh (urban) to Hà Nội (urban) is classified as "cross region" with fee of 540 for 3-6kg package.

---

## Question 4: SLA & On-Time Classification

### Objective:
Evaluate on-time pickup, delivery, and return based on SLA thresholds.

### Method:
- If lead time ≤ SLA → "On time", else "Late"
- Rural routes and high-weight packages most likely to miss SLA
- Returns often unmeasured or delayed due to incomplete timestamps

### Performance Summary:
| Metric             | Average On-time % |
|--------------------|------------------|
| Pickup             | High (~95%)      |
| Delivery           | Varies by 3PL    |
| Return             | Incomplete Data  |

---

## Strategic Recommendations
To scale to **200M orders/month** and reduce **late delivery to 10%**, Shopee should:

1. **Incentivize High-Performing 3PLs**
   - Prioritize carriers like **Shipping Carrier D**
   - Use performance-based contract renewals

2. **Invest in Route Optimization**
   - AI-based routing for rural/complex regions
   - Dynamic 3PL selection per route

3. **Improve Forecasting & Volume Allocation**
   - Forecast peak loads to avoid delays
   - Pre-allocate volume based on historical success rates

4. **Expand Fulfillment Centers Closer to Demand**
   - Especially in underserved rural or "cross region tỉnh" areas

5. **Strengthen SLA Governance**
   - Set stricter SLAs and monitor violations
   - Provide real-time SLA dashboards to 3PLs

---

## Conclusion
Shipping Carrier D emerges as the most reliable and cost-efficient partner. Shopee can achieve its scalability and reliability goals by strategically partnering with high-performing 3PLs, optimizing logistics intelligence, and enforcing data-backed accountability standards across its supply chain.
