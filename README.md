# Wargaming.net API Data Analysis Project

## Disclaimer
This is a World of Tanks video game analysis. All data has been extracted from Wargaming.net API [(link)](https://developers.wargaming.net/reference/all/wot/account/list/?r_realm=eu) using Python and then visualized in Power BI.

## Goal

Goal was to extract data of about 2200 accounts from Wargaming.net API and compare them to my personal account. Main questions to answer were:

- General understanding about sample population
- When the accounts were created? Distribution in time
- How many battles played?
- What is the most played tank in every tier?
- Which tank has the biggest win ratio?
- What is my top 10 most played tanks and their win ratios?



## Contents
The project consists of two parts - first is the data extraction from the API and preparing it for use (Python). Second is creating data model and visualising the data in PowerBI. 

All files are available for preview in 'src' folder and also accessible via below links:

[Main Data Extract Code](src/Players_data.ipynb)

[Tank Data Extract Code](src/Tank-data.ipynb)

[PowerBI Data Model](src/Power%20Bi%20Model.JPG)

[PowerBI Visuals](src/Power%20BI%20_Wargaming%20project.pdf)


## Conclusions

The most accounts in extracted population were created in 2012-2014  and then stabilized after 2014. About 46% of the population did not play more than 500 battles. What is interesting is that about 30% of accounts did not play a single battle. It might be beneficial to search for root cause why there are so many blank accounts and find a way to encourage people to play. 

I have played 371 battles and based on that I fall under the same 46% of 'casual' players. However, my Win Ratio is slightly bigger - 0.52 compared to 0.49.

Overall the most battles played tank is a tank called 'IS-3'. The chart can be sliced by tiers (from 1 to 10) in order to get more specific results. The tank 'T95E2' has the biggest Win Ratio - 0.67. For a more accurate Win Ratio I decided to take only tanks who had more than 50 battles played. 

Lastly, my most played tank was a Tier 5 light tank called 'A-20' with a Win Ratio 0.48 on it. 



### Challenges and what would I do different next time

It was an exciting project to work on even though there were some challenges. One of them was figuring out how to flatten nested JSON file into dataframe. While doing that I was thinking maybe next time I would write a recursive function to flatten it.
