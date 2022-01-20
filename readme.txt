Lost Task

running the task
================
1) start ACT-R 7.21
2) navigate to folder containing lost.py and actr.py
3) open powershell or other commandline tool and type following commands:
4) python -i lost.py
5) "ACT-R connection has been started." should be written on the screen
5) enter startExperiment('human')


change level
============
1) open lost.py file
2) at the top of the file you can find level definitions:
level1 = {'parameters': [], 'layout': '''
xxxSxxxxxx
xxxxxxxxxx
xxOxxxxxxx
xxxxxxxxxx
xxxxTxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
'''}
3) for now ignore parameters
4) change layout to build a map (x is empty space, S is the spaceship, O an obstacle and T the target)
5) if you add a new level, change the levelToPlay variable to your new level, e.g.

myNewLevel = {'parameters': [], 'layout': '''
xxxxxxTxxx
xxxxxxxxxx
xxOxxxxxxx
xxxxxxxxxx
xxxxSxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
'''}

levelToPlay = myNewLevel

6) run the experiment