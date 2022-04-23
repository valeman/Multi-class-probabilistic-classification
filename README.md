# Multi-class-probabilistic-classification

(Preliminary documentation)

Implementation of multi-class probabilistic classification using inductive and cross Venn–Abers predictors described in [Multi-class probabilistic classification using inductive and cross Venn–Abers predictors](https://proceedings.mlr.press/v60/manokhin17a.html)

The VennABERS.py file is a pure Python implementation of the fast Venn-ABERS Predictor described in Vovk2015 for binary classification implemented in https://github.com/ptocca/VennABERS/

A Venn-ABERS predictor outputs two probability predictions of class 1 (these can be considered prediction interval) and is a regularised form of isotonic regression that, unlike isotonic regression, does not suffer from overfitting in small size datasets. The Venn-ABERS predictor can be viewed as a distribution-free calibration function that maps scores output by a scoring classifier to well-calibrated probabilities. A gentle introduction can be found in the tutorial Toccaceli2017 listed on Awesome Conformal Prediction https://github.com/valeman/awesome-conformal-prediction

