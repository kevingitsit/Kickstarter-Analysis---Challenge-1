# Kickstarter Analysis - Challenge 1
Performing analysis on Kickstarter data to find trends.

# Kickstarting with Excel

## Overview of Project

In this project we will look at trends found outcomes based on launch date and in outcomes based on goals.

### Purpose

The purpose of this project was to find what the theather launch outcomes were by specifically looking at month to month trends. We also wanted to see percentage trends in success, failed and canceled through a range of set goal amounts. 

## Analysis and Challenges 


### Analysis of Outcomes Based on Launch Date

I performed my analysis on the first sheet, "Theather Launch Outcomes by Launch Date" by selecting the data in the kickstarter work sheet and inserting a pivot table to help summarize and condense the data. I then filtered the the pivot table by "Parent Category" and "Year", set the row to show as "months", set "outcomes" in the coloumn, and then summed by "count of outcomes".

<img width="298" alt="Screen Shot 2021-10-24 at 11 33 44 PM" src="https://user-images.githubusercontent.com/69704963/138630864-496cc7be-a8ef-4f1f-b85c-846eb0737d67.png">


Since this data is collected over a reference of time, it was fitting to use a line chart to show the success, failed, and canceled data over the course of time (months).

<img width="592" alt="Screen Shot 2021-10-24 at 11 35 35 PM" src="https://user-images.githubusercontent.com/69704963/138630954-b2c248b5-d012-4643-8bb2-e2a90bd5450c.png">


### Analysis of Outcomes Based on Goals

My analysis of "Outcomes Based on Goals" began with creating a new sheet and answering the following questions:

Goal, Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, Percentage Canceled.

One of the excel formulas that I used to assist in collecting this data is COUNTIFS() and SUM(). With COUNTIFS() I was able to add "if" conditional statements for a desired goal range, outcome status, and subcategory. 

Example Code: =COUNTIFS(KickStarter!$D:$D, ">=10000",KickStarter!$D:$D,"<=14999 ", KickStarter!$F:$F, "successful", KickStarter!$R:$R, "plays")

Line chart:

<img width="616" alt="Screen Shot 2021-10-25 at 12 25 31 AM" src="https://user-images.githubusercontent.com/69704963/138634513-e202d6c6-4c8f-4fab-a33c-f2638eb628a3.png">



### Challenges and Difficulties Encountered

Difficulties that could be encountered with our analysis on outcomes based on launch date is our current line chart shows trends for multiple years. If we would want to look at individual years we would need to filter for that specific year. 

Difficulties that could be encountered with our analysis on outcomes based on goals is it doesn't tell us the categories or subcategories of the goal ranges. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  1. The success for outcomes has a positive trend when launched between the months of March to May. 
  
  2. Looking at the hike of failure outcomes in the month of October tells us we should consider another launch date to have a greater possibility of success. 

- What can you conclude about the Outcomes based on Goals?
  1.  45,000 - 49,000 goal range has the highest percentage failure. To have a 67% increase in the success percentage the goal amount should drop by $5,000. 

- What are some limitations of this dataset?
  1. Limitations on this data set is that it only accounts for a specific parent catergory for Outcomes Based on Launch Date and then a specific subcategory for          Outcomes Based on Goals. 

- What are some other possible tables and/or graphs that we could create?
  1. There could have been a bar chart that was used for Outcomes Based on Goals.
