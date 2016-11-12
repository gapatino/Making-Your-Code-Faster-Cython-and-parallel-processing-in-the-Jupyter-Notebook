# Making-Your-Code-Faster-Cython-and-parallel-processing-in-the-Jupyter-Notebook
Repository for the PyData DC 2016 tutorial

Python has multiple options to speed up code execution, including the use of specialized libraries, different compilers or 
paralle processing. However, within the Jupyter Notebook only a subset of methods from those options are available. The current project 
shows the implementation of some of them to solve the following problem:

The function $y=x^{2}$ can be approximated using its derivative $y'=2x$ through the Euler method:  
$y_{(n+1)} = y_n + (step*y')$  
The precision of the approximation depends on the step being very small.  
We want to find the step size that gives a difference < 1e-5 when comparing the values obtained  
using the $y=x^{2}$ formula and the Euler method after evaluating a million points  

The following methods will be covered:

- Cython
- Numpy
- Scipy.integrate
- Numba
- Parallel processing using ipyparallel/ipcluster

The video of the presentation is available at:

https://www.youtube.com/watch?v=MiHddLYZ6cQ

Note: Many other parallel processing methods are also available. I would recommend checking the other talks from PyData DC 2016 on Dask
concurrent.futures
