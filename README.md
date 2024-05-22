# Clustering

In this repo we will have a look at clustering.  
We will go through the k-means and dbscan clustering algorithms and how to implement them in Python as well as in Tableau.

## Task/Procedure

Please work in pairs through the notebook/markdown files in this particular order:

1. [Clustering in Tableau](1_Clustering_in_tableau.md)
2. [Implementing k-means in Python](2_k_means_in_python.ipynb)
3. [Limitations of K-Means and Intro to DBSCAN](3_Limits_kmeans.ipynb)
4. [Clustering with DBSCAN in Python](4_DBSCAN_in_python.ipynb)  
5. [Clustering with k-means in Tableau](5_k_means_tabpy.md)

## Environment & Set-up

Use your nf_sql environment OR create a new environment (clustering_exercise) based on your existing environment you have used for the SQL-Python notebooks by
1. Creating a clone of your existing environment (replace 'name_old_env' accordingly):  
```conda create --clone name_old_env --name clustering_exercise```
2. Activate your cloned environment:  
```conda activate clustering_exercise``` 
3. Check, if scikit-learn, scipy, python-dotenv and seaborn are installed.  
If not, install them in your activated environment.  


Furthermore, for the database connection, add your sql_functions.py and .env file from the [da-external-data-sourcing-repo](https://github.com/neuefische/da-external-data-sourcing) to this repo - again without pushing it to GitHub.  
You can use these terminal commands:  
```bash
cp ../da-external-data-sourcing/.env .
```
```bash
cp ../da-external-data-sourcing/sql_functions.py .
```
