# Case Studies from Algorithms for Cell Reprogramming Strategies in Boolean Networks

## Use of .ipynb files

Files with the .ipynb extention are Jupyter notebooks, that can be used with the colomoto docker.
Instructions on how to install the colomoto docker can be found at https://colomoto.github.io/colomoto-docker/

## Cardiac gene regulatory network

The majority of the computations can be found in the Cardiac.ipynb file.
The static analysis was performed by hand, by comparison of the attractors shown in the notebook.

## Tumour network

The Tumour.ipynb allow to compute the first results for the tumour network. However, the interface with Jupyter does not allow constraints or permanent perturbations yet. As a result, two shell scripts are given, one for the computations with constraints on DNAdamage and ECMicroenv, and one for the permanent perturbations (with more constraints).
These scripts use models written in the tumour directory, and the cabean tool. The scripts are given using the linux version, but can easily be changed to use the mac version.

## PC12 Cell differentiation network

As previously, the static analysis was performed by hand, by looking at the attractors and the interaction graph.
We did not find this version of the network on cellcollective or ginsim, thus the model is provided, both in a folder for sequential reprogramming, and as a single file for attractor based reprogramming strategies.
Two bash scripts allow to compute the perturbations from these models, named "pc12-command-attract-based.sh" and "command-pc12-seq.sh"
