
# mastml-weekly

Week of 2018 June 4-10

## Daily Reports

### Monday

- Get classification images to show up.
- Converted html strings into `xml.dom` DOM elements. (more bug-resistant and inspectable)
- Added new dict for different plots between classification and regression but reuse everything else.
- Investigating ways to automatically provide suggestions to the user based on sklearn documentation.
- Made it so MASTML directly calls sklearn with model parameters from conf, destroys bugs to do with misnaming parameters, and throws readable meaningful errors.
 
### Tuesday

- Sorta got classification working with data splits
- Had good Skype call with Ryan
- Started on demo server where user uploads `.csv` and `.conf` files then spits out `index.html`
- Investigating ways to automatically make a conf template and documentation (better documentation soon hopefully!)

### Wednesday

- Max learned more about matplotlib
- Max came up with general way to decide if model is classifier or regressor
  - https://gist.github.com/robertmaxwilliams/4bcfdfe347488a9fe57b69c8de6d99f7
- Max made a mastml help repl for querying options, models, and tests.
- Luke investigated possible server-side issues with running mastml
  - Flask may be our friend...
  - There are advantages to conf file stuff over Jupyter notebooks

### Thursday

- Testing out ideas for classifier pipelines and deciding best way to do control flow...
- Learning more about sklearn's features...

### Friday

- Learning more about sklearn's features...

## Work Hours

Day | Luke hours | Max hours
--- | --- | ---
Monday | 8 - 4:30 | 8 - 6:15 (10h 15m)
Tuesday | 8 - 4 | 8 - 10 (14h)
Wednesday | 8 - 4:45 | 8 - 7 (11h))
Thursday | 8 - 4 (8h) | 8 - 12 (4h)
Friday | 10-6 (8h) | (0h)
Saturday | | 
Total |  | 
