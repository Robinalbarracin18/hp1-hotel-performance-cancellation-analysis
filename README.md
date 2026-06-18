# HP1 Hotel Performance & Cancellation Analysis

## Business Overview

This project analyzes hotel booking data to understand booking behavior, cancellation risk, average daily rate patterns, seasonality, and customer-related performance indicators.

The goal is to transform raw hotel reservation data into business insights that can help a hotel improve revenue management, reduce cancellation risk, and identify high-value booking patterns.

This project combines exploratory data analysis, data cleaning, dashboarding, and basic predictive modeling.

---

## Business Objective

The main objective of this project is to analyze hotel performance and identify the main factors associated with:

* reservation cancellations,
* booking lead time,
* average daily rate,
* seasonality,
* hotel type differences,
* customer and market segment behavior.

The analysis is designed to support better commercial and operational decisions for hotel management.

---

## Key Business Questions

* What is the overall cancellation rate?
* Which hotel type has higher cancellation risk?
* How does lead time affect cancellation behavior?
* Which market segments show higher cancellation risk?
* How does ADR change across months and hotel types?
* Which periods show stronger pricing opportunities?
* Can reservation data be used to explore cancellation prediction?

---

## Tools Used

* **Python**: data cleaning, exploratory analysis, and modeling.
* **Pandas**: data manipulation and aggregation.
* **Matplotlib / Seaborn**: data visualization.
* **Scikit-learn**: exploratory regression and classification models.
* **Power BI**: dashboard creation and business visualization.
* **Word / PDF**: executive reporting and business conclusions.
* **GitHub**: project documentation and portfolio publication.

---

## Dataset

The project uses a hotel booking dataset containing reservation-level information.

Main variables analyzed include:

* `hotel`
* `is_canceled`
* `lead_time`
* `arrival_date_month`
* `market_segment`
* `distribution_channel`
* `customer_type`
* `adr`
* `reserved_room_type`
* `assigned_room_type`
* `booking_changes`
* `required_car_parking_spaces`
* `total_of_special_requests`
* `reservation_status`

The dataset includes information about booking status, hotel type, customer profile, booking timing, pricing, and operational reservation details.

---

## Project Workflow

```text
Raw Hotel Booking Data
   ↓
Data Cleaning and Preparation
   ↓
Exploratory Data Analysis
   ↓
Cancellation Analysis
   ↓
ADR and Seasonality Analysis
   ↓
Exploratory Predictive Modeling
   ↓
Power BI Dashboard
   ↓
Executive Conclusions
```

---

## Main Dashboard Metrics

| Metric            |      Result |
| ----------------- | ----------: |
| Average ADR       |      101.97 |
| Cancellation rate |      37.08% |
| Average lead time | 104.11 days |

---

## Dashboard Preview

![Dashboard Preview](Images/dashboard_preview.png)

---

## Executive Summary

![Executive Summary](Images/executive_summary.png)

---

## Key Insights

### 1. Cancellation risk is a major business issue

The dashboard shows a general cancellation rate of approximately **37.08%**.

This means that more than one out of every three bookings may be canceled, creating uncertainty in revenue planning and room availability management.

**Business interpretation:**
The hotel should monitor cancellation behavior continuously and apply differentiated policies depending on reservation risk.

---

### 2. Lead time is strongly related to cancellation behavior

Reservations made with greater anticipation tend to show higher cancellation risk.

Long lead times increase uncertainty because customer plans can change before the arrival date.

**Business interpretation:**
Bookings made far in advance should be managed with stronger confirmation strategies, partial prepayment, or differentiated cancellation policies.

---

### 3. ADR shows seasonal behavior

The average daily rate is higher in specific months, especially during stronger demand periods.

This indicates that pricing opportunities are not constant throughout the year.

**Business interpretation:**
The hotel should avoid unnecessary discounts during high-demand months and adjust prices according to seasonality, hotel type, and customer segment.

---

### 4. Hotel type affects both ADR and cancellation risk

City Hotel and Resort Hotel behave differently in terms of pricing and cancellation patterns.

Some periods show higher ADR opportunities, while others show higher cancellation exposure.

**Business interpretation:**
Revenue strategies should not be identical for both hotel types. Each hotel type requires a different pricing and cancellation management approach.

---

### 5. Market segments show different cancellation patterns

Some market segments generate higher cancellation rates than others.

This suggests that not all booking sources or customer groups have the same commercial quality.

**Business interpretation:**
The hotel should evaluate segments not only by booking volume, but also by cancellation risk and average value.

---

## Cancellation Analysis

