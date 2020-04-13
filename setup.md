# Software Setup

Choose an option below.

## Option 1: Google co-labs

<img src='https://www.wispresort.com/uploadedImages/Winter/easy.png' width=20 /> Easy (No software installation; Works for any OS)

[Video Guide](https://labcit.ligo.caltech.edu/~jkanner/gwosc/colab-help-2020.mov)

1) Visit https://colab.research.google.com

2) Click the GITHUB tab

3) Enter "gw-odw/odw-2020" in the search bar, and click enter to search

4) Double click the notebook of your choice

5) At the top of the notebook, uncomment any `pip install` commands by removing the `#`

`#! pip install -q 'gwpy==1.0.1`  <-- Remove the `#` and run

6) Click `run all` from the `runtime` menu at the top

## Option 2: Run in mybinder

<img src='https://www.wispresort.com/uploadedImages/Winter/easy.png' width=20 /> Easy (No software installation; Works for any OS)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gw-odw/odw-2020/master)


## Option 3: You have a Linux or Apple/Mac computer -- Use conda

<img src='https://www.wispresort.com/uploadedImages/Winter/intermediate.png' width=20 /> Intermediate (Some software installation; Will not work on Windows PC)

Note: this workshop will use Python version 3.7

1) Install miniconda: https://conda.io/en/latest/miniconda.html <br/>
Choose the version for Python 3.7. 
See the installation instructions here: https://conda.io/projects/conda/en/latest/user-guide/install/
You may need to restart your computer after installation.

2) Download the IGWN YML file from [IGWN Conda Distribution](https://computing.docs.ligo.org/conda/environments/igwn-py37/)
 * [YML file for linux](https://computing.docs.ligo.org/conda/environments/linux/igwn-py37.yaml)
 * [YML file for osx  ](https://computing.docs.ligo.org/conda/environments/osx/igwn-py37.yaml)

3) Add the conda-forge channel <br/>
`conda config --add channels conda-forge`

4) Create the environment <br/>
`conda env create --file igwn-py37.yaml`

5) Clone the workshop git repo <br/>
`git clone https://github.com/gw-odw/odw-2020.git`

6) Move into the directory with the workshop git repo <br/>
`cd odw-2020`

7) Activate the enviornment <br/>
`conda activate igwn-py37`

8) Start the jupyter notebook server <br/>
`jupyter notebook`

## Option 4: Linux install on Windows 10 with dedicated app (Windows 10 only)

<img src='https://www.wispresort.com/uploadedImages/Winter/hard.png' width=20 /> Advanced (For Windows 10)

Install a Linux distribution on your Windows system. 
See instructions here: https://docs.microsoft.com/en-us/windows/wsl/install-win10

We suggest you install Debian GNU/Linux, which is the closest distribution to what is 
used currently by LIGO/Virgo. Once you have Linux installed, follow the instructions 
in Option 2.

