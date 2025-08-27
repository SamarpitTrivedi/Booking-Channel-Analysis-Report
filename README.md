# Booking Channel Analysis Project

![Project Status](https://img.shields.io/badge/status-Completed-brightgreen)
![Python Version](https://img.shields.io/badge/python-3.11-blue)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-notebook-orange)
![Pandas](https://img.shields.io/badge/pandas-1.6-green)
![Seaborn](https://img.shields.io/badge/seaborn-0.12-purple)
![Last Update](https://img.shields.io/badge/last%20update-August%2028%2C%202025-blue)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

## Overview
This project provides a comprehensive data-driven analysis of a hotel booking dataset to uncover key business insights, identify booking trends, and propose actionable strategies. Insights are intended to support strategic decision-making for revenue optimization and customer retention.

---

## Table of Contents
1. [Problem Statement](#problem-statement)  
2. [Technologies Used](#technologies-used)  
3. [Repository Structure](#repository-structure)  
4. [Dataset](#dataset)  
5. [Methodology](#methodology)  
6. [Key Findings](#key-findings)  
7. [Business Recommendations](#business-recommendations)  
8. [How to Run the Project](#how-to-run-the-project)  
9. [Future Work](#future-work)  

---

## Problem Statement
<details>
<summary>Click to expand</summary>

The core objectives of this analysis were to:

- **Identify Key Observations**: Discover trends in booking volumes, cancellation rates, and channel performance.  
- **Root Cause Analysis**: Understand factors contributing to cancellations and why certain channels or property types outperform others.  
- **Business Recommendations**: Provide actionable strategies to minimize cancellations, improve profitability, and optimize pricing and channel distribution.  

</details>

---

## Technologies Used
<details>
<summary>Click to expand</summary>

- **Python**: Primary programming language for analysis.  
- **Pandas**: Data cleaning, preparation, and manipulation.  
- **NumPy**: Efficient numerical operations.  
- **Matplotlib & Seaborn**: Data visualization and reporting.  

</details>

---

## Repository Structure
<details>
<summary>Click to expand</summary>

- **[Booking Channel Analysis Report.pdf](Booking%20Channel%20Analysis%20Report.pdf)**: Final report summarizing methodology, key findings, and business recommendations.  
- **main.ipynb**: Jupyter Notebook containing all Python code for data cleaning, EDA, visualizations, and insights.  
- **README.md**: Project overview and instructions.  

</details>

---

## Dataset
<details>
<summary>Click to expand</summary>

Key columns used in the analysis:

- **Customer & Property**: `customer_id`, `property_id`, `city`, `star_rating`  
- **Booking Details**: `booking_date`, `check_in_date`, `check_out_date`, `lead_time`, `num_rooms_booked`, `room_type`, `stay_type`, `booking_channel`, `channel_of_booking`  
- **Financials**: `booking_value`, `costprice`, `markup`, `selling_price`, `refund_amount`  
- **Transactional Data**: `payment_method`, `refund_status`, `cashback`, `coupon_redeem`, `Coupon Used?`, `booking_status`, `is_canceled`  

</details>

---

## Methodology
<details>
<summary>Click to expand</summary>

1. **Data Cleaning & Preparation**: Created `is_canceled` flag, handled missing values, removed duplicates, and converted date columns.  
2. **Exploratory Data Analysis (EDA)**: Generated descriptive statistics and calculated key metrics like overall cancellation rate (~20.2%).  
3. **Data Wrangling & Transformation**: Created bins for `lead_time`, extracted day-of-week, and used pivot tables to analyze cancellations and booking values.  
4. **Visualization & Reporting**: Bar charts, line plots, and heatmaps highlight booking patterns and support insights.  

</details>

---

## Key Findings
<details>
<summary>Click to expand</summary>

- **Booking Channels**: OTAs dominate volume but have higher cancellations; direct bookings are more stable.  
- **Cancellation Behavior**:
  - **Day of Week**: Highest cancellations on Friday (5.1%) and Monday (4.3%).  
  - **Lead Time**: Peaks in last-minute and 12–18 day advance bookings.  
- **Property & Room Types**:
  - Star rating and room type affect cancellations and revenue patterns.  
  - Standard rooms have highest booking volumes; premium rooms show seasonal peaks.  

</details>

---

## Business Recommendations
<details>
<summary>Click to expand</summary>

- **Reduce Cancellations**:
  - Implement dynamic, tiered cancellation policies.  
  - Offer incentives for non-refundable bookings.  
  - Target high-risk segments with reminders/promotions.  

- **Increase Profitability**:
  - Promote direct bookings via campaigns.  
  - Upsell/cross-sell services during booking.  
  - Optimize OTA commissions based on performance.  

- **Optimize Pricing & Channel Strategy**:
  - Apply dynamic pricing models based on demand and lead time.  
  - Introduce seasonal packages and long-stay offers.  

</details>

---

## How to Run the Project
<details>
<summary>Click to expand</summary>

1. Clone the repository:  
   ```bash
   git clone <repository-url>
Install required libraries:

bash
Copy code
pip install pandas numpy matplotlib seaborn
Open main.ipynb in Jupyter Notebook or JupyterLab.

Run all cells to replicate the analysis, visualizations, and insights.

</details>
Future Work
<details> <summary>Click to expand</summary>
Predictive Modeling: Build ML models to predict cancellations.

Customer Segmentation: Use clustering to tailor marketing campaigns.

Expanded Analysis: Incorporate external data such as local events or flight information to refine seasonal trend insights.

</details> ```
