# Email-Marketing-Campaign-Performance-Analysis

## Project Background
In the dynamic digital marketing landscape, email remains a vital channel for businesses to engage audiences, drive conversions, and foster customer loyalty. With millions of emails sent daily, businesses generate extensive data on campaign performance, including open rates, click rates, conversions, and subscriber behavior. The challenge lies in transforming this data into actionable insights to optimize email strategies, enhance engagement, and maximize return on investment (ROI).

This project was undertaken to develop an Excel-based dashboard analyzing email marketing performance metrics, focusing on engagement, conversion, and audience behavior across different email types and devices. The dashboard leverages a comprehensive dataset with 20,000 rows and 12 columns: Campaign_ID, Email_ID, Subject_Line, Send_Date, Recipient_ID, Open_Rate, Click_Rate, Conversion_Rate, Unsubscribe_Rate, Bounce_Rate, Email_Type, and Device_Type. The project aims to assist the business in making data-driven decisions to enhance email campaign effectiveness and achieve strategic objectives.

### Key Insights and Recommendations Focused On:
- **Overall Campaign Performance**: Analysis of key performance indicators (KPIs) such as open rate, click rate, conversion rate, unsubscribe rate, and bounce rate to assess overall campaign success.
- **Email Campaign Progression**: Evaluation of the email funnel (sent → opened → clicked → converted) to identify drop-off points and optimize conversion paths.
- **Email Type Distribution**: Examination of the distribution of email types (Transactional, Promotional, Newsletter) to understand campaign composition and its impact on performance.
- **Engagement by Email Type**: Analysis of open, click, and conversion rates across email types to identify high-performing formats and tailor content strategies.
- **Monthly Conversion Trends**: Temporal analysis of conversion rates to uncover seasonal patterns and optimize send timing.
- **Unsubscribe Rate by Device Type**: Assessment of unsubscribe rates across devices (Desktop, Mobile, Tablet) to ensure a consistent user experience and minimize subscriber churn.

An interactive Excel dashboard was developed to visualize these focus areas, offering dynamic charts to explore campaign performance, email type effectiveness, and device-specific trends.

## Data Structure & Initial Checks
The dataset forms the backbone of the Email Marketing Campaign Performance Dashboard, structured to support detailed analysis of engagement and conversion metrics.

### Table Columns:
- **Campaign_ID**: Unique identifier for each campaign (text), ensuring traceability and enabling campaign-specific analysis.
- **Email_ID**: Unique identifier for each email (text), preventing duplication in analysis.
- **Subject_Line**: Email subject line (text), critical for assessing open rate performance.
- **Send_Date**: Date the email was sent (date), used for temporal analysis of engagement and conversions.
- **Recipient_ID**: Unique identifier for recipients (text), supporting audience segmentation.
- **Open_Rate**: Percentage of emails opened (decimal), reflecting initial engagement.
- **Click_Rate**: Percentage of opened emails clicked (decimal), measuring content relevance.
- **Conversion_Rate**: Percentage of clicked emails leading to conversions (decimal), indicating campaign effectiveness.
- **Unsubscribe_Rate**: Percentage of recipients unsubscribing (decimal), assessing audience retention.
- **Bounce_Rate**: Percentage of undelivered emails (decimal), indicating list quality and deliverability.
- **Email_Type**: Type of email (Transactional, Promotional, Newsletter; categorical), key for performance segmentation.
- **Device_Type**: Device used to open the email (Desktop, Mobile, Tablet; categorical), enabling device-specific analysis.

### Key Early Checks:
- **Data Type Validation**: Confirmed appropriate data types: Campaign_ID, Email_ID, Subject_Line, and Recipient_ID as text; Email_Type and Device_Type as categorical; Send_Date as date; Open_Rate, Click_Rate, Conversion_Rate, Unsubscribe_Rate, and Bounce_Rate as decimals.
- **Missing or Null Values**: Checked for missing data in critical columns (e.g., Open_Rate, Conversion_Rate). Handled minimal missing values by excluding incomplete records or imputing with averages where appropriate.
- **Duplicate Records**: Verified Email_ID and Recipient_ID uniqueness to eliminate duplicates that could skew metrics, removing duplicates in Excel if found.
- **Categorical Consistency**: Ensured Email_Type (e.g., only “Transactional,” not “Transaction”) and Device_Type values were standardized for accurate filtering and grouping.
- **Outlier Detection**: Inspected numeric fields (e.g., Open_Rate, Conversion_Rate) for outliers that might indicate data errors or anomalies, flagging them for review.
- **Metric Validation**: Verified calculated metrics (e.g., Open_Rate = Opened/Sent) aligned with reported values, noting a slight discrepancy (25.17% calculated vs. 25.11% reported) likely due to rounding.
- **Date Consistency**: Ensured Send_Date was uniformly formatted and covered the 2020–2025 period for accurate temporal analysis.

# Executive Summary

