
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

+ work on pypi package

Fixes on ryan's code:

+ https://github.com/uw-cmg/MAST-ML/commit/25b81dd50a5e03634efbf802e6947f0dfa291a7b
  + That repeated block of code should be a function, easy
+ https://github.com/uw-cmg/MAST-ML/commit/45e81c5fb23c8643fa5b0b936a98dc8a061adf22
  + should be using path split, not like that 
  
Other stuff:

+ I accidentally the merge, took some time to correct it
+ Fixed up make_fig_ax so now we don't need gridspec or invisible legends

```
  + That repeated block of code should be a function, easy
```
+ did the above again
+ merging is hard when you aren't working side by side all day
+ Plot helper needs help(er)


### Friday

+ Things aren't that bad, I was just frustrated (and hungry) yesterday
+ Made a neat way to get nice plot ticks in general
+ Refactored the max/min stuff
+ Write co-op report

Monday: 
max: 9:00am - 6:30pm
luke: 9:15am - 6:30pm

Tuesday:
max: 9:30am - 4:30pm
luke: 9:30am - 4:30pm

Wednesday:
max: 9:00am - 4:00pm

Thursday:
max: 10:15am - 7:30pm

Friday:
max: 9:00am - 5:00pm
