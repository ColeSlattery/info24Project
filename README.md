#### info24Project

# Main Idea
We will compare the stats of the top 10 NBA scorers over the past ~40 years, to reveal trends about how scoring has changed and what attributes tend to lead to a high scoring season. Over the last 40 years, we tend to see the same players over and over again cracking the top 10 in scoring for the season and wwe want to know what they have in common or not in common. As time has changed, scoring in the NBA has progressed drastically as well. From the addoption of the 3 point line to the positionless and less formal basketball that we have became accostomed to today. 
# Data Collection
To collect our data we started by scraping the names of the top ten scorers for each season from 1980-2023 and  compile them into a dictionary with the years that the player was a top scorer. We then used a csv file containing every player and their NBA ID to save that in another dictionary with the players name.  We used a function to go through each player and used an API we found on GitHub, and matched in their NBA ID from the dictionary to pull out the players stats as a data frame with each row being a season played and the columns being all different stats from the season. From  there we took only the rows from the seasons that the player was a top ten scorer and compiled all of this data into one large dataframe.  
# Data Cleaning
There was not a ton of data cleaning we had to do once we had our main data frame, as in the process of creating it, it was already being cleaned. The only things we did to the data frame was to go through and change the year from a string from the form 1980-81  to an int as just 1980 for easier ordering and categorizing. We used that to add another two columns, grouping the players by decade and by 5ear groups. We also added a column grouping by age groups of >30,<30.

# What we'll do
The end goal of this project is to determine what specific attributes help each player score so much each season. Whether its because of their team, NBA combine stats like (height, weight, speed, vertical, etc.), or if it is complete luck and just a good season. We want to compare these statistics of each top 10 scorer is the past 40 years to see which attribute each of these players have in have in common or what they don't have in common. We can later use this as something to look for in upcoming players to see if they have these attributes that tend to lead to high scoring seasons and have a better idea if these upcoming players will be high scorers on their team. We also want to compare the last 10 or so years to the 30 that came before it and see how the way basketball is being played now compared to then affects scoring for players as well. Does this fast paced game, 3 point orriented game that we watch today equal more scoring or does the slow paced and close range, higher percentage equal more scoring?
# Restrictions
Due to the complexity of playoff structures, we won't be using playoff statistics so that each player can have that benchmark of 82 games that we can compare each of them to. We also will not be adding the defensive ability of each player and each team which may be a major factor because some teams arre easier to score on and other teams have great defenses that lead to offense. This would be a major improvement to this project and could be added when more statistics about this are given to the public.
# Understanding our data
The National Basketball Association is made up of 32 teams with 15 players each. These roster tend to change a lot during the season with trades, signings, injuries, call up's from their G league team (junior team) and a lot more. Every game is 4 quarters with 12 minutes each and players scoring averages are only effected by the games that they play. Taking this into consideration, a player could average more than another player in our data while playing less games. This data is not compiling how much they score every 82 games that they play, rather it is giving us their stats from the games that they did play in the 82 game season. We have added a minimal of 60 games played to be added to our data so that the stats couldn't have too many outliers (ex. Jermey Lin averaging 29 points per game in 2012 when he only played 12 games). Each player in our top 10 will have the points they scored throughout the whole season divided by the the games they played in to determine their scoring average for each team.
# Visualizations
 ![pic1](https://github.com/user-attachments/assets/9010ebd3-8b44-4398-ad99-cf68ddba6ee4)

We found this data to be very interesting because at first we thought there may have been some errors with our data set, but looking into season data and circumstances reveals reasons for the large dips (Lockout season and Covid season).

![pic2](https://github.com/user-attachments/assets/6abceed4-79c1-4771-b005-d1f6de562193)

While team scoring and talent has went drastically in the near past, the top 10 scores seem to have pretty consistent stats throughout the past 40 years.

![pic3](https://github.com/user-attachments/assets/56dc5c70-8849-4972-ba85-452089e50268)

3PT Added in 79-80 season
3pt Attempts Steadily Increasing
Total FG attempts relatively same

![pic4](https://github.com/user-attachments/assets/2353cc33-8ca6-48e5-b0f9-0e87a2cd17c0)

When free throws go up, so do total points and vice versa.

![pic6](https://github.com/user-attachments/assets/346a1908-9d43-4028-880b-9bd155a16f9b)

As seen on the last slide, players peak around age 29. This is again supported here with it being shown that players under 30 score slightly more points than those over 30.



