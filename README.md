# Clustering the Countries
### Problem Statement: 
- Categorise the countries using socio-economic and health factors that determine the overall development of the country. Identify the top-5 countries that are direst need of aid.
### Methodology:
- The dataset was loaded for understanding and some of the column values were changed to actual values.
- EDA was performed which included univariate and bivariate analysis to check data is distribution & relationship between various columns respectively.
- Outliers in data affects the formation of clusters hence, it was handled using capping method.
- To check the cluster tendency hopkin’s test was perrformed.
- The dataset was scaled using StandardScaler as the data were in different ranges.
- The number of clusters was calculated using Silhouette Score and Elbow-curve and number of clusters decided was 3.
- Model Fitting using K-Means and following clusters formed: Cluster 2  high child_mort, low income and gdpp. Cluster 1  low child_mort, high income and gdpp. Cluster 0  child_mort slightly more than cluster 1, income and gdpp lesser than cluster 2.
- The clusters were plotted and cluster profiling was done for child_mort, income and gdpp.
- Model fitting using Hierarchical Clustering: The dendrogram was created using complete linkage instead of single linkage as the dendrograms were not clear.
- The number of clusters according to dendrogram was 4 but considered 3 for analysis.
- Formation of clusters using Hierarchical Clustering: Cluster 0  high child_mort, low income and gdpp. Cluster 2  low child_mort, high income and gdpp. Cluster 1  child_mort slightly more than cluster 2, income and gdp more than cluster 0.
- Again, the clusters were plotted and cluster profiling was done.
- Results from both algorithms were same and top-5 countries which required immediate aid are:
  1. Sierra Leone
  2. Haiti
  3. Chad
  4. Central African Republic
  5. Mali
