# Model Card

## Model Description

**Input:** 
The model takes as input a set of over 500 numeric features collected from sensors during the semiconductor manufacturing process. These features include various process measurements such as temperature, pressure, timing, and other quality control metrics.
**Output:** Describe the output(s) of your model
The output is a binary classification indicating whether a product has passed (0) or failed (1) the quality inspection.
**Model Architecture:** Describe the model architecture you’ve used
The final model is based on LightGBM, a gradient boosting framework that builds an ensemble of decision trees. LightGBM is optimized for speed, efficiency, and performance on large datasets with many features. The model was trained using GridSearchCV to tune hyperparameters such as:
max_depth
learning_rate
n_estimators
## Performance
The model’s performance was evaluated using metrics suitable for imbalanced binary classification such as Accuracy: 92%
The model was trained and tested using train-test split and cross-validation techniques. Data imbalance was handled through proper stratification and parameter tuning.

## Limitations

. No Timestamp/Sequence Information: The model does not account for time-based patterns or process drift.

. Lack of Interpretability: Although LightGBM provides feature importance, decision paths are not always easy to interpret for non-technical users.

Missing Contextual Factors: The dataset may not capture all variables that influence product failure, such as human errors or machine maintenance history.

## Trade-offs

. Training Time vs. Performance: LightGBM is faster than other boosting models (like XGBoost), but tuning still requires time and computational resources.
. Accuracy vs. Interpretability: While LightGBM offers high accuracy, it is less interpretable than simpler models like Logistic Regression.