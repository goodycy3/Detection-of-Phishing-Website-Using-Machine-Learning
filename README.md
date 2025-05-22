# DETECTION OF PHISHING WEBSITES USING MACHINE LEARNING 

## Objective
Phishing website is one of the internet security problems that target the human vulnerabilities rather than software vulnerabilities. It can be described as the process of attracting online users to obtain their sensitive information such as usernames and passwords.The objective of this project is to train machine learning models and deep neural network on the dataset created to predict phishing websites. Both phishing and legitimate URLs of websites are gathered to form a dataset and from them required URL and website content-based features are extracted. The performance level of each model is measured and compared.

## Data Collection
**phishing URL Dataset**
The set of phishing URLs are collected from opensource service called **PhishTank**. This service provide a set of phishing URLs in multiple formats like csv, json etc. that gets updated hourly. To download the data: https://www.phishtank.com/developer_info.php. From this dataset, 5000 random phishing URLs are collected to train the ML models.

**legitimate URL Dataset**
The legitimate URLs are obatined from the open datasets of the University of New Brunswick, https://www.unb.ca/cic/datasets/url-2016.html. This dataset has a collection of benign, spam, phishing, malware & defacement URLs. Out of all these types, the benign url dataset is considered for this project. From this dataset, 5000 random legitimate URLs are collected to train the ML models.

The above-mentioned datasets are uploaded to (https://github.com/goodydeves/PhishBuster/tree/master/ML%20work/DataSets)' folder of this repository.

## Feature Extraction
The below mentioned category of features are extracted from the URL data:

1.   Address Bar based Features 
         In this category 9 features are extracted.
2.   Domain based Features
         In this category 4 features are extracted.
3.   HTML & Javascript based Features
         In this category 4 features are extracted.


So, all together 17 features are extracted from the 10,000 URL dataset and are stored in file in the DataFiles folder.
The features are referenced from the https://archive.ics.uci.edu/ml/datasets/Phishing+Websites.

## Models & Training

Before stating the ML model training, the data is split into 80-20 i.e., 8000 training samples & 2000 testing samples. From the dataset, it is clear that this is a supervised machine learning task. There are two major types of supervised machine learning problems, called classification and regression.

This data set comes under classification problem, as the input URL is classified as phishing (1) or legitimate (0). The supervised machine learning models (classification) considered to train the dataset in this project are:

* Decision Tree
* Random Forest
* Multilayer Perceptrons
* XGBoost
* Autoencoder Neural Network
* Support Vector Machines

All these models are trained on the dataset and evaluation of the model is done with the test dataset. 

### **NOTE** ###
The model XGBoost has the highest accuracy and also The listed (feature extraction) to validate URLs were integrated to a webapplication using django framework to effeciently detect phishing URL links.

**Tools Used** <br>
💡 Jupyter notebook <br>
💡 Pycharm <br>
💡 Postman <br>
💡 Chrom Browser <br> 


# Presentation

📍 The short video presentation for this project is named "Project Summary.mp4" <br>
📍 The slide presentation for this project is named "presentation slides.ppt" <br>
📍 The Write-up Documentation for this project is named "Chapter 1-5 DETECTING PHISHING WEBSITES USING MACHINE LEARNING.pdf"



# Web application 
I created a Web application named <a href="https://phish-buster.vercel.app/">Phishbuster</a> to help Users Validate Website Links. The name of the folder is <b>"Project_Webapp.7z"</b> 
NOTE: The website isn't linked to the ML functionality. But you can check the Project Video.


# ML work 
The ML work folder consists of "Dataset" and "Jupyter Notebook of the project" 
**Phishing Website Detection Training & Testing Models on Datasets.ipynb**
**URL_Feature_Extraction_from_Datasets.ipynb**

# Next Steps
This project can be further extended to the creation of browser extensions (for Chrome, brave, opera mini etc) to help Users by adding to the browser extension to detect Phishing URLs.

Copyright (c) 2021 Goodness Adediran

All rights reserved.  
No part of this software, including source code or documentation, may be reproduced,
distributed, performed, displayed, or transmitted in any form or by any means, without
the prior written permission of the copyright holder.
