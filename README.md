# CS506--Project-

Project Proposal: Predicting NBA Players Minutes Played 

1. Project Description
  This project aims to predict the total minutes an NBA player will play in a given match. Player rotation and minute allocation are heavily influenced by a combination of current season averages, recent form (e.g., last 5 games), coaching tendencies, and daily injury reports. By modeling these factors, we can better understand team rotation strategies and provide actionable insights for fantasy sports and prop betting.

  If predicting exact minutes (a continuous variable) proves too noisy or difficult, our fallback plan is to convert this into a classification problem: predicting whether a player will play *over or under* a specific threshold (e.g., over/under 20 minutes), or simply predicting whether a bench player will see the court at all (yes/no) based on other players time given.

Project Timeline: 
Weeks 1-2 : Finalize data sources, write collection scripts to pull historical box scores, and scrape injury/coach data.
Week 3-4 : Clean the data, handle missing values (especially around injury designations), and perform exploratory data analysis (EDA).
Week 5-6 : Do the baseline model training and train the model using different models. 
Week 7: Finalize the visualization, interpret the results, and work on the final report and presentation.
Week 8 (2 months : Finalize all the work and have final video presentation completed.

2. Project Motivation
    We are motivated by this project since its frustrating not to see your favorite player playing for no reason, or see some good role players not getting enough minutes in the game, and being put into the game really late. Through this we will be able to see how time is allocated for different types of player, and we plan to look at the position they play at as well. We want to see if playing time changes from regular season to playoff times, as how this make a different in how conditioned players are for important games. 

3. Project Goals

  Primary Goal: Predict the number of minutes that an NBA Player will play in a specific game, changing from regular season to playoff games. 
  Secondary Goal: Determine what are the main factors that dictate how much playing time each player gets. For ex: Experience Level, Injuries, Propaganda Surrounding a Player, etc. 

4. Data Collection Plan

   Required Data: We need historical game logs (minutes played, points, rebounds, assists), moving averages for recent form, active coach for the game, and player injury status (e.g., Probable, Questionable, Out).

   Data Collection Method:
     We plan to use Python to extract the data straight from the stats from NBA.
     Also since historical injury designation and coaching timelines are not clearly available in standard API, we plan to web scrape other data from sites like Basketball- Reference to use that data.

5. Modeling and Visualization

   We plan to utilize "scikit- learn" to build our models. We plan to start with a baseline Linear Regression, before looking at tree-based methods like Random Forest or XGBoost.
   We plan on using scatterplots to visualize predicted vs actual minutes, and feature importance bar charts to display the weight of factors like recent stats or injury status.
   We plan to implement an 80/20 train-test split in which we test 20 percent of the data. We plan to be more descriptive as we continue working not he project and progressing more into future weeks with this project. 


  
