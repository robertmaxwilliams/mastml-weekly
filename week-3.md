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

### Friday

- Added bool `configdict['General Setup']['is_classification']` that is set based on name of models.
  - SingleFit takes this as an argument `is_classification` that defaults to false, and
  uses it to choose which kinds of plot to do.
- Made a check for all models being of the same type (classifier or regressor).
  - This makes it simple to implement both types of models without recreating SingleFit and its subclasses
- Removed the check that the csv column conforms to class/regress naming scheme.
- TODO Fix "favorites" logic so that it recognizes that there are different plots to be shown

- Pulled ConfigFileValidator into its own file so that it can be more pythonic.

- maybe TODO: shoot, I forgot.

- Quick start for next week: After fixing the plots, get to work on making data splits work, now that we have the infrastructure for telling classifiers and regressors apart

## Work Hours

Day | Luke hours | Max hours
--- | --- | ---
Monday | holiday (free 8h) | holiday (free 8h)
Tuesday | 8:00 - 3:00 (7h) | 8:00 - 3:00 (7h)
Wednesday | 1:00 - 9:00 (8h) | 1:00 - 9:00 (8h)
Thursday | 8:00 - 6:30 (10h 30m) | 8:00 - 6:30 (10h 30m)
Friday | 9:00 - 4:30 (7h 30m) | 9:00 - 4:30 (7h 30m)
Total | 41h | 41h

Extra this week: 1h, 1h

