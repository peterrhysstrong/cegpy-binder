# cegpy-binders
The following binders provide examples for using the [cegpy](https://github.com/g-walley/cegpy) package.
API documentation can be found at [cegpy.readthedocs.org](https://cegpy.readthedocs.io/en/latest/).

## Basic Example: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/peterrhysstrong/cegpy-binder/HEAD?labpath=1_basic_example.ipynb) 
This first example builds a Chain Event Graph (CEG) from a discrete dataset showing results from a medical experiment.
The dataset used is symetrical, built from a rectangular dataset. These CEGs are known as _stratified_ in the literature.

## Non-stratified Example: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/peterrhysstrong/cegpy-binder/HEAD?labpath=2_non_stratified_example.ipynb) 
This example builds a Chain Event Graph (CEG) from a asymmetric dataset. In simple words, a dataset is asymmetric when the event tree describing the dataset is not symmetric around its root. The class of CEGs built from asymmetric event trees is said to be _non-stratified_.

## CEG Reduction Example: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/peterrhysstrong/cegpy-binder/HEAD?labpath=3_reducing_a_ceg.ipynb) 
A complete CEG shows all possible trajectories that an individual undergoing the process might experience. However, on observing any evidence, certain or uncertain, some edges and nodes become unvisited with probability 1. The CEG model can be reduced such that these edges and nodes are excluded, without any loss of information. Once reduced, the probabilities displayed can be also be revised.

## Sampling Missing Values Example: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/peterrhysstrong/cegpy-binder/HEAD?labpath=4_sampling_missing_values.ipynb)
The package, by default, treats all blank and `NaN` cells as structural missing values. However, sometimes these might occur due to sampling limitations. On the other hand, we might not observe a certain value for a variable (given its ancestral variables) not because that value is a structural zero but because of sampling limitations. 

In this example we cover two things,

1. How to define arguments to allow the package to distinguish between structual and sampling missing values?
1. How to add a value which has not been observed in the dataset due to sampling limitations (i.e. its frequency is a sampling zero)?

## AHC Customisation Example: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/peterrhysstrong/cegpy-binder/HEAD?labpath=5_ahc_customisation.ipynb)
The AHC is typically loaded with certain default parameters. If these are not suitable for your application, these can be modified.
