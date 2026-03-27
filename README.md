# Zomato Delivery Ratings Analysis 

Delivery performance analysis of Zomato's e-commerce data, India's Top 1 delivery service company, analyzing riders' ratings for 
actionable business insights on maintaining high-quality delivery performance. 

## Analysis Overview 
- Zomato is India's Top 1 delivery service company, which provides a variety of food services such as menu information, user recommendations, food delivery, and table reservations, etc. The analysis of delivery ratings of Zomato data aims to evaluate riders' performance on deliveries under different circumstances, such as weather, traffic levels, or area types, to create statistical or ML models to predict delivery ratings, and provide actionable business insights for riders' delivery performance. 

## Dataset 
- The analysis uses the **Zomato Delivery Operations Analytics Dataset** ([Kaggle](https://www.kaggle.com/datasets/saurabhbadole/zomato-delivery-operations-analytics-dataset))

## Tech Stack and Methods 

**Stack:**

- **Data Analysis:** `Python` `Pandas` `NumPy`,
- **Visualization:** `Seaborn` `Matplotlib`,
- **Statistics & ML:** `StatsModels` `Scipy` `Sklearn` 

**Methods:** 

- **Data Preprocessing:**
  -   Detection of missing values, remedial methods for missing values: deletion and imputation, creating new variables for EDA
- **Exploratory Data Analysis:**
  - Describing the dataset: statistical summaries, visualization of ratings, delivery times, and factors of ratings. Concatenation of a subset of the dataset for further analysis with modeling
- **Modeling for prediction**
  -  Statistical modeling for prediction of ratings with new subset data of the original dataset: Linear model, ML models comparison: Linear Model and Random Forest, Model evaluation

## Analysis 
- Evaluate
  - Overall order ratings
  - Distinct riders' ratings
  - Riders with good ratings and bad ratings
  - Occasions of good ratings and bad ratings
  - Comparison of good ratings and bad ratings 
- Evaluate
  - Overall delivery times
  - Distinct rider's average delivery time
  - Comparison of average delivery times under different circumstances
- Linear model to predict
  - rider ratings under different delivery times

## Summary of Findings
- Among about 45000 orders, 140 orders have less than or equal to 3 order ratings, 105 orders from non-peak time, sunny, and low traffic conditions, and 35 orders from unknown delivery time, fog, and low traffic conditions.
- 105 orders with less than or equal to 3-rating have a significantly longer average delivery time, 37 minutes, compared to the 19-minute average delivery time of 311 orders with 5-rating, .
- On sunny and low-traffic days, the rider ratings dropped from the lowest 4.5 to 3.5 or under when the delivery times exceeded 30 minutes.
- Based on the linear model to predict riders' ratings on sunny and low traffic conditions, the deliveries made under 30-minute period have 2.26 higher ratings than the deliveries made over 30-minute period.
- For every 1-minute increase after 30-minute period, the rider ratings begin to drop by 0.09, with an expected rider rating of 3.19 at a 37-minute delivery time.  
- If a rider aims for 4.5 ratings, riders are expected to keep the delivery time of about 22 minutes on sunny and low traffic conditions.
  
## Key Recommendations 
- If the delivery time of a rider can be improved from 37 minutes to 30 minutes, which is about 23% improvement, we can expect an improvement in riders' ratings from 3.19 to 3.8, which is about 16% improvement.

- If a rider aims for 4.5 ratings, riders are expected to keep the delivery time of about 22 minutes on sunny and low traffic conditions.

## EDA
