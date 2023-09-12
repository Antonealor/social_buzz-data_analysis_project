# Social Buzz; Content Category Analysis

## Project Recap

Social Buzz is a start up company in the social media and content creation industry. Its located in San Fransico with 250 employees.
Due to its recent growth, its has found itself with massive amount of data with no capacity to manage and make useful insights of the data in its possession. 
The company therefore, sought the services of Accenture, an experienced data consultancy firm, to be able to deliver the following;

1. An analysis of their content categories that highlight the top 5 categories with largets aggregate popularity.
2. An audit of their big data practice and,
3. Recommendations for a successful IPO.

At Accenture, a project team was set up comprising of Andrew Fleming - The Chief Technical Architect, Marcus Rampton - Senior Principle, and myself Antony Oniala The Data Analyst. This team is working in consultation with the client's team lead by project sponsor among other stakeholders.

I will in particular work to deliver of the objective one of the project while my two colleagues focus on the other. For that reason, the rest of this project will entail the content analysis.

## The Problem

More than 100, 000 data collected everyday amounting to 36, 000 000 variety of data collected every year. There is therefore the need to figure out top 5 categories with the largest pupolarity.

## Data Sources

Following our engagement with the client, and as part of understanding their context and business need, seven different *datasets* as well as a *data model* were available for us to work with being.

- Content.csv
- Reactions.csv 
- ReactionTypes.csv
- Profiles.csv
- User.csv
- Location.csv and
- Session.csv

## Tools

This project was entirely completed using [Excel spreadsheets](www.micrososft.com) 

## Data Cleaning and Preparation

To be able to answer my question at hand, I figured out that i really did not need all the sets of data as I only needed the contentID, category, category types, reactionTypes and reaction score. 

So, I focused on three data sets (as below) only. I began by loading and inspecting individual datasets on the excel spreadsheets. 

- Content.csv
  - Consisted of 4 fields being Serial number, ContentID, Contenttypes and Categories.
  - Had 999 records.
- Reactions.csv and
  - Contained 4 fields being ContentID, ReactionTypes and Datetime with 24, 574 records of data.
- ReactionTypes.csv
  - Comprised of Serial number, Reactions, ReactionTypes, Sentiments and Score as Fields with 16 records of data.
 
1. In each dataset, I removed columns which I deemed not relevant but could affect the outcome of the analysis.
2. I then removed rows with missing values.
3. I ensured that the data types for each of the fields are uniform.
4. I ensured that there arent any duplicate elements in the data.
5. Finally, using reactions.csv table as the base file, I applied VLOOKUP functions to join the relevant columns of the column.csv file and also from the reactiontypes.csv file.
6. The end product was one clean file which I renamed as Accenture_project_clean_data.xlsx 

## Exploratory Data Analysis

To be able to understand the data and explore how it could help me answer the question at hand, I sought to answer some key questions including;

- How many unique categories are there?

- How many reactions are there to the most popular categories?

- What was the month with most posts?

![image](https://github.com/Antonealor/social_buzz-data_analysis_project/assets/105086797/6eec275b-757d-42e7-98d7-a777e929ba6d)

## Data Analysis

Using Excel Pivot tables, I was able to analyze the cleaned data and to gather insights on the top 5 popular content categories. I also used the Chart fucntionality to be able to visualize the data as below;

![socialbuzz](https://github.com/Antonealor/social_buzz-data_analysis_project/assets/105086797/d4442cd8-7d46-4532-b665-d2851d061bae)


I was also interested in discoving what types of contents were most popular and so I used the graph below to visualize that aspect;

![image](https://github.com/Antonealor/social_buzz-data_analysis_project/assets/105086797/26107cd4-01c1-4ee9-b899-40fb64e38544)

## Insights/Results/Findings

1. There are 16 unique categories of contents.
2. The most popular category is Culture content with 8534 reactions.
3. Cumulatively, most posts are made in the month of May
4. Out of 969, 211 sentiment score, 84.55% were positive, 8.57% were neutral while 6.8% were negative.
5. The top five categories of content are Culture, Healthy eating, travel, technology and science.
   
