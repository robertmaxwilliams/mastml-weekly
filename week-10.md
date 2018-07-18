
# mastml-weekly

Week of 2018 

## Daily Reports

### Monday

TODO:
  + prepare for presentation to finkel
  + add a bunch of feautures really quick
  + crash both of our computers
  + accidentally delete all the slides
  + break the dell laptop
  
TODONE
  + gave that presentation, none of the above happened
  + updated mastml hours spreadsheet
  + made metrics show up in output without minus or negative
  + added that metric that Ryan asked for
  + Did government required training :goberserk:
  
Words from Dr. Finkel:
  + Don't let the user know that we use negative score funcs
  + Looks like the project is like pretty ~~good~~ operational
  + Users will probably not use command line interface

### Tuesday

+ Big ol' code review with Ryan
+ Luke leaves to Washington State to visit Aunt and Grandma
+ Luke works on code documentation
+ Luke fixes scoring func bug
+ Max tries to implement testing_only

### Wednesday

We want to have a testing only option, where a specific group is used only for validation. You can do that now, sortof, using groups, but that just lets you use that group as test, not really doing complete held out cross validation. What we really need is data taken out at the very beginnning, that can be processed the exact same way as everything else. All of the processing steps (feature generation, normalziation, removing constant columns, etc) need to be a single opertation that can be applied to some data, then reversed on model predictions. This is what sklearn pipelines does but we weren't able to maintain the pipelines paradigm.

The other option is to keep a list of "blacklisted" indices, and cut them out at split time. This will mess with the splitters, sometimes giving empty splits and other issues like that, but won't cause any design headache.

Oh, we can do it inside of splitters! Perfect!

+ added `validation_column` to `GeneralSetup`
+ made target histogram use y feature name as xlabel
+ did co-op evaluation
+ wrote my co-op report

### Thursday


### Friday

Monday: 
max: 9:00am - 6:30pm
luke: 9:15am - 6:30pm

Tuesday:
max: 9:30am - 4:30pm
luke: 9:30am - 4:30pm

Wednesday:
max: 9:00am - 4:00pm
