# Kickstarting with Excel

## Overview of Project
For this particular project, we determined the efficacy of Louise's various Kickstarter campaigns. Using the collected data, we determined if there was a positive relationship between the outcomes and launch date or outcomes and goals. 

### Purpose
The purpose of this analysis was for the class to demonstrate a wide range of Excel skills and knowledge.  We were able to create pivot tables and charts using data we organized through filters and categories, translated through date conversions, and refined through categories and sub categories.

## Analysis and Challenges
Our first analysis was Outcomes based on Launch Date followed by an Analysis of Outcomes based on Goals.  Before beginning either analysis, we created new columns to create the percentage funded and average donation cells.  We used the Round() function while dividing the goal amount by the pledged amount to generate this number.  We utilized the round() function again when determining the average donation by dividing the donations by the number of backers.  
![Roung.png](https://github.com/WIPartain/kickstarter-analysis/blob/main/roung.png?raw=true)

We also used the text to columns function to seperate the Categories into parent and subcategories.
![Category.png](https://github.com/WIPartain/kickstarter-analysis/blob/main/Category.png?raw=true)

### Analysis of Outcomes Based on Launch Date
We used an epoch translation code which allowed us to effectively determine the date of the launch by creating a Date Created Conversion in Column S. From there, we used the year function to seperate the year of the launch into column R.  
![date.png](https://github.com/WIPartain/kickstarter-analysis/blob/main/date.png?raw=true)
Once we isolated these two variables we created a pivot table filtering on the Parent category and the Years column we just created.  Our columns would be based on the "Outcomes" cells, and our Rows would be based on "Dates Created" which signified our launch dates.

We visualized this data using a Line Chart titled "Theater Outcomes by Launch Date."
![Theater_Outcomes_Vs_Launch.png](https://github.com/WIPartain/kickstarter-analysis/blob/main/Crowdfunding%20Analysis/Resources/Theater_Outcomes_Vs_Launch.png?raw=true)
### Analysis of Outcomes Based on Goals
We created a new data sheet to determined outcomes based on the goals set for each kickstarter campaign in our data set.  We created 12 different ranges for our goals, and used a countifs() function to count the number of times the outcomes resulted in "successful", "failed", or "canceled".  
![Goals_Spreadsheet.png](https://github.com/WIPartain/kickstarter-analysis/blob/main/Goals_Spreadsheet.png?raw=true)
We then used this information to determine the percentage of successful, failed, and canceled.  We then visualized the results in another line graph.  
![Outcomes_Vs_Goals.png](https://github.com/WIPartain/kickstarter-analysis/blob/main/Crowdfunding%20Analysis/Resources/Outcomes_vs_goals.png?raw=true)

### Challenges and Difficulties Encountered
Personally, the major challeneges I encountered during this project centered around the countifs() function in the Outcomes Based on Goals chart.  I had never used that function before, and I found it frustrating until I eventually got the hang of it.  The rest of the project was pretty straightforward. 

## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?
The first conclusion from this analysis is that the "theater" subcategory was the most successful.  Each month consistently had more successes than failures, and only "music" was the other subcategory with a similar trend.  However, "music" did not have nearly as many successes as "theater". We can also determine that the summer months generated the most successes for the "theater" subcategory while the failures stayed pretty consistent.

### What can you conclude about the Outcomes based on Goals?
We can conclude that there is no real correlation between outcomes and the amount set for goals.  The line chart demonstrates that the percentage of success and failure have no real consistency based on this particular data set.

### What are some limitations of this dataset?
Despite having nearly 5000 rows of data, this set still seems relatively small.  I believe a larger dataset over a longer period of time would help us determine trends with more confidence.

I would also like to know what kind of advertising goes into these kickstarter promotions.  It is possible that different methods of marketing affected the number of donors for the promotion, thus contributing to the success of the promotion.

### What are some other possible tables and/or graphs that we could create?

I would be interested in determining which genres generated the most donors or the highest donations on average.  A pie chart would help visualize the number of donors on average per genre.
