# Alphabet Soup Funding Success Predictor

## Project Overview
This project aims to develop a binary classifier that predicts the likelihood of applicants achieving success if they receive funding from Alphabet Soup. The objective is to optimize the model to achieve an accuracy score surpassing 75%.

## Data Preprocessing
The target variable is `IS_SUCCESSFUL`, indicating whether the applicant succeeded after receiving funding. Key steps in data preprocessing included:

- **Feature Selection**: Removed irrelevant columns such as `EIN` and `names`.
- **Binning/Bucketing**: Applied to rare occurrences in the `APPLICATION_TYPE` and `CLASSIFICATION` columns.
- **Encoding**: Transformed categorical data into numeric data using one-hot encoding.
- **Splitting Data**: Divided data into training and testing sets.
- **Scaling**: Ensured uniform data distribution through scaling.

## Model Training and Evaluation
### Initial Model
- **Architecture**: Three layers - input layer (80 neurons), hidden layer (30 neurons), output layer (1 neuron).
- **Activation Functions**: `relu` for input and hidden layers, `sigmoid` for output layer.
- **Training**: 100 epochs, achieving ~74% accuracy on training data and 72.8% on testing data.

### Optimization Attempts
1. **Optimizated Attempt**:
   - **Changes**: Added 2 dropout layers (rate of 0.56) and used `tanh` activation functions.
   - **Results**: 72.86% accuracy on training data and 72.85% on testing data.


## Summary
Despite several optimization attempts, the target accuracy of 75% was not achieved. Thus, the current models are not recommended for deployment. Future work should explore alternative models like the Random Forest Classifier and make further adjustments to preprocessing and model architecture.

## Tools Used
This machine learning task was completed using Visual Studio Code (VS Code) as the integrated development environment (IDE).

---

Created by Alan Lawrence  
Date: June 8, 2024
