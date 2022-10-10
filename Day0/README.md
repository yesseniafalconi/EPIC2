# Introduction and preliminary activities

Please read carefully all the information given below.

This School focuses on python, but there are a few lectures and tutorials on julia and R. We will use python 3.x (as python2 is not supported anymore). Similarly, we will mainly use jupyter notebooks (.ipynb) for the courses taught at this School.

- Jupyter notebooks are very useful tools for learning programming because they provide a visual interface.
- You can see the results of your code live, instead of waiting till your script (.py) finishes running in a terminal.

To be able to use python and jupyter notebooks in your laptop, there are several options:

## OPTION 1: Google Colab (see https://colab.research.google.com/):

<p style="color:blue">Note: We highly recommend this option for participants with little programming experience.</p>

One option is to use Google Colab, for which you would need a Google account, which can be a personal gmail account or an institutional email supported by Google (e.g. all Yachay Tech accounts are Google accounts). The advantage of using Google Colab is that all libraries are installed in a Linux server remotely, so we don't need to worry about compatibility issues, different operating systems, etc. The disadvantage is that Colab provides limited memory resources and very limited disc space since everything is stored in a cloud, so you can only use it to process small datasets.

## How do I test Google Colab?
1. Download this notebook: https://github.com/ciencialatitud0/EPIC_2/blob/main/Introduction/My_first_notebook.ipynb
2. Open Goole Colab
3. Upload the notebook, and run it. If you see a plot of sin(x) vs. x, your local Google Colab works.

## Anaconda/Miniconda (Recommended, see https://anaconda.org/):
Another option is to have python (and all the libraries you need to analyse your datasets) installed in your laptop. This can also be done in many ways, but anaconda is now very popular because it provides good portability and an interface that allows the user to include extra kernels for other programming languages. Anaconda has the advantage that you have all the code you need locally in your laptop. In the long term, using Anaconda will be much more advantageous.

# Installation instructions

## How to install Anaconda?
Download Anaconda from this website: https://www.anaconda.com/products/individual. Choose the package version that best suits the operating system (OS) of your laptop.

### On Linux and MacOSX:
For testing and customising your installation on Linux/MaxOSX laptops/PCs, follow these instructions:

#### Option A: Installation from a terminal (recommended)

1. Open a terminal window.<br>

2. Type the command below:<br>
~~~~html
  $ conda --version
  conda 4.10.3
~~~~

3. That means you have Anaconda 4.10.3 installed.<br>

4. Now, let us check which environment you have:<br>
~~~~html
  $ conda env list
  conda environments:
  base                  *  /Users/webb/opt/anaconda3
~~~~

5. Let us know create a new environment with:<br>
~~~~html
  $ conda create -n py37 python=3.7
  $ conda env list
  conda environments:
  base                  *  /Users/webb/opt/anaconda3
  py37                     /Users/webb/opt/anaconda3/envs/py37
~~~~

6. Now, we activate the environment:<br>
~~~~html
  $ conda activate py37
  $ conda env list
  conda environments:
  base                     /Users/webb/opt/anaconda3
  py37                  *  /Users/webb/opt/anaconda3/envs/py37
~~~~

7. Let us check with libraries are installed by default:<br>
~~~~html
  $ conda list
~~~~

8. Let's install a few extra libraries:<br>
~~~~html
  $ conda install jupyter numpy cython mpi4py git
~~~~

9. Type 'yes' to accept changes, and check that the new libraries are present.<br>
~~~~html
  $ conda list
~~~~

10. Let's now open a jupyter notebook, and we are ready to work.<br>
~~~~html
  $ jupyter notebook
~~~~

10. Once the notebook is open, you can start coding your first notebook:<br>

https://github.com/ciencialatitud0/EPIC_2/blob/main/Introduction/My_first_notebook.ipynb

#### Option B: From within a jupyter notebok (this assumes notebooks are already installed):<br>

https://github.com/ciencialatitud0/EPIC_2/blob/main/Introduction/Installation_from_notebook.ipynb


### On Windows:
If you are using Windows, we highly recommend either:

1. setting up a dual partition in your hard drive with both Windows and Linux, or
2. setting up a Virtual Machine (VM) with a linux distribution. For this:

- Download VirtualBox from: https://www.virtualbox.org/
- Follow the instructions here: https://itsfoss.com/install-linux-in-virtualbox/

After the installation of the VM is successful, follow the instructions provided above for Linux/MacOSX systems to set up your Anaconda installation.

In the long term, you may want to fully switch to Unix-based operating systems. Ubuntu is a popular and user-friendly option.


## How do I test and use Anaconda?
Assumming all the steps above went well, and you were able to create your first jupyter notebook, open a new notebook and follow these two tutorials on jupyter notebooks and basic python:

- https://datacarpentry.org/python-ecology-lesson/jupyter_notebooks/
- https://swcarpentry.github.io/python-novice-gapminder/

Please note that we will **NOT** have time to cover the basics in EPIC 2, so make sure you are familiar with the material above.
