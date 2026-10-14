# Predictive Maintenance of Industrial Machines Using Machine Learning

## Project Overview
This project uses machine learning to predict the Remaining Useful Life (RUL) of industrial machines and classify whether a machine may experience failure within 24 hours.

## Objectives
- Predict the remaining useful life of a machine in hours.
- Classify machines based on the possibility of failure within 24 hours.
- Compare the performance of different machine learning models.
- Visualize model evaluation results.

## Dataset
The dataset contains machine sensor readings, including vibration, motor temperature, current, pressure, RPM, and operating conditions. It includes the target columns `rul_hours` and `failure_within_24h`.

The dataset CSV is not included in this repository. Provide the dataset before running the notebook.

## Machine Learning Models

### Regression
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

### Classification
- Decision Tree Classifier

## Evaluation Metrics

**Regression:** Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² Score.

**Classification:** Accuracy, Precision, Recall, F1 Score, and Confusion Matrix.

## Project Workflow
1. Load and inspect the dataset.
2. Handle missing sensor readings.
3. Extract time-based features.
4. Split data into training and testing sets.
5. Train regression and classification models.
6. Evaluate model performance.
7. Generate comparison graphs and predictions.

## Model Reproduction
The Random Forest model is trained directly in the Jupyter notebook. Its trained model file is not included in this repository because of its large size. Run the notebook with the required dataset to train the model and reproduce the evaluation results.

## Project Files
- `predictive_maintenance.ipynb` — implementation and model training
- `model_evaluation_results.csv` — regression evaluation results
- `classification_evaluation_results.csv` — classification evaluation results
- `mae_comparison.png` — MAE comparison
- `model_metrics_comparison.png` — RMSE and R² comparison
- `actual_vs_predicted.png` — predicted versus actual RUL
- `confusion_matrix.png` — classification evaluation
- `classification_feature_importance.png` — feature importance
- `requirements.txt` — Python dependencies

## Installation
Install the required libraries:

`pip install -r requirements.txt`

## Conclusion
The project compares regression models for remaining useful life prediction and uses a classification model to predict failure within 24 hours. The evaluation metrics and visualizations help assess their performance.
