#Leg-Phase Detection for Quadruped Robots
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
