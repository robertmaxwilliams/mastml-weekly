# mastml-weekly

Week of 2018 June 11-16

## Daily Reports

### Monday
 - Working on making feature selection work for classification models
 
### Tuesday
 - integrating changes to feature selection, generation, and normalization so they work like normal

### Wednesday
 - meeting with Ryan:
 - For next week:
     - Take confusion matrix data from each fold and output best, worst and average and have display to html output of favorites
     - Add classification statistics for CV routines and in single fit. Have statistics output to spreadsheet.
     - After KFoldCV done, start extending to other CV test modules
  - For future (starting say 7/1):
     - Implementation of cluster CV approach. Have work in conjunction with existing grouped CV test. Have pre-clustering of data done using, e.g. K-means or support vector machine, then do CV by holding out each cluster, training on remaining data and predicting on the left-out cluster
     - Implementation of leave-out-element CV approach: scan material compositions in input data file, build composition object with pymatgen.core.Composition.as_dict(), get list of elements present. Then leave out data for each element, and train on remaining data and predict data of that element.
  
Max:
 - feature selection, generation, and normalization all work with regression and classification
Luke:
 - found that sklearn pipelines might be a worthwhile investment

### Thusday

- wrote master template
- Talked with Ryan about master conf template, aka project specifications
- Started trying to use sklearn pipelines to compartmentalize our objects better and get stats and grid search more safely.

### Friday

- Got cluster splitting implemented
- Classification cross validation is closer to being done
- Added more test cases and csv files
- Started integrating sklearn pipelines (improve structure and grid search)

## Work Hours

Day | Luke hours | Max hours
--- | --- | ---
Monday | 9-6 | 8-6:15
Tuesday | 1-10 | 1-10
Wednesday | 9:30-7 | 10:30-6:30
Thursday | 8-4:30 | 8-4:30
Friday | 10-8:50 | 9:30 - 5:15
Saturday | |
Total | |
