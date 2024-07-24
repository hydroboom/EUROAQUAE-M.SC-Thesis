Correlation Matrix and Principal Component Analysis

PCA
The following snippet will do a PCA and show the loadings, the sum of loadings, and the explained variance ratio. 
Principal Component Analysis (PCA) is a statistical technique which is used to reduce dimensionality of a multi-dimension dataset. 
In this case, the example is set with domain_585.csv file which has 4 oceanic variables: Thetao, Pr, Chl, So. The idea of a PCA is 
to create new variables using linear combination of these 4 variables so the dimensions are reduced, in this case from 4 to 2. This
 gives us 2 new components which are called Principal Components, and they explain the variance captured in the whole dataset.
 Explained variance ratio is the ratio that indicates how much of the total variance is captured by each PC. if PC1 is 0.70, then 
it means it captures 70% of the variance in the data. Note that, this doesn't mean that a specific variable is influencing the 
variance more. If you want this information on which variable is putting how much weight on which PC, you will look at the loadings.
 The loadings are coefficients of the linear combination that are defining each PC i.e it shows the contribution of each original 
variable (for example, thetao) to the principal component (say, PC1).

Correlation
There are 2 correlation analyses done here - one for the variables themselves and other one for the variables with Principal Component.
 The basic correlation analysis shows a pairwise correlation between all the pairs of variables in the dataset. The range is from -1 to 1 
where 1 is a perfect positive correlation and 0 is no correlation. For instance, from this dataset it seems PR has no correlation with CHL.
 Now it doesn't necessariliy mean that when there is rainfall or inflow from rivers into the sea, the CHL does not change at all - it 
means that the changes are so small that they cannot be There are numerous factors that influence these phenomenons - for instance So a 
correlation matrix is not the final outcome of checking relation among variables - there may be foreign influences on the variables which
 must be kept in mind.

P-values
This code calculates p-values in two key areas: correlation matrix and principal components. For the correlation matrix, it computes 
p-values to assess the likelihood that the observed correlations between variables are due to chance, with low p-values (typically < 0.05) 
indicating significant correlations. For principal components, it performs a permutation test to generate p-values for the explained 
variance ratios, comparing observed ratios with those from randomized data. Significant p-values here suggest that the principal components
 capture meaningful variance in the data. These p-values help determine the statistical significance of correlations and principal 
components in the dataset.


Notes:
The data/csv file input in this code as demonstration is also included within the folder of the IPYNB.
The base name is also split in portions as a part of using the separated strings in output file name.
Ensure that your input file is in the same format as the demo csv file.
