---
layout: page
title: Breast_Cancer_Data
permalink: /Cancer.html
ref: BC_data
order: 1
---


The human breast cancer data was collected by biopsy of a tissue sectioned at a thickness of $16\mu$m with visium technique. You can access the data [here](https://github.com/bayesrx/SpaceX/tree/main/data) (Ståhl et al., 2016). The locations are seperated into three spatially contiguous clusters, including tumor, intermediate, and normal with the following cluster sizes 114, 67, and 69 spots respectively. The expression levels are measured from $5262$ genes at $250$ spot locations and we used the SPARK method (Sun et al., 2020) with $5\%$ FDR cut-off on p-values to detect $290$ spatially expressed genes for this analysis. The SpaceX method is applied on the breast cancer data to obtain shared and cluster specific co-expression networks. Downstream analysis on these networks helped us to identify shared and cluster specific hub genes. Please see the video below for more details.  


![](BC.mp4){width=100%}


[Go to the Home Page]({{ '/' | absolute_url }})

