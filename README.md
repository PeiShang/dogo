# Hi, Welcome to dota2prediction

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

We have some pro dota2 teams matches data, we want to predict some match result using these data, do you have any idears? Give it a try!

## Datasets
Under /ref folder there are 3 files:
  - **teams_id.csv** : the id of pro teams
  - **heroes_id.csv** : the id of heroes (characters in dota2)
  - **Top_1000_teams_mathces.csv** : matches data of top 1000 pro teams, containing      both features and labels.

The features are:
  - `Radiant_team_id`: team id of radiant side
  - `Dire_team_id`: team id of dire side
  - `Radiant_team_rating`: team's rating of radiant side (offical rating)
  - `Dire_team_rating`: team's rating of dire side (offical rating)
  - `Radiant_team_hero1-5`: heroes that radiant pick
  - `Dire_team_hero1-5`: heroes that dire pick
  - `start_time`: time that the match start
 
The labels (targets) are:
  - `Radiant_win`: if radiant side win the match
  - `Radiant_fb`: if radiant side get the first blood
  - `Radiant_10kill`: if radiant side first get 10 kill

Our model only reach 55% acc on the dev set, a little better than random guess...
Hope you can do it better!
