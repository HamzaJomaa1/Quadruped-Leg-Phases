Leg-Phase Detection for Quadruped Robots
This project focuses on detecting the contact phases of quadruped robot legs (ground contact vs. swing phase) using machine learning techniques. The goal is to improve the locomotion and stability of quadruped robots.

Overview
Quadruped robots excel in navigating challenging terrains where wheeled robots struggle. This project implements a Random Forest Classifier for detecting leg contact states, offering a reliable and efficient approach.

Key features of this project include:

Multi-output classification for detecting contact states of all four legs simultaneously.
Incorporation of torque sensor data to improve accuracy and robustness.
Evaluation of model performance with confusion matrices, accuracy scores, and classification reports.
How It Works
Data Collection: The dataset includes joint angle, torque, and multiple other sensor readings, along with labeled contact states (0 = no contact, 1 = in contact) for each leg.

Model: A Random Forest Classifier is wrapped in a multi-output framework to predict the contact states of all four legs simultaneously. This approach offers high accuracy, interpretability, and robustness to noise.

Results
The model demonstrates:

High accuracy: Consistently above 90% for all legs.
Robust predictions: Minimal misclassifications, as seen in the confusion matrices.
Real-time capability: Lightweight and efficient, suitable for live robotic control.
ML_project
This repository contains code for analyzing sensor data from the Unitree Go1 Dogrobot to classify the surface it walks on. The project uses machine learning techniques to process and analyze data obtained from various sensors available on the robot.

Dataset Overview
The data used in this project comes from the Unitree Go1 Dogrobot and includes:

Joint Angular Position Sensors: 12 sensors capturing the angles of the robot's joints.
Joint Torque Sensors: 12 sensors measuring torque applied to each joint.
Gyroscopes: 3 sensors providing rotational velocity data in three axes.
Accelerometers: 3 sensors capturing linear acceleration data in three axes.
The dataset combines these inputs to identify patterns associated with different surface types.

Code Description
Data Preprocessing:

Sensor data is read and normalized.
Features are extracted from angular positions, torque, gyroscope, and accelerometer data.
Model Training:

Supervised learning models are trained using labeled data of known surface types.
Features are mapped to surface categories.
we have used both LSTM and GRU (RNN models)
Evaluation:

Models are evaluated using metrics like accuracy, precision, recall, and F1 score.
Confusion matrices are used to analyze misclassifications.
Deployment:

The trained model is exported for deployment on the Unitree Go1 Dogrobot for real-time surface classification.
Requirements
Python 3.8 or higher
Libraries: numpy, pandas, scikit-learn
