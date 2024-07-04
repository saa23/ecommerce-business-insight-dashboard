# ecommerce-business-insight-dashboard

This project objective is to gain some insights of ecommerce dataset and utilize excel's features to build an interactive and dynamic dashboard.

# 1. Dataset
The original source dataset is public datasets from Kaggle. It is based on transactions data made at Olist Store, A Brazilian ecommerce, at period **15 October 2016 - 31 August 2018** (around two years). Olist is the largest department store in Brazilian marketplace, therefore the dataset comes with transactions of various type of product categories that include up to 71 types.

Many information and insight we can gain based on the data,such as but not limited to:
- transaction by customers' location like state or city
- transaction by seller's location like state or city
- transaction by product category
- transaction by payments methods
- trend usage of payments methods
- freight performance analysis
- customer review analysis
- customer purchase behavior analysis

Here is the source link: [clik here](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).

File or Tables in the datasets are following:
1. olist_customer_dataset.csv
2. olist_geolocation_dataset.csv
3. olist_order_items_dataset.csv
4. olist_order_payments_dataset.csv
5. olist_order_reviews_dataset.csv
6. olist_orders_dataset.csv
7. olist_products_dataset.csv
8. olist_sellers_dataset.csv
9. product_category_name_translation.csv

And here is the ERD based on the original source:
![erd-schema](./images/erd.png)

## Business Context
This dataset was generously provided by Olist, the largest department store in Brazilian marketplaces. Olist connects small businesses from all over Brazil to channels without hassle and with a single contract. Those merchants are able to sell their products through the Olist Store and ship them directly to the customers using Olist logistics partners.

After a customer purchases the product from Olist Store a seller gets notified to fulfill that order. Once the customer receives the product, or the estimated delivery date is due, the customer gets a satisfaction survey by email where he can give a note for the purchase experience and write down some comments.


# 2. Methods and Processes
Since the dataset is consist of files or here we can tables, it will better if we denormalized it so that there are only much less tables used to build the interactive dashboard.


# 3. Result Previews and Insights
## 3.1. Overview Display
![overview-display](./images/overview-dashboard.png)

The figure above is the dashboard.

It comprises some sections based on insight context. They are as follows:
1. Card Metrics
2. Transactions by Payment Method
3. Transactions by State
4. Transactions by Product Category

All of them will be discussed in the following sections.

## 3.2. Card Metric
![kpi-card](./images/kpi-card.png)

This part, give insight about high-level business metrics.

It tells about:
1. total number of transaction
2. total purchased amount
3. average purchased amount per transaction
4. number of product category
5. number of customer states
6. number of customer cities
7. number of seller states
8. number of seller cities
9. customer review overall and average numbers

<br/>
Using some common knowledges, here are how to interpret the numbers in this section:
- *the higher total transaction or average transaction amount the better*

It indicates the increase revenue obtained. It is the most important metric of a business afterall.

- *the more varied the customers or seller location (state or city) the better*

It indicates that the business has positive growth in terms of market reach. It can also interpreted as the growth of business resilience. 

- *the more varied the product category the better*

It indicates that the business has increase of sales opportunity, especially if combined using strategy of cross-selling or upselling.

In addition is also means the increase in customer attraction of broader customer types.

- *the higher the customer review score the better*

It indicates of the higher customer satisfaction level. 

Based on the data, average review score is 4.2 out of 5. That means there is still plenty of room for growth.

## 3.3. Payment Method
![payment-method](./images/payment-method.png)

The figure above, tells some insights:
- the most commonly used payment method is *boleto* and *credit card*. Both significantly dominated over the other two: debit card and voucher.
- There is positive trend regarding total purchase amount over the time from 2016 to 2018. This indicates that company has positive growth. 

## 3.4. Transaction Amount by Map
![total-amount-map](./images/total-amount-map.png)

## 3.5. Transaction Amount by Product
![total-amount-product](./images/amount-by-product.gif)


