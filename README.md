# GPEXP
Experimental Design for Gaussian Process Regression  
A python package for performing experimental design for Gaussian Process Regression

###General Information

Author: Alex Gorodetsky

Contact: goroda@mit.edu

Copyright (c) 2013-2015, Massachusetts Institute of Technology  
License: GPL2

### Software Dependencies

* python2.7
* numpy
* scipy
* matplotlib (not absolutely necessary but demos require it)
* nlopt: http://ab-initio.mit.edu/wiki/index.php/NLopt

# Overview
Experimental design deals with the issue of determining where to obtain new data in order to build accurate models.
Gaussian process regression is a useful method to build models of raw data or to build surrogate models for complex computational simulations. 

This software is different from most other GP software because it focuses on combining experimental design and Gaussian process regression. It was developed for performing the studies provided in the paper detailing the integrated variance experimental design function (link arxiv paper). It consists of the following options for kernels and experimental design cost functions (though adding new kernels and cost functions is fairly trivial)

Kernels
-------
  * Squared exponential
    * isotropic high dimensional 
    * automatic relevance determination high dimensional
  * Isotropic Matern kernel
  * Mehler Kernel

Experimental Design Cost Functions
----------------------------------
  * Integrated Variance
  * Conditional Entropy
  * Mutual Information
  
