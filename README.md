# Clustering

In this repo we will have a look at clustering.  
We will go through the k-means and dbscan clustering algorithms and how to implement them in Python.

## Task/Procedure

Please work in pairs through the notebook/markdown files in this particular order:

1. [Clustering in Tableau](1_Clustering_in_tableau.md)
2. [Implementing k-means in Python](2_k_means_in_python.ipynb)
3. [Limitations of K-Means and Intro to DBSCAN](3_Limits_kmeans.ipynb)
4. [Clustering with DBSCAN in Python](4_DBSCAN_in_python.ipynb)

## Environment & Set-up

1. Use your nf_sql environment   
2. Check, if scikit-learn, scipy, python-dotenv and seaborn are installed.  
If not, install them in your activated environment.  


Furthermore, for the database connection, add your .env file from the [da-external-data-sourcing-repo](https://github.com/neuefische/da-external-data-sourcing) to this repo.  
You can use this terminal command:  
```zsh
cp ../da-external-data-sourcing/.env .