# Plagiarism Project, Machine Learning Deployment

This repository contains code and associated files for deploying a plagiarism detector using AWS SageMaker.

## Project Overview

This project is tasked with building a plagiarism detector that examines a text file and performs binary classification; labeling that file as either *plagiarized* or *not*, depending on how similar that text file is to a provided source text. Detecting plagiarism is an active area of research; the task is non-trivial and the differences between paraphrased answers and original work are often not so obvious.

This project will be broken down into three main notebooks:

**Notebook 1: Data Exploration**
* Load in the corpus of plagiarism text data.
* Explore the existing data features and the data distribution.

**Notebook 2: Feature Engineering**

* Clean and pre-process the text data.
* Define features for comparing the similarity of an answer text and a source text, and extract similarity features.
* Select "good" features, by analyzing the correlations between different features.
* Create train/test `.csv` files that hold the relevant features and class labels for train/test data points.

**Notebook 3: Train and Deploy Model in SageMaker**

* Upload train/test feature data to S3.
* Define a binary classification model and a training script.
* Train  model and deploy it using SageMaker.
* Evaluate  deployed classifier.


### Dataset
Model is implemented using the data.zip uploaded in this repository

### Libraries
Following Python libraries are used im Implementation
  
 - pandas 
 - numpy
 - sklearn
 - seaborn
 - matplotlib
 
### Steps
1. Clone the repository.
	```
		git clone https://github.com/NarayananAmudha/SageMaker_Plagiarism_Detector.git
	```
2. Open the `Plagiarism_Feature_Engineering.ipynb and Training_a_Model.ipynb` file.
	```
	
		
3.  Run the above code in jupyter notebook with AWS SageMaker account to create train.csv,test.csv and to build and evaluate model.

Please see the [README](https://github.com/udacity/ML_SageMaker_Studies/tree/master/README.md) in the root directory for instructions on setting up a SageMaker notebook and downloading the project files (as well as the other notebooks).

