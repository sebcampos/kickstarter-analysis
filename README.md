# An Analysis of Kickstarter Campaigns
Performing analysis on Kickstarter data to uncover trends

# Kickstarting with Excel

## Overview of Project

### Purpose
Our goal or purpose with this project was to take the given KickStarter dataset and to illustrate/analyze how different campaigns fared in relation to their launch dates and their funding goals. Utilizing the useful software Excel, we were able to allocate the relevant information into smaller datasets and then create visuals depicting the trends in line graphs. Although the numbers in our pivot tables gave us the information we needed, the aid of visuals charting the data was extremely helpful in identifying fluctuations and conveying them to the interested party.
## Analysis and Challenges

### Analysis of Outcomes Based on Goals
![alt text](https://github.com/sebcampos/kickstarter-analysis/blob/master/resources/Outcomes_vs_Goals.png?raw=true)
In the above image we mapped the percentages of all the successful, failed, and cancelled Kickstarters relevant to their goals under the subcategory Plays. This was done utilizing the Excel software. We created a new sheet where a COUNTIF function was used to reference the original dataset and count the outcomes based on filters mentioned above. The data was then populated based on 12 different ranges created from the Kickstarters Goals column. Below is one of the 'scripts' using the function to populate a cell.

`=COUNTIFS(KickStarter!$D:$D, ">=25000",KickStarter!$D:$D, "<30000",KickStarter!$F:F,"failed",KickStarter!R:R,"plays")`

The above code references the original KickStarter data for outcomes within the range of greater than or equal to 25000  and less than 30000. It also ensures that these outcomes are being selected only from rows including the values ``plays" as well as "failed". Once a column was made for each category we used another function to populate four new columns. The first, The Total Projects column, counted all the outcomes we had just collected on this new page and sorted them by their goal. This resulted in a new column Total Projects with a value of total outcomes for each of the 12 ranges/indexes. Finally the last three columns were populated using the total of plays based on category in the given range divided by the total plays in that range. Doing so we created three columns for each category and populated it with the percentage associated with that category and range

`=B3/E3`

The above function took the information from B3 or number of successful outcomes within the range 1000 to 4999 and divided it by the total number of outcomes in the same range populating the a new cell in a new column labeled Percentage Successful. This was applied to all of the previous built columns. Lastly a Chart was rendered to illustrate the data in a more clear format. The x-axis of the chart was populated by the 12 different ranges, the y-axis with the percentage of the different categories , Percentage successful as a blue line, Percentage Failed as an amber line and Percentage Canceled as a grey line

### Analysis of Outcomes Based on Launch Date
![alt text](https://github.com/sebcampos/kickstarter-analysis/blob/master/resources/Theater_Outcomes_vs_Launch.png?raw=true)
In the above chart we depicted the same categories of Success, Failed and Canceled outcomes except this time the data is based on the Launch Date of the Kickstarter and filtered to only display data pertaining to the Theater category. Using the `insert pivot table` function we were able to create a new Excel sheet where we selected the fields of data we were interested in. These being the columns Outcomes,Parent Category, Date Created Conversion,  and Years.

![alt text](https://github.com/sebcampos/kickstarter-analysis/blob/master/ExcelPhotos/Screen%20Shot%202020-09-19%20at%209.12.39%20PM.png?raw=true)

In the above image we can see where the data is selected. Data is funneled or filtered by the parent category and the Date created columns. Then from the original Kickstarter column labeled outcomes, we create the values for our new columns on the new sheet; those being Successful, Failed, and Canceled. Finally we assign the rows values of the new sheet to those of the Date created columns from the original Kickstarter dataset. Finally the values for the table are selected as the count of outcomes in each category.

![alt text](https://github.com/sebcampos/kickstarter-analysis/blob/master/ExcelPhotos/Screen%20Shot%202020-09-19%20at%209.21.24%20PM.png?raw=true)

In the above image we can select the Parent Category to only display outcomes with the Parent Category of Theaters. Under the row labels we have the rows of each
month  and the amount of outcomes that fall under that month for each column. Just like in the last graph, successful outcomes are expressed by the blue line on the graph, amber got the failed outcomes, and yellow for the canceled. The x-axis displays the months of the year and the y-axis displays the amount of Kickstarters.

### Challenges and Difficulties Encountered

Although Excel has great tools for iterating, filtering, and funneling Data it can be quite intimidating. To use these tools we had to dig a little into the subscript of Excel to call the functions that would help us iterate and funnel the appropriate data then perform calculations on this new smaller set of data.
There is also the issue of navigating a pretty intimidating GUI, I myself particularly found this to be true when rendering the charts. Google and my peers helped me by showing me more elegant ways to apply functions, such as applying them to entire columns as opposed to each individual result. Because there are so many different approaches to allocating and or filtering the appropriate data it can seem overwhelming. But These different approaches are useful and can help one decide what would be the most efficient for the task at hand, the only way to find out is to use the resources at hand (the internet, documentation,peers) and to dive right in!


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

For the Outcomes of Kickstarters in the theater category based on their Launch date the graph shows a large and steady increase of successful outcomes beginning in March with 56 successful and 33 failed and peaking in May with 111 successful and only 52 failed. This leads me to the conclusion that KickStarters which begin between these months have a higher chance of success. Another conclusion that could be drawn from this dataset is that plays from September to December have a lower chance of success. We can see that more of percentage of success drop from 59 to 37 as well as an increase in the percentage of cancellation. In December there are only 37 plays with 35 cancelled. It looks like we would want to launch our Kickstarers  plays from March to May! 
  
- What can you conclude about the Outcomes based on Goals?

From the Outcomes based on Goals chart we can see that the percentage of successful outcomes decreases as the Goal value increases. Interestingly we see a spike where the percentage of success actually increases for goals in the ranges of 25000 to 400000 before stabilizing  and then dropping to 0 percentage of success. It can be concluded that the higher the goal the less likely it will be achieved. But it is also noteworthy to say that highest range begins to increase in success percentage again.

- What are some limitations of this dataset?

Some limitations to the data set are that we are only looking through a window of 2009 - 2017
We are also not able to see the outcomes of all the live events, of which there are 114.



- What are some other possible tables and/or graphs that we could create?


