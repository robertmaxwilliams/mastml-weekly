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
## Work Hours

Day | Luke hours | Max hours
--- | --- | ---
Monday | 8:00 - 4:00 | 8:00 - 4:00
Tuesday | 8:00 - 4:15 | 8:00 - 4:30
Wednesday | 8:00 - 7:00 | 8:00 - 7:00
Thursday | 8:00 - 4:00 | 8:00 - 4:00
