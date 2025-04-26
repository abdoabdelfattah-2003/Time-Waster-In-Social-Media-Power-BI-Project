**Time Wasters On Social Media 
----------------------------------------

In the first we are searched about Data set but the challenge was we want the topic of Data set should be valuable and un cleaned, so we searched a lot and a lot  but we didn’t found what we wanted 🤦‍♂️

Finally we founded a Data with valuable but cleaned , so we but the errors on it .

Let’s show you what we did 🏃‍➡️

•	The part of cleaning with python :

**Step 1: Remove the trailing '-' using .str.replace()
![image](https://github.com/user-attachments/assets/d5170783-8f6f-4e59-94ef-4e96c82b2adc)

Then convert values in 'Age' column to numeric, setting any non-numeric values to NaN and Fill missing values with the mean
  ![image](https://github.com/user-attachments/assets/34999118-9f4d-4de5-9d7e-93eae50d83bc)

Convert the values to int in age
 ![image](https://github.com/user-attachments/assets/ac3d90fb-400b-482d-8b0d-9cbdb853bc1a)


**Step 2:To rename gender correctly
 

![image](https://github.com/user-attachments/assets/51192dc1-8cb3-4579-bd2b-c8c9b9cee56e)




**Step 3:To remove'x' from the location
 
![image](https://github.com/user-attachments/assets/be32be43-e11e-47a1-8ea5-1b0877396e5a)

**Step 4:To remove( job:)
 ![image](https://github.com/user-attachments/assets/60641775-7e85-40f4-8ebf-d10fba1ebb4a)



**Step 5:to remove r and u that before the Demographics
 ![image](https://github.com/user-attachments/assets/4d466a45-96e2-4aa7-b7ab-a2d7bbb6debd)


**Step 6:to make all values small letters
 
![image](https://github.com/user-attachments/assets/f42c2ba3-54a8-46ea-96e8-eea27a2acc99)




**Step 7:to remove /
![image](https://github.com/user-attachments/assets/8faec1fb-6c1f-44a0-8902-da7944050b58)

 
Step 8: to rename Device Type correctly
 ![image](https://github.com/user-attachments/assets/49535c03-1114-41be-a233-d55a4bb8d331)


Step 9: to remove'.0' and'.:'

 ![image](https://github.com/user-attachments/assets/77e34df5-f991-4f07-8757-e70752e4078f)

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

    
    
![image](https://github.com/user-attachments/assets/e193314c-ec58-4685-9bbf-406c00c57794)




    
















The part of cleaning with Dashboard : 
Overview page:
 ![image](https://github.com/user-attachments/assets/22003efb-ad22-47d5-bc1e-2eb9dcd48503)

•	Summary: we use cards to extract total time spent on each app.
•	Filters: we use slicer
•	Pages navigator: we use bookmark from view tab
•	Drag average of addiction level and drop in value and use Gauge.
•	Drag average of productivity loss and drop in value and use Gauge for visualization.
•	We use bar chart to visualize total time spent on video by video category and putting category on xaxis and total time on yaxis and putting video category in filter.
•	We use line chart to extract average total time spent on each app by day periods (morning,afternoon,evening,night).
•	We use pie chart to visualize percentage of watch reason for each country (location)and putting watch reason in legend and count of locations in value and putting location in filter.

Engagements page:


![image](https://github.com/user-attachments/assets/dd12a357-bd08-4a50-af62-3004c659c5ed)





•	we use stacked bar chart to extract which video category has more engagements putting category on yaxis and total of engagements on xaxis.
•	We use pie chart to extract average of engagements for  each day periods (morning,afternoon,evening,night).
•	We use line chart to extract the total engagements for each age bin (its size is 10 years min is 18 and max is 64) to each app by putting age on xaxis and sum of engagements on yaxis and putting platform in small multiples. 
•	We use map to know average of engagements for each location (country) we put in bubble size the average of engagementa.
Productivity Page:
![image](https://github.com/user-attachments/assets/11215d27-399e-452d-b854-c2cd60b0c289)

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
![image](https://github.com/user-attachments/assets/1475910d-a79e-46df-87fe-312df8a630aa)


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


