---
layout: page
title: Hypothalamus
permalink: /Hypothalamus.html
ref: MH_data
order: 0
---



Using the MERFISH technique, this dataset is collected from the preoptic region of the mouse hypothalamus, which regulates many social behaviors (Moffitt et al.,
2018). The MERFISH technique measures gene expression of single cells for different cell types, providing insights into the spatial organization of cells in the tissue. The dataset consists of $160$ genes and the corresponding gene expressions are measured across $4812$ spatial locations. These cells have been annotated into 7 different cell types (size) namely astrocyte $(724)$, endothelial cells $(503)$, ependymal cells $(314)$, excitatory neurons $(1024)$, inhibitory neurons $(1694)$, immature neurons $(168)$, and mature neurons $(385)$. You can access the data [here](https://github.com/xzhoulab/SPARK-Analysis/tree/master/processed_data). We apply the SpaceX method to obatin shared and cell-type specific co-expression networks. Next, we identify conserved and cell-type specfic hub genes based on the co-expression netwroks. Please see the video below for more details on the analysis. 


![](MH.mp4){width=100%}


[Go to the Home Page]({{ '/' | absolute_url }})

