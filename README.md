# Debris-Covered Glaciers Classification Project

## Overview

This research project focuses on applying supervised classification methods to distinguish between debris-covered glaciers and non-glaciated areas using remote sensing data. The project utilizes machine learning techniques to automate the identification of glaciers, which is crucial for monitoring climate change impacts and water resource management.

## Research Objectives

- Apply supervised classification methods to identify debris-covered glaciers
- Compare the performance of different machine learning models
- Address class imbalance issues in glacier identification
- Evaluate model accuracy using various metrics

## Dataset

The project uses GIS (Geographic Information System) data of glacier land and ice obtained from Kaggle, containing:

!(https://www.kaggle.com/datasets/dshassan/glacier-land-ice-gis-data)

- 23 features with numerical data
- Approximately 1 million instances
- Features include Land Surface Temperature (LST) and various band ratios
- Binary classification: debris-covered glaciers (1) vs. non-glaciated areas (0)

## Methods

### Data Preprocessing

- Handled missing values in LST using mean imputation
- Addressed class imbalance using SMOTE algorithm
- Split data into 80/20 training/testing sets

### Classification Models

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Random Forest Classifier
4. Gaussian Naive Bayes
5. Decision Tree Classifier

### Validation Methods

- Train-Test Split Evaluation (80/20)
- 5-Fold Cross-validation
- Performance metrics: Accuracy, Precision, Recall, F1-Score

## Results

The Decision Tree Classifier achieved the best performance with:

- Accuracy: 96.90%
- Precision: 95.23%
- Recall: 99.99%
- F1-Score: 97.44%

## Dependencies

- Python 3.x
- Required libraries:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn
  - imbalanced-learn (for SMOTE)

## Installation

```bash
# Create and activate virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # For Unix/macOS
venv\Scripts\activate     # For Windows

# Install required packages
pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn
```

## Usage

1. Clone the repository
2. Install dependencies
3. Run the Jupyter notebook `BigDataFinal.ipynb`
4. The notebook contains all analysis steps and model implementations
