# Project "Churn Probability Prediction for Fitness Centers"

## Project Description

### Data

* Gender
* Residence or work in the area where the fitness center is located
* Employee of a partner company (cooperation with companies whose employees can receive discounts on memberships)
* Initial registration as part of the "refer-a-friend" promotion (used a promo code from a friend when paying for the first membership)
* Availability of a contact phone number
* Age
* Time since first visiting the fitness center (in months)
* Duration of the current membership (month, 3 months, 6 months, year)
* Time remaining on the current membership (in months)
* Attendance of group classes
* Average weekly visit frequency since membership began
* Average weekly visit frequency for the previous month
* Total revenue from other fitness center services: cafe, sporting goods, cosmetics, and Massage Parlor

### Objective:

Based on visitor data for a fitness center chain, we are going to predict the likelihood of churn for each client in the next month and create user profiles using clustering.

### Tasks:
1. Preprocess the data
2. Conduct exploratory data analysis
* Study the mean values ​​of features in two groups: churn clients and recurring clients
* Study the distribution of features for those who churn (churn) and those who remain (not churn)
* Build a correlation matrix
4. Build a user churn prediction model
5. Clusterize users

### Conclusions:

* The analysis showed that customers with memberships of 6-12 months are more likely to stay. These customers have longer lifetimes. Accordingly, the fitness center should encourage customers to purchase long-term memberships.

* This can be achieved through discounts on the first membership ("refer a friend," "partner company employee"). These metrics were weighted in the clustering.

* The fitness center should note that customers in the younger age group are more likely to churn. Marketing efforts should be considered to retain customers under 25.

* Clients with an average frequency of once a week churn more often than clients with an average frequency of 2-3 times a week.

* Clusters in which clients attended more group classes had higher churn rates.

* Clients who stopped attending often had their memberships expired. Pay close attention to clients whose memberships are about to expire. Find out if they are satisfied with everything, what changes or improvements they would like, offer a promotion or special terms. Ensure that the client will renew their membership.

### Libraries and tools used
Python, Pandas, plotly, matplotlib, seaborn, Scikit-learn, classification, clustering, machine learning.
