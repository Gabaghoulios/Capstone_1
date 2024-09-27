# Google Capstone Project

## Purpose

This is the analysis of my Google Data Analytics Certification Capstone Project, offered through Coursera. 
The purpose of this project is to analyze rider habits for Cyclistic, a (fictional) Chicago-based bikeshare company that caters to bike riders with disabilities.
The Cyclistic marketing team wants to know rider habits for casual riders and annually paying members, each.
From the data provided, we will determine what steps will be taken for future marketing campaigns and maximizing annual membership.

## Process

Data processing and analysis was performed using RStudio. As detailed in the course, the data analysis workflow goes as follows:
![Analysis workflow](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*Gm_zDWazPDD_JZUcdQxafA.png)

## Ask

The main questions to guide our process in this case study are:

1. How do annual members and casual riders use Cyclistic bikes dierently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

## Prepare

R was selected for this project due to the volume of data involved. Data was collected between 2019 and 2020.
In the prepare phase the following steps were completed:

* Downloaded two .csv files from divvy-tripdata.com

* Imported the data in RStudio for processing and analysis

These were my observations upon initial inspection of the datasets:


* In the 2019 data, birth year and gender were included in customer information, along with trip duration.
These were not included in the 2020 dataset.

*There was null data in the gender and birthyear columns.

*Ride ID values changed from purely numeric in 2019 to those with mixed values (i.e., numbers and letters) in 2020.

## Process

Before analysis was conducted the rows of data needed to be made consistent.
These were the steps taken to clean the data:

* Change customer type from "Subscriber" to "member" and "Customer" to "casual"

* Added the following additional columns: day, month, year, day of week and ride duration

* Deleted rows of data that contained ride durations with negative values

* Rearranged days of the week in the correct order

*Ensured trip data matched with correct user category

*Converted ride data from factor to numeric type to perform calculations

This allowed me to effectively perform descriptive analysis on the collected rider data.

## Analyze

Descriptive analysis yielded the following results:

* Duration of shortest ride taken: 1

* Median duration of rides: 539

* Average duration of rides: 1189

* Longest ride taken: 10632022

Additionally, differences were noted in the habits of annual members and casual users, illustrated by with this graph:

![Analysis_workflow](https://raw.githubusercontent.com/Gabaghoulios/Capstone_1/refs/heads/main/Plot.jpg)




