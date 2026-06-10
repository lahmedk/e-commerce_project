## e-commerce_project

Overview

This project analyzes an e-commerce dataset using Python to generate insights about sales performance.  

The goal is to demonstrate data cleaning, exploratory data analysis (EDA), and data visualization skills using Python.

Objective

This project answers the following questions:

Which products are ordered most frequently?
Which products generate the highest revenue?
Does revenue vary over time (monthly/seasonally)?
What is the distribution of order statuses?

Dataset

Source: e-commerce Dataset (Decodelabs virtual internship)

The dataset contains information, including:

    OrderId
    Date
    CustomerID
    Product
    Quantity
    UnitPrice
    ShippingAddress
    PaymentMethod
    OrderStatus
    TrackingNumber
    ItemsInCart
    CouponCode
    ReferralSource
    TotalPrice

Tools and Libraries

Python
Pandas
Matplotlib
Seaborn
Jupyter Notebook

Project Workflow
1. Data Cleaning

checked missing values and column formats
Checked for outliers and inconsistencies.

2. Exploratory Data Analysis

Which products are ordered most frequently?
Which products generate the highest revenue?
Are there any trends in revenue?
Which referral sources contribute the most orders?
What payment methods are most commonly used?

3. Data Visualization

Created visualizations including:

    Count plots
    Bar charts
    line chart

Key Findings

1- The histogram shows a right skew in total prices, suggesting the presence
of extreme values
note: should aim to use the median instead mean
2- the boxplot shows outliers present above the value of 3330
3- calculated the total price again for the quantity ordered; High-value orders 
were identified and may represent an opportunity for future customer segmentation.
4- some differences were observed between the quantity ordered and the items
present in the cart, the total price paid is correspondent to the quantity 
ordered, suggesting there might be abandoned items when cashing out. might
need to investigate the cause.
5- payment methods were almost balanced out, however online payment was in
the lead followed by cash payments.
6- Order statuses were almost balanced out, however, cancelled orders and
returned orders shows higher values than the rest which includes shipped,
pending and delivered. might need investigating further to know the cause.
7- 309 orders out of 1200 didn't include coupon codes, the rest which
included a coupon code included FREESHIP which had the higheest count,
followed by WINTER15 and SAVE10  which were balanced out.
8- Instagram was in the forefront of the referral sources, followed by
email and google then facebook and a referral which were almost
balanced out.
9- The data showed a spike in total revenue around june, which may indicate 
possible seasonality, promotional campaigns, or increased customer demand.
10- Chairs had the highest total revenue, followed by printers and laptops.
