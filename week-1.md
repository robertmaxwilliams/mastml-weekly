# mastml-weekly
week of 2018 May 14-21

## Daily Reports

### Monday
- We installed working MASTML on Luke's laptop:
  * Viewed some ipython notebooks, but got errors
  * Installed more conda packages trying to fix those errors
  * viewed documentation and performed their build process
  * Got our images and html file showing an optimization process

- Tried to build from scratch in a docker image, steps are in `install-instuctions.md` (older versoin), but they are imperfect and overcomplex

- Used the dell ubunutu laptop and started building conda on there to get a better grasp in how to build mast-ml

### Tuesday
- Built MAST-ML on ubununtu laptop and it was actually good this time, one 10 steps instead of thirty. The new steps are in `install-instructions.md` (since deleted and made part of mastml docs) and should be usable from any clean linux box.
- Meeting with Ryan
  * Gave use a rundown of the current structure of the project
  * Wants us to not worry about integration, just make stuff
  * The project currectly has lots of regression options, but no classification, so we can do that
  * Use scikit-learn and maybe keras
  * Kernel ridge regression is a good place to start for using the package
  * Boston Housing dataset is a good one
- Reading [Zuf's work log](https://docs.google.com/document/d/1ruQg7kuH_oTWwapB54wWx1ruEYSxhBZgCOugDtwRh4k/edit?usp=sharing)
  * Gained some understanding of the progress of a person who works on this project
- Built on mac and updated build instructions
- Read some of the source and saw how sklearn models are used interchangably
- It seems that there are many classification models already in place?

### Wednesday

- studied Wasserman's All of Statistics
- Printed out a tree of ryan's branch, with tests and builds cut out
- Read through Ryan's summary of the important files and of classification methods we can implement
- Try to modify example `.conf` file, but we got errors
- Try to run unit tests (Ryan says not to worry about it, he's still developing that stuff)
- Make our branch, luke-max
- Update the readme

### Thursday

- Studied **Wasserman's** _All of Statistics_
- Ran classification examples for  tensorflow and keras in a jupyter notebook

## Current goals:

- [x] run mastml hello world
- [ ] (cancelled) run kernel ridge regression on Boston Housing
- [x] replace build docs with our updated instructions
- [ ] build keras model and fold it into mast-ml

## Work Hours

Day | Luke hours | Max hours
--- | --- | ---
Monday | 8:00 - 4:15 | 8:00 - 4:15 
Tuesday | 8:00 - 4:00 | 8:15 - 4:00
Wednesday | 8:00 - 4:00 | 8:00 - 4:00
Thursday | 8:00 - 4:00 | 
Friday | | 
