# Real-Time Face Shape Detection Using Machine Learning

A Flask-based computer vision application that detects facial landmarks and classifies face shapes as **Oval, Round, Square, or Heart**. The project combines MediaPipe, OpenCV, and a trained Random Forest model to provide face-shape predictions through a web interface.

## Project Overview

The application supports webcam-based face detection and image upload. MediaPipe extracts facial landmarks, OpenCV handles image/frame processing and annotation, and the trained Random Forest classifier predicts the face-shape category from the features used during training. Flask connects the processing pipeline to the web interface.

## Features

- Real-time face detection through a webcam.
- Image upload and processing.
- Facial landmark detection using MediaPipe.
- Face-shape classification using a pre-trained Random Forest model.
- Annotated output for visualizing detected facial information.
- Flask-based web interface.
- Four supported categories: Oval, Round, Square, and Heart.

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Main application and machine-learning language |
| Flask | Web application and backend routing |
| MediaPipe | Facial landmark detection |
| OpenCV | Image and webcam-frame processing |
| NumPy | Numerical operations and feature calculations |
| scikit-learn | Random Forest model and machine-learning utilities |
| Joblib / Pickle model file | Loading the saved classifier, depending on the implementation |
| HTML, CSS, JavaScript | Web interface and browser interactions |

## Repository Structure

The exact contents may vary as the project is organized into sprint-based commits.

```text
.
├── app.py
├── Best_RandomForest.pkl
├── Best_Train-Model_RandomForest.ipynb
├── face_landmarker_v2_with_blendshapes.task
├── Face_Shape/
├── Images/
├── assets/
├── static/
├── templates/
├── uploads/
├── requirements.txt
└── README.md
```

## Getting Started

### Prerequisites

- Python installed on your computer.
- A webcam for real-time detection (optional if using image upload).
- Git, if cloning the repository.

### 1. Clone the repository

```bash
git clone https://github.com/kanishk0601/SKIT-CS-2023-2027-72.git
cd SKIT-CS-2023-2027-72
```

### 2. Create and activate a virtual environment

**Windows (Command Prompt):**

```cmd
python -m venv .venv
.venv\Scripts\activate
```

**macOS / Linux:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Run the application

Once the application files and required model assets have been uploaded, run:

```bash
python app.py
```

Open the local address printed by Flask in your browser. The existing project documentation uses `http://127.0.0.1:5000/` as the local address.

## Model and Data

- **Classifier:** `Best_RandomForest.pkl` — the saved Random Forest model used for face-shape prediction.
- **Landmarker asset:** `face_landmarker_v2_with_blendshapes.task` — the MediaPipe task asset used for facial landmark detection.
- **Training notebook:** `Best_Train-Model_RandomForest.ipynb` — notebook for dataset processing, feature extraction, model training, and saving the trained classifier.
- **Dataset:** `Face_Shape/` — the project folder identified in the existing documentation as containing face-shape images. Confirm that the dataset may be redistributed before publishing it publicly.

The model expects features prepared in the same way as during training. If the feature-extraction logic changes, retrain or validate the classifier before using it.

## Team

- **Kanishk Gupta** — Team Lead
- **Hardik** — Team Member

## Development Plan

The project is being organized into the following sprint areas:

1. **Planning** — requirements, dataset review, and project structure.
2. **Detection** — face detection and landmark extraction.
3. **Training** — geometric feature engineering and Random Forest classification.
4. **Integration** — Flask backend and web interface.
5. **Testing** — prediction checks, annotations, and evaluation.
6. **Deployment** — optimization and documentation.

## Limitations and Notes

- Prediction quality depends on the training data, landmark visibility, lighting, camera quality, and the feature-extraction method.
- This project provides an estimated face-shape category; it is not a medical or identity-verification system.
- Webcam access requires browser/device permissions and a compatible camera.
- Confirm all model assets, dataset permissions, dependency versions, and runtime instructions before making a public release.