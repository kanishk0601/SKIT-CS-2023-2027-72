# Random Forest Model Training

## 1. Overview
The project uses a Random Forest Classifier to classify human face shapes into four categories: Heart, Oval, Round and Square.

## 2. Dataset
The notebook uses two separate dataset directories:

- Training: `Face_Shape/training2`
- Testing: `Face_Shape/testing2`

Both datasets are processed using the `process_data()` function to prepare features and labels.

## 3. Feature Extraction
Facial features are extracted using MediaPipe Face Landmarker. The extracted landmark coordinates are used to calculate distances between important facial points.

These numerical features are used as input for the classification model.

## 4. Model Configuration
The model is implemented using Scikit-learn's `RandomForestClassifier`.

Configuration:
- Algorithm: Random Forest
- Number of estimators: 1500
- Random state: 20

## 5. Model Training
The processed training features and labels are passed to the classifier using:

`rf_model.fit(X_train, y_train)`

## 6. Model Evaluation
The trained model predicts labels for the testing dataset using:

`rf_model.predict(X_test)`

The notebook evaluates performance using:
- Accuracy Score
- Classification Report

## 7. Model Saving
The trained classifier is saved using Python's Pickle library.

Model filename: `Best_RandomForest.pkl`

This saved model is loaded by the Flask application to predict face shapes.

## 8. Supported Classes
- Heart
- Oval
- Round
- Square
