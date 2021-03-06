# Software Setup

## Option 1: Google co-labs

<img src='https://www.wispresort.com/uploadedImages/Winter/easy.png' width=20 /> Easy (No software installation; Works for any OS)

You can open any notebook in the Google Co-labs.

1) Visit https://colab.research.google.com

2) Click the GITHUB tab

3) Enter "gw-odw/odw-2019" in the search bar, and click enter to search

4) Double click the notebook of your choice

5) At the top of the notebook, add these 2 lines to install needed python modules

`! wget -q https://raw.githubusercontent.com/gw-odw/odw-2019/master/requirements.txt -O requirements.txt` <br/>
`! pip install -q -r ./requirements.txt`



## Option 2: Use conda

<img src='https://www.wispresort.com/uploadedImages/Winter/intermediate.png' width=20 /> Intermediate (Some software installation; Will not work on Windows PC)

1) Install miniconda: https://conda.io/en/latest/miniconda.html <br/>
You may need to restart your computer after installation

2) Download or clone the git repo: https://github.com/gw-odw/odw-2019/archive/master.zip <br/>
`git clone https://github.com/gw-odw/odw-2019.git`

3) Add the conda-forge channel <br/>
`conda config --add channels conda-forge`

4) Move into the directory with the workshop git repo <br/>
`cd odw-2019`

5) Create the enviornment <br/>
`conda create --name odw2019 python=2.7`

6) Install the software <br/>
`conda install --name odw2019 --file requirements.txt` <br/>
`conda install --name odw2019 -c conda-forge jupyter` <br/>

7) Activate the enviornment <br/>
`conda activate odw2019`

8) Start the jupyter notebook server <br/>
`jupyter notebook`

