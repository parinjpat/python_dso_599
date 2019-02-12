# python_dso_599
Python Final Project Repository
# import file and selected columns
import pandas as pd
data=pd.read_csv('movies_metadata.csv')
data.head()
# The original dataset includes 45,466 records and 24 fields.
data.shape
# we selected the meaningful fields.
newdata=pd.read_csv('movies_metadata.csv',usecols=[0,2,3,8,10,12,13,14,15,16,19,22,23])
newdata.head()
#After our selection, the new dataset includes 45,466 records and 13 fields.
newdata.shape
newdata.dtypes
# Basic Statistics for numeric variables.
#?? python does not treat budget and popularity as int/float.
newdata.describe().transpose()
