# instapy

This package applies grayscale and sepia image filters to images. 

There are three different implementations of the filters, a pure python implementation, a numpy implementation and a numba implementation. The numpy sepia filter is tunable.

It is possible to generate a timing report. This will print out the report to a file timing-report.txt.

Created as an assignment solution in the subject IN3110 at UiO.

## Installation
### Pre-requisites
Python version 3.7 or higher.

__Required dependencies and suggested versions:__\
Numpy version 1.21.*\
Pillow version 9.0.1\
Numba version 0.55.1 \
Line-profiler version 3.5.1

__How to install the dependencies:__ 
The dependencies should be automatically installed when you install the package, but to do it manually run: 

`pip install numpy pillow numba line-profiler`

### How to install and use instapy package
From this program's root directory (not "instapy") run:
```
pip install .
```
All the packages and required dependencies should be installed with this command.

## Run
### Run package
The package has been made to be used through the terminal. Type in from root directory:
```
instapy [-h] [-o OUT] [-g] [-se] [-sc SCALE] -i {python,numba,numpy,cython} [-r] file
```
Where the arguments enclosed within the brackets are optional. Type `instapy --help` for full information on how to use and run the package.

### Run tests
Type `pytest` or `pytest -v` for verbose.

### Run timing report
Type `[your python compile command] -m instapy.timing`, e. g. `python3 -m instapy.timing` from this package's root directory.
