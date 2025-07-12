This project implements a modular simulation pipeline to predict NCAA tournament outcomes using historical data and machine learning. The workflow was built in Python with Jupyter Notebooks and follows these key steps:

1. *Data Ingestion*: Loads and organizes historical data from Kaggle.

2. *Feature Engineering*: Constructs predictive features, including team statistics and seed differences.

3. *Model Training*: Trains an XGBoost model using a leave-one-season-out cross-validation strategy to prevent overfitting and simulate real prediction scenarios.

4. *Prediction & Calibration*: Predicts point differences and maps them to win probabilities using a spline-based calibration.

5. *Output Writer*: Formats predictions to match Kaggle’s submission requirements, with support for expert overrides.

Four simulations were tested using different combinations of variables. The best results were achieved when both team statistics and seed information were used, confirming their combined predictive power.
