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
### 3.1 Languages & Packages
* R programming language
* lubridate: A package for working with dates and times in R.
* here: A simpler way to find your files
* skimr: Compact and flexible summaries of Data
* janitor: Simple tools for examing and cleaning Dirty Data
* tidyverse: A collection of R packages for data wrangling and visualization.
* ggplot2: A data visualization package in R.
* dplyr: A package for data manipulation in R.
### 3.2 Environments Used
* Windows 11
* RStudio
* Tableau
### 3.3 Cleaning & Manipulation
I began by renaming the files at folder origin by removing the word "merged" from the file's name. 
I then loaded the following packages into RStudio and opted for long (or Narrow) format over Wide format when given the choice.  
```
library(here)
library(skimr)
library(janitor)
library(tidyverse)
library(dplyr)
library(ggplot2)
library(lubridate)
```
The next step included importing datasets located in the working directory.

```
dailyActivity <- read.csv("dailyActivity.csv", header = TRUE)
dailyCalories <- read.csv("dailyCalories.csv", header = TRUE)
dailyIntensities <- read.csv("dailyIntensities.csv", header = TRUE)
dailySteps <- read.csv("dailySteps.csv", header = TRUE)
heartrate_seconds <- read.csv("heartrate_seconds.csv", header = TRUE)
hourlyCalories <- read.csv("hourlyCalories.csv", header = TRUE)
hourlyIntensities <- read.csv("hourlyIntensities.csv", header = TRUE)
hourlySteps <- read.csv("hourlySteps.csv", header = TRUE)
minuteCaloriesNarrow <- read.csv("minuteCaloriesNarrow.csv", header = TRUE)
minuteIntesitiesNarrow <- read.csv("minuteIntensitiesNarrow.csv", header = TRUE)
minuteMETsNarrow <- read.csv("minuteMETsNarrow.csv", header = TRUE)
minuteSleep <- read.csv("minuteSleep.csv", header = TRUE)
minuteStepsNarrow <- read.csv("minuteStepsNarrow.csv", header = TRUE)
sleepDay <- read.csv("sleepDay.csv", header = TRUE)
weightLogInfo <- read.csv("weightLogInfo.csv", header = TRUE)
```
In order to preview the files I proceeded with running the block of code below.
```
head(dailyActivity)
head(dailyCalories)
head(dailyIntensities)
head(dailySteps)
head(heartrate_seconds)
head(hourlyCalories)
head(hourlyIntensities)
head(hourlySteps)
head(minuteCaloriesNarrow)
head(minuteIntesitiesNarrow)
head(minuteMETsNarrow)
head(minuteSleep)
head(minuteStepsNarrow)
head(sleepDay)
head(weightLogInfo)
```
Using R allows commands across multiple files to be completed efficiently and quickly. 

![Case Study - File Preview in R Environment](https://github.com/karanewell/BellaBeatCaseStudy/assets/141681843/1d0164b5-fe60-46e1-8278-c619597e9ab5)

Initially, I had to take into consideration which program to assess the datasets provided in the source file. Upon realizing several of the files contained thousands of rows, R was the ultimate choice. Since there are so many lines of data I wanted to prioritize seeing if all users were listed in each dataset. 

Let's run the code using n_unique in conjunction with the ID columns.

```
n_unique(dailyActivity$Id)
n_unique(dailyCalories$Id)
n_unique(dailyIntensities$Id)
n_unique(dailySteps$Id)
n_unique(heartrate_seconds$Id)
n_unique(hourlyCalories$Id)
n_unique(hourlyIntensities$Id)
n_unique(hourlySteps$Id)
n_unique(minuteCaloriesNarrow$Id)
n_unique(minuteIntesitiesNarrow$Id)
n_unique(minuteMETsNarrow$Id)
n_unique(minuteSleep$Id)
n_unique(minuteStepsNarrow$Id)
n_unique(sleepDay$Id)
n_unique(weightLogInfo$Id)
```
Through running this code we discover the total number of participants is more accurately equal to 33. The following columns returned less than 33 participants. 

```
> n_unique(heartrate_seconds$Id)
[1] 14
> n_unique(minuteSleep$Id)
[1] 24
> n_unique(sleepDay$Id)
[1] 24
> n_unique(weightLogInfo$Id)
[1] 8
```
Until further information can be gathered *weightLogInfo* and *heartrate_seconds* datasets will be disregarded from the case study as the sample sizes are too small to be conclusive.

In order to assure accuracy in the datasets I will initiate the command to find the different types (character, integer, number) of each column contained within the data using STR command.

```
str(dailyActivity)
str(dailyCalories)
str(dailyIntensities)
str(dailySteps)
str(hourlyCalories)
str(hourlyIntensities)
str(hourlySteps)
str(minuteCaloriesNarrow)
str(minuteIntesitiesNarrow)
str(minuteMETsNarrow)
str(minuteSleep)
str(minuteStepsNarrow)
str(sleepDay)
```

## PHASE FOUR: ANALYZE
*Utilize data analysis tools to draw conclusions*

Determine the significance of removed datasets. Both heart rate and weight can be gathered by participants in order to better to understand consumer activity. As such with the limited data, and lack of participants these two datasets were deemed inconclusive and unreliable. 
## PHASE FIVE: SHARE
*Interpret and communicate results to make data-driven decisions*
## PHASE SIX: ACT
*Put insights to work in order to solve the original problem*
### Conclusion & Recommendations

## References & Acknowledgements
[FitBit Fitness Tracker Data](https://www.kaggle.com/datasets/arashnic/fitbit)

[Bellabeat](bellabeat.com)

[FitBit Data Statistics](https://www.businessofapps.com/data/fitbit-statistics/)

[Coursera ROCCC](https://www.coursera.org/lecture/data-preparation/what-is-bad-data-lHirM)

[Google Data Analytics Course](https://www.coursera.org/professional-certificates/google-data-analytics)

[Merit America](https://meritamerica.org/)
