# Call Center Analysis
## Performance analysis of a Call Center

### Author: Tshifhiwa Maimela
#### 04 August 2023

_The Analysis showcase the Tableau Dashboard for the Call Center Performance



### INTRODUCTION

An analysis to better understand customer retention, customer interaction and to identify the areas that need improvement to better understand our customers and provide better service. Lastly, to identify systems that need improvement as well as systems that are increasing the productivity.
Stakeholders asked for recommendations from insights gained when analyzing customer interaction database based on the following questions:
1.  What is the most reccuring problem the customer is facing?
2.  Which state has most active customers?
3.  What is the avearage satisfaction score for customers?



## 1. Ask
💡 **Business Task: Analyze customer interaction to gain insight into what customers issues are and how to improve the service**  

Understanding the Key Performance Indicators (KPi)'s 


## 2. Prepare
+ Dataset used is from the Data World website in the "Real World Fake Data" directory.

+ Found in Kaggle
  
+ Data include information about Customer name, call day, response time, call duration, reason, city and state. e.t.c


## 3. Process

I used Google Sheets to clean my data. 
* I changed the Call_timestamp column data type from “General” to “Date”.
* I also changed the “call duration in minutes” and “csat_score” columns from “General” to “Number” data types.
**The picture below shows how data looked like after converting to number type.**
  
![image](https://github.com/MaimelaT/Call-Center-Analysis/assets/139053059/087aad86-b940-46f8-bf4e-001c766ed9ff)
  
* I therefore converted the dataset to zero decimal place. 
* The call_timestamp column shows that the data is dated 2020 and in October. Therefore, I extracted the “day” to a new column and named it “Call_days” and also formatted it as a “Number” data type because it is already known that the dataset is from 2020 October.
* I used the MID function to extract the number of days and the used the SUBSTITUTE Function to remove the “/” in my data. I also ensured there are no empty cells in my data.

## 4. Tableau

After cleaning and organizing the dataset, I uploaded it on Tableau:

#### Data Validation

- I double-checked the data formats of columns.
- I converted the call_timestamp and call_day to date and Number data types respectively.
- I changed the call_centre data type from a normal string to a city string.
- The csat_score column has many empty cells and therefore won’t be used in this analysis.







