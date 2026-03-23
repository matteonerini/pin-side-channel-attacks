# Machine Learning for PIN Side-Channel Attacks Based on Smartphone Motion Sensors

This repository contains code to reproduce the paper:

> M. Nerini, E. Favarelli, M. Chiani, "[Machine learning for PIN side-channel attacks based on smartphone motion sensors](https://ieeexplore.ieee.org/document/10061187)," IEEE Access, 2023.

## Code

The `dataset.txt` file contains a 5400 x 17 matrix in which:

* each row is a sampled digit.
* each column is a feature: the first is the pressed digit and the following are motion sensor values.

The `PIN_recognition.ipynb` Jupiter Notebook contains the code to replicate the results in the paper.

The files `rf-prod.csv`, `svm-prod.csv`, `mlp-prod.csv`, and `knn-sum.csv` have been obtained throguh `PIN_recognition.ipynb` and are attached for an easier replication of the figures.
