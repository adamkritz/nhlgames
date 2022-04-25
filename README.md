# nhlgames

----
## **George Washington University, Machine Learning 1 - DATS6202, Spring 2022**  
This is the repository for our Machine Learning I final project.

## Group Members:  
[Adam Kritz](https://github.com/adamkritz)  
[Sahara Ensley](https://github.com/Saharae)

## References:  
**Data:** [NHL Game Data](https://www.kaggle.com/datasets/martinellis/nhl-game-data?select=game.csv)   
In our final report we utilized 2 functions written by our Professor, Professor Huang of George Washington University.
His full github can be found [here](https://github.com/yuxiaohuang).
The specific file we utilized can be found [here](https://github.com/yuxiaohuang/teaching/blob/master/gwu/machine_learning_I/spring_2022/code/utilities/p2_shallow_learning/pmlm_utilities_shallow.ipynb).

## TO RUN:  
The results of our project can be found under the "Final Report" folder of this repo.
If you would like to run the notebook yourself you can open it in Jupyter Notebook or Google Colab.  
We put the relevant data files for our project in the "Data" folder, however the full data can be found
at the above link.

# Project Goal

The goal of this project is to create a model that can successfully predict the winner of NHL games, given the events that occurred in those games, statistically better than roughly 52.5% accuracy, which is about the best possible accuracy for the random model. This project will reveal to hockey analysts and teams what factors are important to win games, and what factors are potentially overrated.

# Motivation and Background

Hockey predictions have become a hot topic in recent years. Hockey fans praise hockey's unpredictability, citing how exciting it is to know that any team has a chance. This is usually contrasted with sports like basketball, where it is rare for underdogs to win. Here is a video of former NBA star and current NBA commentator Charles Barkley talking about why he enjoys hockey playoffs, saying that "you have no idea who is going to win." Vox put out a video on this phenomenon as well, claiming that the reason that hockey underdogs do better than basketball is due to a higher luck element in hockey.

But is hockey really so difficult to predict? Compared to other sports, hockey analytics are minimal. The few hockey betting sites that exist use extremely simple algorithms to predict which team will win, and often get it wrong. There is very little other published work about hockey analysis, mostly results from other projects with varying success. Either teams and other groups are not using complex analytics, or they do not want to publish their work publicly.

Aside from leveraging models to aid in sports betting and playoff predictions, having an accurate prediction tool can be useful for teams in post-game analysis. Models can highlight patterns of success or failure that might not be obvious when looking at raw statistics.

Our project will attempt to answer whether hockey is a difficult sport to predict. We will use multiple modeling techniques and select the best model to predict the result of hockey games given both pre-game statistics and in-game events.

# Data Source and Description

Our data comes from the NHL Game Dataset on Kaggle. The dataset was uploaded by Martin Ellis and most recently updated a year ago. The dataset contains data pulled from NHL.com from the 2000-2001 season until the 2019-2020 season.

The dataset is incredibly robust and contains multiple .csv files of data on players, coaches, teams, and games. For our project, we will only be using three of these files, games.csv, game_teams_stats.csv, and team_info.csv. Games.csv contains information about the games that happened, game_teams_stats.csv contains information about the teams that played in those games, and team_info.csv is the connecting set for these two files.

Our final data set contains data from 23716 games, with an entry for each team, for a final size of 47432 rows. We decided to combine the data from each game into a single row to allow our model to have a full view of the game so our final dataframe is 23716 samples.



