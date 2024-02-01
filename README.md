# Machine Learning for PIN Side-Channel Attacks Based on Smartphone Motion Sensors

This code package is related to the paper:

M. Nerini, E. Favarelli and M. Chiani, "[Machine Learning for PIN Side-Channel Attacks Based on Smartphone Motion Sensors](https://ieeexplore.ieee.org/document/10061187)," IEEE Access, 2023.

If you use this code or any modified part of it, please cite our paper.

## Abstract

Motion sensors are integrated into all mobile devices, providing useful information for a variety of purposes. However, these sensor data can be read by any application and website accessed through a browser, without requiring security permissions. In this paper, we show that information about smartphone movements can lead to the identification of a Personal Identification Number (PIN) typed by the user. To reduce the amount of sniffed data, we use an event-driven approach, where motion sensors are sampled only when a key is pressed. The acquired data are used to train a Machine Learning (ML) algorithm for the classification of the keystrokes in a supervised manner. We also consider that users insert the same PIN each time authentication is required, leading to further side-channel information available to the attacker. Numerical results show the feasibility of PIN cyber-attacks based on motion sensors, with no restrictions on the PIN length and on the possible digit combinations. For example, 4-digit PINs are correctly recognized at the first attempt with an accuracy of 37%, and in five attempts with an accuracy of 63%.

## Content of Code Package

The `dataset.txt` file contains a 5400 x 17 matrix in which:

* each row is a sampled digit.
* each column is a feature: the first is the pressed digit and the following are motion sensor values.

The `PIN_recognition.ipynb` Jupiter Notebook contains the code to replicate the results in the paper.

The files `rf-prod.csv`, `svm-prod.csv`, `mlp-prod.csv`, and `knn-sum.csv` have been obtained throguh `PIN_recognition.ipynb` and are attached for an easier replication of the figures.
