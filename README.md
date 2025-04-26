**Time Wasters On Social Media 
----------------------------------------

In the first we are searched about Data set but the challenge was we want the topic of Data set should be valuable and un cleaned, so we searched a lot and a lot  but we didn’t found what we wanted 🤦‍♂️

Finally we founded a Data with valuable but cleaned , so we but the errors on it .

Let’s show you what we did 🏃‍➡️

•	The part of cleaning with python :

**Step 1: Remove the trailing '-' using .str.replace()

Then convert values in 'Age' column to numeric, setting any non-numeric values to NaN and Fill missing values with the mean
  
Convert the values to int in age
 
![image](https://github.com/user-attachments/assets/d5170783-8f6f-4e59-94ef-4e96c82b2adc)

**Step 2:To rename gender correctly
 





**Step 3:To remove'x' from the location
 

**Step 4:To remove( job:)
 


**Step 5:to remove r and u that before the Demographics
 

**Step 6:to make all values small letters
 




**Step 7:to remove /
 
Step 8: to rename Device Type correctly
 





Step 9: to remove'.0' and'.:'
 
Final Step:
df.to_csv('team_project.csv')
To save changes to a new csv file

•	The part of cleaning with Power Query :

Step 1: 
We dropped columns ( id, Debt, Owns Property, Video ID, Watch Time, Importance Score)

Step 2 : 
Replace value (
•	Other in column Gender to male 
•	Atshool in column CurrentActivity to At School
•	Athome in column CurrentActivity to At Home
•	Atwork in column CurrentActivity to At Work
•	Mobile-Data in column ConnectionType to Mobile Data
•	Gming in column Video Category Gaming


Step 3 :

Transform format lowercase to column( Profession, 
Platform)

Step 4 :

Split in column ( Number of session, video category, Engament, time spend on video, scroll rate, productivity loss, self-control , addiction level)

    
















The part of cleaning with Dashboard : 
Overview page:
 
•	Summary: we use cards to extract total time spent on each app.
•	Filters: we use slicer
•	Pages navigator: we use bookmark from view tab
•	Drag average of addiction level and drop in value and use Gauge.
•	Drag average of productivity loss and drop in value and use Gauge for visualization.
•	We use bar chart to visualize total time spent on video by video category and putting category on xaxis and total time on yaxis and putting video category in filter.
•	We use line chart to extract average total time spent on each app by day periods (morning,afternoon,evening,night).
•	We use pie chart to visualize percentage of watch reason for each country (location)and putting watch reason in legend and count of locations in value and putting location in filter.

Engagements page:







•	we use stacked bar chart to extract which video category has more engagements putting category on yaxis and total of engagements on xaxis.
•	We use pie chart to extract average of engagements for  each day periods (morning,afternoon,evening,night).
•	We use line chart to extract the total engagements for each age bin (its size is 10 years min is 18 and max is 64) to each app by putting age on xaxis and sum of engagements on yaxis and putting platform in small multiples. 
•	We use map to know average of engagements for each location (country) we put in bubble size the average of engagementa.
Productivity Page:

**1. The relationship between productivity loses and addiction
----------------------------------------------------
•	Chart Type: Stacked Area Chart 
•	Purpose: Show The relationship between productivity and addiction
•	XAxis: Productivity Loses
•	YAxis: Addiction level
•	Insights: This chart will help you to understand the relationship between productivity losses and addiction and when the addiction rate increases, productivity decreases.

**2. Users Selfcontrol
---------------------
•	Chart Type: Pie chart
•	Purpose: Show how selfcontrol of users It effects on the time the users spent on social media
•	Value: Total time spent
•	Legend: Selfcontrol rate
•	Insights: This will help us to know how selfcontrol affects the time we spent on social media and when the selfcontrol rate increases, time spent decreases.


** 3. Productivity Loses
--------------------------
•	Chart Type: Line chart
•	Purpose: Show The relationship between productivity loses and time spent on social media
•	XAxis: productivity loses
•	YAxis: Time spent
•	Insights: This helps visualize the time we spent in social media effects on our productivity

 4 Productivity Loss by Profession 
 --------------------------
•	Chart Type: Stacked column chart 
•	Purpose: Show which profession have most productivity Loss rate
•	XAxis: Profession
•	YAxis: Productivity Loss.
•	Legend: Profession
•	Insights: We know that the students have high productivity Loss rate



Profit page:


**1. Platform Popularity
-----------------------
•	Chart Type: Dount chart
•	Purpose: Show the distribution of users across different social media platforms.
•	XAxis: Platform (Instagram, Facebook, etc.)
•	YAxis: Total Time Spent(min)
•	Insights: This chart will help you understand which platforms are most popular among users and which ones drive the most time spent.

**3. Time Spent per Platform
----------------------------
•	Chart Type: Stacked Column Chart
•	Purpose: Show the total or average time spent on each platform.
•	XAxis: Platform
•	YAxis: Total Time Spent(min) 
•	Legend: Gender
•	 Insights: This will help analyze how much time is spent on different platforms and by which groups

**3. Platform by Device Type
   --------------------
•	Chart Type: Clustered Bar Chart
•	Purpose: Compare platform usage across different device types.
•	XAxis: Platform
•	YAxis: Total Time Spent(min)
•	Legend: DeviceType (Smartphone, Tablet, Computer)
•	Insights: This helps visualize how users engage with platforms across different devices, showing if one platform is more popular on mobile vs. desktop.

5. Platform Usage by Connection Type
   ----------------------------
•	Chart Type: 100% Stacked Bar Chart
•	Purpose: Show the proportion of connection types (WiFi vs. Mobile Data) used on different platforms.
•	XAxis: Platform
•	YAxis: sessions.
•	Legend: ConnectionType (WiFi, Mobile Data)
•	Insights: Understand how connection types vary by platform, e.g., do users of certain platforms rely more on mobile data than WiFi?

6. Platform Usage by Age Group
   ----------------------------
•	Chart Type: Funnel
•	Purpose: Show how platform usage differs across age groups.
•	XAxis: Platform
•	YAxis: Age
•	Color: Total Time Spent(min)
•	Insights: This visual can reveal which platforms are more popular among different age groups.

**8. User Satisfaction per Platform
---------------------
•	Chart Type: Stacked Column Chart 
•	Purpose: Show the satisfaction score across different platforms.
•	XAxis: Platform
•	YAxis: Average of Satisfaction
•	Insights: This will help you understand how satisfied users are with the content or experience on each platform.


