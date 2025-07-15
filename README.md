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
![Image](https://github.com/user-attachments/assets/170c5e9f-a775-4d1b-9f3a-a6dda93813d6)

## Insights Deep-Dive
**Email Campaign Progression**

The email marketing campaign, with 20,000 emails sent over 2020–2025, reveals a robust yet improvable performance profile. The campaign achieved a 25.11% open rate, translating to 5,033 emails opened, which aligns with industry benchmarks (20–30%) and indicates moderate success in capturing audience attention. However, the significant drop from sent to opened emails (74.89% not opened) suggests that subject lines or send timing may not fully resonate with recipients, presenting an opportunity for optimization. Progressing through the funnel, the 10.04% click rate (2,012 clicks) reflects that 40% of openers engaged with the content, signaling relevant email content but potential weaknesses in call-to-action (CTA) clarity or appeal. The conversion rate of 2.74% (590 conversions) is a critical bottleneck, as only 29.32% of clickers completed the desired action, highlighting issues in post-click experiences, such as landing page design or offer relevance. 
![Image](https://github.com/user-attachments/assets/2ef5603a-04ac-4b7a-8ac3-f3b184fd6c43)  

**Email Type Distribution**

The near-equal distribution of email types—Transactional (33.46%), Promotional (33.37%), and Newsletter (33.17%)—reflects a balanced campaign strategy that caters to diverse audience needs, from operational communications to promotional offers and informational content.
![Image](https://github.com/user-attachments/assets/8515c733-09d3-4dca-a2cd-8a1222afcb0d)

**Engagement by Email Type**

The engagement metrics reveal nuanced differences across email types. Promotional emails lead with a 25.14% open rate, 10.06% click rate, and 2.77% conversion rate, likely driven by compelling offers or targeted CTAs that resonate with recipients. Newsletters perform closely behind, with a 25.15% open rate, 10.00% click rate, and 2.74% conversion rate, suggesting consistent but unremarkable engagement that could benefit from more dynamic content. Transactional emails, surprisingly, trail with a 25.04% open rate, 10.05% click rate, and 2.72% conversion rate, an unexpected underperformance given their typically high relevance (e.g., order confirmations). This lower open rate for transactional emails may point to generic or uninspiring subject lines, warranting further investigation into subject line optimization or send timing.
![Image](https://github.com/user-attachments/assets/311e1c12-74aa-40c3-915e-a11a78f0c84f) 

**Monthly Conversion Trends**

Temporal analysis of conversion rates over 2020–2025 shows remarkable stability, ranging from 2.66% in February to 2.82% in April and December, with a tight variance of 0.16%. The peaks in April and December likely reflect seasonal trends, such as spring promotions or holiday sales, which drive higher audience intent to convert. Conversely, the dips in February (2.66%) and November (2.67%) may indicate audience fatigue, competing holidays, or suboptimal campaign timing, suggesting a need to explore external factors or adjust send schedules. 
![Image](https://github.com/user-attachments/assets/11e33348-dea6-4517-bfdf-979c7dcacdf8)

**Unsubscribe Rate by Devices**

The unsubscribe rate analysis by device type—Desktop (1.007%), Mobile (1.003%), and Tablet (0.999%)—reveals near-identical performance, with a negligible 0.008% range. This consistency indicates a seamless user experience across devices, with tablets’ slightly lower unsubscribe rate potentially reflecting a more intentional or engaged audience, though the difference is minimal and does not signal device-specific issues.
![Image](https://github.com/user-attachments/assets/c913b60a-9a6c-4e2f-ac60-7987416b1e0d)


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
