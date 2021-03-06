## In Tests We Trust — TDD with Python And Python Modules and Packages

**Python Modules and Packages**
***Python Modules:***

There are actually three different ways to define a module in Python:

1. A module can be written in Python itself. 2- module can be written in C and loaded dynamically at run-time, like the re (regular expression) module. 3- A built-in module is intrinsically contained in the interpreter, like the itertools module.

***in this sectcion we well focus on the mudule written by python All you need to do is create a file that contains legitimate Python code and then give the file a name with a .py extension. That’s it! No special syntax or voodoo is necessary.***

**The Module Search Path**

***When the interpreter executes like import mode statement . searches for mod.py in a list of directories assembled from the following sources:***

- The directory from which the input script was run or the current directory if the interpreter is being run interactively

- The list of directories contained in the PYTHONPATH environment variable, if it is set. (The format for PYTHONPATH is

OS-dependent but should mimic the PATH environment variable.)

- An installation-dependent list of directories configured at the time Python is installed

**The import Statement**
we can import module like this IMmport < module name>

Each module has its own private symbol table
and we can use

from <module_name> import <name(s)>

Executing a Module as a Script
Any .py file that contains a module is essentially also a Python script, and there isn’t any reason it can’t be executed like one.

**Python Packages**

***Packages allow for a hierarchical structuring of the module namespace using dot notation. In the same way that modules help avoid collisions between global variable names, packages help avoid collisions between module names.***


## Recursion

**Recursion**

**The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function.**

***What is base condition in recursion? In the recursive program, the solution to the base case is provided and the solution of the bigger problem is expressed in terms of smaller problems.***