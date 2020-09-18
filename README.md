# bayesreg
Flexible Bayesian penalized regression modelling

This is a comprehensive, user-friendly toolbox implementing the state-of-the-art in Bayesian linear regression, logistic and count regression. The toolbox provides highly efficient and numerically stable implementations of ridge, lasso, horseshoe, horseshoe+, log-t and g-prior regression. The lasso, horseshoe, horseshoe+ and log-t priors are recommended for data sets where the number of predictors is greater than the sample size, and the log-t prior provides adaptation to unknown levels of sparsity. The toolbox allows predictors to be assigned to logical groupings (potentially overlapping, so that predictors can be part of multiple groups). This can be used to exploit a priori knowledge regarding predictors and how they may be related to each other (for example, in grouping genetic data into genes and collections of genes such as pathways).

Count regression is now supported through implementation of Poisson and geometric regression models. To support analysis of data with outliers, we provide two heavy-tailed error models in our implementation of Bayesian linear regression: Laplace and Student-t distribution errors. Most features are straightforward to use and the toolbox can work directly with MATLAB tables (including automatically handling categorical variables), or you can use standard MATLAB matrices.

The toolbox is very efficient and can be used with high-dimensional data. Please see the scripts in the directory "examples\" for examples on how to use the toolbox, or type "help bayesreg" within MATLAB. An R version of this toolbox is now available on CRAN. To install the R package, type "install.packages("bayesreg")" within R.

To cite this toolbox:
Makalic E. & Schmidt, D. F.
High-Dimensional Bayesian Regularised Regression with the BayesReg Package
arXiv:1611.06649 [stat.CO], 2016

UPDATE VERSION 1.9 (17/07/2020):

-Added support for count regression via Poisson and geometric regression models

-Added sparsity adaptive log-t shrinkage prior (option 'logt')

-Improved sparsification [br_sparsify]

References:

Enes Makalic and Daniel F. Schmidt (2016). High-Dimensional Bayesian Regularised Regression with the BayesReg Package, arXiv:1611.06649 [stat.CO]

Daniel F. Schmidt and Enes Makalic (2020). Log-Scale Shrinkage Priors and Adaptive Bayesian Global-Local Shrinkage Estimation, arXiv:1801.02321 [math.ST]

Daniel F. Schmidt and Enes Makalic (2019). Bayesian Generalized Horseshoe Estimation of Generalized Linear Models. ECML PKDD 2019: Machine Learning and Knowledge Discovery in Databases. pp 598-613
