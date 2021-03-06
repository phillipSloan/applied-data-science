# Applied Data Science Project: Mental Health and Screen Time
Investigating whether and how the amount of screen time (using phones, computers, and tablets) a person spends at age 16 
affects their levels of depression and anxiety at age 18.

# Visualisations

### NaN Values in Diagnosis Variables
Heatmap of the four diagnosis variables: has_dep_diag, dep_score, dep_thoughts, secd_diag.
NaN entries represented as 0 (dark) and not NaN entries represented as 1 (bright). 
The lines show that there are rows of missing values across all four diagnosis variables. 
The variable with the least data is dep_thoughts, the other three diagnosis variables have almost equal amounts of data.

![NaN vs not NaN entries fo diagnosis variables](https://github.com/phillipSloan/applied-data-science/blob/main/images/nan-diagnosis-heatmap.png?raw=true)

### Correlation Matrix Heatmap
Heatmap of the pearson correlation matrix of the 4513 rows that have at least one not NaN diagnosis variable. 
It shows that none of the screen time columns are correlated with a diagnosis column.
All correlation values all <0.03. Method used:

![pearson Correlation Matrix Heatmap showing no correlation between mental health and screen time](https://github.com/phillipSloan/applied-data-science/blob/main/images/correlation-matrix-heatmap.png?raw=true)



Heatmap of the spearman correlation matrix:
![Spearman Correlation Matrix Heatmap showing no correlation between mental health and screen time](https://github.com/phillipSloan/applied-data-science/blob/main/images/correlation-matrix-heatmap-spearman.png?raw=true)


### Strip Plots
Strip plots of the 4513 rows that have at least one at least one not NaN diagnosis variable. 
The rows of the plot are the different screen times features, the columns of the plot are the four different diagnosis values. 
A value of 0 represents a NaN value other than for has_dep_diag where 0 means No and 1 means Yes. 
The strip plot shows that there is no correlation between screen time and any of the diagnosis values.

![Strip Plot](https://github.com/phillipSloan/applied-data-science/blob/main/images/strip-plot-no-nan-diag.png?raw=true)

### Correlation Matrix Heatmap for Negatively Correlated Variables
A heatmap of the correlation matrix of the 4513 rows that have at least one diagnosis available.
The aim with this visualisation was to try and find a negative correlation between these variables and diagnosis variables. No correlation was found, the most negative correlation found was -.031

![Correlation Matrix Heatmap showing no correlation between mental health and variables thought to positively affect a childs mental health](https://github.com/phillipSloan/applied-data-science/blob/main/images/neg-correlation-matrix.png?raw=true)

### Dimensionality Reduction - PCA
Principal Component Analysis for all of the data. 1 (yellow) implies a diagnosis of depression, 0 (purple) implies no diagnosis of depression.

![PCA for mental health and screen time](https://github.com/phillipSloan/applied-data-science/blob/main/images/PCA.png?raw=true)

### Dimensionality Reduction - UMAP
Unified Manifold Approximation Projection for all the data. The first demonstrates when the parameter nneighbours is 50 and the second shows nneighbours at 500 which allows a demonstration of a local and global view of the data. Very little changes between them. Like PCA, 1 (yellow) implies a diagnosis of depression, 0 (purple) implies no diagnosis of depression.
![UMAP for mental health and screen time nneighours 50](https://github.com/phillipSloan/applied-data-science/blob/main/images/UMAP-50.png?raw=true)
![UMAP for mental health and screen time nneighbours 500](https://github.com/phillipSloan/applied-data-science/blob/main/images/UMAP-500.png?raw=true)

### Confusion Matrix for Machine Learning Algorithms
A single confusion matrix as despite several different models (and variations of the same model) being ran, they all created the same resultant confusion matrix.
![Confusion Matrix](https://github.com/phillipSloan/applied-data-science/blob/main/images/Confusion%20Matrix.png?raw=true)
