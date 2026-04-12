# Project "Testing Hypotheses to Increase Revenue in an Online Store. A/B Test"

## Project Description

### Data

***Hypothesis Table***
* Hypothesis — Brief Description of the Hypothesis;
* Reach — User Reach on a 10-point Scale;
* Impact — User Impact on a 10-point Scale;
* Confidence — Confidence in the Hypothesis on a 10-point Scale;
* Efforts — Resource Costs for Testing the Hypothesis on a 10-point Scale. The Higher the Efforts Value, the More Expensive the Hypothesis Testing.

***Orders Table***
* TransactionId — Order ID;
* VisitorId — ID of the User Who Placed the Order;
* Date — Date the Order was Placed;
* Revenue — Order Revenue;
* Group — A/B Test Group the Order was Placed in.

***Visitors Table***
* date — Date;
* group — A/B Test Group;
* visitors — Number of Users on the Specified Date in the Specified A/B Test Group

### Goal:
By running this project we pursue the goal to prioritize hypotheses, run an A/B test, and analyze the results.

### Tasks:

Step 1. Hypothesis Prioritization

1.1. Apply the ICE framework to prioritize hypotheses.

1.2. Apply the RICE framework to prioritize hypotheses.

Step 2. A/B Test Analysis

2.1. Plot a graph of cumulative revenue by group.

2.2. Plot a graph of cumulative average order value by group.

2.3. Plot a graph of the relative change in the cumulative average order value of group B versus group A.

2.4. Plot a cumulative conversion graph by group.

2.5. Plot a graph of the relative change in cumulative conversion for group B versus group A.

2.6. Plot a graph of the number of orders by user.

2.7. Plot a graph of order values.

2.8. Calculate the statistical significance of differences in conversion between groups using raw data.

2.9. Calculate the statistical significance of differences in average order value between groups using raw data.

2.10. Calculate the statistical significance of differences in conversion between groups using cleaned data.

2.11. Calculate the statistical significance of differences in average order value between groups using cleaned data.

Step 3. Decide whether to test the test based on the results.

### Conclusions:

- There are statistically significant differences in conversion between groups A and B (both raw and cleaned data);

- There are no statistically significant differences in average order value between groups A and B (both raw and cleaned data).

This test can be stopped and considered successful. User-to-customer conversion for group B is statistically significantly higher than for group A. However, the average order value does not differ between the groups.

### Tools and skills used in the project:

Python, Pandas, A/B testing, plotly, matplotlib, SciPy libraries, statistical hypothesis testing
