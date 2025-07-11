# did-you-forget

## Overview
In the highly competitive online grocery delivery market, ensuring a seamless and customer-centric shopping experience is crucial. A common issue faced by customers is forgetting to purchase essential items. To address this, your task is to design and implement a "Did You Forget?" system that assists users by suggesting items they may have forgotten to add to their cart before checking out. \
(kaggle competition link: https://www.kaggle.com/competitions/did-you-forget-b-25/overview)

## Problem Statement
Develop a machine learning-based recommendation system that identifies and suggests items likely forgotten by customers based on their shopping behavior, past purchases, and current cart contents.

## Objective
* Build a recommendation system to predict the remaining items from the last order that the customer might have forgotten to order based on customer's previous order.
* The recommendation system should make recommendations: one that contains a set of 5 SKUs as recommendation.
* Generate the recommendations for all the orders available in last_orders_subset.csv

## Data
There are two datasets: \
**all_except_last_orders.csv** \
The above file contains all the orders made by customers of an online retail store for a specific duration of time. \
**last_orders_subset.csv** \
This file contains the SKUs that contains the last order (most recent) by the customers. But it contains only a subset (around 70% to 80%) of the SKUs from the order. The remaining SKUs are withheld as the items that the customer have forgotten to order.

## Evaluation Criteria
On submission of the recommendation submissions will be evaluated with the actual test set (withheld) using recall@5 metrics. recall metrics will be measured using: \
$$\frac{1}{N}\sum_{i=1}^{N}\frac{\text{Number of forgotten items identified by the model}}{\text{Number of items forgotten by the customer in order}}$$


## Citations
```
@misc{did-you-forget-b-25,
    author = {manaranjan pradhan},
    title = {Did you forget B23},
    year = {2025},
    howpublished = {\url{https://kaggle.com/competitions/did-you-forget-b-25}},
    note = {Kaggle}
}
```
