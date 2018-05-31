# mastml-weekly

Week of 2018 May 21-25

## Daily Reports

### Monday
- labor day
 
### Tuesday

- discovered that the word 'classification' or 'regression' needs to be in the csv column name and conf file for it to know what to do.
- Talked with Ryan:
  - Decided not to start refactoring right now.
  - He thinks making a working classification model inside MASTML is a very good goal.

### Wednesday

- Almost got confusion matrix to plot.
  - Succeeded!!
  - In your CSV, you CANNOT PUT SPACES AFTER YOUR COMMAS (or they end up in the column names and break it down.)
- names of test are delimted with underscores and the first one is the key used to group them for Favorites.
- Now there is a grand total of 5 classification models. 
- TODO add cross validation for classification (use sklearn tool)

### Thursday

- Started adding a flag to the input file to choose whether you want to do classification or regression.
  - The alternative would be to have each model specify which columns to use, or split them automatically based on name.
  - Having the models choose their own data gets really involved so we won't do it now. It seems that doing this without redoing the way conf files are layed out would be messy/impossible.
- Luke made a quick iPython notebook on the web that can run mastml and display the figures.

## Work Hours

Day | Luke hours | Max hours
--- | --- | ---
Monday | holiday | holiday
Tuesday | 8:00 - 3:00 | 8:00 - 3:00
Wednesday | 1:00 - 9:00 | 1:00 - 9:00
