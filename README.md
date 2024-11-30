### 6.5 Task: Clustering Analysis with K-Means

#### 1. **Install and Import Libraries**
   - Begin by installing and importing all necessary libraries in your Jupyter notebook. You will need libraries such as `pandas`, `numpy`, `matplotlib`, `seaborn`, and `sklearn` for data manipulation, visualization, and running the k-means algorithm.

#### 2. **Import and Clean Data**
   - Import your dataset and perform any necessary cleaning, manipulations, and reprocessing. This might include:
     - Renaming columns for clarity or standardization.
     - Handling missing values.
     - Dropping irrelevant columns.
   
   - **Key consideration:** The k-means algorithm can only handle **numerical variables**, so make sure to remove or encode any categorical columns appropriately.

#### 3. **Standardize the Data**
   - The k-means algorithm is sensitive to the scale of the features, and differences in variable scales can lead to biased results. **Standardize** your data by scaling it (e.g., using `StandardScaler` from `sklearn`) to ensure that each feature contributes equally to the clustering process.

#### 4. **Use the Elbow Technique**
   - Apply the **elbow technique** to determine the optimal number of clusters for your k-means algorithm. This involves plotting the **within-cluster sum of squares (inertia)** against the number of clusters. Look for the "elbow" point in the plot, where the inertia starts to level off. This point indicates the optimal number of clusters.
   
#### 5. **Choose the Number of Clusters**
   - Based on the elbow plot, make an **informed decision** about the number of clusters you will use. In a markdown cell, for this task I decided to use 3 since the slope of the plot platued at this marker. 

#### 6. **Run the K-Means Algorithm**
   - Run the **k-means algorithm** on your dataset using the chosen number of clusters. Use `KMeans` from `sklearn` to fit the model to your data and assign clusters.

#### 7. **Add Clusters to DataFrame**
   - Attach a new column, such as `'cluster'`, to your dataframe. This column will contain the cluster assignments for each data point (trip).
   
   - This will enable you to create visualizations that show how different variables are distributed across the clusters.

#### 8. **Create Visualizations**
   - **Generate visualizations** to explore your clustered data.

#### 10. **Calculate Descriptive Statistics**
   - Use the `groupby()` function to calculate descriptive statistics (mean, median, standard deviation, min, max, count, etc.) for the clusters based on **trip duration** of the riders in the Citbike dataset. 
