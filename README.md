
# A Comprehensive Analysis of the 365datascience Newsfeed Using Tableau

This project takes a deep dive into the actual collection of posts from the 365datascience newsfeed. By using Tableau, a data visualization tool, the project aims to uncover hidden patterns and interesting trends within the newsfeed data.

## Objective:  
This project is on a mission to unlock the secrets of user interaction with the 365 platform's Newsfeed. We'll be building a custom Tableau dashboard, a data visualization tool, to analyze user activity from the beginning of 2023 (January 1st) to the end of May (May 31st). 
By diving deep into the Newsfeed data, we'll be crafting charts and graphs that reveal user behavior patterns and trends. This intel will be the key to unlocking improvements for the Newsfeed, ultimately making it more engaging for users.
 
## Charts to make:
To create these visualizations in Tableau, you can follow these steps:
### Dual Chart: Monthly Count of Posts and Average Likes per Post
#### Bar Chart for Monthly Count of Posts: 

    Drag the Date field to the Columns shelf.

    Change the date level to Month.

    Drag the Number of Posts field to the Rows shelf.
#### Line Chart for Average Likes per Post:

    Drag the Average Likes field to the Rows shelf.

    Right-click on the Average Likes axis and select Dual Axis.

    Synchronize the axes and format the charts as needed.

### Horizontal Bar Charts for Post Subtypes:
#### Overall Number of Posts per Subtype:

    Drag the Post Subtype field to the Rows shelf.

    Drag the Number of Posts field to the Columns shelf.

    Sort the chart to rank the subtypes.
#### Likes Generated by Each Subtype:

    Duplicate the previous chart.

    Replace the Number of Posts field with the Number of Likes.
#### Comments Generated by Each Subtype:

    Duplicate the previous chart.

    Replace the Number of Likes field with the Number of Comments.
### Horizontal Bar Chart for User Activity on the Newsfeed:
    Drag the User Activity field to the Rows shelf.

    Drag the Number of Users, Number of Active Users, and Number of Engaged Users fields to the Columns shelf.

    Format and sort the chart to clearly display the different user activity metrics.

## Project Starts Here:
We have the following data from the 365datascience database.

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/c984ad39-8822-40d5-b807-884f4fb53a0d)


### Open a New Worksheet:
In Tableau, open a new worksheet.

### Set the Time Range:
    Drag the Post Date field into the Columns shelf.

    Click on the Post Date pill in the Columns shelf and change the date format from Year to Month.

    Right-click the Post Date pill again and select Discrete.

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/31daa252-1e6c-4f0f-a019-1f9e34500c77)

### Display Monthly Post Count:
    Drag the Number of Posts field into the Rows shelf.

    Click on the Number of Posts pill and ensure it is set to Sum.

    Show the mark labels by clicking on Label in the Marks card and checking the Show mark labels option.

    Change the graph type to a Bar chart by selecting the Bar chart icon from the Marks card.

    Adjust the view to Entire View for better visibility.

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/c2fc64bd-9135-4f21-bdc7-929c94afb7ae)

### Compute Average Likes per Post:
    Go to Analysis > Create Calculated Field.

    Name the calculated field Avg Likes per Post.

    Enter the following formula:
    SUM([Total Likes]) / SUM([Number of Posts])

    Click OK to create the field.

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/25dd13ab-5f3a-4979-916b-30098499bc21)

### Add the Average Likes per Post to the Graph:
    Drag the Avg Likes per Post field into the Rows shelf.

    Right-click on the Avg Likes per Post axis and select Dual Axis.

    Right-click again on the Avg Likes per Post axis and select Synchronize Axis.

    Right-click on the Avg Likes per Post field in the Rows shelf and select Format.

    In the formatting pane, under the Pane tab, set the numbers to display two decimal places.

    On the Marks card, click on the dropdown menu for Avg Likes per Post and select Line.

    Right-click on the Post Date filter and select Show Filter to display the filter on the worksheet.

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/ca2cdf97-e154-44ad-8205-66cda597a4b2)

## Horizontal bar charts that rank the following post subtypes:
Posts per subtype:

  ![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/d414704c-a635-4eb2-afb2-715b962aecd1)

Likes generated by each subtype:

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/cda0ef70-78df-4e3d-a30f-458f29b243d5)

Comments generated by each subtype:

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/c9fe7109-5657-41e5-9925-c1a755d88683)

## Creating Newsfeed User Engagement Tab
Create a horizontal bar chart to show user activity on the newsfeed using the newsfeed_project_2 database. This chart should display the number of users who visited the newsfeed, the number of active users, and the number of active users who engaged through likes, comments, or manual posts.

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/d3b41467-b2b7-4ca1-a9eb-9a336b08d3ef)

Dragging the values on the sheet we get:

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/6a2e1c00-1cb0-43a3-ab4c-c440d84869d3)

## Creating Cards
Will now create the cards for Total Posts, Total Comments, and Average likes as follows:


Total Comments and Total Likes:

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/62271f51-d086-4f92-9703-975adb9d59f2)

Total Posts and Active Users:

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/459c4882-0273-4bba-b210-e46e865d4776)

## Creating Dashboard:
Arranging all the sheets on the dashboard:

![image](https://github.com/Anshulpb02/Newsfeed-Analysis-Dashboard/assets/99670506/dac0cf27-4a4a-4a00-be90-faba2c8beed9)

This is the end of the project.
