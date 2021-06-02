# Computational Neuroscience Crash Course 2021 (beginners)

Given the increasing complexity of neural data and the generalized use
of theoretical models in neuroscience, more and more neuroscientists
rely on computationnal tools for modelling or data analysis. We would
like to offer the possibility to those who feel that their maths /
informatics background is a bit short to update their maths and to get
familiar with basic techniques for data analysis/modelling using the
Python language. The Computational Neuroscience Crash Course (CNCC)
will span over two years, with a first part focusing on the maths and
programming pre-requisites, and a second part next year
on data analysis (and possibly modelling to follow).  

For all courses (maths and programming), we'll provide some
theoretical background, propose small exercises for participant to
work on their own and then solve the exercises together and make sure
everybody has acquired the related concepts and techniques. Courses
will be taught in English.  
 
**Contact**
- Arthur Leblois:  arthur.leblois@u-bordeaux.fr
- Nicolas Rougier: nicolas.rougier@inria.fr
- Eduarda Gervini Zampieri Centeno: egervinizamp@u-bordeaux.fr
- Nikolaos Vardalakis: nikolaos.vardalakis@u-bordeaux.fr

<br/><br/>

## Schedule

This year and due to the pandemic, the whole course will be online.
To avoid very long presentations over Zoom, **you'll have to read the material in advance**. The different topics will be briefly revised during the course. Please have a look at the [schedule](figures/Schedule.png) . 

## The (mini) project

The goal of the project is to sort (automatically) audio files that
correspond to the recording of adult or juvenile songbirds. If you
listen to the audio files, you will hear that the sound is quite
different between an adult (song) and a juvenile (babbling). This
means we can probably process the audio files in order to decide if it
corresponds to an adult or a juvenile and the goal is thus to write a
function `songsort(directory)` that will automatically sort
all the files present in some-path and label them accordingly.  

