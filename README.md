# Credit-card-approval-prediction
The purpose of this project is to use credit scoring techniques that assess the risk in lending to a particular client and build a scorecard model. Credit scoring means applying a statistical model to assign a risk score to a credit application and it is a form of Artificial Intelligence, based on predictive modelling, that assesses the likelihood of a customer defaulting on a credit obligation, becoming delinquent or insolvent.

Setting up a credit scorecard to automate even a partial percentage of new customer account decisions is a smart way to strike the right balance between managing risk and optimizing resources.

The first step to creating a credit scorecard is to define what the scorecard should predict. There are two main categories of bad accounts that credit managers aim to avoid – those that pay slowly (but will eventually pay, whether it’s 30, or 60 days late) and those that file for bankruptcy or go out of business (and will never be able to pay). This requires a general understanding of a company’s bad accounts in order to choose which data elements make the most sense for the scorecard.
Task
Build a machine learning model to predict if an applicant is 'good' or 'bad' client, different from other tasks, the definition of 'good' or 'bad' is not given. You should use some techique, such as vintage analysis to construct you label. Also, unbalance data problem is a big problem in this task.

Content & Explanation 

There're two tables could be merged by ID:

- application_record :	


ID	Client number	


CODE_GENDER	Gender	


FLAG_OWN_CAR	Is there a car	


FLAG_OWN_REALTY	Is there a property	


CNT_CHILDREN	Number of children	


AMT_INCOME_TOTAL	Annual income	


NAME_INCOME_TYPE	Income category	


NAME_EDUCATION_TYPE	Education level	


NAME_FAMILY_STATUS	Marital status	


NAME_HOUSING_TYPE	Way of living	


DAYS_BIRTH	Birthday	Count backwards from current day (0), -1 means yesterday


DAYS_EMPLOYED	Start date of employment	Count backwards from current day(0). If positive, it means the person currently unemployed.


FLAG_MOBIL	Is there a mobile phone	


FLAG_WORK_PHONE	Is there a work phone	


FLAG_PHONE	Is there a phone	


FLAG_EMAIL	Is there an email	


OCCUPATION_TYPE	Occupation	


CNT_FAM_MEMBERS	Family size	


- credit_record :


Feature name	Explanation	Remarks


ID	Client number	


MONTHS_BALANCE	Record month	The month of the extracted data is the starting point, backwards, 0 is the current month, -1 is the previous month, and so on


STATUS	Status

0: 1-29 days past due 

1: 30-59 days past due 

2: 60-89 days overdue 

3: 90-119 days overdue 

4: 120-149 days overdue 

5: Overdue or bad debts

X:write-offs for more than 150 days 

C: paid off that month X: No loan for the month
