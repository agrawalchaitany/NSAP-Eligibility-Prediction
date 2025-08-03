# NSAP Eligibility Prediction

## Overview
This project implements a machine learning solution to predict eligibility for the National Social Assistance Program (NSAP) in India. It uses demographic and socio-economic data to classify applicants into appropriate NSAP schemes, automating and improving the allocation process.

## Problem Statement
The National Social Assistance Program (NSAP) provides financial assistance to the elderly, widows, and persons with disabilities from below-poverty-line (BPL) households through various sub-schemes. Manual verification and scheme assignment is time-consuming and error-prone. This project creates a multi-class classification model to streamline this process, ensuring timely and accurate benefit delivery.

## Dataset
The project uses the district-wise pension data under NSAP available in:

- `nsapallschemes.csv`

## Technology Stack
- **IBM Watson Studio/Cloud Pak for Data**: Primary platform for model development
- **Watson Machine Learning (WML)**: For model deployment and serving
- **AutoML**: Used for automated model selection and optimization
- **Python**: Core programming language
- **Jupyter Notebooks**: For exploratory data analysis and model development

## Project Structure

```
NSAP-Eligibility-Prediction/
├── assettypes/
│   ├── auto_ml.json                # AutoML configuration
│   └── wx_prompt.json              # Watson prompt configuration
├── assets/
│   ├── .METADATA/                  # Project metadata
│   ├── data_asset/
│   │   └── nsapallschemes.csv      # NSAP dataset
│   ├── environment/                # Python environment definitions
│   ├── notebook/                   # Jupyter notebooks for analysis
│   └── wml_model/                  # Watson Machine Learning models
└── README.md                       # This file
```

## Implementation Details

The project follows these main steps:

1. **Data Preparation**: Loading and preprocessing the NSAP dataset
2. **Exploratory Data Analysis**: Understanding data distributions and relationships
3. **Feature Engineering**: Creating relevant features for better prediction
4. **Model Training**: Using IBM AutoML to select and optimize classification models
5. **Model Evaluation**: Assessing model performance with appropriate metrics
6. **Deployment**: Deploying the best model to IBM Cloud for inference

## Setup and Usage

### IBM Cloud Account Setup
- Create an IBM Cloud account or use existing credentials
- Set up Watson Studio/Cloud Pak for Data service

### Project Setup
- Clone this repository
- Import the project into Watson Studio or run locally

### Running the Project
- Execute notebooks in the recommended order
- Follow documentation within each notebook for specific instructions

## Model Deployment

The trained model is deployed using Watson Machine Learning, allowing for:

- Real-time predictions via API
- Batch scoring for large applicant datasets
- Integration with government systems

## Results

The model achieves **[metrics to be added after evaluation]** in predicting the appropriate NSAP scheme for applicants, potentially improving the efficiency and accuracy of benefit allocation.

