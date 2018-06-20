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
Monday | 9-6 (9h) | 8-6:15 (10h 15m)
Tuesday | 1-10 (9h) | 1-10 (9h)
Wednesday | 9:30-7 (9h 30m) | 10:30-6:30 (8h)
Thursday | 8-4:30 (8h 30m) | 8-4:30 (8h 30m)
Friday | 10-8:50  (10h 50m) | 9:30 - 5:15 (7h 45m)
Saturday | 8 - 4 (8h) |
Total | 54h 50m |  43h 30m

Extra this week: 14h 50m, 3h 30m

Excess from last week: 5h 30m, 1h	

Accumated total: 20h 20m, 4h 30m
