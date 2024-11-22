# Machine Failure Prediction using Decision Tree

This project uses a Decision Tree Classifier to predict machine failure based on sensor data. The model demonstrates the effectiveness of hyperparameter tuning in improving prediction accuracy.

## Project Overview
Predicting machine failure is critical for ensuring operational efficiency and minimizing downtime. In this project:
- A Decision Tree Classifier is trained on sensor data to classify whether a machine will fail.
- The baseline model achieves **0.81 accuracy** without hyperparameter tuning.
- Hyperparameter tuning using `GridSearchCV` boosts the accuracy to **0.89**.

## Dataset
The dataset consists of sensor readings collected from machines, with features including temperature, pressure, vibration, and more. The target variable is binary, indicating machine failure (`0` or `1`).

## Approach
1. **Data Preprocessing**:
   - Handled missing values and normalized sensor readings.
   - Split the dataset into training and testing sets.

2. **Model Training**:
   - **Baseline Model**: A simple Decision Tree Classifier trained without hyperparameter tuning.
   - **Tuned Model**: GridSearchCV is used to optimize hyperparameters (`max_depth`, `min_samples_split`, etc.).

3. **Evaluation**:
   - Metrics: Accuracy, precision, recall, and F1-score are used to assess performance.
   - The tuned model shows significant improvement in predictive performance.

## Results
| Model               | Accuracy |
|---------------------|----------|
| Baseline Decision Tree (No Tuning) | 0.81     |
| Tuned Decision Tree (GridSearchCV) | 0.89     |

## Dependencies
- Python 3.8+
- pandas
- scikit-learn
- matplotlib

## Conclusion
This project highlights the importance of hyperparameter tuning in improving machine learning model performance. The tuned Decision Tree demonstrates significantly better accuracy, making it a reliable choice for predicting machine failures based on sensor data.

---
