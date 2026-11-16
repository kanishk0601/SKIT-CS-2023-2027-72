# Face Detection and Landmark Extraction

## 1. Overview
The project uses MediaPipe Face Landmarker to detect facial landmarks from input images and webcam frames.

## 2. Technology Used
- MediaPipe Tasks
- OpenCV
- NumPy
- Python

## 3. Detection Process
1. Capture an image or webcam frame using OpenCV.
2. Convert the frame from BGR to RGB.
3. Create a MediaPipe image object.
4. Pass the image to the Face Landmarker.
5. Extract facial landmarks from the detection result.
6. Use the landmarks to calculate facial features.
7. Draw facial landmarks on the processed image.

## 4. Feature Extraction
The application uses selected facial landmarks to calculate distances:

- Forehead to chin (face height)
- Left cheek to right cheek (face width)
- Left eye to right eye (eye distance)
- Nose tip to left eye
- Nose tip to right eye
- Chin to left cheek
- Chin to right cheek
- Forehead to both eyes

These measurements are passed to the trained Random Forest model for face shape classification.

## 5. Supported Face Shapes
- Heart
- Oval
- Round
- Square

## 6. Model Integration
The extracted facial features are supplied to the pre-trained Random Forest classifier stored in `Best_RandomForest.pkl`.

The predicted class is displayed on the processed image.

## 7. Output
The application displays the detected face landmarks and predicted face shape for supported input images and webcam frames.
