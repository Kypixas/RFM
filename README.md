# RFM Analysis - Graded Task Overview

## Project Description
This project focuses on performing RFM (Recency, Frequency, Monetary) analysis on a dataset from the `rfm` table in the `turing_data_analytics` BigQuery database. The goal is to identify customer segments based on their purchasing behavior and derive actionable insights to guide marketing strategies.

---

## **Key Objectives**

1. **Data Filtering**:
   - Use only one year of data from `2010-12-01` to `2011-12-01`.
   - Calculate recency from the reference date `2011-12-01`.

2. **RFM Calculation**:
   - Calculate **Recency**, **Frequency**, and **Monetary Value**.
   - Use SQL and BigQuery's `APPROX_QUANTILES` function to segment these values into quartiles (R, F, M scores from 1 to 4).
   - Validate results with the `rfm_value` and `rfm_quantiles` tables.

3. **RFM Scoring**:
   - Combine R, F, and M scores into an overall RFM score.
   - Segment customers into categories:
     - Best Customers
     - Loyal Customers
     - Big Spenders
     - Lost Customers
     - Others

4. **Visualization**:
   - Create a dashboard in Tableau/Power BI/Looker Studio to present RFM scores, customer segments, and monetary value distribution.

5. **Insights and Recommendations**:
   - Provide actionable recommendations based on customer segmentation and revenue contributions.

---

### **Visualizations**
1. **RFM Score Distribution**:
   - Bar charts showing the count of customers in each RFM segment.
   ![image](https://github.com/user-attachments/assets/438124ca-685d-437e-8fed-551b43bfaf9b)

2. **Revenue Contribution by Segment**:
   - Pie chart displaying monetary value associated with each segment.
     ![image](https://github.com/user-attachments/assets/1e12197c-12c0-46fb-8254-35e0f0e13c3d)

## **Insights and Analysis**
---
### **Key Findings**
1. **Customer Segments**:
   - **Champions** and **Loyal Customers** form the majority of the customer base, indicating strong engagement and high value.
   - Segments like **Dormant** and **Customers Needing Attention** highlight opportunities for re-engagement to reduce attrition.
   - **Promising** and **Potential Loyalists** offer potential for growth if nurtured effectively.

2. **Revenue Distribution**:
   - The **Champions** segment alone contributes significantly to revenue. Retaining this group is critical.
   - **Loyal Customers** are another substantial revenue source. Enhanced engagement could increase their value further.
   - Segments like **Potential Loyalists** have growth potential and warrant targeted efforts.

3. **At-Risk Segments**:
   - **Dormant** and **At-Risk** customers highlight the need for improved retention strategies.

---

## **Recommendations**

1. **Retention**:
   - Prioritize "Champions" by offering rewards, personalized offers, and exclusive privileges.
   - Create loyalty programs to maintain their high spending levels.

2. **Growth Stimulation**:
   - Encourage "Loyal Customers" and "Potential Loyalists" to increase purchase frequency through:
     - Targeted promotions.
     - Gamification strategies.

3. **Re-engagement**:
   - Focus on "At-Risk" and "Customers Needing Attention" with activation campaigns:
     - Provide limited-time discounts.
     - Send personalized email reminders.

4. **Long-Term Strategy**:
   - Develop predictive models to identify at-risk customers earlier.
   - Monitor customer movement across segments to measure the effectiveness of strategies.

---


---

## **Technology Stack**
- **Data Extraction and Analysis**: SQL (BigQuery)
- **Visualization**: Tableau 

---

