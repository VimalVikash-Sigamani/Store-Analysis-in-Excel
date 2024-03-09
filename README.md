# Store-Analysis

### Table of Contents
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning/Preparation](#data-cleaningpreparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Analysis & Data Visualizaation](#data-analysisdata-visualization)
- [Results/Findings](#resultsfindings)
- [Recommedations](#recommedations)

### Project Overview
Vrinda online store wants to create an annual sales report for 2022. so that, Vrinda can understand their customers and grow more sales in 2023.

<include online store image>

### Data Source

<Include Source Excel sheet>
  
  - **Index:** Unique sequentially value for each orders.
  - **Order ID:** Unique order number for each orders. 
  - **Cust ID:** Customer ID
  - **Gender:** Customer gender
  - **Age:** Customer age
  - **Date:** Order date
  - **Status:** Order status
  - **Channel:** Channel through which order placed
  - **SKU:** Unique code assigned to each products
  - **Category:** Product category
  - **Size:** Product size
  - **Qty:** Number of product ordered
  - **Currency:** Indian rupee INR
  - **Amount:** Sale amount
  - **Ship-City:** Shipped City
  - **Ship-State:** Shipped State
  - **Ship-Postal-Code:** Shipped Postal Code
  - **Ship-Country:** Shipped Country

### Tools
- Excel
  	Data Cleaning, Data Analysis, Data Visualization

### Data Cleaning/Preparation
In the initial data preparation phase, we performed the following tasks
1. Data corrections.
2. Null values check.
3. Data formatting.

### Data Processing:
1. Created new column 'Age Group' from 'Age' column using IFS formula in order to address business question. Categorized the customers as below
   - Age >= 50, then 'Senior'
   - Age >= 30, then 'Adult'
   - Age < 30, then 'Tennager'
2. Extracted only Month data from Date column in order to address business question.

### Exploratory Data Analysis (EDA)
EDA involved in exploring the A/B test data to answer some questions, such as:
1. What was the conversion rate of all users?
2. What is the user conversion rate for the control and treatment groups?
3. What is the average amount spent per user for the control and treatment groups, including users who did not convert?
4. Extract the user ID, user’s country, user’s gender, user’s device type, user’s test group, whether or not they converted (spent > $0), and how much they spent in total ($0+).

### Data Analysis & Data Visualization

1. Compare the sales and orders for 2022. Which month got the highest sales and orders? </br>

   In March 2022, we experienced the highest sales and number of orders.
   
   <img width="361" alt="Sales Vs Orders" src="https://github.com/VimalVikash-Sigamani/Store-Analysis-in-Excel/assets/161229746/8b109573-2911-417d-864f-a12cd4ad1f2a">

3. Who purchased more in 2022? Men or Women? </br>

   Women made more purchases than men.
   
   <img width="366" alt="Men Vs Women" src="https://github.com/VimalVikash-Sigamani/Store-Analysis-in-Excel/assets/161229746/a33588c2-d2e9-4ee5-9203-17dd1bc14dec">
   
5. What are different order status in 2022? </br>

   92% of orders were delivered.
   
   <img width="359" alt="Status" src="https://github.com/VimalVikash-Sigamani/Store-Analysis-in-Excel/assets/161229746/a0989ee6-07de-415e-85ad-eaf87e17838d">

6. Identify top 5 states contributing to the sales? </br>

   Maharashtra, Karnataka, Uttar Pradesh, Telangana and Tamil nadu are top five states.

   <img width="360" alt="Top 5 States" src="https://github.com/VimalVikash-Sigamani/Store-Analysis-in-Excel/assets/161229746/7571e9a7-cb15-4329-9c9e-082e213edc01">

7. Which channel is contributing to maximum sales? </br>

   Amazon contributes the maximum sales.

     <img width="359" alt="Channels" src="https://github.com/VimalVikash-Sigamani/Store-Analysis-in-Excel/assets/161229746/12b697e8-4ed1-40ad-87ab-6dd6bf1b09ee">

8. Highest selling category? </br>

   Set emerges as the highest-selling product.
   
    <img width="364" alt="Category" src="https://github.com/VimalVikash-Sigamani/Store-Analysis-in-Excel/assets/161229746/e30b31ca-6d79-454c-947c-fcec33cb5738">

9. Relation between age and gender based on number of orders? </br>

   Age group of adult women (30-49 years) contributes the most, making up approximately 35% of the total.
   
    


    [Click here](https://docs.google.com/spreadsheets/d/1GU7lqwdvYfTGoxPXMLb5SucVjKEtxCC-vlK9KNT1xH8/edit#gid=392375140) for detailed calculations.

 
### Results/Findings
- Women exhibit a higher likelihood of purchasing compared to men, constituting approximately 64% of total sales.
- The top three states are Maharashtra, Karnataka, and Uttar Pradesh, collectively contribute to approximately 69% of total sales.
- The adult age group (30-49 years) makes the maximum contribution, accounting for around 50% of total sales.
- Amazon, Myntra, and Flipkart serve as the top contributing channels, collectively contributing approximately 81% of total sales.
- The top-selling products are Set, Kurta, and Western dress collectively contribute to approximately 88% of total sales.
 
### Recommedations
To boost sales in 2023, focus on targeting female customers aged 30-49 residing in Maharashtra, Karnataka, and Uttar Pradesh. Show advertisements, offers, and coupons on Amazon, Myntra, and Flipkart platforms.

