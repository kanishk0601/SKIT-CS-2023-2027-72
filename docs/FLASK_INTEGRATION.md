
# Flask Application Integration

## Overview
The project uses Flask to connect the face-shape detection model to the web interface. It handles image uploads, real-time webcam streaming, and displaying prediction results.

## Image Upload
The upload functionality:
1. Accepts an image from the user.
2. Converts the image into RGB format.
3. Detects facial landmarks using MediaPipe.
4. Extracts facial features.
5. Predicts the face shape using the trained Random Forest model.
6. Draws facial landmarks and prediction text on the image.
7. Saves the annotated image and displays the result.

## Application Routes

| Route | Function |
|---|---|
| `/uploads/<filename>` | Serves uploaded and annotated images |
| `/video_feed` | Streams webcam frames |
| `/real_time` | Displays the real-time detection interface |

## Technologies Used
- Flask
- Python
- OpenCV
- MediaPipe
- NumPy
- Scikit-learn
- HTML, CSS, and JavaScript

## Integration Outcome
The Flask backend connects the trained machine learning model with the frontend, enabling users to upload images and perform real-time face shape detection.
