
# Alphabet Soup Neural Network Model Project

This project focuses on developing a deep learning model to predict the success of funding applications for Alphabet Soup. By analyzing the organization’s structured data, we aim to improve classification accuracy in predicting which applications are more likely to succeed.

## Project Overview

This project includes the following key steps:

1. **Data Import and Preprocessing**:
   - Imported `charity_data.csv` and examined the structure.
   - Removed non-beneficial columns (`EIN` and `NAME`) to simplify data.
   - Replaced infrequent values in categorical features (`APPLICATION_TYPE` and `CLASSIFICATION`) with "Other" to improve model generalization.
   - Converted categorical variables to numeric using one-hot encoding.

2. **Feature Selection**:
   - Applied feature importance analysis using a Random Forest model to identify and drop low-importance features.
   - Selected features included categorical variables like `APPLICATION_TYPE`, `AFFILIATION`, and `CLASSIFICATION`, and numeric columns such as `ASK_AMT`.

3. **Data Splitting and Scaling**:
   - Split the dataset into training and testing sets.
   - Scaled features using `StandardScaler` to normalize the input data.

4. **Neural Network Model Development**:
   - Developed multiple architectures for a deep learning model using Keras with TensorFlow.
   - Configurations ranged from simple to complex models, with layers, dropout, batch normalization, and L2 regularization.
   - Compiled each model with binary cross-entropy loss, using the Adam optimizer and tracking accuracy.

5. **Model Evaluation and Optimization**:
   - Initial models achieved an accuracy of approximately 73%.
   - Further optimizations included adjusting learning rates, class weights, and applying early stopping.
   - The final model achieved an accuracy of 72.73%, balanced with minimal overfitting.

6. **Alternative Model Exploration**:
   - Considered alternative models like Random Forests or Gradient Boosted Trees, which may capture non-linear relationships and offer higher interpretability.

## Report Summary

The final model achieved satisfactory performance with an accuracy of 72.73%, balancing model complexity and interpretability. Future recommendations include exploring alternative machine learning models, such as tree-based algorithms, which may provide better insights and handle categorical features more effectively.

For a detailed breakdown of the analysis, please refer to the [report file](Alphabet_Soup_Neural_Network_Report.md).

## Files in Repository

- **README.md**: This file, providing an overview of the project and instructions.
- **Alphabet_Soup_Neural_Network_Report.md**: Detailed report on data processing, model development, and evaluation.
- **charity_data.csv**: Input data file for training and evaluating the neural network model.

## Requirements

To run this project, ensure you have the following libraries installed:

- `pandas`
- `scikit-learn`
- `tensorflow`

## Running the Model

1. Clone the repository and navigate to the project directory.
2. Run the data preprocessing, model training, and evaluation scripts as detailed in the Jupyter notebook or Python files provided.
3. Review model performance metrics and adjust configurations if necessary.

---
This notebook, report and README, were enhanced with the assistance of CHATGPT  
For further information on the analysis, model configurations, and performance optimization, refer to the [Alphabet Soup Neural Network Report](Alphabet_Soup_Neural_Network_Report.md).
