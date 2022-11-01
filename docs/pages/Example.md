---
layout: page
title: Example
menubar: docs_menu
toc: true
show_sidebar: false
---


### Data inputs

The first input is **Gene_expression_mat** which is $N \times G$ dataframe. Here $N$ denotes the number of spatial locations and $G$ denotes number of genes. 

The second input is **Spatial_locations** is a dataframe which contains spatial coordinates.

The third input is **Cluster_annotations**.

The fourth input is **sPMM**. If TRUE, the code will return the estimates of sigma1_sq and sigma2_sq from the spatial Poisson mixed model.

The fifth input is **Post_process**. If FALSE, the code will return the posterior samples of $\Phi$ and $\Psi^c$ (based on definition in equation 1 of the SpaceX paper) only. Default is TRUE and the code will return all the posterior samples, shared and cluster specific co-expressions.

The final input is **numCore**. The number of requested cores for parallel computing and default is set to be 1. 

### Output
You will obtain a list of objects as output.

**Posterior_samples**	contains all the posterior samples.

**Shared_network** provides the shared co-expression matrix (transformed correlation matrix of $G_{s} = \Phi \Phi^{T}$).

**Cluster_network** provides the cluster specific co-expression matrices (transformed correlation matrices of $G_{c} = \Phi \Phi^{T} + \Psi^{c} {\Psi^{c^{T}}}$).


### Example
Here we provide an example to run the SpaceX method. 
``` r
# Reading the Breast cancer data

# Spatial locations
head(BC_loc)

# Gene expression for data
head(BC_count) 

# Data processing
G <-dim(BC_count)[2] # number of genes
N <-dim(BC_count)[1] # number of locations
```

Next, we'll apply the SpaceX method on the Breast cancer dataset.

``` r
# Application to SpaceX method
BC_fit <- SpaceX(BC_count,BC_loc[,1:2],BC_loc[,3],sPMM=FALSE,Post_process = TRUE, numCore=2)

# Shared_network :: Shared co-expression matrix
# Cluster_network :: Cluster specific co-expression matrices
```
[Go to the Home Page]({{ '/' | absolute_url }})
