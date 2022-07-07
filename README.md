# Kickstarter-analysis

Performing analysis on Kickstarter data to uncover trends

## Overview of Project

Playwriter Louise is looking to start a crowd funding campaign to fund her upcoming play “Fever” with a goal of $10000. She wants our assistance to make her campaign successful by analysing information on how different campaigns performed based on the campaign data provided. We will be sorting and filtering the data, preparing various Pivot tables with different combinations, and visualising them with charts

## Purpose

To provide a visualized report on how campaigns fared in relation to various factors such as category, their launch dates and their fundraising goals and pledges to make Louise’s campaign successful. 

## Analysis and Challenges

The raw data provided includes all campaign details. This will be sorted, filtered, and conditionally formatted. The below screen shot of excel sheet shows conditional formatting applied on the outcomes column so that we can view successful/canceled/failed campaigns all at one glance. 

![image](https://user-images.githubusercontent.com/108366412/177680647-edd99388-eead-4ebe-97ef-ffd5efd1150d.png)

Columns such as Percentage funded, Average donation, Date Created Conversion and Date Ended Conversion will be added so that further analysis can be done on them. Also, the category column will be splitted into parent category and subcategory.

![Kickstarter_added_columns](https://user-images.githubusercontent.com/108366412/177682978-bcb9b9c0-0ec6-4dec-b3ec-2a6aaca23e4b.png)

The following parent category chart derived from a Pivot table, shows Outcomes of campaigns across all parent categories. From the chart, it can be derived that theater category has the highest number of campaigns and has 60% success ratio. Other successful categories are music and film& video. Categories such as Journalism, Food and Publishing has the least number of successful campaigns 

![image](https://user-images.githubusercontent.com/108366412/177681019-fde3d4e4-1492-4459-90f3-1129b2746839.png)

![image](https://user-images.githubusercontent.com/108366412/177681031-9d696f7b-66b2-47f4-84f1-84c7a9a5a770.png) 
 
The following sub-category chart derived from a Pivot table, shows Outcomes of campaigns across all sub-categories. The chart clearly shows we have maximum number of outcomes in plays which belongs to theater category and it also has the maximum number of successful campaigns (694 successful campaigns). 

![image](https://user-images.githubusercontent.com/108366412/177681059-37f7d94a-040d-4202-ae72-0e298997006a.png)

![image](https://user-images.githubusercontent.com/108366412/177685691-1b55dde3-b10a-4bb3-812f-41d48318e81b.png)
 
Launch Date (specifically the month of the year) has a strong impact on the number of campaigns launched and its outcome. This can be determined by the below pivot chart. Number of successful campaigns launched in May (111), June (100) and July (87) is significantly higher than those in December (37) and January (56). Number of failed campaigns around the year ranges from 33 to 50. Thus, this chart also shows that in colder months, there are fewer campaings launched overall.

![image](https://user-images.githubusercontent.com/108366412/177686379-962c187f-db94-4c88-a4a8-2f2b49f75a30.png)

### Analysis of Outcomes Based on Launch Date

The below graph shows even deeper understanding of the outcomes of theater campaigns by launch dates. The number of successful campaigns is more prominent in the months of May (111), June (100), and July (87). Here, it is important to note that the number of failed campaigns is almost same across the year (Ranges between 31 to 50 failed outcomes) but in the month of November, December, Juanuary, and March there are fewer successful campaigns (54, 36, 56, 56 successful campaigns respectively) due to which the success ratio drops in those months. 

![image](https://user-images.githubusercontent.com/108366412/177683327-3f044782-d344-4701-8da4-0c449809d667.png)

### Analysis of Outcomes Based on Goals

The following chart shows the percentage of successful/failed/cancelled campaigns with respect to the goals it had set. Campaigns with a goal of $10000 or lower has a higher chance of success. As the goal reaches $15000, one cannot be sure of the success of campaign. The graph seems to fluctuate with successful and failed campaigns beyond $15000.

![image](https://user-images.githubusercontent.com/108366412/177681143-7e13908f-bc69-4660-8c6b-a79d81e603d6.png)

### Challenges and Difficulties Encountered

   * Data included campaigns from several categories taken at different time of the year across various countries. Data needed sorting and filtering as the first step so that only important information pertaining to our needs can be further analysed. With so many different aspects of a campaign, it became difficult to determine which columns are important and which one can be dropped.

   * The dates for Launch and Deadline for the campaigns were in Unix timestamp format - new format I learnt while doing this project. It needed to be converted in a standard date format to be able to derive results.

   * There were few outliers in the data due to which conditional formatting on Percentage funded didn’t show strong conclusions.

   * Running Pivot tables with various combinations to see which fits best for the required results. The initial results I got had the sum of Ids instead of count of Ids which became a huge task to overcome. I acheived the correct outcome by constantly trying various Pivottable Fields setting.

## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?

   1. Timing of campaign launch is a huge determinant for the outcome of campaigns. It is best to launch a campaign in May and June when there is better response to campaigns. 

   2. In December and Jaunary the probability of a successful campaign is low as there are not many successful campaigns registered in that period against number of failed campaigns.  

### What can you conclude about the Outcomes based on Goals?

   * Chances of having a successful campaign is higher when the goal is within $10000. 

   * Once the campaign is $15000 and beyond, the outcome of a campaign is highly uncertain. 

### What are some limitations of this dataset?

   * Key idea of campaign could have been specified in just one or two words instead of a blurb. It can help in analysis and can assist in finding the "why" behind a success or failure 

   * Data on the marketing tools used to attract audience can also be added. Tools such as flyers, online campaigns, and radio/tv advertisements 

   * Data on target audiences such as their age, income, profession. This can boost chances of a successful campaign

   * Data seems to be providing more information on campaigns in categories like theater, music, and film & video/television and less on Journalism, publishing, games, food and photography category. Similarly, more information is available for US and UK campaigns and very few campaigns are from other countries. Equal focus should have been given across all categories in all countries.  

### What are some other possible tables and/or graphs that we could create?

   * The above analysis covered the year and month the campaign was launched. We can also cover the duration of the campaign. For achieving campaign duration, we can get the number of days between the start date and end date of the campaign and include the derived information in our analysis to check how fast campaigns performed in terms of achieving its goal.
   
   * We can remove few outliers and see if it makes any difference in results. 
   
   * We can prepare a chart with goal vs pledged information to determine how close the campaigns came in acheiving their goal. This will also help in deciding if setting unreasonable goals is one of the reasons for failure of a campaign or not. 