For the project, you'll need to team with someone else such as to work
together at one computer ([pair
programming](https://en.wikipedia.org/wiki/Pair_programming)). When
one is typing, the other is reading an commenting and for maximum
efficiency, you'll have to switch roles frequently. This can be done
online by sharing the screen of someone.  

For the project, we'll use Jupyter notebook and we'll start with the
[project/introduction.ipynb](project/introduction.ipynb) notebook.

<br/><br/>
## Mathematical lessons

### [Linear Algebra](lessons/math/01-linear-algebra-arthur.pdf)

<img src="figures/indent.png" align="left"/>

This course will introduce vectors and matrices, how to peform operations such
as addition & multiplication on these objects. The correspondence with geometry
and the resolution of a system of linear equations will be explained.

**Prerequisites**: None  
**On-line courses**:

[Wikipedia | Linear Algebra](https://en.wikipedia.org/wiki/Linear_algebra)

<img src="figures/indent.png" align="left"/>

[Mathematics for Computational Neuroscience](https://www.sheffield.ac.uk/polopoly_fs/1.13304!/file/maths.pdf): only Part 1, Chapter 2, 1-3 (ignore the least square approx in 4). 

[Ch4 Linear Algebra (Owen&Corrado, Stanford U)](https://web.stanford.edu/class/nbio228-01/handouts/Ch4_Linear_Algebra.pdf)

[Matrices | Introduction, notation, properties](https://www.dsprelated.com/freebooks/mdft/Matrices.html)

**Exercises**:
 PDF link: https://drive.google.com/file/d/1i2xM37M35iSrTbXoNOX5qQFARRrH2MTn/view?usp=sharing

<br/>

### Signal Processing

<img src="figures/indent.png" align="left"/>

We'll explain first what is the Fourier transform that is ubiquituous in signal
processing, what is spectral analysis and how to compute correlation in order
to reveal similarity between signals.

**Prerequisites**: None  
**On-line courses**:


What is signal processing, and why? https://www.youtube.com/watch?v=YmSvQe2FDKs

<img src="figures/indent.png" align="left"/>

Basic signals and their graphs: https://technobyte.org/signal-systems-types-differences/

Sampling Theorem: https://www.dsprelated.com/freebooks/mdft/Sampling_Theory.html

[Autocorrelation](https://en.wikipedia.org/wiki/Autocorrelation) and [Cross-correlation](https://en.wikipedia.org/wiki/Cross-correlation):
(in both pages, focus on the case of ‘deterministic signals’ and ignore the case of random vectors)

Autocorrelation : https://www.dsprelated.com/freebooks/mdft/Autocorrelation.html

<img src="figures/indent.png" align="left"/>

Crosscorrelation : https://www.dsprelated.com/freebooks/mdft/Cross_Correlation.html

Video explanation and demo : https://www.youtube.com/watch?v=_r_fDlM0Dx0

The case of neurons and spikes : https://www.med.upenn.edu/mulab/analysis.html

Fourier transform :

<img src="figures/indent.png" align="left"/>

https://en.wikipedia.org/wiki/Fourier_transform (up to 5.1 basic properties)

https://www.dsprelated.com/freebooks/mdft/Fourier_Theorems.html

https://www.youtube.com/watch?v=spUNpyF58BY

From DFT to FFT : https://www.dsprelated.com/freebooks/mdft/Why_DFT_usually_called.html

<img src="figures/indent.png" align="left"/>

Intuitive definition : https://sites.northwestern.edu/elannesscohn/2019/07/30/developing-an-intuition-for-fourier-transforms/

More complete definition : https://physiology.med.cornell.edu/people/banfelder/qbio/resources_2016/S.2_fourier.pdf

A video course on the basics of Fourier transform : https://www.ibiology.org/talks/fourier-transform/

To go beyond, the history and many applications of Fourier transforms : http://www.yalescientific.org/2010/12/fourier-transform-natures-way-of-analyzing-figures/

<img src="figures/indent.png" align="left" height="85"  >

.  Common applications of the Fourier Transform (Spectrograms) : https://www.dsprelated.com/freebooks/mdft/Spectrograms.html

<br/>

### [Differential Equations (optional)](lessons/math/differential-equations-optional.pdf)

<img src="figures/indent.png" align="left"/>

We'll cover first-order differential equations (that can for example describe
the evolution of a membrane potential). We'll see how to analyze and solve such
equation. 

**Prerequisites**: None  
**See also**:
[Wikipedia | Differential Equations](https://en.wikipedia.org/wiki/Differential_equation) &
[Mathematics for Computational Neuroscience](https://www.sheffield.ac.uk/polopoly_fs/1.13304!/file/maths.pdf)

<br/>

<br/><br/>

## Programming lessons

### [Installation](lessons/programming/01-installation.md)

<img src="figures/indent.png" align="left"/>

This lesson aims at providing the student with a clean development environment,
including Python installation and essential packages, a decent text editor, and
a shell. We'll also introduce the Python & IPython shells, the Jupyter notebook
and explains how to run a python script from the command line.  

**Prerequisites**: None  
**See also**: [Anaconda installation](https://docs.anaconda.com/anaconda/install/), 
[Datacamp tutorial for Windows](https://www.datacamp.com/community/tutorials/installing-anaconda-windows),
[Datacamp tutorial for MacOS](https://www.datacamp.com/community/tutorials/installing-anaconda-mac-os-x),
[Miniconda tutorial Windows](https://katiekodes.com/setup-python-windows-miniconda/)
[Miniconda tutorial MacOS](https://docs.conda.io/projects/continuumio-conda/en/latest/user-guide/install/macos.html),
[Tutorial on Jupyter Notebooks](https://www.dataquest.io/blog/jupyter-notebook-tutorial/),
[A gallery of interesting Jupyter Notebooks](https://github.com/jupyter/jupyter/wiki/A-gallery-of-interesting-Jupyter-Notebooks),
[Ten simple rules for writing and sharing computational analyses in Jupyter Notebooks](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1007007)

<br/>


### [Introduction](lessons/programming/02-introduction.md)

<img src="figures/indent.png" align="left"/>

We introduce here Python, a powerful and easy to learn programming language. It
has *efficient high-level data structures and a simple but effective approach
to object-oriented programming* (Python website). However, we'll only
cover the strict minimum necessary for getting started with numerical computing.

**Prerequisites**: [Installation](#installation)  
**See also**: [Official Python tutorial](https://docs.python.org/tutorial), [Dive into Python](https://diveintopython3.problemsolving.io/),
[Learn Python](https://www.learnpython.org/)

<br/>

### [Numerical computing](https://docs.scipy.org/doc/numpy/user/quickstart.html)

<img src="figures/indent.png" align="left"/>

This lesson gives an overview of NumPy, the core library for performant
numerical computing, with support for large, multi-dimensional arrays and
matrices, along with a large collection of high-level mathematical functions to
operate on these arrays.

**Prerequisites**: [Introduction](#introduction)  
**See also**: [Scipy Lecture Notes](https://scipy-lectures.org/), 
[Numpy for Matlab users](https://docs.scipy.org/doc/numpy/user/numpy-for-matlab-users.html),
[From Python to Numpy](https://www.labri.fr/perso/nrougier/from-python-to-numpy/),
[Numpy Absolute Beginners](https://numpy.org/doc/stable/user/absolute_beginners.html)

<br/>

### [Data Visualization](https://matplotlib.org/3.1.0/tutorials/introductory/pyplot.html)

<img src="figures/indent.png" align="left"/>

We'll explore the matplotlib library which is a Python 2D plotting library
which produces publication quality figures in a variety of hardcopy formats and
interactive environments across platforms. Matplotlib can be used in Python
scripts, the Python and IPython shells, the Jupyter notebook, web application
servers, and four graphical user interface toolkits.

**Prerequisites**: [Numerical computing](#numerical-computing)  
**See also**: [Matplotlib tutorial](https://github.com/rougier/matplotlib-tutorial), 
[Ten Simple Rules for Better Figures](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1003833)

<br/>

### [Scientific computing](http://scipy-lectures.org/intro/scipy.html)

<img src="figures/indent.png" align="left"/>

This lesson, from the scipy mlecture notes, will cover scipy which is a
scientific-computing libraries, such as the GSL (GNU Scientific Library for C
and C++), or Matlab’s toolboxes. Scipy is the core package for scientific
routines in Python; it is meant to operate efficiently on numpy arrays, so that
numpy and scipy work hand in hand.

**Prerequisites**: [Numerical computing](#numerical-computing)  
**See also**: [Elegant Scipy](https://github.com/elegant-scipy/elegant-scipy), 
[Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/),
[Python SciPy Tutorial - A Guide for Beginners](https://phoenixnap.com/kb/scipy-tutorial#ftoc-heading-1), 
[SciPy Tutorial for Beginners](https://www.mygreatlearning.com/blog/scipy-tutorial/)

<br/><br/>

## Open Science & FAIR data
### [The Open Science movement](https://en.wikipedia.org/wiki/Open_science) & [FAIR data](https://en.wikipedia.org/wiki/FAIR_data)

<img src="figures/indent.png" align="left"/>

**See also**: [FOSTER](https://www.fosteropenscience.eu/resources), 
[Ouvrir la Science](https://www.ouvrirlascience.fr/open-science/),
[UNESCO & Open science](https://en.unesco.org/science-sustainable-future/open-science),
[FAIR by FOSTER](https://www.fosteropenscience.eu/learning/open-and-fair-research-data/#/id/5e3741af3ccdf1010dbc6f26),
[The FAIR Guiding Principles for scientific data management and stewardship](https://www.nature.com/articles/sdata201618)


## 

[Computational Neuroscience Crash Course (CNCC 2021)](https://github.com/bordeaux-neurocampus/CNCC-2021-beginner)  
Copyright © 2021 Arthur Leblois & [Nicolas P. Rougier](http://www.labri.fr/perso/nrougier) – [CC-BY 4.0 International](https://creativecommons.org/licenses/by/4.0/legalcode) license.

[Anaconda]:   https://www.anaconda.com/
[Emacs]:      http://www.emacs.org/
[vim]:        https://www.vim.org/
[Atom]:       https://atom.io/
[Notepad++]:  https://notepad-plus-plus.org/
[IPython]:    http://www.ipython.org/
[Jupyter]:    http://www.jupyter.org/
[NumPy]:      http://www.numpy.org/
[Scipy]:      http://www.scipy.org/
[Matplotlib]: http://www.matplotlib.org/
[Cython]:     https://cython.org/
[Numba]:      https://numba.pydata.org/
