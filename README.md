# Store-Analysis

### Table of Contents
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Data Processing](#data_processing)
- [Data Analysis & Data Visualization](#data-analysis-and-data-visualization)
- [Interactive Dashboard](#interactive-dashboard)
- [Results/Findings](#resultsfindings)
- [Recommedations](#recommedations)

### Project Overview
Vrinda Online Store aims to generate a comprehensive annual sales report for 2022 to gain insights into their customer base and strategize for increased sales in 2023.

<include online store image>

### Data Source

To reference the data source [Click here](https://github.com/VimalVikash-Sigamani/Store-Analysis-in-Excel/blob/7cca5575af41ee795e7e349ad69899151a681ca5/Vrinda%20Store%20Data%20Analysis_Backup%20copy.xlsx)
  
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
  - Data Cleaning
  - Data Processing
  - Data Analysis
  - Data Visualization

### Data Cleaning
During the initial data preparation phase, the following tasks were undertaken:
1. Correcting data errors.
2. Checking for null values.
3. Formatting the data.

### Data Processing
1. The 'Age Group' column was generated from the 'Age' column using the IFS formula to address a specific business inquiry. Customers were categorized as follows:
   - If Age is greater than or equal to 50, labeled as 'Senior'.
   - If Age is greater than or equal to 30, labeled as 'Adult'.
   - If Age is less than 30, labeled as 'Teenager'.
2. The Month data was extracted exclusively from the Date column to cater to a business query.

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

   <img width="387" alt="Age group Vs Gender" src="https://github.com/VimalVikash-Sigamani/Store-Analysis-in-Excel/assets/161229746/6d89c06a-4a21-42f3-b109-d68269b713c6">


10. Annual Report 2022_Dashboard:

    <img width="927" alt="Annual Report 2022 - Dashboard" src="https://github.com/VimalVikash-Sigamani/Store-Analysis-in-Excel/assets/161229746/7202fd98-8536-4cfd-8190-adfa93263142">

### Interactive Dashboard
To access the interactive dashboard:
   [Click here to view the interactive dashboard](https://docs.google.com/spreadsheets/d/1GU7lqwdvYfTGoxPXMLb5SucVjKEtxCC-vlK9KNT1xH8/edit#gid=392375140)
 
### Results/Findings
- Women exhibit a higher likelihood of purchasing compared to men, constituting approximately 64% of total sales.
- The top three states are Maharashtra, Karnataka, and Uttar Pradesh, collectively contribute to approximately 69% of total sales.
- The adult age group (30-49 years) makes the maximum contribution, accounting for around 50% of total sales.
- Amazon, Myntra, and Flipkart serve as the top contributing channels, collectively contributing approximately 81% of total sales.
- The top-selling products are Set, Kurta, and Western dress collectively contribute to approximately 88% of total sales.
 
### Recommedations
- To boost sales in 2023, focus on targeting female customers aged 30-49 residing in Maharashtra, Karnataka, and Uttar Pradesh. Show advertisements, offers, and coupons on Amazon, Myntra, and Flipkart platforms.

