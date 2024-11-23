# E-Commerce Sales Data Analysis Project  

## Context  
This project focuses on the analysis of an e-commerce sales dataset from a London-based online retail shop specializing in gifts and homeware. The dataset captures sales transactions over one year and provides insights into customer purchasing behavior, product trends, and sales patterns. By analyzing this data, we aim to uncover actionable insights that can help the business optimize operations, improve customer satisfaction, and increase profitability.  

## Dataset Overview  
The dataset consists of **500,000 rows** and **8 columns**, representing various aspects of sales transactions.  

### Key Columns  
- **TransactionNo**: A unique identifier for each transaction (e.g., "C" indicates cancellations).  
- **Date**: The date of the transaction.  
- **ProductNo**: A unique identifier for each product.  
- **ProductName**: The name of the product or item.  
- **Price**: The price per unit of the product (£).  
- **Quantity**: The number of units purchased per transaction (negative values indicate cancellations).  
- **CustomerNo**: A unique identifier for each customer.  
- **Country**: The customer's country of residence.  

## Objectives  
1. Clean the dataset to handle missing values and outliers.  
2. Analyze customer purchasing behavior and identify trends in sales.  
3. Identify the most purchased products in each country.  
4. Examine the number of products purchased per transaction by customers.  
5. Visualize sales trends for the top 20 products within a specific time frame.  

## Data Cleaning Process  
To ensure the dataset was ready for analysis:  
- **Handling Missing Values**: Missing data in `ProductNo`, `ProductName`, and `Price` were filled based on groupings and mode calculations. For example, `ProductName` was filled using the most frequent product name for a given `ProductNo`.  
- **Date Conversion**: The `Date` column was converted to datetime format for time-series analysis.  
- **Handling Null Values**: Missing `Quantity` values were replaced with the column's mean value.  
- **Removing Duplicates**: Duplicate rows were identified and marked for potential removal.  

## Exploratory Data Analysis (EDA)  

### Key Insights  
1. **Most Purchased Products by Country**:  
   - For each country, the most frequently purchased product was identified using mode analysis. This helps highlight popular products for targeted marketing.  
   - A bar chart was created to visualize the most purchased products by country.  

2. **Customer Transaction Analysis**:  
   - The number of products purchased in each transaction by customers was analyzed.  
   - Transactions with the top 50 highest frequencies were visualized using a bar chart, grouped by `CustomerNo`.  

3. **Sales Trends of Top 20 Products**:  
   - The top 20 most purchased products were analyzed over a selected time frame (2018–2019).  
   - A grouped bar chart displayed sales trends for these products on a daily basis.  

### Data Visualization  
- **Bar Chart**: Showcased the most purchased products by country.  
- **Stacked Bar Chart**: Highlighted the number of products purchased by customers in top transactions.  
- **Time-Series Chart**: Illustrated daily sales trends for the top 20 products.  

## Recommendations  
1. **Inventory Management**:  
   - Maintain sufficient stock for top products in countries where demand is high.  
   - Address cancellation issues by improving stock availability for all ordered items.  

2. **Targeted Marketing**:  
   - Create promotional campaigns centered around top-selling products in each country.  
   - Use customer segmentation to design personalized offers for high-value customers.  

3. **Customer Retention**:  
   - Develop loyalty programs to encourage repeat purchases.  

4. **Sales Forecasting**:  
   - Use historical data to forecast demand for specific products during peak periods.  

## Tools and Libraries Used  
- **Python Libraries**:  
  - **Pandas**: Data manipulation and cleaning.  
  - **NumPy**: Numerical computations.  
  - **Matplotlib & Seaborn**: Data visualization.  

## Conclusion  
This project demonstrates how e-commerce data can be analyzed to extract meaningful insights that inform business decisions. By identifying trends, understanding customer behavior, and making data-driven recommendations, businesses can improve operational efficiency, increase revenue, and enhance the overall customer experience.
