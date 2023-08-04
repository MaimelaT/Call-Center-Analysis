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


## 2. 💻 Prepare
+ Dataset used is from the Data World website in the "Real World Fake Data" directory.

+ Found in Kaggle
  
+ Data include information about Customer name, call day, response time, call duration, reason, city and state. e.t.c


## 3. 🛠 Process

I used Google Sheets to clean my data. 
* I changed the Call_timestamp column data type from “General” to “Date”.
* I also changed the “call duration in minutes” and “csat_score” columns from “General” to “Number” data types.
**The picture below shows how data looked like after converting to number type.**
  
![image](https://github.com/MaimelaT/Call-Center-Analysis/assets/139053059/087aad86-b940-46f8-bf4e-001c766ed9ff)
  
* I therefore converted the dataset to zero decimal place. 
* The call_timestamp column shows that the data is dated 2020 and in October. Therefore, I extracted the “day” to a new column and named it “Call_days” and also formatted it as a “Number” data type because it is already known that the dataset is from 2020 October.
* I used the MID function to extract the number of days and the used the SUBSTITUTE Function to remove the “/” in my data. I also ensured there are no empty cells in my data.

## 4. 📊 Tableau

After cleaning and organizing the dataset, I uploaded it on Tableau:

#### Data Validation

- I double-checked the data formats of columns.
- I converted the call_timestamp and call_day to date and Number data types respectively.
- I changed the call_centre data type from a normal string to a city string.
- The csat_score column has many empty cells and therefore won’t be used in this analysis.


a)	Determined the number of calls the call center received each day.

![image](https://github.com/MaimelaT/Call-Center-Analysis/assets/139053059/516df7bd-a045-4c75-81f8-17dad0708745)


b)	I checked the most used channel of communication using Google sheets graph to create a pie chart.

![image](https://github.com/MaimelaT/Call-Center-Analysis/assets/139053059/41aee828-5b8e-47da-83b8-43192b828ef3)

The results showed that the most used channel of communication is the Call-center with 10639 users. This shows that users prefer to call in order to communicate.
•	This organization can increase the number of call agents.
•	Even if the call center is mostly used, can does it have a more positive outcome?
•	The web has the least number user interaction.
•	We need to find out why it has the least number of interaction and how we can improve it?


c)	I used the MS excel to create a Map chart to identify where most user interaction is located.

![image](https://github.com/MaimelaT/Call-Center-Analysis/assets/139053059/8ee3477a-15e1-4786-846b-21ef59c20504)

The results show that California is the state with most users’ interaction, followed by Texas.
•	I can use this information to find what problems California is facing and why
•	Find what channel of communication is mostly used in California and Texas and if that channel led to positive results.
•	Find the reason of users calling in and see if its positive or negative.
•	Which call center do users prefer to call in and see if the preferred location yields positive results.

Wyoming has the least number of users’ interaction.

•	Find out if least calls mean that they are happy and have nothing to complain about.


d)	A Column chart to find out the most reasons why users call in.

![image](https://github.com/MaimelaT/Call-Center-Analysis/assets/139053059/5ffab6ed-2b85-4ce9-9a9d-c287b6913a55)

From the results, most users call in with Billing questions
•	What exactly are the users asking about billing?
•	The answer will lead to understanding which method of payment is more effective and which one is problematic and then improve it.


e)	I used Google sheets to create a Bar chart to depict the time that the center receives most calls or interaction.

![image](https://github.com/MaimelaT/Call-Center-Analysis/assets/139053059/dac81833-3bb2-46bb-aca8-8e71d9bf806c)

From the results, users mostly call within SLA time frame.
•	The most used channel of communication is the Call center so this information can help us ensure the are enough Call agents available to assist with users.
•	Since Chatbox is the second most used channel of communication, it will be best to ensure strong internet communication around SLA timeframe.



# 5. Dashboard

![image](https://github.com/MaimelaT/Call-Center-Analysis/assets/139053059/849eff91-f3a2-4e1f-b686-977199ae0ff3)


## 6. 📋 Conclusion

* California and Texas have the highest number of customer interaction.
* Customers prefer the Call center followed by the Chat box as the channel of communication.
* The average call per day is consistent throughout the month.
* Majority of customers contact the call center **withing SLA time.**
* Most users have **Billing Question** at the top of their list.


## 🧗‍♀️ Recommendations

* Have more Call agents available at around
* Doing a Lean Engineering principle called line balancing, the call center can take 1/3rd of call agents working at Above SLA timeframe and place them on the "Withing SLA" time frame.
      * This way the call centre wont have to spend more money hiring agents but all shift them around according to Customer retention.
  * Find out exactly what the issue is around the **Billing question** and then implement solutions.
  * Find out which method of billing do customers prefer.
  * Imorove the design of the website to be more user-friendly.
 
------------------------------------------------------------------------------------------------------------------------------------------------------------------
