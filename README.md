# Car_price_Prediction
Used Car Price Segment Prediction and Market Analysis

1. Project Overview

This project focuses on analyzing the used car market using the Car_Details.csv dataset. The primary objective is to build a machine learning model capable of classifying a car's price into defined segments (Low, Medium, High). Additionally, the project conducts exploratory analysis to understand the trend of car mileage over manufacturing years.

2. Goals & Problem Solved

Primary Goal: Develop a robust Random Forest Classifier to accurately segment used car prices.

Business Value: Provide quick, data-driven price segment estimates for dealerships and online platforms, aiding in inventory management and pricing strategy.

Analytical Goal: Analyze and visualize the trend of average car mileage across different manufacturing years.

3. Data Collection and Acquisition

The data was sourced from the Car_Details.csv file, containing approximately 8,128 records and 13 features.

Key Acquired Variables:

selling_price (Target variable, converted to price range)

year, km_driven, fuel, transmission

mileage, engine, max_power

4. Methodology Snapshot

Step

Description

Preprocessing

Cleaned and converted units (kmpl, CC, bhp). Imputed missing values with the median. Created features like car_brand and car_age.

Target Transformation

The continuous selling_price was converted into a categorical target (Low, Medium, High) using quantile binning.

Model

Random Forest Classifier was trained to perform the price segment prediction.

Evaluation

The model was evaluated using both classification metrics (F1, Accuracy, Precision, Recall) and regression context metrics (R2, RMSE).

5. Key Performance Highlights (Test Set)

The Classification Model shows high accuracy in segmenting car prices:

Metric (Classification)

Result

Accuracy Score

0.8679

Precision Score (Weighted)

0.8711

Recall Score (Weighted)

0.8679

F1 Score (Weighted)

0.8689

Regression Metrics (Context)

R-squared (R2 Score): 0.9734

Root Mean Squared Error (RMSE): ₹141,037.63 (Approximate error in predicting the continuous price)

6. Modules/Libraries Used

The project relies on standard data science libraries:

pandas & numpy: Core data manipulation and numerical operations.

sklearn (Scikit-learn): Modeling (RandomForestClassifier), preprocessing (StandardScaler), and all metric calculations (accuracy_score, f1_score, etc.).

matplotlib.pyplot & seaborn: Visualization of trends and the Confusion Matrix.

7. Visualizations

The project generated two main visualizations:

Confusion Matrix: Shows the classification accuracy for the 'Low', 'Medium', and 'High' price segments.

Average Mileage Trend Line Graph: Illustrates the change in average car mileage across different manufacturing years.# car-price-prrediction
