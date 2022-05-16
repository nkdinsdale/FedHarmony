# FedHarmony
## Code implementation for FedHarmony (MICCAI 2022)

This is a working release of the code for FedHarmony Any issues please contact: nicola.dinsdale@cs.ox.ac.uk. Further code will be added in time.

Software Versions 
-----------------
Python 3.6.8

PyTorch 1.10.1

![network architecture](/figures/architecture.png)

Code supplied was used for the age prediction task but the framework is general. The architecture used needs to have three sections as shown in the figure above:
- Feature extractor
- Label Predictor
- Domain Predictor

## Scripts

The training procedure is formed of three distinct phases:
- Stage 1: harmonisation_main --> train the model for each site separately
- Stage 2: fed_equal --> aggregate weights according to FedEqual regime
- Stage 3: get_gaussians --> fit gaussian to data for each site separately

If you use code from this repository please cite the appropriate paper:
FedHarmony: COMING SOON
Unlearning Scanner Bias for MRI Harmonisation:
```@article{DINSDALE2021117689,
title = {Deep learning-based unlearning of dataset bias for MRI harmonisation and confound removal},
journal = {NeuroImage},
volume = {228},
pages = {117689},
year = {2021},
doi = {https://doi.org/10.1016/j.neuroimage.2020.117689},
author = {Nicola K. Dinsdale and Mark Jenkinson and Ana I.L. Namburete}
}
```

![pca alignment](https://github.com/nkdinsdale/FedHarmony/blob/main/figures/mygif.gif?style=centerme)
