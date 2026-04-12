# Project "Business Performance Analysis in Yandex.Afisha"

## Project Description

### Data

***Visits table (server log with website visit information):***
* Uid — Unique User Identifier
* Device — User Device Category
* Start Ts — Session Start Date and Time
* End Ts — Session End Date and Time
* Source Id — Identifier of the Advertising Acquisitionn Source

***Orders table (order information):***
* Uid — Unique User identifier of the User Who Placed the Order
* Buy Ts — Order Date and Time
* Revenue — Yandex.Afisha Revenue from This Order

***Costs table (marketing cost information):***
* source_id — Advertising Source Identifier
* dt — Date
* costs — Costs for This Advertising Source on this Day

### Goal:
Based on Yandex.Afisha website visit data, we need to study how people use the product.
We also need to help marketers optimize marketing costs and find optimal advertising sources.

### Tasks:

Step 1. Preprocess data

Step 2. Build reports and calculate metrics

2.1. Product:
* DAU, WAU, MAU
* Stickiness
* ASL or average session lasting
* Retention rate by visit

2.2. Sales:
* Time it takes to make a purchase
* Purchase frequency
* Average order value by cohort by month
* Retention rate by purchase
* Lifetime value of one customer (LTV, CAC, ROMI)

2.3. Marketing:
* Advertising costs
* Cost per customer acquisition
* ROMI, return on advertising costs
* Analysis of resource traffic by device type

Step 3. General conclusion

### Conclusions:
The average session duration is 60 seconds. On average, users start buying within a minute after the session's start. This means users know exactly what they want to buy.

***DAU***, number of unique users per day: 908
***WAU***, number of unique users per week: 5,716
***MAU***, number of unique users per month: 23,228

***Stickiness*** (monthly) - 3.9%
A normal stickiness (monthly) is around 20-18%. In this case, it's 3.9%, meaning users only visited once per month on average.

After the first month, the number of visitors and buyers in the cohort drops significantly.

***Retention by visits*** During the first month, we observe a low retention rate:
* before December 2017 - from 7.7% to 8.5%
* since December 2017 - from 6% to 4.2%

This is an important signal that we need to focus on retaining customers in the first month, as the majority of active customers abandon the service during this period.

At the same time, in all cohorts, the ***average order value*** of users increases the month after the month of their first purchase.

Since December 2017, the number of customers in each subsequent cohort has been declining. This means that Yandex.Afisha continues attracting fewer new customers over time.

The ***first cohort*** brings in the most revenue, even after a year of its existence.
The first cohort has the highest retention rate after a year. It is necessary to study the first cohort in more detail and identify the factors that are keeping it engaged.

***Advertising Sources***

Top 3 Months by Spending per Advertising Source: November, December, October 2017

Advertising sources 9 and 10 have the lowest spending. However, they don't generate much revenue, so they aren't optimal. (Based on ROMI, source 9 is in 4th place, and source 10 is second to last.)

Top 3 sources by revenue-to-cost ratio: channels 1, 2, and 5.

Channel 3 turned out to be the least effective channel. It's the most expensive and only ranks 6th in revenue.

***Devices***

Users access Yandex.Afisha primarily via PCs and rarely access the service via mobile devices. Perhaps the mobile version of the site isn't user-friendly enough, making it more difficult to place orders.

• The number of sessions on a PC is 2.7 times greater than on a mobile device.
• Session duration on a PC is 4 times greater than on a mobile device.

### Tools and skills used in the project:

Python, Pandas, plotly, matplotlib, seaborn libraries, data preprocessing, exploratory data analysis, cohort analysis, product metrics, unit economics
