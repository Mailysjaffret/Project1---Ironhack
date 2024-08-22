# Project1---Ironhack

## Module 1 Project: Behind the Olympic Glory

# Project Group Names
Amir Abdul, Marco Morás, Maïlys Jaffret, & Sasha Crowe

# Project Intro.
We asked ourselves what is behind the glory of an Olympic win.
By looking at modern Olympic data, we took a first look into this very compelling topic.


# Questions asked / hypothesis
What do ‘successful’ countries have in common? 
We hypothesize that some winning components are at play, such as GDP per capita, population size, host effect, & star athletes.

We measured Olympic success by combined medal count
At what point on that metric do we draw the line as successful? We looked at the top 10 winners or top number of hosts (question depedent)

TIME CONSTRAINTS: last 10 Olympics 
-> 1984 Summer LA, USA to 2024 Paris, France
-> 1988 Winter Calgary, Canada to 2022 Beijing, China


# Methodology
Cleaning Process:
Drop unnecessary columns
Drop data before 1984
Drop any country that was not an Olympic participant
Renaming columns and merging df
Data type change (numeric values)
Date data processing (split)
Filling nan (selected columns)
Drop remaining nan, less than 0.5%

→ Countries dataframe
→ Athletes dataframe
→ GDP dataframe



# Analysis & Conclusion
By winning component:

GDP per capita & Population size
- None of the Top Winners are among the top 10 countries with highest GDP per capita
- But 4 are in the top 10 countries with highest population, indicating a potential influence here
- The top ten winning countries have over double GDP per capita (128% ↑) than the total average of Olympic participating countries combined
- The top ten winning countries have over 10x the median population (11,138% ↑) than the median of Olympic participating countries combined

Host-effect   
- Total medals are higher for host countries when NOT hosting, however there is a low sample size bias here to consider

Star athletes   
- Star athletes contribute a positive relation between their number of participation and number of medals
- Gender gap is closing with time
- Age appears to differ between winter & summer Olympics but further analysis needed to confirm as we didn't split the data


# Data Source Links
Ten csv files in total

Eight from Kaggle:
- Olympic_Games_Medal Tally.csv (1896-2022 records of medal count per country & season/year)
- https://www.kaggle.com/datasets/muhammadehsan000/olympic-historical-dataset-1896-2020?select=Olympic_Games_Medal_Tally.csv

- Olympic_Athlete_Bio.csv (1896-2022 records of each Olympic athlete & their bio. info.)
- https://www.kaggle.com/datasets/muhammadehsan000/olympic-historical-dataset-1896-2020?select=Olympic_Athlete_Bio.csv

- Olympic_Athlete_Event _Results.csv [results by athletes (medals)
- https://www.kaggle.com/datasets/muhammadehsan000/olympic-historical-dataset-1896-2020?select=Olympic_Athlete_Event_Results.csv

- Olympic_Games.csv (1896-2022 records of who hosted by season/year)
- https://www.kaggle.com/datasets/muhammadehsan000/olympic-historical-dataset-1896-2020?select=Olympics_Games.csv

- medals_total.csv (2024 records of medals per country)
- https://www.kaggle.com/datasets/muhammadehsan000/paris-2024-summer-olympic-games-dataset?select=medals_total.csv

- medals.csv [2024 athlete distribution of medals across different sports & events]
- https://www.kaggle.com/datasets/muhammadehsan000/paris-2024-summer-olympic-games-dataset?select=medals.csv

- medallists.csv (2024 medalists names, their countries, and the medals they won)
- https://www.kaggle.com/datasets/muhammadehsan000/paris-2024-summer-olympic-games-dataset?select=medallists.csv

- athletes.csv (2024 athletes' names, nationalities, and the sports they competed in)
- https://www.kaggle.com/datasets/muhammadehsan000/paris-2024-summer-olympic-games-dataset?select=athletes.csv

Two from World Data Group
- Global population over time
- https://data.worldbank.org/indicator/SP.POP.TOTL

- Global GDP per capita over time
- https://data.worldbank.org/indicator/NY.GDP.PCAP.CD?end=2023&start=1984&view=chart
