# Hotel_Booking_Analysis
Predictive model to forecast hotel booking cancellations. Uses logistic regression and handles imbalanced data to optimize occupancy &amp; minimize revenue loss. Evaluates with F1, Precision, Recall, &amp; Kappa.

Project Description for GitHub Repository: Hotel Booking Cancellation Prediction

This repository contains the analysis and predictive modeling work for forecasting hotel booking cancellations.

Problem: Hotel booking cancellations pose a significant challenge for revenue management and operational planning in the hospitality industry. Accurately predicting which bookings are likely to be canceled allows hotels to implement proactive strategies, such as targeted re-engagement campaigns or dynamic overbooking, to optimize occupancy and minimize revenue loss.

Objective: To develop a robust machine learning model capable of identifying bookings at high risk of cancellation based on historical booking patterns and customer information.

Methodology & Key Highlights:

    Data Preprocessing: Utilized a comprehensive dataset of hotel booking records, involving data cleaning and preparation steps to ensure data quality.
    Predictive Modeling (Logistic Regression): Implemented a logistic regression model to predict the binary outcome of "booking status" (canceled vs. not canceled).
    Addressing Imbalanced Data: The dataset exhibited a significant class imbalance (fewer cancellations than confirmed bookings). To mitigate this challenge and build a more effective model, techniques such as stratified sampling were employed during data splitting.
    Comprehensive Model Evaluation: Performance was rigorously assessed using a suite of metrics crucial for imbalanced classification tasks:
        Accuracy: Overall correctness.
        Sensitivity (Recall): Ability to correctly identify actual cancellations (minimizing missed cancellations).
        Specificity: Ability to correctly identify non-cancellations.
        Precision (Positive Predictive Value): Reliability of cancellation predictions (minimizing false alarms).
        F1-Score: Harmonic mean of Precision and Recall, providing a balanced measure of performance.
        Kappa Coefficient: Assesses agreement between predictions and actuals, correcting for chance agreement, particularly useful for imbalanced datasets.
        No Information Rate (NIR): Baseline performance benchmark.
    Threshold Optimization: Explored various classification thresholds beyond the default 0.5 to find an optimal balance between Precision and Recall, specifically focusing on maximizing the F1-Score for better minority class prediction. This involved analyzing Precision-Recall curves and identifying the threshold that best suits the business need for balancing false positives and false negatives.

Impact & Learning:

This project demonstrates the process of building, evaluating, and refining a predictive model for a real-world business problem. It highlights the importance of:

    Understanding and addressing data imbalance.
    Selecting appropriate evaluation metrics for specific business goals.
    Optimizing model performance through threshold adjustment to meet practical operational requirements.
    Leveraging R for data analysis, modeling, and comprehensive performance reporting.

Tools: R, RStudio, caret, ROCR, lessR (for model training and evaluation).
