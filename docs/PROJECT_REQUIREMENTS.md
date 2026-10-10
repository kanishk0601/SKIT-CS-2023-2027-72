# Project Requirements

## Project Title
Real-Time Face Shape Detection Using Machine Learning

## 1. Problem Statement
Manual face-shape identification can be subjective and time-consuming.
This project aims to automate face-shape classification using facial
landmarks, geometric features, and machine learning.

## 2. Objectives
- Detect faces from webcam input or uploaded images.
- Extract facial landmarks using MediaPipe.
- Calculate facial features for classification.
- Classify faces as Oval, Round, Square, or Heart.
- Display predictions through a Flask web application.

## 3. Functional Requirements
- Capture webcam frames or accept uploaded images.
- Detect facial landmarks.
- Process landmarks into model-compatible features.
- Predict the face-shape category using a trained Random Forest model.
- Display the prediction and available visual annotations.

## 4. Non-Functional Requirements
- Provide a simple and understandable interface.
- Process input efficiently.
- Handle missing faces and invalid image inputs gracefully.
- Support local execution without relying on paid external APIs.
- Keep the application modular and maintainable.

## 5. Technology Stack
- Python
- Flask
- MediaPipe
- OpenCV
- NumPy
- Scikit-learn
- HTML, CSS, and JavaScript

## 6. Expected Outcomes
A functional web application that detects facial landmarks
and predicts one of four face-shape categories.

## 7. Team
- Kanishk Gupta — Team Lead
- Hardik — Team Member
