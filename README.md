# Big-Health-Data
Final project
Data Source:

https://physionet.org/content/mimiciii-demo/1.4/

https://physionet.org/content/mimiciii/1.4/

Data decription: https://mimic.physionet.org/mimictables/

## Introduction

The repository contains final CSE-6250 project code created by Team 03.  
The entire project development cycles were divided into two stages. Feature Engineering, Model Training.

## Setup and Data Preprocessing and Model Design


(i)  Feature Engineering as part of preprocessing:

Environment Specification:

PySpark on Local windows OS environment (with 100 GB space, 12.0 GB RAM, and 2.30 GHz processor ).

We loaded following tables into PySpark:

	- ADMISSIONS.csv
	- CHARTEVENTS.csv
	- DIAGNOSES_ICD.csv
	- D_ICD_DIAGNOSES.csv
	- ICUSTAYS.csv
	- LABEVENTS.csv
	- OUTPUTEVENTS.csv
	- PATIENTS.csv

feature_builder.prepare_data script: will take care of the orchestration process for filtering a building the features.

On the other side repository script contains the data layer implementation done with pyspark. 

(ii) Data statistical description:

the code located in the Data statistical description.ipynb

(iii) Data pre-process

the code located in the Data pre-process_machine learning.ipynb

the main purpose of this code is to create the features_svmlight.train file:


1 7:2.0  14:3.85
 

the first item is the mortality(yes 1/no 0), and the label and it will
be followed by a series of feature-value pairs sorted by the feature index (idx) value.

(iv) machine learning models

the code located in the Machine learning models.ipynb

We adopted four models in this part:
logistic regression
support vector machine
decision tree
random forest

(v) RNN

the code located in the RNN model.ipynb






