# Statistical Analysis of Hotel Booking Cancellations

## Project Overview

This project analyses hotel booking cancellation behaviour using statistical modelling techniques.

The objective is to identify factors associated with hotel booking cancellations and develop a logistic regression model to estimate cancellation risk.

---

## Dataset

Dataset:
https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand

The dataset contains hotel reservation records including:

- Hotel type
- Lead time
- Customer type
- Deposit type
- Market segment
- Previous cancellations
- Special requests

---

# Statistical Methods

The following methods were applied:

## Exploratory Data Analysis

Analysed:

- Cancellation distribution
- Hotel type differences
- Lead time patterns
- Deposit type behaviour

## Hypothesis Testing

### Hotel Type and Cancellation

Pearson chi-square test was used.

### Lead Time Difference

Welch independent samples t-test was applied.

## Logistic Regression Model

Binary logistic regression was used to identify booking characteristics associated with cancellation.

---

# Results and Findings

## Cancellation Rate

After preprocessing:

- Not cancelled bookings: 75,011
- Cancelled bookings: 44,195

Cancellation rate:

37.07%

---

## Hotel Type Findings

Cancellation rates:

- City Hotel: 41.8%
- Resort Hotel: 27.8%

The difference was statistically significant but the effect size was relatively weak.

---

## Lead Time Findings

Cancelled bookings had:

- Mean lead time: 144.9 days

Non-cancelled bookings had:

- Mean lead time: 80.1 days

Longer booking lead time was associated with higher cancellation risk.

---

# Logistic Regression Performance

Model evaluation:

| Metric | Result |
|---|---|
| Accuracy | 80.64% |
| Sensitivity | 59.33% |
| Specificity | 93.20% |
| Precision | 83.71% |
| AUC | 0.848 |

---

# Source Code

The complete R implementation is available here:

[hotel_booking_analysis.R](hotel_booking_analysis.R)

The code includes:

- Data cleaning
- Exploratory analysis
- Hypothesis testing
- Logistic regression
- Model evaluation

---

# Conclusion

The analysis shows that cancellation behaviour is influenced by multiple booking characteristics rather than hotel type alone.

The logistic regression model demonstrated good predictive performance, but further validation using new data is required before operational use.
