# Challenge: It's not my fault!
## Champions
Alex Donkers/Ekatrina Petrova*

## Number of people per team: 
4

## Anticipated workload:
approx. 24 hours per person, including the time for preparation of the presentation

## Problem description:
About 15 to 30% of building energy in commercial buildings is wasted due to poor maintenance, improperly controlled equipment, and user behavior. In this regard, the proper functioning of Heating, Ventilation, and Air Conditioning (HVAC) systems is crucial, as they account for 38% of the total building energy consumption. Detecting anomalies and diagnosing critical faults in HVAC system components such as chillers and Air Handling Units (AHU) is essential, as such faults may lead to poor system performance systems and result in significant energy consumption [1]. 

The vast amount of available data from Building Management Systems (BMS), Energy Management Systems (EMS), Internet of Things devices, etc., have enabled powerful data-driven solutions that aim to improve and optimize the energy consumption of buildings by detecting, diagnosing and preventing system faults in (near) real time [2]. However, there are several challenges that currently hinder the streamlined application of automated Fault Detection and Diagnosis (FDD) approaches. On one hand, datasets with labelled faults are scarce, which challenges the efficient implementation of data-driven pproaches. On the other hand, typical FDD results lack context and explicit semantic definition, as well as representations that allow their reuse. An appropriate combination of data-driven and symbolic approaches has the potential to address such challenges. 

## Objectives:
Based on the above, the tasks in this challenge include:

1.	Identify anomalies in HVAC system operation using data from an existing building and a data-driven FDD approach. One way to achieve that is to rely on a stepwise approach combining a prediction model (e.g., LSTM) that learns to predict a certain output of the HVAC system based on the time-delayed set of inputs and outputs, and a clustering model (e.g., K-Means), which helps identify patterns or anomalies in the data by grouping similar data points together. Other approaches are also possible (e.g., Principal Component Analysis, Gaussian Porcess Regression, CNN-LSTM, Support Vector Machines, etc.).
2.	Create the semantic model of the building, its systems and the related faults (A-Box). For this purpose, you can use multiple existing ontologies such as [BOT](https://w3c-lbd-cg.github.io/bot/), [Brick](https://brickschema.org/), etc. [3,4]. You can also refer to the available representations in .ttl format to get you started [5]. To describe and contextualise the faults, you can either use an existing FDD ontology or one created for the purpose. 
3.	Visualise the semantically defined and contextualised faults in the context of the data stream in an simple web-based user interface.

## Research Questions:
RQ1: How to contextualise and semantically describe FDD results using semantic technologies?
RQ2: How to enable the reusability of semantic FDD datasets for HVAC systems in buildings?

## Datasets available:  
1.	LBNL Fault Detection and Diagnosis Datasets: 
https://data.openei.org/submissions/5763
2.	Building 59 datasets:  https://datadryad.org/stash/dataset/doi:10.7941/D1N33Q and https://bbd.labworks.org/ds/bbd/lbnlbldg59 
3.	Fault types and symptoms: https://www.nature.com/articles/s41597-023-02197-w 

## Tools:
1.	https://streamlit.io/, an open-source Python framework for interactive AI/ML data apps
2.	Several ML and data visualisation libraries are available, e.g., [TensorFlow](https://www.tensorflow.org/), [PyTorch](https://pytorch.org/), [Keras](https://keras.io/), [Pandas](https://pandas.pydata.org/), [Seaborn](https://seaborn.pydata.org/), [Matplotlib](https://matplotlib.org/), and many more. 
3.	[RDFLib](https://rdflib.readthedocs.io/en/7.0.0/gettingstarted.html): a Python package for working with RDF


## References: 

[1] Maryam Sadat Mirnaghi and Fariborz Haghighat. Fault detection and diagnosis of large-scale hvac systems in buildings using data-driven methods: A comprehensive review. Energy and Buildings, 229:110492, 2020.
[2] Yang Zhao, Tingting Li, Xuejun Zhang, and Chaobo Zhang. Artificial
intelligence-based fault detection and diagnosis methods for building energy systems: Advantages, challenges and the future. Renewable and Sustainable Energy Reviews, 109:85–101, 07 2019.
[3] Rasmussen, Mads Holten et al. BOT: The Building Topology Ontology of the W3C Linked Building Data Group. 143 – 161, 01 2021.
[4] Balaji, Bharathan et al. Brick : Metadata schema for portable smart building applications.  226:1273-1292, 09 2018.
[5] Lawrence Berkeley National Laboratory. (2022). LBNL Fault Detection and Diagnostics Datasets [data set]. Retrieved from https://dx.doi.org/10.25984/1881324; https://data.openei.org/submissions/5763.
