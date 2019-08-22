{{ cookiecutter.project_name }}
==============

{{ cookiecutter.project_short_description }}


Installation
------------

**Requires a C++ 14 compiler and cmake**

 - `pip install ./{{ cookiecutter.project_name }}`

Build a binary wheel
--------------------
 
A binary wheel ease the redistribution of your project and can be installed with *pip* on a client machine without a compiler.

**Create wheel**

 - `cd {{ cookiecutter.project_name }}`
 - `python setup.py bdist_wheel`
 - `pip install ./{{ cookiecutter.project_name }}`
 
 The wheel is created in the directory `{{ cookiecutter.project_name }}/dist`, it will be named `{{ cookiecutter.python_package_name }}-XXXXX.whl` where `XXXXXX` are name tags identifying the current platform and Python version. 
 
**Install wheel**
 
Whells can be installed with *pip*:
 
 - `pip install wheel_name.whl`
 
 Note that a binary wheel is specific to a platform and to a python version (a wheel built on Windows with Python 3.5 can only be installed on Windows with Python 3.5).

Tests
-----

Tests are run automatically at the end of a build: the build will fail if tests are not successful. 
