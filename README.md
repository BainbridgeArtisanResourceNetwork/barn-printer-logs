# barn-printer-logs

There are two versions of notebooks in here:
  - original one in the notebooks/ directory loading metrics from data/ directory.
  - latest one, using a notebook in the ./ directory loading metrics from a Google Sheet.

## New version 

Using Google Colaboratory environment, the notebook `Evaluate_3D_Printer_Logs.ipynb` loads captured printer statistics, and generates graphs with optional downloads. It requires a Google account and permission to use it. You may not have access to the printer logs - they're in a Google Sheet I maintain in a BARN-specific account. But you can see the current version of the data captured in this notebook.

## Older Version

This is a capture and quick analysis of the statistics we capture from our collection of 3D printers. There's not a lot of data available - mainly print-time and filament-used. These are cumulative values, and have (so far) recorded them intermittently.

This is also intended to be educational and demonstrative to other org members, to learn how to:
* use a Python virtual environment
* use a Jupyter notebook in the virtual environment
* use Pandas/numpy/scipy for data import, preparation, and (basic) analysis
* use Matplotlib/Seaborn for basic visualization

## Local Setup

There is a requirements.txt here that captures the packages I loaded into a virtual environment, but many of them came in as transitive d ependencies. The list of packages I started with is a lot smaller and for the most part should not be version-specific. With that in mind, here's the basic instructions to setup:

* some version of Python 3 and pip should be installed.
* you should be in the directory with the repo, or where you want to install your virtual environment
* mkdir pyenv
* python3 -m venv pyenv
* source pyenv/bin/activate
* pip install --upgrade pip
* pip install wheel
* pip install pandas
* pip install scipy
* pip install matplotlib
* pip install s3fs
* pip install seaborn
* pip install scikit-learn
* pip install jupyter

--30--

Now when you're in this directory, should execute the command ```jupyter notebook``` and follow the instructions
to open a browser to the appropriate location.

From there, just open the document(s) in the ```notebooks/``` directory and run all cells. 

