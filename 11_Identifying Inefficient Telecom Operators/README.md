# Project "Identifying Inefficient Telecom Operators"

## Project Description

### Data

**Dataset telecom_clients.csv:**
* user_id — Client Account ID
* tariff_plan — Client's Current Tariff Plan
* date_start — Client Registration Date

**Dataset telecom_dataset.csv:**
* user_id — Client Account ID
* date — Statistics Date
* direction — Call Direction (Out - Outgoing Call, In - Incoming Call)
* internal — Whether the Call is an Internal Call between the Client's Operators
* operator_id — Operator ID
* is_missed_call — Whether the Call Was Missed
* calls_count — Number of Calls
* call_duration — Call Duration (Excluding Wait Time)
* total_call_duration — Call Duration (Including Wait Time)

### Purpose:
Service is developing a new feature that will provide managers with information about their least effective agents. Ineffective agents are those with a high number of missed incoming calls (internal and external), as well as high wait times for incoming calls. Such operators may also make few outgoing calls if they are working on outbound calls.

It is necessary to define ineffectiveness criteria, identify patterns, and test hypotheses.

Identifying ineffective employees will increase the value of service to the client, thereby potentially increasing the client's lifetime value. A motivation system for agents will also be developed in collaboration with HR.

### Tasks:

Step 1. Review general information. Data preprocessing

1.1. Review missing values. Remove or fill in missing values.

1.2. Review type conformance. Convert data to the appropriate types;

1.3. Review and process duplicates;

1.4. Add a new column ['waiting_time'] to the telecom_dataset dataset, which calculates the wait time for a call.

1.5. Add a new column ['average wait time_per_call'] to the telecom_dataset dataset, which calculates the average wait time for a call.

1.6. Combine the telecom_clients and telecom_dataset datasets to test the hypothesis.

Step 2. Exploratory Analysis

2.1. Examine the data distributions: identify any anomalies, if any, and assess the presence of outliers. Work with outliers.

2.2. Identify relationships between data.

2.3. Determine the number of agents clients have.

2.4. Analyze the wait time for incoming external calls. Based on the data distribution, identify criteria for identifying ineffective agents. Determine the threshold beyond which wait time is considered high.

2.5. Analyze the proportion of dropped calls by agent. Based on a study of the data distribution, identify criteria for identifying ineffective operators. Determine the threshold below which the number of missed incoming calls will be considered high.

2.6. Analyze the number of outgoing calls. Based on a study of the data distribution, identify criteria for identifying ineffective operators. Determine the threshold below which the number of outgoing calls will be considered insufficient.

Step 3. Hypothesis Testing

3.1. Hypothesis Testing of the Difference in Incoming Call Wait Time Depending on the Tariff Plan

3.2. Hypothesis Testing of the Difference in the Number of Missed Incoming Calls Depending on the Tariff Plan

3.3. Hypothesis Testing of the Difference in the Number of Outgoing Calls Depending on the Tariff Plan

Step 4. Conclusions and Recommendations

### Conclusions:

**1. Number of operators per client:**

* 50% of clients have no more than 2 operators;
* 75% of clients have no more than 4 operators.

**2. Can operators handle both outgoing and incoming calls?**

* 49.82% of operators handle both outgoing and incoming calls.
* 50.18% of operators handle only one group of calls.

**3. Ineffective Agent Criteria - Wait Time for an Incoming External Call**

A threshold of 15 seconds has been established, beyond which the wait time will be considered high. Accordingly, agents who answer an incoming external call for more than 15 seconds will be considered ineffective.

**4. Ineffective Agent Criteria - Number of Missed Calls**

A threshold of 6 calls has been established, beyond which the number of missed calls will be considered high. Accordingly, agents who miss more than 5 calls per day will be considered ineffective.

**5. Ineffective Agent Criteria - Number of Outgoing Calls**

A threshold of 7 calls has been established, below which the number of outgoing calls will be considered insufficient. Accordingly, agents who make fewer than 6 calls per day will be considered ineffective.

### Libraries and Tools Used
Python, Pandas, plotly, matplotlib, seaborn, NumPy, SciPy, LabelEncoder (from sklearn.preprocessing), exploratory data analysis, data preprocessing, statistical hypothesis testing.
