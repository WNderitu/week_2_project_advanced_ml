# **Customer Segmentation using Clustering Analysis**
---
## 1. Project Goal
The goal of this project is to analyze customer data and perform Customer Segmentation using clustering algorithms. By understanding customer demographics, spending habits, product preferences, purchasing behavior, promotions acceptance and customer complaints businesses can tailor marketing strategies, product offerings and enhance customer satisfaction.
## 2. Context/ Problem Statement
Businesses often struggle to identify distinct customer segments and align their offerings accordingly. This project addresses this challenge by analyzing a Customer Personality Analysis dataset to uncover valuable insights about customer behavior and preferences.
## 3. Key Data Sources
The Data is sourced from https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis
## 4. Data Characteristics
* The data has 29 columns and 2240 entries.
* There are 26 numerical columns and 2 categorical features. 
## 6. Key insights from Exploratory Data Analysis
* Univariate Analysis:
  * Demographics:
    * Majority of customers have no kids and teenagers, are married and have undegraduate degree level.
    * Average yearly income is 52,247 while average age of customers is 45 years. 
  * Spending habits: Average total spend is 607. 
  * Product preferences: highest average spend on wines, lowest average spend on fruits and sweets. 
  * Purchasing behaviour:
    * On average, most customers purchase in store  while the least purchase via catalogues.
    * There is low purchases via deals. 
  * Promotions Acceptance: low acceptance rate of promotions
  * Customer complaints: low rate of customer complaints
* Bivariate Analysis:
  * Revealed correlations:
    *  Customers who spend more overall also tend to spend more on wines and meat products and do store purchases. 
    *  Customers who purchase via the catalog correlate with high total spend and purchase of meat products.
    *  Customers with only kids does not correlate with high total spend
* Multivariate Analysis:
  * Identified customer segments through clustering are high-spenders, budget conscious, customers with no children and family-oriented. 
## 7. Performance Measurement
* Clustering performance will be avaluated using Silhouette Score and Elbow Method.
* The model will be succeful if it's able to segment the customers into clusters that are well-defined and interpretable.
## 8. Scope of Solution Space
* Model: K-Means Clustering for segmentation used.
* Data Transformations:
  * Encoding categorical variables using One-Hot Encoding
  * Transformation of skewed data using using boxcox transformation
  * Handling of outlier using robust scaling and winsorization
  * Scaling numerical data with MinMax Scaler and standardScaler.
* Feature Engineering:
  * Derived new features such as:
    * Total spend
    * months enrollment - show how long a client has been enrolled
    * has teen and kid - show if a customer has both teen and kid
    * Age  - from year of birth using current year as 2014
  * Deletion of unneccessary features such as:
    * date_enrollment
    * ID
    * Year_Birth
    * Z_CostContact
    * Z_Revenue
## 9. Constraints / Potential Challenges
* Data Quality:
  * Renaming of some of the columns to meaningful names
  * The dataset had some missing values in 24 rows which were dropped
  * The categorical columns had redudant categories, which were merged to be more meaninful.
  * Most of the numerical columns had outliers.
* Model Interpretability:
  * Ensuring cluster labels are meaningful and actionable.
## 10. Stakeholders
* Marketing Team:
  * To utilize insights for targeted campaigns to increase acceptance of promotions, consider offering discounts to high spenders and deals to the budget conscious customers.
  * Develop campaigns to increase purchases via the web
* Product Management: Align product offerings with customer needs.
* Business Strategy Team: Enhance overall customer experience and profitability. 
