# Project "A/B Test for an International Online Store"

## Project Description

### Data

**ab_project_marketing_events.csv — 2020 Marketing Events Calendar**
* name — Marketing Event Name;
* regions — Regions Where the Advertising Campaign Will Be Conducted;
* start_dt — Campaign Start Date;
* finish_dt — Campaign End Date.

**final_ab_new_users.csv — all users who registered in the online store between December 7 and 21, 2020**
* user_id — User ID;
* first_date — Registration Date;
* region — User Region;
* device — Device from Which Registration Took Place.

**final_ab_events.csv — all new user events from December 7, 2020, to January 4, 2021;**
* user_id —User ID;
* event_dt — Event Date and Time;
* event_name — Event Type;
* details — Additional Event Data. For Example, for Purchases, This Field Stores the Purchase Price in Dollars.

**final_ab_participants.csv — test participants table.**
* user_id — User ID;
* ab_test — Test Name;
* group — User Group.

### Goal:

A task from an international online store. An A/B test has been launched. The technical specifications and test results are available.

### Tasks:

1. Conduct exploratory data analysis
2. Evaluate A/B testing results
3. Draw conclusions based on the results

### Conclusions:
1. The "Christmas & New Year Promo" marketing event took place in the last 5 days of the period, starting from December 25, 2020.
Region: EU, N.America. Overlapping the A/B test with marketing activities is incorrect; this could have affected the A/B test results.

2. There are 4 events in the funnel, sorted by frequency:

* login - 58,697 users
* product_page - 38,929 users
* purchase - 19,569 users
* product_cart - 19,284 users

Some users place an order without going through the "add to cart" step.
This is because there are fewer transactions at this step than at the "order" step. This is the case in the dataset
as a whole, in group A, and in group B.

The largest number of users are lost at the third step. Only 50% of users make a purchase
after viewing the product page.
At the second step, 36% of users are lost. After registration, 66% of users
view product pages.
Between the "add to cart" step and the order, the conversion rate is 99%.

3. Users experience a different number of events:

* 25% of users experience 4 events.
* 50% of users experience up to 6 events.
* 75% of users experience up to 9 events.
* Outliers start at 16 to 36 events per user.
* Maximum outlier is 36 events per user.

4. 776 users were in both Group A and Group B, but in different tests (either in the recommender_system_test test from Group A or the interface_eu_test test from Group B).

There are no users who participated in both groups in the same test.

5. The number of events is not evenly distributed across days.

The average number of events per day is 18,516.

* 25% of days have a below-average number of events: from 10,000 to 12,515. For example, the periods December 29-27 and December 7-December 9 are the start and end of the test. December 30th saw the lowest number of events, with virtually no events recorded.

* 25% of days recorded events between 12,515 and 18,516. For example, the period from December 25th to 26th inclusive and December 12th.

* 25% of days recorded events between 18,516 and 23,670. For example, the days of December 13th, 16th, 17th, 18th, and 24th.

* 25% of days recorded events between 23,670 and 32,559. For example, the periods of December 14th-15th and December 19th-23rd.

The peak day with the highest number of events was December 21st. December 22nd was in second place.

6. Evaluation of A/B testing results showed:

* There is a significant difference between the shares of the product_page event in the two groups in terms of conversion rate. Group A has a higher conversion rate than Group B.

* There is a significant difference between the purchase event conversion rates in the two groups. Group A has a higher conversion rate than Group B.

* There is no significant difference between the product_card event conversion rates in the two groups.

Therefore, the expected result was not confirmed. Test Group B did not show a better conversion rate than Control Group A.

### Libraries and tools used
Python, Pandas, plotly, matplotlib, SciPy, NumPy, A/B testing, statistical hypothesis testing.
