# A-B-Testing-Coupon-Campaign
The following outlines the **purpose of the data analysis**, an **explanation of the data**, key **methodologies**, and **business results**. A visualization of the results is published in **Tableau**. 

**Business Problem**
The company is an online retailer specializing in handmade items. While key engagement metrics—such as time spent on the website and referral rates—are strong, only **13% of visitors  ultimately make a purchase**.

To encourage transactions, the company plans to send **discounted coupons** to registered users who have not made a purchase in the last two months. Before implementing this strategy, the data science team will conduct an A/B test to measure whether offering coupons leads to a significant increase in sales.

**Business Goal**
While increased number of user is crucial for sizing up the company, the company's primary goal is to **increase total revenue** (key metric). This project will analyze data from the A/B test to assess both the **causal impact** of the coupon campaign on purchasing behavior and its overall **monetization effect** on sales.

**Dataset** 

The dataset contains the following variables relevant to customer behavior and monetary metrics (transaction and revenue).

| Variable Name  | Description | Notes | 
| ------------- | ------------- | ------------- |
| id  | Unique customer identifier  |
| trans_after  | Number of transactions after the experiment |
| revenue_after | Total revenue after the experiment |
| test_coupon | Whether the user received a coupon | 1: Yes, 0: No|
| channel_acq | Channel of acquisition for the customer when they first signed up to the company's website | 1: Google, 2: Facebook, 3: Instagram, 4: Referral, 5: Other|
| num_pst_purch | Number of previous purchases |
| spent_last_purchase | Total spent in previous purchase |
| weeks_since_visit | # weeks since last visit |
| browsing_minutes | Time spend on website in last visit| unit: minutes|
| shopping_cart | Whether the user added a product to the shopping cart in last visit (but did not transact) | 1: Yes, 0: No|

There are a total of 5000 rows of unique users who were randomly selected to participate in the experiment.
