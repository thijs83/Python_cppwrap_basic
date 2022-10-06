# Basic Python C++ wrapper tutorial

This repository is a first step to understanding how to include c++ code into python. The library used for this Pybind11.


To also be able to debug the c++ when you are running the python script in Visual Studio Code, add the following extension: Python C++ Debugger


To easily start off, follow the code below.

```
git clone https://github.com/thijs83/Python_cppwrap_basic.git
cd Python_cppwrap_basic
mkdir build
cd build
cmake .. -DCMAKE_BUILD_TYPE=Debug
make
```

Now open the Python_cppwrap_basic folder in VS code en open both the python code complex.py and the ComplexCpp.cpp script in the include folder. Set some breakpoints in both scripts and click in the python window to activate that scipt for the debugger. Now press the play button and you will see in the terminal a question that you need to answer with y (yes) or n (no). You need to answer y so the debugger can get super user permission to latch to the c++ process, which is different from the python proces.

NOTE: It could be that the debugger stops, but it will work if you run it again (play button)!

if everything is done correctly, both c++ and python scripts can be debugged.

![Alt text](images/setup.png?raw=true "Complete setup for debugging")


![Alt text](images/play_script.png?raw=true "Setup to run script")
