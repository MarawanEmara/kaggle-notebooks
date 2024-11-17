# Titanic: Machine Learning from Disaster

## Overview

This solution uses a Random Forest classifier with extensive feature engineering to predict survival on the Titanic. The model achieved a score of 0.78947 on the public leaderboard.

## Feature Engineering

- **Name Processing**: Extracted titles and created name length features
- **Family Features**:
  - Combined SibSp and Parch into family size
  - Created IsAlone indicator
- **Numerical Binning**:
  - Age categories (Child, Teen, Adult, Middle, Senior)
  - Fare quartiles
- **Cabin Information**:
  - Extracted deck information from cabin numbers
  - Handled missing values
- **Ticket Analysis**:
  - Extracted ticket prefixes
  - Created numerical features from tickets
- **Interaction Features**:
  - Age \* Class interaction

## Model Details

- Algorithm: Random Forest Classifier
- Cross-validation strategy: 5-fold
- Feature importance analysis included
- Hyperparameter optimization via grid search

## Technical Implementation

- Robust preprocessing pipeline
- Missing value handling
- Label encoding for categorical variables
- Feature selection based on importance
