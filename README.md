# hctsa_phenotypingWorm

A Matlab code package for running [hctsa](github.com/benfulcher/hctsa) analysis on movement speed data of five strains of the nematode worm *Caenorhabditis elegans*: the CB4856 (Hawaiian wild isolate), and N2 (lab) strains, and the mutants *dpy-20(e1282)* (morphological mutant), *unc-9(e101)* (neural mutant), and *unc-38(e264)* (neural mutant).
A summary of the analysis is [published here](http://www.cell.com/article/S2405471217304386/fulltext).

## The data
The data were very kindly provided by Andre Brown and Bertalan Gyenes, Imperial College London, and can be downloaded, along with all of the *hctsa* calculations, either by running `downloadComputedData`, or [from figshare](https://dx.doi.org/10.4225/03/580478f951263)
See [wormbase](wormbase.org) for more information about the data, including gene knockouts.
Note that the Hawaiian strain, CB4856, is labeled as `H` here.

## hctsa feature extraction

In addition to the data file, `HCTSA.mat`, containing the results of *hctsa* feature extraction ([on figshare](https://dx.doi.org/10.4225/03/580478f951263)), this repository also requires [hctsa](github.com/benfulcher/hctsa) to be installed and paths to this package added (through the `startup.m` script in the *hctsa* package).

* `wormAnalysis` contains the main steps for processing and analysis
* `worm_TopFeatures` allows more in-depth plotting for individual features
* `paperMainTextFigures` reproduces the figures in the main text of the implementation paper
* `doFilter` is a function for filtering different sets of features and normalizing

## python analysis

[Luiz Gustavo](https://github.com/lgaalves) has worked up an analysis of the HCTSA data using [scikit-learn](https://scikit-learn.org) in python in [this repository](https://github.com/lgaalves/hctsa_phenotypingWorm_python).
