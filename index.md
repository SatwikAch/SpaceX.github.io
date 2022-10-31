---
layout: default
---

# Method Overview

![SpaceXpipeline](SpaceX_Overview.jpg) The SpaceX (**spa**tially dependent gene **c**o-**ex**pression network) is a Bayesian methodology to identify both shared and cluster-specific co-expression network across genes. These clusters can be cell type specific or based on spatial regions. SpaceX uses an over-dispersed spatial Poisson model coupled with a high-dimensional factor model which is based on a dimension reduction technique for computational efficiency.

The Figure above shows the overall conceptual flow of our pipeline. **Panel A** is an image of a tissue section from the region of interest. **Panel B** shows spatial gene expression and biomarkers which are recorded from that tissue section with the help of sequencing techniques. **Panel C** is the resulting data matrix of gene expression along with spatial locations and cluster annotations on the tissue. All these serve as input for the SpaceX model to obtain the shared (**Panel D**) and cluster-specific co-expression networks (**Panel E**). Finally, we use these networks for downstream analysis to detect gene modules and hub genes across spatial regions (**Panel F** & **Panel G** respectively) for biological interpretation.
