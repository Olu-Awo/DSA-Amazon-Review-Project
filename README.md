# DSA-Amazon-Review-Project
This an excel based analytic project prepared after a three month training with DSA (The Incubator Hub) , the project consist of a data set from Amazon  review page, which includes product details, name, category, price, discount, ratings e.t.c.

This is where I put to work all I have learnt in the excel class after training.

## Project Topic: AMAZON PRODUCT REVIEW

### Project Overview: 
This data analysis project is aimed at analysing product and customer review data to generate insights that can guide product improvement, marketing strategies, and customer engagement, and in turn, assist all stakeholer to make an informed decision for the growth of the organisation. 

### Data Source: 
The data is a CSV file supplied by The Incubator Hub downloaded from my LMS into my local drive, it consist of 1465 rows and 16 columns.

### Tools Used: 
All the work was done using Microsoft excel to perform the following:
- Data collection
 - Data cleaning
 - Creating calculated column
 - Creating Pivot Table
 - Creating Dash board

 #### Data Cleaning and Preparation
 I perfomed the following action in the data cleaning and preparation stage.
 - Data collection: by uploading the data from my local drive
   - Deleting some columns not needed.
   - Removing duplicated rows
   - removing blank rows
   - spliting columns with unneccessary long words and extracing the key words
 #### Exploiratory Data Analysis
At the EDA stage, the following questions (Q) were answered by taking the following actions (A);
 - Q1: What is the average Discount percentage by Product category?
   - A: Insert Pivot Table, Rows: category, Values: discount percentage (set to Average)
 - Q2:How many products are listed under each category?
   - A: Insert Pivot Table, Rows: category, Values: product id (set to Count)
 - Q3: What is the total number of reviews per category?
   - A: Insert Pivot Table, Rows: category, Values: review id (set to Count)
 - Q4: Which product has the highest average ratings?
   - A: Insert Pivot Table, Rows: Product name, Values: rating (set to Average), Sort descending by Average rating.
 - Q5: What is the average actual price versus the discounted price by category?
   - A: Insert Pivot Table, Rows: category, Values: Actual price (set to Average), Discount price (set to Average)
 - Q6: Which product has the highest number of reviews?
   - A: Insert Pivot Table, Rows: Product name, Values: rating (set to Max), Sort by descending order.
 - Q7: How many products have a discount of 50% or more?
   - A: Created a new colunms named percentage rating and using excel function: 
    - ``` excel function
     =IF(G3>=50%,"above 50%","below50%")
     ```
    - Insert pivot Table, Row: Percentage ratimg, Values: Product id, (set to count)
  - Q8: What is the distribution of product ratings?
    - A: Insert Pivot Table, Rows: Rating, Values: product id (set to Count)
- Q9: What is the total potential revenue by category?
  - A: Created a new colunms named potential revenue and using excel function: 
    - ``` excel function
     =actual price * rating count
      ```
    - Insert pivot Table, Row: Category, Values: Potential revenue(Sum)
  - Q11: How does the rating relate to the level of discount?
   - A: Insert scatter plot, x-axis: Discount percentage, y-axis: Rating, used trending lines to show correlation.
 - Q12: How many products have fewer than 1,000 reviews?
   -  A: Used the 'CountIF' function
      ```
      =COUNTIF(N2:N1350, "below 1000 reviews")
      ```
      ```
      =COUNTIF(N3:N1351, "above 1000 reviews")
      ```
- Q13: Which categories have products with the highest discounts?
  - A: Insert Pivot Table, Rows: Category, Values: Discount percentage (set to Max), Sort by descending order.
- Q14: Identify the top 5 products in terms of rating and number of reviews combined.
  - A: Added a cloumn: rating * rating count, sorted by descending order, picked top 5.
### Visualisation  
This involved visualising the data by creating a Dash board
   
 - [Amazon case study Table (1).pdf](https://github.com/user-attachments/files/21072420/Amazon.case.study.Table.1.pdf)

![Amazon case study dash board (1)](https://github.com/user-attachments/assets/72f71194-50bc-4ff9-8429-9b4b4dfc22ee)

### Conclusions
From the above dashboard, the following conclusions were drawn:
- Some Products have high discount and yet low rating. This indicates that high discount does not necessarily bring more sales,therefore discount shold be placed on products straegically.
- Only 3 categories (computer & accessories, electronics, home & kitchen) have high product, other categories should also be focus on to see possibilites in sales.
- Some Products have high ratings as well as high review, Promoting these products should be a focal point as they already gain customer trust.

##### Data analysed and prepared by:
Olusola Awolokun.
