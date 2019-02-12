# python_dso_599
Python Final Project Repository
# import file and selected columns
import pandas as pd
data=pd.read_csv('movies_metadata.csv',usecols=[0,2,3,8,10,12,13,14,15,16,19,22,23])
data.head()
