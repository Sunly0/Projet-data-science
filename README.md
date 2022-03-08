# projet-data-science
Projet de science des données sur les iris

import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
from datetime import datetime
import dateutil.parser
import re

#La commande ci-dessous signifie que la sortie de plusieurs
#commandes dans une cellule sera sortie en une seule fois

from IPython.core.interactiveshell import InteractiveShell
InteractiveShell.ast_node_interactivity = "all"

#La commande ci-dessous indique à jupyter d'afficher 
#jusqu'à 80 colonnes, ce qui permet de garder tout visible.

pd.set_option('display.max_columns', 80)
pd.set_option('expand_frame_repr', True)

%matplotlib inline

sns.set_palette("hls")
from sklearn import preprocessing
from sklearn.cluster import KMeans

from scipy import stats as stats
from sklearn.model_selection import train_test_split, cross_val_score
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error, make_scorer
import statsmodels.api as sm

