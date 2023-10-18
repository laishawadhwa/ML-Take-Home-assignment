![image](https://github.com/laishawadhwa/ML-Take-Home-assignment/assets/25785830/2ded5d21-cab1-45b0-ab0a-9b98d53f40fe)# Dynamic Pricing engine and Sales Forecasting

Price optimization involves leveraging historical data to determine the optimal pricing strategy for a product or service, with the aim of maximizing a company's profitability. Businesses continually enhance their products by adding or upgrading features, which incurs costs in terms of time, effort, and the company's reputation. Therefore, striking the right balance between pricing that is too high, potentially leading to customer loss, and pricing that is too low, resulting in revenue loss, is crucial.

 Problem Statement: The process of maximizing profitability takes into account a multitude of factors, including demographic data, operating costs, customer survey insights, and more. The nature of the business and the product being offered also significantly influence the pricing strategy. Your job is to build a demand forecasting and price optimization model for the e-commerce store.
 The demand forecasting model needs to prodict sales in order to maximize the gross profit.
The price optimization model needs to predict what is the price at which the product should be priced -  you have 8 options of discount to choose from for the product : **5%,10%, 15%, 20%, -5%, -10%, -15%, -20%**

 DataSet: You have been given retail products data with the following features:

- **customers (integer) -** monthly demand for a given subcategory of goods
- **freight_price (float) -** freight price of the company goods
- **fp1, fp2, fp3 (float) -** freight price of competitors 1,2,3 goods respectively
- **product_category_name -** (categorical) - broad group category name
- **product_id (categorical) -** detailed group subcategory name
- **product_description_lenght (integer) -** Number of words in the subcategory description
- **product_score (float) -** user rating for subcategories of the company goods
- **ps1, ps2, ps3 (float) -** user rating for subcategories of competitors 1,2,3 respectively
- **product_photos_qty (integer) -** number of photos for each subcategory (product_id)
- **product_weight_g (integer) -** unit weight in grams
- **total_price (float) -** montly revenue which can be calculated using formula: total_price = unit_price * qty
- **month_year (string) -** data in the format (dd-mm-yyyy) within the range between 01-01-2017 and 01-08-2018. Only months and years are important here.
- **year (integer) -** year which was taken from the 'month_year'
- **month (integer) -** month which was taken from the 'month_year'
- **qty (integer) -** monthly sales per subcategory
- **unit_price (float) -** monthly unit price of subcategory good of company goods
- **comp_1, comp_2, comp_3 (float) -** unit price [within the subcategory] of competitors 1,2,3 goods respectively
- **lag_price (float)** - unit price on the previous month
- **weekend (integer) -** number of weekends per month
- **weekday (integer)** - number of weekdays per month
- **holiday (integer) -** number of holidays per month
- **s (float) -** unknown parameter

## Evaluatuon Metric: 
Weighted mean absolute error (WMAE):

where

n is the number of rows
ŷ i is the predicted sales
yi is the actual sales
wi are weights. w = 5 if the week is a holiday week, 1 otherwise


 ## Deliverables: What do you need to submit?
 - GitHub Repo + Documentation of your project
 - Loom Video
 - EDA of the dataset
 - State your assumptions and limitations for building models.
 - Write up everything that you think needs to be known to us. Whether it's your choice of data impuatation technique or choice of algorithm it's encouraged you share as much detail as possible about your approach.
 - If you're given more time and data, how will you use it to make a better model? Be as specific as possible here, highlighting what data will you need and how would it help given more time.
   
