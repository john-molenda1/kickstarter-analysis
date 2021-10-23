# kickstarter-analysis
Excel Kickstart Project

## Project Overview
The purpose of this project was to analyze a variety of fundraisers that have taken place from 2009 - 2017. Using 
information like fundraising goal, amount pledged, parent category, subgateory, and launch date to determine how
that influenced the outcome of the project. Louise can then use our information to inform her decision making on future
fundraising campaigns. 

## Analysis & Challenges
### Analysis
I performed my analysis by adding additional columns to the original kickstarter sheet (i.e. adding a years column using the =Year() function, average donation by dividing pledge amount by number of backers, and using this function: =(((J2/60)/60)/24)+DATE(1970,1,1) to convert the launch date and deadlines into readable dates.

After that, I inserted pivot tables to show Louise how outcomes of fundraisers were attributed to goal amounts, outcomes were influenced by launch date, and a descriptive statistics worksheet where I showed her the mean, median, standard deviation, lower/upper quartiles, and the IQR of both goals and means for the successful and failed fundraisers. 

From there, I created line charts and bar charts from the pivot tables to best visualize how goal amounts and months of the year impacted the eventual outcome of each fundraiser. 

### Challenges
My biggest difficulty came in the 'Outcomes Based on Goals' Sheet. The number of sucessful and failed plays weren't displaying correctly and I couldn't figure out why. After much trial and tribulation, I realized my issue was that when first filling out the original =COUNTIFS() function, I had selected the wrong column in the Kickstarter worksheet, and when I autopopulated the rest of the column by clicking the bottom right corner of the cell, the issue was present in all the cells. That was really the only major issue I encountered that took a while to fix, but I could forsee an issue in the Edinburgh Research sheet by having selected the wrong lookup value or table array in my VLOOKUP function. 

## Results
### Theater Outcomes by Launch Date
1) The best month to launch a theater fundraising project is in May as there were 111 successful outcomes that month, with no significant increase in failed or canceled outcomes in May. 
2) There is a continued dropoff in the number of successful outcomes (and no decrease in failed/canceled ones) for the remained of the year. If you haven't launched your fundraised by May, then your fundraiser rapidly begins losing its chance of success.
### Outcomes Based on Goals
Fundraisers with a goal set at less than $1000 stands the greatest chance of success. As the goal increases, we see a steady decline in the likelihood of goal success until the 
goal reaches $30,000. Goal success reaches a second fead in the $35,000 - $44,999 range. However, once the goal is in excess of $45,000, the fundraiser stands essentially no chance of succeeding. 
### Dataset Limitations
We have no idea what external factors could have influenced the success or failure of a fundraiser. The fundraiser may have failed due to a terrible idea, a recession, or just poor execution. Similarly, campaigns may have succeeded due to a great idea, a great organizer, donors being in a great mood, etc. We just have no way of knowing how the data may be skewed by that. 
### Other possible tables/graphs
We could have greated a seperate pivot table that analyzed average percentage of goal pledged by date created, parent category, subcategory. From the current pivot chart, we don't know if the fundraiser failed by $1 or $100,000 as they're both showing up as failed (same scenario for cancelled and successful). 

While we had an outcome based on goal chart, and a theater outcomes by launch date chart, we could have done the same for some of the other categories like # of backers, average donation amount, launch year, or whether or not it was a staff pick. 

