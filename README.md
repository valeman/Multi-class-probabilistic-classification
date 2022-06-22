# Multi-class probabilistic classification using Venn-ABERS (Conformal) prediction

[![DOI](https://zenodo.org/badge/458585236.svg)]([https://zenodo.org/](https://zenodo.org/badge/458585236.svg)

(Preliminary documentation)

![Log loss wavefront dataset](https://github.com/valeman/Multi-class-probabilistic-classification/blob/main/results/wavefront%20log%20loss.png)

![Brier loss wavefront dataset](https://github.com/valeman/Multi-class-probabilistic-classification/blob/main/results/wavefront%20brier%20loss.png)

Implementation of multi-class probabilistic classification using inductive and cross Venn–Abers predictors described in [Multi-class probabilistic classification using inductive and cross Venn–Abers predictors](https://proceedings.mlr.press/v60/manokhin17a.html). This code has also been released on [Papers with Code](https://paperswithcode.com/search?q_meta=&q_type=&q=Multi-class+probabilistic+classification+using+inductive+and+cross+Venn–Abers+predictors).

The VennABERS.py file is a pure Python implementation of the fast Venn-ABERS Predictor for binary classification implemented in https://github.com/ptocca/VennABERS/ as published in NeurIPS paper [Large-scale probabilistic predictors with and without guarantees of validity](https://proceedings.neurips.cc/paper/2015/hash/a9a1d5317a33ae8cef33961c34144f84-Abstract.html)

Unlike other methods such as Platt's scaler and Isotonic Regression Venn-ABERS predictors (being a form of conformal prediction) contain inbuilt mathematical guarantees of validity (lack of bias). In addition Venn-ABERS predictors are multi-output predictors that output two probability predictions of class 1. Such two probability prediction of assigning label 1 for each test objectc can be considered prediction interval. The interval width contains valuable information about degree of certainty of prediction, such information is not available when using other calibration methods such as Platt's and isotonic regression. 

In addition Venn-ABERS is a more advanced and regularised form of isotonic regression that, unlike isotonic regression, does not suffer from overfitting in non-large size datasets.

The Venn-ABERS predictor can be viewed as a distribution-free calibration function that maps scores output by a scoring classifier to well-calibrated probabilities. A gentle introduction can be found in the tutorial by Paolo Toccaceli (2017) listed on Awesome Conformal Prediction https://github.com/valeman/awesome-conformal-prediction

