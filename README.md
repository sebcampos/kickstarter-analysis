# An Analysis of Kickstarter Campaigns
Performing analysis on Kickstarter data to uncover trends

# Kickstarting with Excel

## Overview of Project

### Purpose
Our goal or purpose with this project was to take the given KickStarter dataset and to illustrate/analyze how different campaigns fared in relation to their launch dates and their funding goals. Utilizing the usefull software Excel, we were able to allocate the relevant information into smaller datasets and then create visuals depicting the trends in line graphs. Althought the numbers in out pivot tables gave us the information we needed, the aid of visuals charting the data was extremely helpful in identifying fluctuations and conveying them to the interested party.
## Analysis and Challenges

### Analysis of Outcomes Based on Goals
![alt text](https://github.com/sebcampos/kickstarter-analysis/blob/master/resources/Outcomes_vs_Goals.png?raw=true)
In the above image we mapped the percentages of all the successful, failed, and cancelled Kickstarters relevant to their goals under the subcategory Plays. This was done utilizing the Excel software. We created a new sheet where a COUNTIF function was used to reference and count the outcomes based on filters mentioned above. The data was then populated based on a 12 different ranges based on the Kickstarters Goals column that we created. Below is one of the 'scripts' using the function to populate a sell.

`=COUNTIFS(KickStarter!$D:$D, ">=25000",KickStarter!$D:$D, "<30000",KickStarter!$F:F,"failed",KickStarter!R:R,"plays")`

The above code references the original KickStarter data for outcomes within the range of less than or equal to 25000  and less than 30000. It also ensures that these outcomes are being selected only from rows including the values "plays" as well as "failed". Once a column was made for each category we used another function to populate four new columns. The first, The Total Projects column, counted all the outcomes we had just collected on this new page. resulting in a new column Total Projects for each of the 12 ranges or indexes. Finally the last three columns where populated using the the total of plays based on category in the given range divided by the total plays in that range. Doing so we created three columns for each category and populated it with the percentage associated with that category and range

`=B3/E3`

The above function took the information from B3 or number of succesfull outcomes within the range 1000 to 4999 and divided it by the total number of outcomes in the same range populating the a new cell in a new column labled Percentage Successfull. This was applied to all of the previous built columns. Lastly a Chart was rendered to illustrate the data in a more clear format. The x-axis of the chart was populated by the 12 different ranges, the y-axis with the percentage of the different categories , Percentage successfull as a blue line, Percentage Failed as an amber line and Percentage Canceled as a grey line

### Analysis of Outcomes Based on Launch Date
![alt text](https://github.com/sebcampos/kickstarter-analysis/blob/master/resources/Theater_Outcomes_vs_Launch.png?raw=true)
In the above chart we illustrated the same categories of Success, Failed and Canceled outcomes except this time the data is based on the Launch Date of the Kickstarter. Using the insert pivot table function we were able to create an new Excel sheet where we selected the fields of data we were interested in. These being the columns Outcomes,Parent Category, Date Created Conversion,  and Years.
![alt text]
### Challenges and Difficulties Encountered

Although Excel has great tools for iterating, filtering, and funelling Data it can be quite intimidating. To use these tools we had to dig a little into the subscript of Excel to call the functions that would help us iterate and funnel the appropriate data then perform calculations on this new smaller set of data.
There is also the issue of navigating a pretty intimidating GUI, I myself particularly found this to be true when rendering the charts. 


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  
- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?