The cancellation analysis focuses on identifying which booking characteristics are associated with higher risk.

Main dimensions analyzed:

* cancellation by hotel type,
* cancellation by market segment,
* cancellation by customer type,
* cancellation by lead time,
* cancellation by reservation behavior.

Supporting visualizations:

![Hotel Type Cancellation](Images/hotel_type_cancellation.png)

![Lead Time Cancellation](Images/lead_time_cancellation.png)

![Market Segment Cancellation](Images/market_segment_cancellation.png)

---

## ADR and Seasonality Analysis

ADR was used as a proxy for booking value.

The analysis evaluates how average daily rate changes across months and hotel types.

Supporting visualization:

![ADR Seasonality](Images/adr_seasonality.png)

**Important note:**
ADR does not represent total revenue by itself. It does not fully capture length of stay, cancellation risk, distribution costs, or total booking value. However, it is useful for analyzing pricing behavior and revenue opportunities.

---

## Predictive Modeling

The project includes exploratory machine learning models to evaluate whether hotel reservation data can help predict:

* booking cancellation,
* ADR behavior.

The modeling work is exploratory and should not be considered a production-ready prediction system.

The purpose of this section is to test whether variables such as lead time, customer type, market segment, and booking characteristics contain useful predictive signals.

---

## Business Recommendations

### 1. Apply differentiated cancellation policies

The hotel should not use the same cancellation policy for every booking.

Possible actions:

* stricter policies for high-risk bookings,
* more flexible conditions for reliable customer types,
* additional confirmation steps for long lead-time reservations.

---

### 2. Use partial prepayment for high-risk advance bookings

Reservations made with high lead time may benefit from partial prepayment.

Possible actions:

* request 20%–30% prepayment for selected high-risk bookings,
* apply this strategy during high-demand periods,
* use it carefully to avoid discouraging reliable customers.

---

### 3. Adjust pricing by season and hotel type

ADR changes across months and hotel types.

Possible actions:

* increase prices during high-demand periods,
* reduce unnecessary discounts in strong months,
* apply different strategies for City Hotel and Resort Hotel.

---

### 4. Monitor high-risk market segments

Some segments may bring volume but also higher cancellation risk.

Possible actions:

* evaluate each segment by cancellation rate and ADR,
* prioritize segments with healthier value-risk balance,
* review commercial agreements with high-risk segments.

---

## Repository Structure

```text
HP1_Hotel_Performance_Cancellation_Analysis/
├── Data/
│   ├── hotel_bookings.csv
│   └── hotel_bookings_cleaned_from_HP1.csv
├── Notebooks/
│   ├── hotel_performance_analysis.ipynb
│   └── hotel_regression_models.ipynb
├── Dashboard/
│   └── hotel_performance_dashboard.pbix
├── Reports/
│   ├── hotel_business_report.docx
│   └── cancellation_analysis_report.pdf
├── Images/
│   ├── dashboard_preview.png
│   ├── executive_summary.png
│   ├── hotel_type_cancellation.png
│   ├── lead_time_cancellation.png
│   ├── adr_seasonality.png
│   └── market_segment_cancellation.png
└── README.md
```

---

## File Size Notes

Some files may not be included if they exceed GitHub upload limits.

If the raw dataset or Power BI file is not available in the repository, the project is still documented through:

* notebooks,
* dashboard screenshots,
* executive report,
* cancellation analysis report,
* README documentation.

---

## Limitations

This project is a portfolio case study and has some limitations:

* ADR is used as a proxy for value, but it is not the same as total revenue.
* The dataset does not include real profit margins.
* Distribution costs are not included.
* External factors such as local events, competitor pricing, and marketing campaigns are not included.
* Predictive models are exploratory and not ready for operational use.
* Some business conclusions would require validation with real hotel management data.

---

## Future Improvements

Future versions of this project could include:

* more advanced cancellation prediction,
* customer segmentation,
* revenue forecasting,
* room revenue estimation using length of stay,
* channel profitability analysis,
* comparison between confirmed revenue and lost revenue,
* deployment of an interactive dashboard online.

---

## Final Conclusion

This project shows how hotel booking data can be used to identify cancellation risk, pricing opportunities, and business patterns.

The analysis found that cancellation behavior, lead time, ADR seasonality, hotel type, and market segment are important factors for hotel performance.

By combining Python, Power BI, exploratory modeling, and executive reporting, this project provides a business-oriented view of hotel operations and revenue management opportunities.

---

## Author

**Robin Albarracín**
Data Analytics Student | SQL | Excel | Power BI | Python
Chile
