# Bellabeat Case Study with R
*Examination and Analysis of Bellabeat related Consumers and Product Usage - A Google Certificate Data Analytics case study* 

![BellaBeat Icon 4x4](https://github.com/karanewell/BellaBeatCaseStudy/assets/141681843/32a0b72c-8429-4017-b790-e98929c9d9c1)
# INTRODUCTION
Welcome to my Google Capstone Project - Case Study 2: How Can a Wellness Technology Company Play It Smart?

I will be taking on the role of Junior Analyst assigned to the marketing analyst team of BellaBeat for the last six months. The company, Bellabeat, is a high-tech manufacturer of products for women that monitors biometric and lifestyle data to help women better understand how their bodies work and make healthier choices. In a recent meeting with the team, I learned the company has the potential to become a larger player in the global smart device market. Urška Sršen, co-founder and Chief Creative Officer of Bellabeat, believes that analyzing smart device fitness data could help unlock new growth opportunities for the company. To provide value to the team, and to answer key business questions, I will follow the six steps of the data analysis process: **ask**, **prepare**, **process**, **analyze**, **share**, and **act**.

## PHASE ONE: ASK
*Define the problem and confirm stakeholder expectations*
### 2.1 ABOUT THE COMPANY
Urška Sršen and Sando Mur founded Bellabeat, a high-tech company that manufactures health-focused smart products. Sršen used her background as an artist to develop beautifully designed technology that informs and inspires women around the world. Collecting data on activity, sleep, stress, and reproductive health has allowed Bellabeat to empower women with knowledge about their own health and habits. Since it was founded in 2013, Bellabeat has grown rapidly and quickly positioned itself as a tech-driven wellness company for women. By 2016, Bellabeat had opened offices around the world and launched multiple products.

![Bellabeat_character Icon](https://github.com/karanewell/BellaBeatCaseStudy/assets/141681843/4ab994fa-a476-469b-88c6-1571c71b112c)


### 2.2 Characters and Products
#### Characters
*Following is a guide to the key stakeholders for the project:*
* **Urška Sršen**: Bellabeat’s co-founder and Chief Creative Officer (Primary)
* **Sando Mur**: Mathematician and Bellabeat’s cofounder; key member of the Bellabeat executive team (Primary)
* **Bellabeat marketing analytics team**: A team of data analysts responsible for collecting, analyzing, and reporting data that helps guide Bellabeat’s marketing strategy. (Secondary) 
#### Products
*Bellabeat has two main offerings in circulation and three retail products reliant on app connectivity for tracking:*
* **Bellabeat app**: Provides users with health data related to their activity, sleep, stress, menstrual cycle, and mindfulness habits. This data can help users better understand their current habits and make healthy decisions. The Bellabeat app connects to their line of smart wellness products.
   * **Leaf**: Bellabeat’s classic wellness tracker can be worn as a bracelet, necklace, or clip. The Leaf tracker connects to the Bellabeat app to track activity, sleep, and stress.
   * **Time**: Wellness watch combines the timeless look of a classic timepiece with smart technology to track user activity, sleep, and stress. The Time watch connects to the Bellabeat app to provide you with insights into your daily wellness
   * **Spring**: A water bottle that tracks daily water intake using smart technology to ensure appropriate hydration throughout the day. The Spring bottle connects to the Bellabeat app to track hydration levels.
* **Bellabeat membership**: Bellabeat also offers a subscription-based membership program for users. Membership gives users 24/7 access to fully personalized guidance on nutrition, activity, sleep, health and beauty, and mindfulness based on their lifestyle and goals.
### 2.3 Business Task
The company has invested in traditional advertising media, such as radio, out-of-home billboards, print, and television, but focuses
on digital marketing extensively. Analyze smart device usage data in order to gain insight into how consumers use non-Bellabeat smart devices to help guide upcoming marketing strategies for the company. The analysis will be presented to the BellaBeat Executive Team. 
### 2.4 Business Objectives
1. What are some trends in smart device usage? 
2. How could these trends apply to BellaBeat customers? 
3. How could these trends help influence BellaBeat's marketing strategy?
### 2.5 Deliverables
* A clear summary of the business task
* A description of all data sources used
* Documentation of any cleaning or manipulation of data
* A summary of analysis
* Supporting visualizations and key findings
* High-level content recommendations based on the analysis
   
## PHASE TWO: PREPARE
*Collect and store data for analysis* 

![BellaBeat Source Files](https://github.com/karanewell/BellaBeatCaseStudy/assets/141681843/09a60197-af9a-4525-8516-09cb1d312dbc)

### 2.1 Dataset
The data is sourced from [FitBit Fitness Tracker Data](https://www.kaggle.com/datasets/arashnic/fitbit) (CC0: Public Domain license), stored on Kaggle and made available by [Mobius](https://www.kaggle.com/arashnic). The data found is considered to be open source. User has waived rights as defined by public domain. Dataset is free to be used externally for analysis. Fitbit users consented to the submission of personal tracker data, including minute-level output for physical activity, heart rate, and sleep monitoring. It includes information about daily activity, steps, and heart rate that can be used to explore users’ habits.
### 2.2 Data Information
* Files: 18
* Type: CSV
* Participants: 30
* Responses from: Amazon Mechanical Turk Survey
* Timeframe: 03.12.2016-05.12.2016
* Formats: Long and Wide datasets present
### 2.3 Data Integrity (ROCCC)

![Red Bellabeat Reliability](https://github.com/karanewell/BellaBeatCaseStudy/assets/141681843/cc0b9552-b848-4296-9e87-36d408d29cff)![Orange Bellabeat](https://github.com/karanewell/BellaBeatCaseStudy/assets/141681843/564aaa6b-a86e-4786-891a-8f964722a680)![Green Bellabeat](https://github.com/karanewell/BellaBeatCaseStudy/assets/141681843/ba8b6d87-edd6-4a43-adae-49081dc7e23d)


* **Reliable**: Potential Sample Selection Bias present in the data collected. In 2016 Fitbit had accumulated over 23 million users. The sample collected could vastly underrepresent the population of women Bellabeat seeks to attract for upcoming strategies with only 30 user responses in the dataset. The reliability of the dataset is determined to be low. 
* **Original**: Mechanical Turk (MTurk) is a crowd-sourcing platform provided by Amazon that helps in the distribution of micro-tasks among a user-base of thousands of registered participants[^1] The originality score is rated low due to the method of crowd-sourcing through a third-party vendor to gather information from anonymous participants.
* **Comprehensive**: The provided datasets include many variables and can be considered comprehensive for the analysis based on the established business objectives for the project. However, the lack of contributing factors that encompass one's health such as age and health conditions potentially skew the data leaving the score between low and medium. 
* **Current**: The data was gathered in 2016 and encompasses a time period of two months. The information is considered to be outdated and therefore receives a low score.
* **Cited**: Information was not received directly from FitBit and distributed by a third party. Cited score is low. 

[^1]https://api.drum.lib.umd.edu/server/api/core/bitstreams/ad87d60f-4cfa-4f26-bda8-3d3984b3f5d1/content  
### 2.4 Data Limitations 
Primary limitations in the data provided include: predetermined conditions of participants, the validity of participant gender, unknown data surrounding age, small data sample compared to amount of total 2016 23 million FitBit users. May contain human error if any included values were manually inputted into the tracking system.  

I will move forward with examining the data on hand and provide recommendations based on the trends. 

## PHASE THREE: PROCESS
*Clean and transform data to ensure integrity*
### 3.1 Environments Used
* Windows 11
* Google Sheets
* Tableau
### 3.3 Cleaning & Manipulation 

INITIAL Observations - if automatically tracked - several user's data was set to 0 across several days for step count. In the time span of the participants there were many rows and dates note included in the sleep data.

For the purpose of this case study I will be looking at daily habits and consumer usage along with hourly data provided from the participants. If the company finds minute details are necessary the team can create a plan to move forward with examining at a later date. 

I started my process by creating two new Google spreadsheet files and naming them "dailyActivity_all" and "hourlyActivity_all" respectively. I cleaned the date columns by ensuring the tabs each had the mm/dd/yyyy format and separated date and time into two separate columns in the hourly spreadsheet. 

There were a handful of label title inconsistencies which I proceeded to update: Moderate vs Fairly, Light vs Lightly, and SedentaryMinutes vs SedentaryActiveMinutes

The hourly spreadsheet includes: steps, calories, and intensity

From there I created a weekday column to better assist with my trend analysis later on. 

```
=CHOOSE(WEEKDAY(B2,2),"Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday")
```

## PHASE FOUR: ANALYZE
*Utilize data analysis tools to draw conclusions*

Using the formula =COUNTUNIQUE I was able to gather the distinct values of the Id column in each tab to validate the number of participants 

-daily_activity: 33
-sleep_recorded_days: 24
-hourly:
  -steps: 33
  -calories: 33
  -intensity: 33

Through running this code we discover the total number of participants is more accurately equal to 33. 

The following columns returned limited participants: heartrate_seconds: 14 and weightLogInfo: 8


## PHASE FIVE: SHARE
*Interpret and communicate results to make data-driven decisions*
## PHASE SIX: ACT
*Put insights to work in order to solve the original problem*
### Conclusion & Recommendations
Production and Marketing Opportunities:
* Weight Scale “Beat the Scale” connected to the app to reduce potential error of manual input and increase frequency and interest for use of product to better understand one's metrics and habits
* Wearable band for nighttime tracking to ensure users are getting a holistic view of their health and include regular heart monitoring

Future Projects:
Extensive heart rate and weight data can be gathered by participants in order to better understand consumer activity as such with the limited data, and lack of participants these datasets were deemed inconclusive and unreliable. Determine the significance of removed datasets at a later date as necessary.

## References & Acknowledgements
[FitBit Fitness Tracker Data](https://www.kaggle.com/datasets/arashnic/fitbit)

[Bellabeat](bellabeat.com)

[FitBit Data Statistics](https://www.businessofapps.com/data/fitbit-statistics/)

[Coursera ROCCC](https://www.coursera.org/lecture/data-preparation/what-is-bad-data-lHirM)

[Google Data Analytics Course](https://www.coursera.org/professional-certificates/google-data-analytics)

[Merit America](https://meritamerica.org/)
