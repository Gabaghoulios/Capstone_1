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

1. How do annual members and casual riders use Cyclistic bikes differently?
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

A more detailed breakdown of data can be found below:

### Trip Data Summary

| Member Type | Day of the Week | Average Ride Length (seconds) |
|-------------|------------------|-------------------------------|
| Casual      | Sunday           | 5061                          |
| Member      | Sunday           | 973                           |
| Casual      | Monday           | 4752                          |
| Member      | Monday           | 822                           |
| Casual      | Tuesday          | 4562                          |
| Member      | Tuesday          | 769                           |
| Casual      | Wednesday        | 4480                          |
| Member      | Wednesday        | 712                           |
| Casual      | Thursday         | 8452                          |
| Member      | Thursday         | 707                           |
| Casual      | Friday           | 6091                          |
| Member      | Friday           | 797                           |
| Casual      | Saturday         | 4951                          |
| Member      | Saturday         | 974                           |

## Share

As the data suggests, the majority of rides come from casual riders, with the majority of them taking place on Thursdays.

## Act

We now return to the 3 driving questions of this case study:


1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

From our analysis we can draw the following conclusions and make recommendations:

1. Casual members use Cyclistic more than annual members, but this trend may reverse when casual users are made aware of perks such as reduced rental rates
2. Casual riders would benefit from annual membership via benefits such as reduced rates, expedited login, and access to exclusive features and events
3. In order to leverage social media for boosting membership, Cyclistic could share promotions on platforms such as Facebook, Instagram and TikTok. Collecting video testimonies from current members
would serve as an effective strategy to put a more human face on reasons to subscribe. Cyclistic could also promote special events such as bike parties with special rates on social media platforms
in order to draw more users into a paid subscription. To maximize conversion, it is recommended to implement such events on days with the highest ridership, for instance, Thursdays. This could foster
a sense of community with paying members and encourage increased registration with Cyclistic. It may also be helpful to highlight environmental reasons for increasing affordable bike ridership. Most
importantly, interviewing riders with disabilities would also provide effective social evidence for more users to join Cyclistic, highlighting the benefits that specially designed bicycles have for
transporting people with disabilities in a clean, safe and effective manner and how it fosters community with them and riders without disabilities as well.

## Implementation

The timeline of implementation for this project will go as follows:

(Create visual of a timeline)

## Conclusions

Cyclistic is a popular bike sharing company that continues to serve Chicagoans throughout the city. However, the majority of its users are not subscribed to its paid services, which include perks such as
reduced rates and expedited login, to streamline the ride and rental processes. This presents a problem for Cyclistic, as this presents an obstacle for the company to acheive a consistent source of revenue.
To rectify this, it is recommended that Cyclistic implement a social media marketing campaign aimed at boosting membership and ridership. As Thursdays are the days with most activity, it would be best to 
set up an event on those days; such events could include bike parties in which casual users and annual members can mingle together and build a sense of community, which may encourage casual users to register for
annual membership. Furthermore, videos and/or writtent testimonies can be collected at these events and shared on social media platforms such as Instagram or TikTok-with user permission-to boost credibility and 
encourage membership. It may also be helpful to highlight environmental reasons for increasing affordable bike ridership. Most
importantly, interviewing riders with disabilities would also provide effective social evidence for more users to join Cyclistic, highlighting the benefits that specially designed bicycles have for
transporting people with disabilities in a clean, safe and effective manner and how it fosters community with them and riders without disabilities as well.
