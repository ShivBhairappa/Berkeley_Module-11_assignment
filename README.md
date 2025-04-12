Used Car Price Analysis
Project Overview
This project analyzes a dataset of 426,000+ used cars originally sourced from Kaggle. The goal is to determine what factors influence the price of a used car, providing actionable insights to a used car dealership aiming to optimize its inventory and pricing strategy.
CRISP-DM Framework
1. Business Understanding
Used car dealerships want to understand what makes a used car more or less valuable. By identifying key features that affect price, they can better acquire and price inventory.
2. Data Understanding
•	Dataset: ~426K used car listings
•	Key features: price, year, manufacturer, model, condition, fuel, odometer, transmission, drive, type, etc.
•	Issues Identified: Missing values in several columns, particularly cylinders, condition, and paint_color.
3. Data Preparation
•	Removed entries with missing or zero price
•	Calculated car age as 2025 - year
•	Selected relevant features for analysis
•	Sampled 10,000 rows for modeling and exploratory analysis
4. Modeling
We applied regression models including:
•	Linear Regression
•	Decision Tree Regressor
•	Random Forest Regressor
Performance was evaluated using R^2 and MAE.
5. Evaluation
Key insights:
•	Newer cars (lower car_age) strongly correlate with higher price
•	Lower mileage (odometer) is also positively correlated with price
•	Transmission type, drive type, and condition affect pricing
•	Manufacturer and vehicle type (e.g., SUV, truck) also play significant roles
6. Deployment
Deliverables include:
•	This README with summary findings
•	A Google Colab notebook containing EDA, visualizations, and model code
Recommendations for Used Car Dealerships
•	Prioritize inventory with low mileage and recent model years
•	SUVs and trucks tend to retain higher value
•	Automatic transmissions and clean titles are valued higher by consumers
•	Consider regional preferences (available via state) when pricing
Files
•	vehicles.csv: Sample data for quick modeling
•	used_car_analysis.ipynb: Colab notebook for analysis and modeling

