.. toctree::
   :maxdepth: 1


Python from a standing start
----------------------------

Here are some notes on my python setup, plus resources for learning python.  The intended audience
is undergrad/grad/post-docs interested in modeling and data analysis in python.



Books and tutorials
+++++++++++++++++++

                                                     
-  `IPython (2.0) notebook basics <http://nbviewer.ipython.org/github/ipython/ipython-in-depth/blob/master/examples/Notebook/Notebook%20Basics.ipynb>`_. To get the notebook: click on the link and then 
   right click on the download arrow in the upper right corner.  IPython comes with the anaconda install described below.  
   To open the notebook with ipython in OSX or Linux, launch a terminal (or in Windows, cmd.exe), cd to the directory that
   contains the *Notebook Basics.ipynb* file and type::

      ipython notebook
   
   Your default browser will open the dashboard page, click on the link that says *Notebook Basics*.

- `Python Crash Course <http://nbviewer.ipython.org/github/barbagroup/CFDPython/blob/master/lessons/00_Quick_Python_Intro.ipynb>`_, part of `CFD Python <https://github.com/barbagroup/CFDPython/blob/master/README.md>`_
   
- `Lecture notes as IPython notebooks <http://nbviewer.ipython.org/github/jrjohansson/scientific-python-lectures/blob/master/Lecture-0-Scientific-Computing-with-Python.ipynb>`_ by `J. R. Johansson <http://dml.riken.jp/~rob/>`_   (Download from https://github.com/jrjohansson/scientific-python-lectures by either cloning the repository or clicking the *download zip* button on the right hand side).

- `Python Scientific Lecture Notes <http://scipy-lectures.github.com/>`_

- `Johnny Lin's Python for Atmospheric/Ocean Sciences <http://www.johnny-lin.com/pyintro/>`_

- `Python for Data Scientists <http://blog.yhathq.com/posts/data-science-in-python-tutorial.html>`_


- My favorite O'Reilly book is:

  - `Python for Data Analysis <http://shop.oreilly.com/product/0636920023784.do>`_

- Some other resources:

  - If you know Matlab, there is `Numpy for Maltab users <http://wiki.scipy.org/NumPy_for_Matlab_Users>`_
  
  - `Numpy beginners guide <http://www.packtpub.com/numpy-mathematical-2e-beginners-guide/book>`_

  - `Learning Ipython <http://www.packtpub.com/learning-ipython-for-interactive-computing-and-data-visualization/book>`_

  - `The official Python tutorial <http://docs.python.org/tut/tut.html>`_

  - `Python for high performance computing <http://www.packtpub.com/python-high-performance-programming/book>`_

  - `Numpy cookbook <http://www.packtpub.com/numpy-for-python-cookbook/book>`_


Installation
++++++++++++

1) I use the `Anaconda Python Distribution <https://store.continuum.io/cshop/anaconda/>`_, which is a curated
   set of `python packages <http://docs.continuum.io/anaconda/pkgs.html>`_ that is installed with the 
   `conda package manager <http://docs.continuum.io/conda/>`_   I install in my user home directory (/Users/phil
   on my osx laptop) and add /Users/phil/anaconda/bin  to my $PATH (OSX) or the path environment variable (Windows)

2) A good editor for working with python is `Sublimetext <http://www.sublimetext.com>`_ (which is written in Python)

2) I write lecture notes using IPython notebook, but I do
   my interactive work using `Ipython <http://nbviewer.ipython.org/urls/raw2.github.com/yhat/DataGotham2013/master/notebooks/1%20-%20Tools%20Overview.ipynb?create=1#IPython>`_, either from inside emacs using `python-mode <http://www.emacswiki.org/emacs/ProgrammingWithPythonModeDotEl>`_ or launching
   a qtconsole with an alias to the following command (for Macs)::

       ipython qtconsole --matplotlib=osx

       or on Windows/Linux

       ipython qtconsole --matplotlib=qt4

   This launches an interactive window and starts two threads, one for commands and one for plotting, so that you can
   update graphs without having the terminal block





