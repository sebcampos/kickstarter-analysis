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
=COUNTIFS(KickStarter!$D:$D, ">=25000",KickStarter!$D:$D, "<30000",KickStarter!$F:F,"failed",KickStarter!R:R,"plays")
The above code references the original KickStarter data for outcomes within the range of less than or equal to 25000  and less than 30000. It also ensures that these outcomes are being selected only from rows including the values "plays" as well as "failed"


The Blue line represents the percentage of successful plays while the orange depicts the percentage of failed plays. The number of cancelled plays remains a steady 0 throughout the entire dataset as no plays were cancelled.

### Analysis of Outcomes Based on Launch Date
![alt text](https://github.com/sebcampos/kickstarter-analysis/blob/master/resources/Theater_Outcomes_vs_Launch.png?raw=true)

### Challenges and Difficulties Encountered



## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
  
- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?

