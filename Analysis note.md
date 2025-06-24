## Dataset Description
### Provided file: Amazon case Study.xlsx

### Columns Include
- product_id
- product_name
- category
- discounted_price
- actual_price
- discount_percentage
- rating
- rating_count
- about_producer
- user_id
- user_name
- review_id
- review_title
- review_content
- img_link
- product_link

  ## Data Cleaning
  I took the following steps before asking the analysis questions
- deleted columns not needed for this analysis
- Added three new calculated columns (Potential revenue, Price range bucket, rating score)
- Removed duplicates
- Checked for blanks and errors
- Removed rows with imcomplete data

  ### Visualisation
  - All visuals were generated using Excel
  - Key Charts include Bar and Line charts
 
  ### Dashboard
  The Dashboard includes;
  - Key Metrics
  - Category-level Insights
  - Product-Level insights
  - Price Ratinga and Trends

## Data Analysis 
### Q1. What is the average discount percentage by product category?
Used a pivot table: Rows = Category, Values = Average of Discount Percentage

**Top Category:**
- Electronics

### Q2. How many products are listed under each category?
Used a pivot table: Rows = Category, Values = Count of Product Name 


### Q3. Total number of reviews per category?
Used a pivot table: Rows = Category, Values = Sum of rating_count

### Q4. Which products have the highest average ratings?
Used a pivot table: Rows = Product name, Values = Rating set to average

### Q5. What is the average actual price vs the discounted price by category?
Used a pivot table: Rows = Category, Values = Actual Price set to average, discount price set to average

### Q6. Which products have the highest number of reviews?
Used a pivot table: Rows = Product name, Values = Sum of rating_count

### Q7. How many products have a discount of 50% or more?
Used Excel "COUNTIF" function: =COUNTIF(amazon!F2:F1383, ">=50")
![image](https://github.com/user-attachments/assets/fcef8b09-5f18-48d1-ac40-6345f52b2e57)

### Q8. What is the distribution of product ratings (e.g., how many products are rated 3.0,
4.0, etc.)?
Used a pivot table: Rows = Rating, Values = Count of product_name

### Q9.  What is the total potential revenue (actual_price × rating_count) by category?
Used a pivot table: Rows = Categories, Values = Sum of Potential revenue

### Q10.  What is the number of unique products per price range bucket (e.g., <₹200,
₹200–₹500, >₹500)?
Used a pivot table: Rows = Price Range Bucket, Values = Count of Product_name

### Q11.  How does the rating relate to the level of discount?
Used a pivot table: Rows = Rating, Values = Discount_price set to average

### Q12.  How many products have fewer than 1,000 reviews?
Used Excel "COUNTIF" function: =COUNTIF(amazon!H2:H1383, "<1000")
![image](https://github.com/user-attachments/assets/960242f4-1dab-4721-96bb-e775706ebcd8)

### Q13.  Which categories have products with the highest discounts?
Used a pivot table: Rows = Categories, Values = Discount_percentage set to Max

### Q14.  Identify the top 5 products in terms of rating and number of reviews combined.
Used a pivot table: Rows = Product name, Values = Sum of rating score

 #### Key Insights
- Most customers leave positive reviews (4–5 stars), but negative reviews provide deeper product feedback
- negative reviews will be useful for customer service improvements
- Verified reviews are more trustworthy indicators of quality

  ### Recommendations
  - Product Development: Investigate common complaints in 1–2 star reviews.
  - Customer Service: Track verified negative reviews for follow-up.
  - Marketing: Highlight positive keywords in campaigns.
  - Operations: Improve delivery processes mentioned in negative reviews.
 
  ### Conclusion
  This analysis reveals the importance of review sentiment in understanding customer satisfaction. With most reviews being positive, brands can use these insights for marketing, while negative feedback points to actionable product and service improvements. The dashboard provides a dynamic way for stakeholders to explore trends and patterns.







 







