# Bacteria-Species-Classification-ML-Framework  

[![Python](https://img.shields.io/badge/Python-3.7%2B-green.svg)](https://www.python.org/)  
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)  
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0%2B-brightgreen.svg)](https://scikit-learn.org/)  

## Overview  
This repository contains the code and documentation for a computational framework that leverages machine learning techniques to enable accurate classification of bacterial species, even closely related strains.

The framework integrates genomic analysis methods, such as motif screening and single nucleotide polymorphism (SNP) extraction, to derive informative features from bacterial genomes. These genomic insights are then fed into machine learning models, which are trained to reliably differentiate between bacterial species based on their distinctive patterns and characteristics.

## Table of Contents  
1. [Notebooks](#notebooks)  
   - [Feature Preprocessing](#feature-preprocessing)  
   - [Feature Engineering - Feature Transformation](#feature-engineering---feature-transformation)  
   - [Machine Learning - Embedded Method](#machine-learning---embedded-method)  
2. [Data](#data)  
3. [Usage](#usage)  

## Notebooks  

### Feature Preprocessing  
The `Feature Preprocessing.ipynb` notebook focuses on the following tasks:  
- Appending all motifs features into an Excel file  
- Aligning the motifs (gap filling)  
- Removing features with high missing values  
- Eliminating non-informative features  

### Feature Engineering - Feature Transformation  
The `Feature Engineering - Feature transformation.ipynb` notebook covers the following steps:  
- Tokenizing the sequences and encoding the label classes  
- Extracting the single nucleotide polymorphism (SNP) information for all feature columns  
- Creating a new dataframe that contains the strain label, class label, and SNPs information for machine learning training  

### Machine Learning - Embedded Method  
The `Machine Learning_Embedded Method - Top 20.ipynb` notebook includes:
- Feature scaling
- Feature selection using an embedded method  
- Training the selected top 20 features set with Random Forest and SVM (both tuned and untuned)  
- Model evaluation and prediction  
- K-fold validation, learning curve analysis, t-SNE visualization of selected featurees, feature importance analysis  

## Data  
The `final_snp.xlsx` file is the input data file that was generated during the feature engineering step. It contains the SNP motifs information that is used for the machine learning model training.  

## Usage  
You can open and run the notebooks using Anaconda Jupyter Notebook. Follow these steps:  

1. Open the notebooks in the following order:  
   - `Feature Preprocessing.ipynb`  
   - `Feature Engineering - Feature transformation.ipynb`  
   - `Machine Learning_Embedded Method - Top 20.ipynb`  
   The `final_snp.xlsx` file is used as the input for the machine learning notebook.  

Alternatively, you can use Google Colab to run the notebooks directly in the cloud. Simply upload the notebook files to your Google Drive and open them in Google Colab.
