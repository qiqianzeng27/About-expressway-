# About-expressway-
Short-Term Expressway Traffic Flow Prediction
📋 Project Overview
This research project develops and evaluates a comprehensive data-driven framework for short-term traffic flow prediction on expressways by integrating multi-source heterogeneous data. The study addresses the critical challenge of accurate traffic forecasting, which is essential for intelligent transportation systems, congestion management, and travel safety enhancement.

🎯 Key Objectives
1.Develop an integrated prediction framework combining traffic monitoring and meteorological data
2.Systematically compare eight machine learning algorithms across multiple performance dimensions
3.Identify optimal models for short-term (1-hour ahead) traffic flow prediction
4.Provide empirical evidence and practical guidance for traffic management applications

📊 Dataset Description
Source: Qinbin Expressway, October 2025
Sample Size: 372 hourly observations
Original Variables: 17 raw variables categorized into:
Temporal Features: Timestamps, hour indicators, holiday/weekend flags
Traffic Metrics: Directional flows (north-to-south, south-to-north) and cumulative totals
Meteorological Data: Temperature, weather conditions, precipitation, wind speed from northern and southern stations

Feature Engineering: Expanded to 53 predictive features including:
Multiple lagged traffic variables (1-12 hours)
Rolling statistical measures (means, standard deviations over 6, 12, 24-hour windows)
Cyclically encoded time variables (hour_sin, hour_cos, weekday_sin, weekday_cos)
Cross-domain interaction terms
Spatial difference features between monitoring stations

🧠 Models Evaluated
Eight representative data mining algorithms were systematically compared:
a.Linear Models：Linear Regression, Ridge Regression, Lasso Regression
b.Tree-Based：Decision Tree
c.Ensemble Methods：Random Forest, Gradient Boosting
d.Other Methods：Support Vector Regression (SVR), K-Nearest Neighbors (KNN)	Kernel-based and instance-based learning

📈 Evaluation Framework
A multi-dimensional evaluation approach was implemented:

Accuracy Metrics:
R² Score: Coefficient of determination
MAE: Mean Absolute Error (vehicles)
RMSE: Root Mean Square Error (vehicles)
MAPE: Mean Absolute Percentage Error (%)

Operational Metrics:
Training Time: Computational efficiency
Overfitting Degree: Difference between training and test R²
Model Stability: Consistency across different data splits
