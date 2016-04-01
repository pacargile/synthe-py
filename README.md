# synthe-py
Python hooks and glue code for Bob Kurucz synthe.for program

Files:

synthe.f90 -> Fortran code that is directly taken from Bob's synthe.for code
synthe.py  -> Python code using ctypes to access the hooks placed in the fortan

Steps to install:

1) Compile the fortran code into a shared object library with something like:

gfortran -shared -fPIC -o libsynthe.so synthe.f90

2) Edit the path to this shared library within the synthe.py python code
