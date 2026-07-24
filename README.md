# Shopee Delivery Optimization - Power BI

## I. Introduction

### 1. Introduction to Dataset
  Dataset: Shopee Delivery Order datasets
  Datasets demonstrates each delivery orders including time delivery, price and relevant information.
  The dataset consists of two tables:

  - FACT_ORDERS: information of each orders and its delivery process
  - DIM_CANCEL_REASON: the reason to cancel order and its order

### 2. Business Question

The Manager want to figure out if there are any ways to optimize the operation by optimizing delivery time.

Two main questions are settled for this case:

- How much is the average order preparation time?
- What is the ratio of late delivery? Suggest solutions to solve this problem.

## II. Data transformation and processing

- Exported data to Power Query to clean, made a table of date dimension to connect to the main tables
- Built a Star Schema with the FACT_ORDERS being the primary table
- Performed some DAX formulas to calculate key metrics and create a filter
- Visualized on the interactive dashboard and recommended solutions for business questions

## III. Visualization

### Overview
<img width="1228" height="705" alt="image" src="https://github.com/ptnam190901-ai/Power-BI---Shopee-Logistics/blob/main/Shopee_Delivery_Dashboard.pdf" />

### Insights
- The time required to prepare packages for delivery reaPcowhere BsI D eitsksto ppeak at the end and the beginning of the year. This can be explained by the Tet holiday, during which people intensively purchase items online for decorations and groceries. The surge in orders leads to traffic congestion and delays in the delivery process.
- In the first week of each month, packages tend to take longer to be delivered than in other weeks. Delivery units may consolidate orders from the previous month to reduce delivery costs, which can result in longer preparation times.
- The order cancellation rate exceeds 30%. Among the cancellation reasons recorded by the Shopee system, late delivery accounts for the second-highest proportion.

### Rationale:
- Delivery Unit 3 consistently experiences more late deliveries than other units throughout the observed period, with
the number of late deliveries exceeding those of the second-highest unit by more than one-third.
- Late deliveries mainly occur in major cities in Vietnam, such as Hanoi, Long An, and Ho Chi Minh City, which are
densely populated areas.


## IV. Recommend
- Distribute packages more evenly among delivery units, particularly by reducing the excessive workload assigned to Delivery Unit 3.
- Since late deliveries are concentrated around Hanoi and Ho Chi Minh City, Shopee should establish centralized delivery hubs in these two major locations so that delivery units can collect goods from a single fixed point, improving efficiency.
- Increasing personnel in the peak period and avoid backlogging lots of goods before holidays or promotion seasons.
