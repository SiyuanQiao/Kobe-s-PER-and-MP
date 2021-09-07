# Kobe-s-PER-and-MP

## Section 1 Import file 

This is an image about his stats bby different number (8,24)
![image](https://user-images.githubusercontent.com/90233968/132284284-680237ac-fd95-4bd8-9160-a32914efc1fc.png)

## Section 2 Creating chart and plot using Colab
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
%matplotlib inline
import plotly.graph_objects as go

data = pd.read_csv( '/content/advanced_stats.csv', parse_dates=['Season'])

df = pd.read_csv("/content/advanced_stats.csv",sep=",")
d = dict(zip(df.index,df.values.tolist()))
df.set_index('Season')[['PER','OWS']].plot.bar()
plt.show()

x.scatter_3d(data, x="Age", y= 'MP', z= 'PER')
