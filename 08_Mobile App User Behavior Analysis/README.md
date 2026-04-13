# Mobile App User Behavior Analysis

## Project Description

The designers plan to change the fonts throughout the app, but there's a risk that users might feel unfamiliar with it. Users were divided into three groups: two control groups with the old fonts and one experimental group with the new ones.

### Data

Each log entry represents a user action or event.

* Event name;
* Unique user ID;
* Event time;
* Experiment numbers: 246 and 247 users are control groups, and 248 usera are in the experimental group.

### Objective:
Using mobile app usage data for grocery sales, analyze the sales funnel and evaluate the results of A/A/B testing. Make a decision based on the A/A/B testing results.

### Tasks:
1. Preprocess the data
2. Conduct exploratory data analysis:
- Determine which events are in the logs and how frequently they occur.
- Check the order in which events occur. Are all events consistent?
- Calculate the proportion of users progressing to the next step of the funnel (relative to the number of users in the previous step) using the event funnel.
- Identify the step where the most users are lost.
- Find the proportion of users who complete the first event and complete the payment.
3. Examine the experiment results.
- Check for a statistical difference between samples 246 and 247 (control groups for the A/A experiment).
- Check for a statistical difference between the test group and the control groups.

### Conclusions
No statistically significant differences were found between the two control groups, 246 and 247. This is one of the criteria for the success of an A/A test.

No statistically significant differences were found between the control and experimental groups, meaning that the hypothesis that changing the font on the homepage would affect conversion metrics was not confirmed.

**Sales Funnel**
* MainScreenAppear - 7,419 users
* OffersScreenAppear - 4,593 users
* CartScreenAppear - 734 users
* PaymentScreenSuccessful - 3,539 users
* Tutorial - 840 users

**Order of Events**
* Stage 1 MainScreenAppear - appears first for 98.5% of unique users.
* Stage 2 OffersScreenAppear - appears second for 91.47% of unique users.
* Stage 3 CartScreenAppear - appears third for 47.32% of unique users.
* Stage 4 PaymentScreenSuccessful is the fourth step for 47.05% of unique users.

**Share of users who proceed to the next step**
* % of users who proceed to the second step: 62%
* % of users who proceed to the third step: 81%
* % of users who proceed to the fourth step: 95%

The second step is the most common point of lost users. After landing on the homepage, only 62% of users proceed to the product offers page. 47.7% of users complete the checkout process from the first step to payment.

### Libraries and tools used
Pandas, A/B testing, plotly, matplotlib, seaborn libraries, data visualization, statistical hypothesis testing, product metrics, event analytics.
