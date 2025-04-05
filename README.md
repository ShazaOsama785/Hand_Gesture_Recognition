# Hand_Gesture_Recognition
A machine learning project for real-time hand gesture classification using MediaPipe landmarks and a Support Vector Machine (SVM) model. Trained on the large-scale HaGRID dataset.

The input to this project is a CSV file containing hand landmark data (i.e., x, y, z coordinates of 21 hand keypoints) extracted using MediaPipe from real-time webcam frames or pre-recorded gesture datasets. 

The output is a trained machine learning model capable of classifying hand gestures into multiple predefined categories.

Each gesture is represented by a set of 21 3D landmarks detected per frame using MediaPipe’s Hands solution. These landmarks are then flattened and used as features to train a Support Vector Machine (SVM) classifier.

The CSV file contains normalized landmark coordinates along with their corresponding gesture labels. Feature scaling and preprocessing were performed before training the model.

This repository contains:

A Jupyter notebook (.ipynb) used for data preprocessing, model training, evaluation, and visualization.

The best trained model saved as a .pkl file (SVM) achieving high classification accuracy.

A Python script for real-time gesture recognition using webcam input and MediaPipe.

Sample input/output videos showing gesture detection in real time.

📁 Demo Videos:https://drive.google.com/file/d/1TvwJ-y95IXhKd_eYwMl5O5GhSbCD-mDj/view?usp=drive_link
