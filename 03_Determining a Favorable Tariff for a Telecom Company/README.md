# Project "Determining a Favorable Tariff for a Telecom Company"

### Project Description

### Data

***Users Table (User Information):***
* user_id — unique user ID
* first_name — user name
* last_name — user last name
* age — user age (years)
* reg_date — tariff activation date (day, month, year)
* churn_date — tariff termination date (if omitted, the tariff was still active at the time of data download)
* city — user's city of residence
* tariff — tariff plan name

***Calls Table (Call Information):***
* id — unique call number
* call_date — call date
* duration — call duration in minutes
* user_id — caller ID

***Messages Table (Message Information):***
* id — unique message number
* message_date — message date
* user_id — sender ID message

***Internet Table (Internet Session Information):***
* id — unique session number
* mb_used — internet traffic used during the session (in megabytes)
* session_date — internet session date
* user_id — user ID

***Tariffs Table (Tariff Information):***
* tariff_name — tariff name
* rub_monthly_fee — monthly subscription fee in rubles
* minutes_included — number of minutes of talk time per month included in the subscription fee
* messages_included — number of messages per month included in the subscription fee
* mb_per_month_included — internet traffic volume included in the subscription fee (in megabytes)
* rub_per_minute — cost per minute of talk time above the tariff package (e.g., if the tariff includes 100 minutes of talk time per month, the fee will be charged starting from the 101st minute)
* rub_per_message — the cost of sending a message in excess of the tariff plan
* rub_per_gb — the cost of an additional gigabyte of internet traffic in excess of the tariff plan (1 gigabyte = 1024 megabytes)

### Goal:
Customers are offered two tariff plans: "Smart" and "Ultra". To adjust the advertising budget, the sales department wants to understand which plan generates more revenue.
Using customer data from a mobile operator, analyze customer behavior and find the optimal plan.

### Tasks:
1. Data preprocessing
- Converting data to the required types
- Detecting data errors: call duration and traffic volume
2. Calculating and adding to the table for each user:
* Number of calls made and minutes spent by month;
* Number of messages sent by month;
* Internet traffic volume consumed by month;
* Monthly revenue per user.
3. Exploratory Data Analysis
* How many minutes of talk time does a user of each plan require per month?
* How many messages does a user of each plan require per month?
* How much internet traffic does a user of each plan require per month?
4. Hypothesis Testing
* The average revenue of users of the Ultra and Smart plans differs.
* The average revenue of users in Moscow differs from that of users in other regions.

### Conclusions:
The behavior of customers of two tariff plans, Smart and Ultra, was analyzed. The Ultra plan generates more revenue. The advertising budget should be adjusted based on this information.

* The average revenue per user of the Smart plan (in this sample) is 1 294.64 rubles.
* The average revenue per user of the Ultra plan (in this sample) is 2 071.07 rubles.

Next, the hypothesis was tested that, in the general population, the average revenue of Smart plan users differs from the average revenue of Ultra plan users. There is no reason to reject this hypothesis.

***SMART Plan***
1. The sample includes 2 229 subscribers, representing 69.35% of the total sample.
Subscribers exceed their limits in all categories: calls, messages, and internet traffic. This means that subscribers incur additional charges in addition to their monthly fees for each category. The majority of revenue comes from additional charges for "extra" services – 57.5% of total revenue for the tariff. The monthly fee accounts for 42.5%.

2. Revenue for the Smart Plan is as follows:

* additional charges for internet – plan = 46.5%
* monthly fee – 42.5%
* additional charge for call minutes – 9.6%
* additional charge for messages – 1.4%

3. Subscribers use an average of 417 minutes of call time per month. The plan includes 500 minutes of talk time.
4. Subscribers send an average of 38 messages per month. The plan includes 50 messages per month.
5. Subscribers require an average of 16 GB of internet traffic. The plan includes 15 GB of internet traffic, meaning that, on average, subscribers are 1 GB short per month.
6. The hypothesis was tested that, in the general population, the average revenue of Moscow users does not differ from that of users in other regions on the Smart plan. The data confirmed this hypothesis; there is no reason to reject it.

***ULTRA Plan***
1. The sample included 985 subscribers, representing 30.65% of the total sample.
2. Subscribers to this tariff never exceeded their call or text limit over the course of the year. Subscribers only exceeded their limit on data traffic. The majority of revenue comes from the subscription fee, accounting for 94.2%. Data traffic surcharges account for only 5.8%.
3. Subscribers use an average of 545 minutes of talk time per month. The tariff includes 3,000 minutes of talk time, i.e., almost five times more than the average subscriber needs. Therefore, subscribers overpay for call minutes and don't use them, which benefits the operator.
4. Subscribers send an average of 59 messages per month. The tariff includes 1,000 messages, i.e., almost 17 times more than the average subscriber needs. Therefore, subscribers overpay for messages and don't use them.
5. Subscribers require an average of 20 GB of internet traffic. The plan includes 30 GB of internet traffic, i.e., 1.5 times more than the average subscriber needs. Therefore, subscribers overpay for internet traffic and don't use it fully.
6. We have no reason to reject the hypothesis that the average revenue of Moscow users is no different from that of users in other regions on the Ultra plan.

### Libraries and tools used
Python, Pandas, plotly, matplotlib, Numpy, SciPy libraries, data preprocessing, exploratory data analysis, data visualization, descriptive statistics, statistical hypothesis testing.
