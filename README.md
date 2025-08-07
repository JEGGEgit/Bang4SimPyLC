Bang4SimPyLC with sequence and bang-bang control for SimPyLC
--------------------------------------------------------

Here you can find the entire original **SimPyLC** project:
https://github.com/QQuick/SimPyLC/

**Bang4SimPyLC** is just an an extension of *SimPyLC* for learning purposes.

Installation
------------

Installation for Windows, Linux is described in:
**"SimPyLC_HowTo"**
https://github.com/QQuick/SimPyLC/blob/master/simpylc/simpylc_howto.pdf

Usage
-----

1. Go to directory SimPyLC/simulations/one_armed_robot
2. **Replace original file with "world.py" and "control.py" and add this "sequence.py"**
3. Click on world.py (or run world.py from the command line) - requires Python 3.10 installed
4. Force the "go" bit in the "movement control window"
5. The one arm robot torso will then follow 3 predefined angles
6. "Reset" bit in the "sequence control window" repeats the whole sequence

Demo
----

Robot torso movement with simple *bang-bang control* without overshoot. 
But this version doesn't calculate the braking distance, as suggested in the **"SimPyLC_HowTo"** guide.


This **bang-bang controller** uses maximal acceleration to the halfway position, then does maximal deceleration until the goal is reached.
And this is what it looks like:

![alt text](https://github.com/JEGGEgit/Bang4SimPyLC/blob/main/demo/bang4simpylc640x360.gif?raw=true)
https://github.com/JEGGEgit/Bang4SimPyLC/blob/main/demo/bang4simpylc1366x768.gif


Notes
-----

The GUI operation as described (Mouse Wheel and PageUp/Dwn) didn't work for me. I'm running the simulation on Windows 10 64-bit (1511) with Python 3.10 32-bit.

And yes, in real life, I'm an old-school PLC programmer. I do simulations directly on the manufacturer's development environment, including Omron's Sysmac Studio.

But I also like Python and this concept of **SimPyLC** using Python with OpenGL visualisation.

*Enjoy What You Do*

EOF













