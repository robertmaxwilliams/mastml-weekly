# mastml-weekly

Week of 2018 May 21-25

## Daily Reports

### Monday

- Finished up ch 1 exercises of Wasserman and started reading ch 2
- Luke continues mercilessly refactoring root level `.py` files
- Max starts modifying unit tests so they apply to latest code

### Tuesday 

- Had a meeting with Ryan
- Luke created diagrams for classification tasks outside of ML
- Max deletes a lot of stuff to begin unit testing framework

### Wednesday

- First unit test passes
- Luke destroys miles of code, improving readability and flexibility

### Thursday

- Max seems to have discovered a flaw/limitation in MASTMLInitializer.py:
  - `ConfigFileParser` is initialized with a filename
  - then you call `.get_config_dict` with a path
  - This is awkward, but can be worked with if you know what's going on. The docstrings lie
  and say that you initialize with an object, even though it needs a filename. This should also be fixed.
  - However, the methods that subclass `ConfigFileParser` always call `.get_config_dict`
  with the current working directory, making it awkward to call config files in other folders
- Luke
  - started switching files to 100 char col width,
  - removed all the unnecessary return statements in all the python files,
  - added some todos/guidelines to the readme, and
  - significantly refactored FeatureSelection.py to be shorter, faster, more readable, and follow `pylint`'s style guidelines.
- Converted `sys.exit` to python exceptions.
- Added error created conf files for tests.
- Started removing `errors_present` thing, TODO finished that tomorrow.

### Friday

- Solved some ch 2 exercises in Wasserman
- Began trying to integrate Tuesday's classifier model into main MASTML flow
  - (spent most of day on this)
  - basically we are trying to make another SingleFit.py, which is for classifiers instead of regression
  - This is our most important task right now
  - Called a `spike` in extreme programming speak
- Finished removing `errors_present` and merged `unit_tests_fixes` branch with `max-luke` branch
- Spent most of workday at picnic table outside under shade tree

## Work Hours

Day | Luke hours | Max hours
--- | --- | ---
Monday | 8:00 - 4:00 (8h) | 8:00 - 4:00 (8h)
Tuesday | 8:00 - 4:15 (8h 15m) | 8:00 - 4:30 (8h 30m)
Wednesday | 8:00 - 7:00  (11h) | 8:00 - 7:00 (11h)
Thursday | 8:00 - 4:00 (8h) | 8:00 - 4:00 (8h)
Friday | 8:00 - 4:00 (8h) | 8:00 - 4:00 (8h)
Total | 43h 15m | 43h 30m 

Deficit from last week: 3h 15m, 3h 30m

Extra this week: 3h 15m, 3h 30m

_Note: I didn't fudge these, I swear they just happened to come out like this._
