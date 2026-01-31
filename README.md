# Overall Dataset Analysis (Understanding the trends of data)

## Overview
This project analyzes a dataset by merging **orders**, **users**, and **restaurants** into a **final dataset** (`final_dataset.csv`). It serves as the source of truth for studying order trends, revenue, user behavior, and restaurant performance.

## Repository Structure
INNOMATICS HACKATHON/
│
├── datasets/ # Raw and final data files
│ ├── orders.csv
│ ├── users.json
│ ├── restaurants.sql
│ └── final_dataset.csv
│
├── notebook/ # Kaggle notebook with analysis
│ └── nootebook.ipynb
│
├── README.md
└── .gitignore

## Analysis Steps
1. **Load and merge datasets** using LEFT JOINs:
   - `orders.user_id → users.user_id`
   - `orders.restaurant_id → restaurants.restaurant_id`
   merged majorly based on USERID.
2. **Feature engineering**:
   - Convert order dates, extract quarter/month
   - Create rating ranges
   - Calculate order counts and average order values
3. **Insights**:
   - City-wise and cuisine-wise revenue
   - Gold vs Regular membership behavior
   - High-value users and restaurants
   - Seasonal trends and top-performing quarters
4. **Export final dataset**
   
## Key Insights

1. Gold members contribute disproportionately to revenue

2. Top cities and cuisines can be identified by total revenue and average order value

3. High-rated restaurants attract more orders

4. The dataset enables user behavior and restaurant performance analysis

## How to Run

1. Open food_delivery_analysis.ipynb in VS Code, Jupyter, or Kaggle
2. Ensure the data/ 
               folder is present, 
3. Run all cells sequentially to reproduce the merged dataset and analyses.

Overall, this project demonstrates how integrating transactional, user, and restaurant data can drive actionable insights for decision-making.

## **Use Case**

This dataset and analysis can be applied to:

1. **Business Strategy** – Identify top cities, cuisines, and premium customers to focus marketing and expansion efforts.

2. **Customer Segmentation** – Target Gold members for promotions, loyalty programs, or personalized offers.

3. **Restaurant Performance** – Assess which restaurants generate the most revenue and maintain high ratings.

4. **Demand Forecasting** – Predict peak quarters and seasons for operational planning and resource allocation.

5. **Decision Support** – Use revenue and order patterns to optimize menu, pricing, and delivery strategies.
