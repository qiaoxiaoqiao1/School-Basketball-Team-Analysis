# School-Basketball-Team-Analysis

This is a diary-like file to document the progress we have made in some periods.


2018.6.10 ---2018.7.5

  To do the analysis of our school basketball team project, initially I want to get the access of the website API to directly fetch some data we want to work with, but after some emails with the website staffs, I cannot directly get the access from their site.
  I also tried scrapy and beautiful soup to scrape data from the website , but since the website have a lot of restrictions and log in session, I couldn't do that either.
  Since then till now, I have been working on copying the data from the website into the txt file and design our own database.
  Since the data I got in txt file are unstructured file, I found between lines of the text there are some pattern i can take advantage of to create some regexes in Python and found a way to reorganize them into nicely structured csv files so that I can directly import those files into my designed database. For those files please refer to the .py files i uploaded.

2018.7.6 - 7.15

  During this period we developed the whole database structure for future analysis, please refer to the schema and the sql for more information.

2018.7- 7.23
  This week we modified some parts of the database. Specifically, we added a new table called "Team_Cumulative" since we found some parts of the stats in this table are very valuable in calculating some critical stats such as "PER","Efficient Shooting Percentage" and such.
So I uploaded the modified version of SQL for creating tables.

7.23-7.30
  During this period we think of some ideas about how to evaluate a player.
  First we noticed that their are some breakdowns about each player's "play type", which is how they finish his possessesion when shooting the ball.
  From this point, I decided to choose "PPP" as the evaluation parameter: compare each player's overall PPP, and then compare their each  play type's PPP with the overall PPP to get the idea of "In what way is this player's performance most efficient". The results is pretty nice to me!
  Please refer to "strength and weakness" folder to get mor details.
