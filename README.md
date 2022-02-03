# Kickstarter Analysis on Theater Campaign Outcomes

## Overview of Project

### Purpose
>The purpose of this project is to provide an analysis of the [Kickstarter](https://github.com/timbialek/Kickstarter_Analysis/blob/main/Kickstarter_Challenge.xlsx) data to help Louise's better understand why her play Fever fell short of her $2,885 goal.  She asked us to look at the outcomes based on launch dates and fund-raising goals and provide an analysis based on our findings.


---   


## Analysis and Challenges
>To perform this analysis, I used excel to manipulate the crowdfunding data that was provided in the Kickstarter file.
om

### Analysis of Outcomes Based on Launch Date
>The first analysis that was created was for the Theater Outcomes by Launch Date which uses a pivot table to show how many theater campaigns were successful, failed or canceled by launch month.  
From that pivot table I then created a Line chart, [Outcomes by Launch Date](https://github.com/timbialek/Kickstarter_Analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png), that trends by Launch date against the three different Outcome types.  On the chart you can easily visualize the relationship by month between the successful and failed campaigns.


### Analysis of Outcomes Based on Goals
>For the second part of the analysis the excel file looks at the Play Outcomes based on the fund-raising goals. Plays are a subset of the Theater category which will allow us to look at smaller population that is specific to the same kind of campaign Louise did fund raising for. In this part of the analysis, we grouped the funding goals in buckets and then used the countifs excel formula to populate the number of successful, failed and canceled campaigns in the worksheet.  Once that was completed, I then added additional columns to summarize the total number of campaigns and to display the outcomes as percentages to provide an easier way of interpreting the results.
I then used the outcomes percentages and goal buckets to create a line chart, [Outcomes based on Goals](https://github.com/timbialek/Kickstarter_Analysis/blob/main/Resources/Outcomes_vs_Goals.png), to display the relationship between the goal buckets and outcomes. 
>> In addition, below is a view of the Outcomes by goal table to go along with the graph.  I feel the table adds a little more depth to the analysis so the viewer can see the actual volumes in each category.  The graph shows that 100% of the campaigns in the $45,000 - $49,999 are successful but when looking at the table you can see there was only one play in that category. ![Outcomes by Goals Table.png](https://github.com/timbialek/Kickstarter_Analysis/blob/main/Resources/Outcomes_Based_on_Goals_Table.png)


### Challenges and Difficulties Encountered
>The countif functions in excel was the challenging part of creating the analysis and getting it to pull back the correct values based on the buckets, outcome and subcategory. 
While not incredibly difficult to overcome it did take some trial and error to setup the ranges within the formula to get the values to populate correctly. 
Another possible challenge with this analysis could be in converting the date fields that were in the excel file.  If you didn’t know that the dates were in Unix code it would have been difficult to figure out how to convert them into something readable.

---

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
	* Theater shows launched in May had the most successful campaigns with the late spring and early summers months (April-July) having a high number of successful campaigns.  When looking at the graph [Outcomes by Launch Date](https://github.com/timbialek/Kickstarter-Analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png) it starts to trend up in the spring, peaks in May, and then trends down through September until it gets to a small spike in October
	* The Theater shows that start in October have a higher number of failures compared to any other month year.  
	* Since Louise launched her campaign in June and this month has a has the second highest volume of successful campaigns the timing of her launch data does not appear to be a major factor in not meeting her goal.

- What can you conclude about the Outcomes based on Goals?

	* In reviewing the [Outcomes based on Goals](https://github.com/timbialek/Kickstarter_Analysis/blob/main/Resources/Outcomes_vs_Goals.png) the highest percentage of successful outcomes are in the < $1000 and between $1000 and $4,999 range having a 76% and 73% success rate respectively.
	* Generally speaking, if a play has a goal of over $15,000 there is only a 50% or less that it will succeed.  
	* Louise's goal was only $2,885 and the success rate for plays in the $1,000-$4,999 range is 73% that puts her in a category that is typically successful.

- What are some limitations of this dataset? 
	* It would be more helpful to break down the plays down by genre to see if there are particular types that are more successful than others
	* There is a mix of currencies in the data and without converting them we should only be comparing like currencies in the analysis
	* The data has no indicator for why people donated to particular campaign


- After looking at the Outcomes based on launch date and goals it is not apparent why Louise's play did not reach its fundraising goals.  Her launch date was in June and her goal of $2,885 both ranked in the second most successful categories for their respective analysis.  Some additional tables/charts that could be helpful in uncovering why her campaign didn't reach is goal would be as follows:

	* Campaign Length to determine if longer or shorter campaign had a higher success rate
	* Number of backers to determine if she is getting enough support compared to the other campaigns
	* Pledged Amount to see if the backers of her play are contributing as much as backers of other plays
	* Staff Picks to see if there is an impact to the success of a play based on if the staff identifies it as one of their picks
	* Modify the Launch date table to only show the subcategory of Plays.  The overall Theater category also includes musicals and spaces which could be skewing the results.
