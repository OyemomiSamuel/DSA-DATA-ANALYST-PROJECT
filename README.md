# DSA-DATA-ANALYST-PROJECT
 Case Study 1: Amazon Product Review Analysis - Using pivot tables, helper columns, and calculated columns to analyze the data and provide insights based on specific business questions.
 
## COMPREHENSIVE DOCUMENTATION OUTLINING EACH STAGE AND METHOD APPLIED DURING THE PROJECT WORKFLOW

### Project Overview

This case study analyzes Amazon products and review data to identify actionable insights for enhancing product development, customer engagement, and marketing strategies. The dataset comprises 1,465 rows and 16 columns, including detailed product information such as name, category, price, discount, ratings, and customer reviews.

The tools used include:

•	Microsoft Excel

•	Pivot Tables

•	Helper and Calculated Columns

•	Charts and Slicers

•	Dashboard Layout Design

### Task 1: Average Discount Percentage (%) by Category

•	A pivot table was created with Category as rows and Discount % as values (set to average).

Insight: Categories like Electronics | Earpads, Electronics | PhoneCharms, and Computers&Accessories | CableConnectionProtectors offer the highest average discounts (up to 90%).

### Task 2: Number of Products per Category

•	Used a pivot table to count Product Name per category.

Insight: Computers&Accessories | USBCables categories dominate product count, indicating high competition.

### Task 3: Total Reviews per Category

•	I created a pivot table with sum of Review Count grouped by category.

Insight: Categories with the most reviews (Electronics | In-Ear) showed strong customer engagement.

### Task 4: Products with Highest Average Ratings

•	Pivot table was used to calculate average rating per product.

•	It was sorted in descending order, to identify top-rated items.

### Task 5: Average Actual vs Discounted Price by Category

•	I added two value fields (average of actual price and discounted price) in a pivot table grouped by category.

Insight: It allows comparison of perceived savings across categories.

### Task 6: Products with Highest Number of Reviews

•	I chose to use pivot table instead of normal excel filter because of some duplicate product entries. So, I dragged product name to rows, and rating count to values (set to sum) to identify most popular items.

### Task 7: Products with ≥50% Discount

•	I added a new column called “High Discount” (using IF function i.e =IF(J2:J1465>=0.5,"Yes","No"))

•	I then used the helper column to flag products with discounts >=50% by creating a pivot table to count the products that have high discounts. Also, I checked which categories give the most discounts (by dragging the category into rows in pivot table).

### Task 8: Distribution of Ratings

•	Created a frequency distribution (using pivot table by dragging ratings to rows, and product name to values set to count) for ratings like 3.0, 3.5, 4.0, 4.5 and 5.0.

### Task 9: Total Potential Revenue by Category

•	Helper column was created with name “total potential revenue” (Actual Price * Rating Count).

•	Summarized via pivot table by category by dragging category to rows, and potential revenue to values set to Sum.

•	The revenue column was formatted using Currency (₹).

### Task 10: Unique Products per Price Bucket

•	Created price bins: <₹200, ₹200-₹500, >₹500

•	Used pivot table to count (distinct count) unique products in each range.

### Task 11: Relationship Between Rating and Discount

•	Scatter chart plotted with Rating on X-axis and Discount % on Y-axis.

•	Insight: No strong correlation found because the dots were scattered (No pattern formed, and the R2 value was not up to 0.99). Also, higher ratings = lower discounts due to the downward slope trendline.

### Task 12: Products with <1,000 Reviews

•	Used a filter to flag products below 1000 reviews.

•	It helps to identify underexposed products.

### Task 13: Categories with Highest Discounts

•	Created a pivot table for average discount % per category, dragged category to rows and percentage discount to values set to average. Formatted as percentage (2 decimal places) and sorted in descending order.

### Task 14: Top 5 Products by Combined Rating and Review Score

•	Pivot table was created

•	Rows: product name

•	Values: rating plus reviews (the helper column earlier created) set to Sum

•	Sorted from Largest to Smallest

•	Used value filter to find the top 5 performers.

## Dashboard Creation

### 1.	Design Plan:
   
-	Clean dark teal theme

-	Top banner with title and KPIs

-	Slicers added for Rating Group

### 2.	Visuals Used:

-	Column charts for average discount % by category, number of products per category, total reviews per category, and distribution of product ratings.

-	Pie chart for top 5 product rating

-	Doughnut chart for rating distribution

### 4.	Interactivity:

-	Used slicers to allow dynamic filtering

-	All charts updated automatically via pivot tables

### 5.	Structure:

-	Title at the top

-	Charts were arranged in sections matching the task objectives

-	Clear, uncluttered layout

## Project Summary and Insights

-	Most Competitive Categories: Mobile accessories have the most listings and engagement.
  
-	Customer Behavior: Ratings mostly fall between 3.5 and 4.5, showing good but not exceptional satisfaction.
  
-	Strategic Opportunity: Promote highly rated but under-reviewed products for visibility.
  
-	Revenue Focus: Categories with high prices and high engagement showed the highest revenue potential.
  
-	Marketing Direction: Bundle or promote top 5 scoring products; be cautious with deep discount strategies.
  
This dashboard and analysis provide actionable insights for product positioning, inventory focus, and promotional planning.




