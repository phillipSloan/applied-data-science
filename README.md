# Applied Data Science Project: Mental Health and Screen Time
Investigating whether and how the amount of screen time (using phones, computers, and tablets) a person spends at age 16 
affects their levels of depression and anxiety at age 18.

# Visualisations

### NaN Values in Diagnosis Variables
<a href="#nan-values-in-diagnosis-variables"></a>

Heatmap of the four diagnosis variables: has_dep_diag, dep_score, dep_thoughts, secd_diag.
NaN entries represented as 0 (dark) and not NaN entries represented as 1 (bright). 
The lines show that there are rows of missing values across all four diagnosis variables. 
The variable with the least data is dep_thoughts, the other three diagnosis variables have almost equal amounts of data.

![NaN vs not NaN entries fo diagnosis variables](https://github.com/phillipSloan/applied-data-science/blob/main/images/nan-diagnosis-heatmap.png?raw=true)

### Correlation Matrix Heatmap
<a href="#correlation-matrix-heatmap"></a>

Heatmap of the correlation matrix of the 4513 rows that have at least one not NaN diagnosis variable. 
It shows that none of the screen time columns are correlated with a diagnosis column.
All correlation values all <0.03.


![Correlation Matrix Heatmap showing no correlation between mental health and screen time](https://github.com/phillipSloan/applied-data-science/blob/main/images/correlation-matrix-heatmap.png?raw=true)


### Correlation Matrix Heatmap for Negatively Correlated Variables
<a href="#correlation_matrix_heatmap_for_negatively_correlated_variables"></a>
A heatmap of the correlation matrix of the 4513 rows that have at least one diagnosis available.
The aim with this visualisation was to try and find a negative correlation between these variables and diagnosis variables. No correlation was found, the most negative correlation found was -.031

![Correlation Matrix Heatmap showing no correlation between mental health and variables thought to positively affect a childs mental health](https://github.com/phillipSloan/applied-data-science/blob/main/images/neg-correlation-matrix.png?raw=true)

### Dimensionality Reduction - PCA <a name="PCA"></a>
Principal Componant Analysis for all of the data. 1 (yellow) implies a diagnosis of depression, 0 (purple) implies no diagnosis of depression.
![PCA for mental health and screen time](https://github.com/phillipSloan/applied-data-science/blob/main/images/PCA.png?raw=true)

### Dimensionality Reduction - UMAP <a name="UMAP"></a>
![UMAP for mental health and screen time](https://github.com/phillipSloan/applied-data-science/blob/main/images/UMAP-50.png?raw=true)
![UMAP for mental health and screen time](https://github.com/phillipSloan/applied-data-science/blob/main/images/UMAP-500.png?raw=true)
