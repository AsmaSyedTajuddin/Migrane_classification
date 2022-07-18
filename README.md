# Migrane_classification
Migrane_classification

![infographic-migraine-cute-info-graphic-149979031](https://user-images.githubusercontent.com/100385953/179564429-0e335371-0920-4dd6-924f-83bab2c26619.jpg)

Migraine Prediction Using Machine Learning

In this notebook, the target is to classify the type of migraine (a type of headache), given a set of features that are extracted from patient's medical records.

Data Loading

The first step is to load dataset into memory.

The dataset has 400 training examples & 24 set of features.

EDA (Explorarory Data Analysis):
Typical aura with migraine       247
Migraine without aura             60
Familial hemiplegic migraine      24
Typical aura without migraine     20
Basilar-type aura                 18
Other                             17
Sporadic hemiplegic migraine      14

From the figure, it can be seen that:

The most common type of migraine in the dataset is Typical Aura With Migraine
Migraine Wtihout Aura holds the second position with second most common place
Other 5 types of heartbeats in the dataset are less frequent as compared to the first two

<img width="701" alt="Screenshot 2022-07-18 at 19 00 31" src="https://user-images.githubusercontent.com/100385953/179564058-3e3067bc-eefa-4919-ae63-d97ecf5aaedd.png">

Sampling Dataset

We have unequal number of samples in each class of dataset, which means that we are dealing with imbalanced classification. We need to resample the dataset in order to make a machine learning model that learns all instances well. For this, we'll apply random oversampling & undersampling techniques.

For undergoing this procedure, we'll follow following steps:

First, we extract the features of each class from dataset
Then, we apply sampling to each of the classes by assigning equal number of instances to each class
Then we concatenate each of the dataframes in a single dataframe that contains equal samples of each class

<img width="819" alt="Screenshot 2022-07-18 at 19 01 26" src="https://user-images.githubusercontent.com/100385953/179564239-ac02dc58-1e0f-4d12-a781-184773ac33f4.png">
