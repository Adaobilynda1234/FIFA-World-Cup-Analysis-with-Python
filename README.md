# FIFA-World-Cup-Analysis-with-Python
--------------------------------------------
# Introduction
The World Cups dataset show all information about all the World Cups in the history from 1930 to 2014, while the World Cup Matches dataset shows all the results from the matches contested as part of the cups.
------------------------------------------------
# Importation of Libraries
-----------------------------
import pandas as pd

import numpy as np

import matplotlib.pyplot as plt

import seaborn as sns

import warnings

warnings.filterwarnings('ignore')

%matplotlib inline

# installation of plotly and cufflinks
--------------------------------
!pip install plotly

!pip install cufflinks

# importation of the libraries
----------------------------------------------
import plotly as py

import plotly.io as pio

pio.renderers.default = 'notebook'

import cufflinks as cf

from plotly.offline import iplot

py.offline.init_notebook_mode(connected = True)

cf.go_offline()

# importation of Datasets
Dataset was gotten from https://www.kaggle.com/datasets/abecklas/fifa-world-cup?resource=download
----------------------------------
world_cups = pd.read_csv('WorldCups.csv')

players = pd.read_csv('WorldCupPlayers.csv')

matches = pd.read_csv('WorldCupMatches.csv')

# The data was cleaned,aggreated and Analyzed the complete documentation is shown on the Jupyter notebook
-----------------------------------------------
# Conclusion
The following was deducted from the analysis of the data

The 5 top winning countries from(1930-2014) includes Brazil,Italy,Germany,Uruguay and Argentina

1)Countries with the highest goals includes Germany,Brazil and Argentina


2)Highest overall yearly attendance was recorded in 1994


3)More Team qualified for World cup from 1998-

4)The most goals were scored in 2014


5)More matches were played from 1998-2014(since more teams qualified too)


6)Uruguay vs Brazil recorded the highest match attendance on 16th July,1950


7)The rate at which team win at home matches is greater than the rate they win at away matches
​
