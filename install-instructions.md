### Luke Miles and Max Williams instructions

#### for installing MAST-ML, tested on Ubuntu and Mac

1. install conda
2. make an empty environment
  `conda create --name testml`
3. Enter the environment
  `source activate testml`
4. `conda install python nbformat`
5. (make sure it's version 3)
6. git checkout the good branch
7. If you're on MacOS, see section **Hack for MacOS** below.
8. `python setup.py build`
9. `python setup.py install`
10. `cd examples`
11. `python ../MASTML.py example_input.conf`
12. open `index.html` and see your pretty picture
13. So easy!!

#### Hack for MacOS
Copied from https://stackoverflow.com/questions/21784641/installation-issue-with-matplotlib-python

I assume you have installed the pip matplotlib, there is a directory in you root called `~/.matplotlib`.
Create a file `~/.matplotlib/matplotlibrc` there and add the following code: `backend: TkAgg`