### Overview of Findings
The email marketing campaign, spanning 2020–2025 with 20,000 emails sent, demonstrates solid performance with a 25.11% open rate and a 10.04% click rate, though the 2.74% conversion rate suggests opportunities to strengthen the conversion funnel. Low unsubscribe (1.00%) and bounce rates (2.02%) reflect high audience retention and deliverability. The email type distribution is nearly balanced (Transactional: 33.46%, Promotional: 33.37%, Newsletter: 33.17%), indicating a diversified strategy. Promotional emails slightly outperform others in click (10.06%) and conversion rates (2.77%), while transactional emails lag in open rates (25.04%). Monthly conversion rates remain stable (2.66%–2.82%), with peaks in April and December (2.82%) suggesting seasonal opportunities. Unsubscribe rates are consistent across devices (Desktop: 1.007%, Mobile: 1.003%, Tablet: 0.999%), confirming a uniform user experience.
![Image](https://github.com/user-attachments/assets/e5dc59f8-ce4b-4447-bef6-f4243e156e11)

## Insights Deep-Dive
**Email Campaign Progression**

The email marketing campaign, with 20,000 emails sent over 2020–2025, reveals a robust yet improvable performance profile. The campaign achieved a 25.11% open rate, translating to 5,033 emails opened, which aligns with industry benchmarks (20–30%) and indicates moderate success in capturing audience attention. However, the significant drop from sent to opened emails (74.89% not opened) suggests that subject lines or send timing may not fully resonate with recipients, presenting an opportunity for optimization. Progressing through the funnel, the 10.04% click rate (2,012 clicks) reflects that 40% of openers engaged with the content, signaling relevant email content but potential weaknesses in call-to-action (CTA) clarity or appeal. The conversion rate of 2.74% (590 conversions) is a critical bottleneck, as only 29.32% of clickers completed the desired action, highlighting issues in post-click experiences, such as landing page design or offer relevance. 
 ![Image](https://github.com/user-attachments/assets/7703f3c4-65f6-46af-872c-2fe8204778fd)

**Email Type Distribution**

The near-perfect equilibrium between transactional (33.46%), promotional (33.37%), and newsletter (33.17%) emails reflects a strategically balanced approach to audience communication. This distribution mitigates reliance on any single email category, reducing engagement volatility risks. The parity suggests intentional resource allocation across: 1) Relationship-building newsletters, 2) Revenue-driving promotional offers, and 3) Operational transactional messages—creating a holistic communication ecosystem. Notably, the absence of category dominance prevents audience fatigue while allowing synergistic cross-promotion opportunities (e.g., embedding promotional CTAs in transactional emails).
![Image](https://github.com/user-attachments/assets/396fa145-aa58-4baf-9117-e450b97b6801)
  
**Engagement by Email Type**

The engagement metrics reveal nuanced differences across email types. Promotional emails lead with a 25.14% open rate, 10.06% click rate, and 2.77% conversion rate, likely driven by compelling offers or targeted CTAs that resonate with recipients. Newsletters perform closely behind, with a 25.15% open rate, 10.00% click rate, and 2.74% conversion rate, suggesting consistent but unremarkable engagement that could benefit from more dynamic content. Transactional emails, surprisingly, trail with a 25.04% open rate, 10.05% click rate, and 2.72% conversion rate, an unexpected underperformance given their typically high relevance (e.g., order confirmations). This lower open rate for transactional emails may point to generic or uninspiring subject lines, warranting further investigation into subject line optimization or send timing.
 ![Image](https://github.com/user-attachments/assets/3a8e51cf-8d26-43ef-ad8f-4eda4dacf2a3)

**Monthly Conversion Trends**

Temporal analysis of conversion rates over 2020–2025 shows remarkable stability, ranging from 2.66% in February to 2.82% in April and December, with a tight variance of 0.16%. The peaks in April and December likely reflect seasonal trends, such as spring promotions or holiday sales, which drive higher audience intent to convert. Conversely, the dips in February (2.66%) and November (2.67%) may indicate audience fatigue, competing holidays, or suboptimal campaign timing, suggesting a need to explore external factors or adjust send schedules. 
![Image](https://github.com/user-attachments/assets/b7c85080-adc9-4631-a246-a3277d408bf2)

**Unsubscribe Rate by Devices**

Device-level unsubscribes show statistically insignificant variation—desktop (1.007%), mobile (1.003%), and tablet (0.999%)—effectively eliminating device-specific user experience issues as primary attrition drivers. This near-uniformity instead points toward systemic factors: 1) Global content relevance gaps, 2) Uniform frequency sensitivity across devices, or 3) List segmentation deficiencies. The absence of mobile-specific attrition (typically the highest due to rendering issues) confirms responsive design effectiveness. However, desktop’s marginally higher rate may hint at multi-device users formally unsubscribing when accessing preference centers on larger screens.
![Image](https://github.com/user-attachments/assets/b50bb917-303d-45ff-b95d-80dd36cff728)
  
### Critical Opportunities & Recommendations  
1. **Reduce Unsubscribes**:  
   - Implement preference centers for frequency control.  
   - Segment lists to avoid irrelevant sends (e.g., inactive users).  

2. **Optimize Mid-Year Conversions**:  
   - Run summer-specific promotions (June-August).  
   - A/B test subject lines/content during November slump.  

3. **Leverage Transactional Emails**:  
   - Test adding promotional CTAs (e.g., "While you’re here, check this out!").  

4. **Improve List Health**:  
   - Clean inactive emails to reduce bounce rates.  
   - Re-engagement campaign for subscribers not opening in 6+ months.  

5. **Capitalize on High Intent**:  
   - Retarget clicked-but-didn’t-convert users with tailored offers.  
