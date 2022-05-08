## CS598Deep-Learning-for-Healthcare Final Project

# Overview

This repository contains code necessary to run the final project of CS 598 Deep Learning for Healthycare. The code part includes three main models: RNN, Retain, and Crossover rention models (3 models) inside this file. All these models are tested on real-world clinical dataset MIMIC-III. 


# Requirements

* Python >=3.5


# Running the Code

In ./data, you will find the well-preprocessed data in pickle form. We can also re-generate the data as follows:

1. Download MIMIC data and put DIAGNOSES_ICD.csv and PRESCRIPTIONS.csv in ./data/
2. run the code in ./code/. Please run preprocess first, and you can then any files thereafter.

Please note: We only download the DIAGNOSES_ICD.csv and put in github because PRESCRIPTIONS.csv is too big (700+ mb).  Github does not allow any file larger than 25 mb.


In ./code, you will find all the code needed for this project. In addition to the pre-process code, there are 3 files and they are RNN, RETAIN, and Crossover rention models (3 models)

Data information in ./data:


seq.pkl: This is the major dataset for this project. It is a list of list. The list contains patients and each patients contains vist.

pids.pkl: This contains the patient ID

rtypes.pkl: This contains the event ID

types.pkl: This contains the event ID's index

vids.pkl: This contains the visit ID

# Model Comparation


RETAIN can provide sequential prediction of medication combination based on a two-level neural attention model that detects influential past visits and significant clinical variables within those visits.


To compare the performance of these models, we used precision rate, retaintion rate as well as F1 score. 


# Cite

The paper does not provide any code. All the codes are provided by our group. 














