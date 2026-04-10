# Project "Banking Data Analysis"

## Project Description

### Data:

* children — number of children in the family
* days_employed — total work experience in days
* dob_years — client's age in years
* education — client's education level
* education_id — education level identifier
* family_status — marital status
* family_status_id — marital status identifier
* gender — client's gender
* income_type — employment type
* debt — whether the client was in arrears on loans
* total_income — monthly income
* purpose — purpose of the loan

### Objective:
Based on client solvency statistics, we aim to study whether marital status and the number of children affect the client's ability to repay a loan on time. Client: the bank's credit department.
The results of the study will be taken into account when developing a credit scoring model — a specialized system that evaluates a potential borrower's ability to repay a loan to the bank.

### Tasks:
1. Data Preprocessing
* Identify and fill in missing values
* Replace float data types with integers
* Remove duplicates
* Highlight lemmas in the loan purpose column values
* Categorize the data: List the distionaries we identified for this dataset
2. Exploratory Issues for the Examination:
* Is there a relationship between having children and on-time loan repayment
* Is there a relationship between marital status and on-time loan repayment
* Is there a relationship between income level and on-time loan repayment
* How do different loan purposes affect on-time loan repayment

### Conclusions:
When analyzing the bank's customer solvency statistics, the following results were obtained:
1. Customers without children are the most likely to take out loans and the least likely to be late with payments. 
2. Married or cohabiting clients are the most likely to take out loans and the least likely to default on loan payments.
3. Lower-middle-class clients (with monthly incomes of 50,000-70,000 rubles) are the least likely to default on loan payments. Low-income clients (with monthly incomes of 20,000-30,000 rubles) are the most likely to default on loan payments.
4. Car and education loan clients are the most likely to default on loan payments. Housing loan clients are the least likely to default.

### Libraries and tools used
Python, Pandas, plotly, matplotlib, seaborn, PyMystem3 libraries, lemmatization, data preprocessing.
