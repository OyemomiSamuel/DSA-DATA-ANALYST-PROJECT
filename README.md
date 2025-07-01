# DSA-DATA-ANALYST-PROJECT

 Case Study 1: Amazon Product Review Analysis - Using pivot tables, helper columns, and calculated columns to analyze the data and provide insights based on specific business questions.


## 📚 Table of Contents

- [DSA-DATA-ANALYST-PROJECT](#dsa-data-analyst-project)
- [COMPREHENSIVE DOCUMENTATION OUTLINING EACH STAGE AND METHOD APPLIED DURING THE PROJECT WORKFLOW](#comprehensive-documentation-outlining-each-stage-and-method-applied-during-the-project-workflow)
  - [Project Overview](#project-overview)
  - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
  - [Data Cleaning and Preparation](#data-cleaning-and-preparation)
  - [Research Questions, Approach, Insight and Decision Tip](#research-questions-approach-insight-and-decision-tip)
    - [Task 1: Average Discount Percentage (%) by Category](#task-1-average-discount-percentage--by-category)
    - [Task 2: Number of Products per Category](#task-2-number-of-products-per-category)
    - [Task 3: Total Reviews per Category](#task-3-total-reviews-per-category)
    - [Task 4: Products with Highest Average Ratings](#task-4-products-with-highest-average-ratings)
    - [Task 5: Average Actual vs Discounted Price by Category](#task-5-average-actual-vs-discounted-price-by-category)
    - [Task 6: Products with Highest Number of Reviews](#task-6-products-with-highest-number-of-reviews)
    - [Task 7: Products with ≥50% Discount](#task-7-products-with-50-discount)
    - [Task 8: Distribution of Ratings](#task-8-distribution-of-ratings)
    - [Task 9: Total Potential Revenue by Category](#task-9-total-potential-revenue-by-category)
    - [Task 10: Unique Products per Price Bucket](#task-10-unique-products-per-price-bucket)
    - [Task 11: Relationship Between Rating and Discount](#task-11-relationship-between-rating-and-discount)
    - [Task 12: Products with <1,000 Reviews](#task-12-products-with-1000-reviews)
    - [Task 13: Categories with Highest Discounts](#task-13-categories-with-highest-discounts)
    - [Task 14: Top 5 Products by Combined Rating and Review Score](#task-14-top-5-products-by-combined-rating-and-review-score)
- [Dashboard Creation](#dashboard-creation)
- [Project Summary](#project-summary)
- [Recommendations](#recommendations)

 
## COMPREHENSIVE DOCUMENTATION OUTLINING EACH STAGE AND METHOD APPLIED DURING THE PROJECT WORKFLOW

### Project Overview

This case study analyzes Amazon products and review data to identify actionable insights for enhancing product development, customer engagement, and marketing strategies. The dataset comprises 1,465 rows and 16 columns, including detailed product information such as name, category, price, discount, ratings, and customer reviews.

The tools used include:

•	Microsoft Excel [Download here](https://www.microsoft.com)

•	Pivot Tables

•	Helper and Calculated Columns

•	Charts and Slicers

•	Dashboard Layout Design

### Exploratory Data Analysis (EDA)

Exploratory Data Analysis (EDA) is a critical (usually first) step in the data analysis process. It involves systematically examining and summarizing the key characteristics of a dataset, both statistically and visually, to have a clear understanding of its structure, patterns, and potential anomalies.

EDA helps analysts and stakeholders to uncover valuable insights, detect inconsistencies and/or missing values, identify relationships between variables, and form hypotheses that guide deeper analysis or model development.

In this Amazon Product Review Analysis, EDA was used to:

1. Understand product distribution across categories

2. Identify highly reviewed and top - rated products

3. Analyze price ranges and discount levels

4. Detect missing or duplicated entries

5. Observe relationships between ratings, reviews, and revenue

### Data Cleaning and Preparation

Text cleaning and formatting was carried out at the initial stage of this project using excel functions like TRIM, PROPER, LEFT, RIGHT, SUBSTITUTE, FIND, LEN, IF, and so on.

### Research Questions, Approach, Insight and Decision Tip

### Task 1: Average Discount Percentage (%) by Category

- A pivot table was created with Category as rows and Discount % as values (set to average).

Insight: 

- Categories like Electronics | Earpads, Electronics | PhoneCharms, and Computers&Accessories | CableConnectionProtectors offer the highest average discounts (up to 90%).

Decision Tip:

- Focus promotions on high-discount categories with good ratings for volume sales, and maintain premium pricing for strong-rated, low-discount items.


### Task 2: Number of Products per Category

- Used a pivot table to count Product Name per category.

Insight: 

- Computers&Accessories | USBCables categories dominate product count, indicating high competition. Others are more niche with fewer listings.

Decision Tip:

- Consider investing in less saturated categories to reduce competition and stand out in listings.


### Task 3: Total Reviews per Category

- I created a pivot table with sum of Review Count grouped by category.

Insight: 

- Categories with the most reviews (Electronics | In-Ear) showed strong customer engagement while some categories received disproportionate customer engagement.

Decision Tip:

- Leverage high-review categories for cross-selling or bundling opportunities.


### Task 4: Products with Highest Average Ratings

-	Pivot table was used to calculate average rating per product.

-	It was sorted in descending order, to identify top-rated items.

Insight: 

-	These products signal strong customer satisfaction.

-	Some may be hidden gems with good quality but low visibility.

Decision Tip:

-	Promote these highly rated products more prominently - even if review count is lower.


### Task 5: Average Actual vs Discounted Price by Category

-	I added two value fields (average of actual price and discounted price) in a pivot table grouped by category.

Insight:

- It allows comparison of perceived savings across categories.

-	Some categories show aggressive discounting (high price drop), which may affect perceived value.

-	Others show a minimal difference, suggesting premium strategy.

Decision Tip:

-	Balance discount depth to preserve brand value perception while still attracting deal-seekers.


### Task 6: Products with Highest Number of Reviews

-	I chose to use pivot table instead of normal excel filter because of some duplicate product entries. So, I dragged product name to rows, and rating count to values (set to sum) to identify most popular items.

Insight:

-	These are high-visibility leaders in the catalog.
-	They may already be market leaders or viral products.

Decision Tip:

-	Use these products as anchors for bundles, ads, and spotlight promotions


### Task 7: Products with ≥50% Discount

-	I added a new column called “High Discount” (using IF function i.e =IF(J2:J1465>=0.5,"Yes","No"))

-	I then used the helper column to flag products with discounts >=50% by creating a pivot table to count the products that have high discounts. Also, I checked which categories give the most discounts (by dragging the category into rows in pivot table).

Insight:

-	Several products are being pushed aggressively.

-	Some may use discounts to compensate for low reviews.

Decision Tip:

-	Audit heavily discounted products to ensure they have quality to match, or adjust pricing strategy.


### Task 8: Distribution of Ratings

-	Created a frequency distribution (using pivot table by dragging ratings to rows, and product name to values set to count) for ratings like 3.0, 3.5, 4.0, 4.5 and 5.0.

Insight:

-	Majority of products were clustered between 3.5 and 4.5 stars.

-	Few products below 3.0 indicates sellers may have removed poorly rated listings.

Decision Tip:

-	Aim to move the average rating upward, focus on product quality and post-sale support.


### Task 9: Total Potential Revenue by Category

-	Helper column was created with name “total potential revenue” (Actual Price * Rating Count).

-	Summarized via pivot table by category by dragging category to rows, and potential revenue to values set to Sum.

-	The revenue column was formatted using Currency (₹).

Insight:

-	Some categories have low volume but high revenue potential.

-	Others have high traffic but low average prices, meaning thin margins.

Decision Tip:

-	Use this to prioritize marketing spending and focus on high-potential categories with solid ratings.


### Task 10: Unique Products per Price Bucket

-	Created price bins: <₹200, ₹200-₹500, >₹500

-	Used pivot table to count (distinct count) unique products in each range.

Insight:

-	Most products likely fall in the ₹200–₹500 range.

-	Very few fall in the premium > ₹500 range, which could be limiting high-ticket sales.

Decision Tip:

-	Consider adding more premium-priced offerings to capture higher-end customers.


### Task 11: Relationship Between Rating and Discount

-	Scatter chart plotted with Rating on X-axis and Discount % on Y-axis.

Insight: 

- No strong correlation was found because the dots were scattered (No pattern formed, and the R2 value was not up to 0.99). Also, higher ratings = lower discounts due to the downward slope trendline.

-	Some high rated products also have high discounts (possible promotional strategy).

Decision Tip:

-	Use discounts strategically and not as a cover for poor quality, but as a boost for existing good products.


### Task 12: Products with <1,000 Reviews

-	Used a filter to flag products below 1000 reviews.

-	It helps to identify underexposed products.

Insight:

-	These are underexposed or new products.

-	Many may have high ratings but low visibility.

Decision Tip:

-	Run campaigns to boost visibility and reviews for good products with low engagement.


### Task 13: Categories with Highest Discounts

-	Created a pivot table for average discount % per category, dragged category to rows and percentage discount to values set to average. Formatted as percentage (2 decimal places) and sorted in descending order.

Insight:

-	Mobile Cables or Tech Accessories may offer 70% and above discounts, especially in competitive areas.

Decision Tip:

-	Reevaluate profit margins in these categories and avoid over discounting products that perform well.


### Task 14: Top 5 Products by Combined Rating and Review Score

-	Pivot table was created

-	Rows: product name

-	Values: rating plus reviews (the helper column earlier created) set to Sum

-	Sorted from Largest to Smallest

-	Used value filter to find the top 5 performers.

Insight:

-	These are the strongest performers overall: highly rated and heavily reviewed.

-	It is ideal for hero banners, landing pages, and best seller placements.

Decision Tip:

- Make these products your flagship products in marketing efforts, feature them in ads, top searches, and so on.


## Dashboard Creation

### 1.	Design Plan:
   
-	Clean dark teal theme

-	Top banner with title and KPIs

-	Slicers added for Rating Group

### 2.	Visuals Used:

-	Column charts for average discount % by category, total reviews per category, and distribution of product ratings.

-	Bar charts for number of products per category, and total potential revenue by category.

-	Pie chart for top 5 product rating

### 4.	Interactivity:

-	Used slicers to allow dynamic filtering

-	All charts updated automatically via pivot tables

### 5.	Structure:

-	Title at the top

-	Charts were arranged in sections matching the task objectives

-	Clear, uncluttered layout

![DSA Amazon case study dashboard](https://github.com/user-attachments/assets/f8dde138-79e8-41c6-8462-c1b0230779ec)


## Project Summary

-	Most Competitive Categories: Electronics | Earpads, Electronics | PhoneCharms, and Computers&Accessories | CableConnectionProtectors have the most listings and engagement.
  
-	Customer Behavior: Ratings mostly fall between 3.5 and 4.5, showing good but not exceptional satisfaction.
  
-	Strategic Opportunity: Promote highly rated but under-reviewed products for visibility.
  
-	Revenue Focus: Categories with high prices and high engagement showed the highest revenue potential.
  
-	Marketing Direction: Bundle or promote top 5 scoring products; be cautious with deep discount strategies.
  
This dashboard and analysis provide actionable insights for product positioning, inventory focus, and promotional planning.


## Recommendations

-	Certain categories were excessively discounted. Aim to balance promotional offers with maintaining product value.

-	Increase the visibility of top-performing products, as many highly rated items have few reviews. 

-	A 4.0+ rating typically signals customer trust. Focus on improving underperforming products.

-	High review volume combined with higher prices drives greater revenue. Prioritize marketing efforts on high-revenue categories.

-	Saturated vs. underserved categories: Focus expansion efforts on less competitive markets.




