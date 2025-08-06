# PROJECT TITLE 
# Fault detection (pass/fail) using SECOM Manufacturing Test Dataset

## PROJECT SUMMARY
This project uses data from a semiconductor factory to automatically detect whether a product has passed or failed quality checks. Each product is tested using hundreds of sensors that measure different parts of the manufacturing process—like temperature, pressure, and timing. By analyzing these sensor readings with machine learning, the system learns to recognize patterns that lead to faulty products. This helps manufacturers catch problems early, avoid costly errors, and ensure only high-quality products are delivered. The goal is to improve efficiency and reduce waste by using data to support smarter decision-making in the production line.

## DATA
This project uses data from a semiconductor factory to automatically detect whether a product has passed or failed quality checks. Each product is tested using hundreds of sensors that measure different parts of the manufacturing process—like temperature, pressure, and timing. By analyzing these sensor readings with machine learning, the system learns to recognize patterns that lead to faulty products. This helps manufacturers catch problems early, avoid costly errors, and ensure only high-quality products are delivered. The goal is to improve efficiency and reduce waste by using data to support smarter decision-making in the production line.

## MODEL 
In this project, I experimented with several machine learning models, including Random Forest, Gradient Boosting, Logistic Regression, XGBoost, and LightGBM. Each model was trained and evaluated on the SECOM dataset to detect faulty products. After comparing their performance, LightGBM was selected as the final model due to its superior prediction accuracy and efficiency. LightGBM is a gradient boosting framework that is optimized for speed and performance, especially on large and high-dimensional datasets like SECOM. It handles missing values well, works efficiently with imbalanced data, and provides fast training and prediction times—making it ideal for real-world fault detection tasks.

## HYPERPARAMETER OPTIMSATION
To improve the performance of the machine learning models, I used GridSearchCV to perform hyperparameter tuning. This method systematically tests different combinations of parameters to find the best set for optimal model performance. For the final LightGBM model, I tuned key hyperparameters such as:
max_depth (limits the depth of each tree)
learning_rate (controls how much the model learns in each step)
n_estimators (number of boosting iterations)
GridSearchCV helped identify the best combination of these parameters based on cross-validation performance.

## RESULTS
The final LightGBM model accurately predicts whether a product from the semiconductor manufacturing line will pass or fail quality checks. This means that manufacturers can now detect faulty products early, potentially even before final testing. By identifying patterns linked to failure, the model helps engineers understand which process factors contribute most to defects. This enables faster decision-making, reduces waste, and lowers production costs. In business terms, the model supports quality assurance, process optimization, and improved operational efficiency, ultimately leading to better product reliability and customer satisfaction. 

## EMAIL
anvonet@gmail.com


