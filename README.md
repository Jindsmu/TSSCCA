# TSSCCA Project README

## Overview

This project implements a Temporal-Spatial Sparse Canonical Correlation Analysis (TSSCCA) model for analyzing the longitudinal temporal dynamics between genetic data and brain imaging features. It contains the main function code, running code, and simulated data code. Below is a breakdown of the files in the project.

File Breakdown

##### 1\. runTSSCCA.m

Description: This is the main script to execute the TSSCCA model. It serves as the entry point for running the analysis. By calling this script, users can load the necessary datasets, set the parameters, and execute the analysis for temporal and spatial modeling of genetic and imaging data.



How to use: Simply run this script in MATLAB, ensuring that all required data files are available.



##### 2\. TSSCCA.m

Description: This is the core function of the project. It implements the Temporal-Spatial Sparse Canonical Correlation Analysis (TSSCCA) method, which models the relationship between genetic data and brain imaging features across multiple time points, while incorporating spatial and temporal consistency.



How to use: This function is called by the runTSSCCA.m script. Users should not need to run it directly unless debugging or modifying the model.



##### 3\. Simulated\_TSSCCA\_data.mat

Description: This file contains simulated data used for testing the TSSCCA model. It includes both genetic data and brain imaging features, designed to represent typical data that would be input into the model.



How to use: Load this file within MATLAB using the load command to explore the simulated dataset or use it for model testing.



##### 4\. getNormalization.m

Description: This function normalizes the data before applying the TSSCCA model. Data normalization is crucial for ensuring that all variables are on the same scale.



How to use: This function is automatically called by runTSSCCA.m as part of the preprocessing stage.



##### 5\. updateD.m, updateDs.m, updateDV\_FP.m

Description: These are utility functions used for updating specific parameters during the optimization process in TSSCCA. They handle the temporal and spatial updates within the model.



How to use: These functions are called within TSSCCA.m and should not require direct use unless modifying or debugging specific parts of the optimization process.



### How to Run the Code

Ensure that you have MATLAB installed.



Download the necessary files and place them in a directory.



Open MATLAB and navigate to the directory where the files are located.



Run the script runTSSCCA.m to start the model execution.



The results will be output based on the parameters set within runTSSCCA.m.
