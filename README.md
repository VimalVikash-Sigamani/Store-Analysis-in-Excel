# Store-Analysis

### Table of Contents
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning/Preparation](#data-cleaningpreparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Analysis](#data-analysis)
- [Other Insights](#other-insights)
- [Statistical Analysis](#statistical-analysis)
- [Results/Findings](#resultsfindings)
- [Recommedations](#recommedations)

### Project Overview
Vrinda online store wants to create an annual sales report for 2022. so that, Vrinda can understand their customers and grow more sales in 2023.

<include online store image>

### Data Source

<Include Source Excel sheet>
  
  - **index:** Unique sequentially value for each orders.
  - **Order ID:** Unique order number for each orders. 
  - **Cust ID:** Customer ID
  - **Gender:** Customer gender
  - **Age:** Customer age
  - **Date:** Order date
  - **Status:** Order status
  - **Channel:** Channel through which order placed
  - **SKU:** Customer ID
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
- 	Data Cleaning, Data Analysis, Data Visualization

### Data Cleaning/Preparation
In the initial data preparation phase, we performed the following tasks
1. Data corrections.
2. Null values check.
3. Data formatting.

### Data Processing:
1. Created new column 'Age Group' from 'Age' column using IFS formula in order to address business question. Categorized the customers as below
   	Age >= 50, then 'Senior'
   	Age >= 30, then 'Adult'
   	Age < 30, then 'Tennager'
2. Extracted only Month data from Date column in order to address business question.

### Exploratory Data Analysis (EDA)
EDA involved in exploring the A/B test data to answer some questions, such as:
1. What was the conversion rate of all users?
2. What is the user conversion rate for the control and treatment groups?
3. What is the average amount spent per user for the control and treatment groups, including users who did not convert?
4. Extract the user ID, user’s country, user’s gender, user’s device type, user’s test group, whether or not they converted (spent > $0), and how much they spent in total ($0+).

### Data Analysis

1. Compare the sales and orders for 2022. Which month got the highest sales and orders?
2. Who purchased more in 2022? Men or Women?
3. What are different order status in 2022?
4. Identify top 5 states contributing to the sales?
5. Which channel is contributing to maximum sales?
6. Highest selling category?
7. Relation between age and gender based on number of orders?

   ### Other Insights
- Disturbation of amount spent.
  
  <img width="625" alt="Disturbation of amount spent" src="https://github.com/VimalVikash-Sigamani/Globox-A-B-Testing/assets/161229746/b5639513-2ad8-4235-9683-84f2bef3d6ba">

- Relationship between the test metrics (conversion rate and average amount spent) and the user’s device.

  <img width="664" alt="Device insights" src="https://github.com/VimalVikash-Sigamani/Globox-A-B-Testing/assets/161229746/d563abf6-2884-4d4f-ae48-99e7e6bbe437">

  
- Relationship between the test metrics (conversion rate and average amount spent) and the user’s gender.

  <img width="667" alt="Gender insights" src="https://github.com/VimalVikash-Sigamani/Globox-A-B-Testing/assets/161229746/bcf4157e-51cf-44ed-a728-f048541d52e5">


- Novelty effects

  <img width="592" alt="Novelty effect" src="https://github.com/VimalVikash-Sigamani/Globox-A-B-Testing/assets/161229746/91dfdda4-ca20-46ed-9ca2-63cf697444e7">

  

### Statistical Analysis
We measured below two key metrices and Hypothesis testing is done on these metrices to determine the outcome of A/B testing.

1. Conversion rate:
   -  Null Hypothesis H0: P1 = P2
   -  Alternative Hypothesis H1: P1 != P2

2. Average amount spent:
	 - Null Hypothesis H0: u1 = u2
   - Alternative Hypothesis H1: u1 != u2

Google sheet is used to perform Hypothesis testing and Confidence interval calculation using Z-TEST and T-TEST model. [Click here](https://docs.google.com/spreadsheets/d/1GU7lqwdvYfTGoxPXMLb5SucVjKEtxCC-vlK9KNT1xH8/edit#gid=392375140) for detailed calculations.

 **Conversion rate:**
- Z-Test is used to measure the Conversion rate.
- Pooled Sample Proportion = 0.04278446356 
- Standard Error = 0.001829526081 
- Test Statistics = -3.86429177
- P-Value = 0.0001114119853

For conversion rate metric, P=0.0001 is less than significance thershold limit (0.05) and statistically significant. Hence we reject the null hypothesis and proved that there is a difference in user conversion rate between the control and treatment groups.

With 95% Confidence level we determined that difference in conversion rate will falls between 0.0035% and 0.0107%.

**Average amount spent:**
- T-Test is used to measure the Average amount spent.
- Mean of group A = 3.37451752 
- Mean of group B = 3.390866667
- Standard Deviation of group A = 25.93638327 
- Standard Deviation of group B = 25.41410528 
- Standard Error = 0.2321405061 
- Test Statistics = -0.07042780472
- Degree of Freedom = 24342 
- P-Value = 0.9438537398

For average amount spent metric, P=0.944 is not less than significance thershold limit (0.05) and statistically insignificant. Hence we fail to reject the null hypothesis and proved that there is no difference in average amount spent per user between the control and treatment groups.

With 95% Confidence level we determined that difference in average spending of users will falls between -0.4387% and 0.4715%

### Results/Findings
Statistical evidence shows that there is significant increase in conversion rate, hence its proves that users who saw banner at top of the website are tend to make more purchase than the users who didn't see the banner. So adding the banner will increase the purchase.

On other hand, statistical evidence shows that there is no significant increase in average amount spend by the users, its proves that the banner doesn't influence the users to spend more on their purchase. 

Eventhough number of purchase are increased, amount spend on the purchase is not increased. Hence there is no increase in reveneue.

### Recommedations
Business to iterate the experiment for longer duration and with large number of users which will provide us more reliable results.

