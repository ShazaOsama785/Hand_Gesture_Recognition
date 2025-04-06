# Hand Gesture Classification Using MediaPipe Landmarks
A machine learning project for real-time hand gesture classification using MediaPipe landmarks and a Support Vector Machine (SVM) model. Trained on the large-scale HaGRID dataset, this system recognizes static gestures in live webcam footage.

# 🎯Overview
This project implements a hand gesture classification system that:
- Uses MediaPipe to extract 21 hand landmarks.
- Preprocesses those landmarks into features.
- Trains a Support Vector Machine (SVM) classifier.
- Performs real-time predictions using webcam input.
  
# 📚 Dataset – HaGRID
-Classes: 18 gesture types (e.g., ✌️ Peace, 👍 Like, 🛑 Stop, 🤟 Call Me, 👎 Dislike).
-Size: Over 500,000 annotated images.
-Usage: Filtered and preprocessed for static gesture recognition using extracted landmarks.

# Input & Output
Input: A CSV file containing hand landmark data — specifically the x, y, z coordinates of 21 keypoints, extracted from webcam frames or pre-recorded gesture datasets using MediaPipe.

Output: A trained SVM model capable of classifying hand gestures into multiple predefined categories with high accuracy.

# Method
# -Landmark Extraction
Uses MediaPipe Hands to detect 21 landmarks per hand.

# -Feature Engineering
Flattens and normalizes (x, y, z) coordinates into a fixed-length feature vector.

# Model Training
Trains a Support Vector Machine using scikit-learn on the extracted features.

# Real-Time Inference
Uses OpenCV to access webcam input and display gesture predictions live.

# 📁 Demo Videos 
https://drive.google.com/file/d/1TvwJ-y95IXhKd_eYwMl5O5GhSbCD-mDj/view?usp=drive_link
