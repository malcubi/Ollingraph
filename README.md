######################
###   OLLINGRAPH   ###
######################
Version 1.0:   Miguel Alcubierre, February 2017.

Contact:       malcubi@nucleares.unam.mx

This is a python code to plot simple graphs and animations.
It is supossed to have similar functionality to the old
xgraph and ygraph packages, and expects the data files in
the same format (see below).

The plots are quite simple and meant for quick/dirty interactive
visualization, they are not supposed to be used for paper figures
(use gnuplot or something similar for that).

To use it type:

./ollingraph  file1 file2 ... filen

or if you have the local directory "." in your PATH just type:

ollingraph  file1 file2 ... filen

Otherwise you can put it in /usr/local/bin so it can be found
from anywhere.

The data files are assumed to be of the same type.

Before using it make sure that "ollingraph" has execute permission:
chmod +x ollingraph.

The data files are expected to have the following format:

0D files ending in .tl:

	1. One comment line starting with # or " with the file name.

	2. A series of lines with the data points, with the x and y values
	separated by blank spaces.

1D (evolution type) files ending in (.xl, .yl, .zl, .rl, ...):

	1. Each time step begins with a comment line starting with # or "
	that contains the time in the format:  #Time = float
	
	2. A series of lines with the data points, with the x and y values
	separated by black spaces.
	
	3. One or more blank lines to separate the next time step.
