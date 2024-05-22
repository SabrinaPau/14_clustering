# Using TabPy: Clustering in Tableau

You can execute Python code within Tableau by using TabPy.  
We have already showed you in the Live Demo how to integrate the K-Means algorithm in Tableau:

# How to use K-Means within Tableau with TabPy:
1. Create calcuated field
2. Use the following code:
```
SCRIPT_INT('
import numpy as np
from sklearn.cluster import KMeans
from sklearn.preprocessing import StandardScaler

X = np.column_stack([_arg1, _arg2])
X = StandardScaler().fit_transform(X)

km = KMeans(n_clusters = 3).fit(X)
return km.labels_.tolist()
',
AVG([Air Time]), AVG([Arr Delay]))
```
3. Drag calculation on colour --> will be used as table calculation
4. Edit table calculation and choose compute using 'Specific Dimensions'

**There will appear error messages until you have chosen a suitable dimension for the calculation.**


# Task
As K-Means has its limitations, as you have already learned [here](3_Limits_kmeans.ipynb), use DBSCAN for clustering the different airlines based on their average Air Time and average Arrival Delay in the flight data **in Tableau**.  

## DBSCAN in Tableau
Steps:
1. Connect to your flight data source.
2. Make sure, Tableau is connected to TabPy.
3. Choose a suitable way of visualizing the different airlines and their average Air Time and average Arrival Delay.
3. Create calculated field including the DBSCAN clustering code.
Use the K-Means code as orientation, only the model and its parameter need to be changed.
3. Cluster the airlines based on their average Air Time and average Arrival Delay using DBSCAN Clustering.

