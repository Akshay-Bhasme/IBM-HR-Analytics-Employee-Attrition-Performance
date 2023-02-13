# IBM-HR-Analytics-Employee-Attrition-Prediction
## Employee attrition prediction

The data set presents an employee survey from IBM, indicating if there is attrition or not. The data set contains approximately 1500 entries. Given the limited size of the data set, the model should only be expected to provide modest improvement in indentification of attrition vs a random allocation of probability of attrition.
## The Data
(Data source: https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset.)

IBM has gathered information on employee satisfaction, income, seniority and some demographics. It includes the data of 1470 employees. To use a matrix structure, we changed the model to reflect the followin data

CHECK TABLE
Name Description

AGE Numerical Value

ATTRITION Employee leaving the company (0=no, 1=yes)

BUSINESS TRAVEL (1=No Travel, 2=Travel Frequently, 3=Tavel Rarely)

DAILY RATE Numerical Value - Salary Level

DEPARTMENT (1=HR, 2=R&D, 3=Sales)

DISTANCE FROM HOME Numerical Value - THE DISTANCE FROM WORK TO HOME

EDUCATION Numerical Value

EDUCATION FIELD (1=HR, 2=LIFE SCIENCES, 3=MARKETING, 4=MEDICAL SCIENCES, 5=OTHERS, 6= TEHCNICAL)

EMPLOYEE COUNT Numerical Value

EMPLOYEE NUMBER Numerical Value - EMPLOYEE ID

ENVIROMENT SATISFACTION Numerical Value - SATISFACTION WITH THE ENVIROMENT

GENDER (1=FEMALE, 2=MALE)

HOURLY RATE Numerical Value - HOURLY SALARY

JOB INVOLVEMENT Numerical Value - JOB INVOLVEMENT

JOB LEVEL Numerical Value - LEVEL OF JOB

JOB ROLE (1=HC REP, 2=HR, 3=LAB TECHNICIAN, 4=MANAGER, 5= MANAGING DIRECTOR, 6= REASEARCH DIRECTOR, 7= RESEARCH SCIENTIST, 8=SALES EXECUTIEVE, 9= SALES REPRESENTATIVE)

JOB SATISFACTION Numerical Value - SATISFACTION WITH THE JOB

MARITAL STATUS (1=DIVORCED, 2=MARRIED, 3=SINGLE)

MONTHLY INCOME Numerical Value - MONTHLY SALARY

MONTHY RATE Numerical Value - MONTHY RATE

NUMCOMPANIES WORKED Numerical Value - NO. OF COMPANIES WORKED AT

OVER 18 (1=YES, 2=NO)

OVERTIME (1=NO, 2=YES)

PERCENT SALARY HIKE Numerical Value - PERCENTAGE INCREASE IN SALARY

PERFORMANCE RATING Numerical Value - ERFORMANCE RATING

RELATIONS SATISFACTION Numerical Value - RELATIONS SATISFACTION

STANDARD HOURS Numerical Value - STANDARD HOURS

STOCK OPTIONS LEVEL Numerical Value - STOCK OPTIONS

TOTAL WORKING YEARS Numerical Value - TOTAL YEARS WORKED

TRAINING TIMES LAST YEAR Numerical Value - HOURS SPENT TRAINING

WORK LIFE BALANCE Numerical Value - TIME SPENT BEWTWEEN WORK AND OUTSIDE

YEARS AT COMPANY Numerical Value - TOTAL NUMBER OF YEARS AT THE COMPNAY

YEARS IN CURRENT ROLE Numerical Value -YEARS IN CURRENT ROLE

YEARS SINCE LAST PROMOTION Numerical Value - LAST PROMOTION

YEARS WITH CURRENT MANAGER Numerical Value - YEARS SPENT WITH CURRENT MANAGER

## Set1. Feature Engineering
- Numercial features= Normalization
- Categorical features= Label encoding

## Set2. Feature Engineering
- Numercial features= Normalization
- Categorical features= One hot encoding

## Result Table:
![image](https://user-images.githubusercontent.com/87875987/218481367-09ce877e-113e-4f82-97e4-ccf2ac0f6619.png)

## Conclusion:
- Here if we see we care more about people who are highly probable to leave the company. And it is okay if we predict some of the Attrition= No as Attrition= Yes,but we cannot afford that if model predicts Attrition=yes as Attrition=No as we may lose those people.

- So looking at the Confusion matrix we always need False Negative value to be zero ideally and large False Positive value is acceptable.

- Looking at the confusion matrix values for all models, we know only Logistic Regression has the least False Negative value. So Logistic Regression will fulfill the purpose in detecting Attrition probable employees.









