# ASL Visualizer

## Overview

ASL Visualizer is a real-time Computer Vision and Machine Learning project that recognizes predefined American Sign Language (ASL) hand gestures using a webcam.

The system captures live video, detects the user's hand, processes the detected hand gesture, and uses a K-Nearest Neighbors (KNN) machine learning model to predict the corresponding ASL sign.

The project demonstrates the application of computer vision, hand tracking, image processing, and machine learning for real-time gesture recognition.

---

## Problem Statement

Communication can be difficult between people who use American Sign Language (ASL) and people who are not familiar with sign language.

The objective of this project is to develop a computer vision-based system that can recognize predefined ASL hand gestures from a webcam and display the predicted gesture in real time.

---

## Objectives

- Detect a hand from a live webcam feed.
- Track the detected hand using computer vision techniques.
- Process the detected hand gesture for classification.
- Recognize predefined ASL gestures using a KNN classifier.
- Display the predicted gesture in real time.

---

## Features

- Real-time webcam input
- Hand detection and tracking
- Hand gesture recognition
- KNN-based classification
- Real-time ASL prediction
- Visual display of the recognized gesture

---

## Technologies Used

- **Python**
- **OpenCV**
- **CVZone**
- **MediaPipe**
- **NumPy**
- **Scikit-learn**
- **Joblib**
- **K-Nearest Neighbors (KNN)**

---

## System Workflow

```text
Webcam Input
     ↓
Hand Detection
     ↓
Hand Tracking
     ↓
Gesture Processing
     ↓
KNN Classification
     ↓
ASL Prediction
     ↓
Display Result
```

---

## Project Structure

```text
ASL_visualiser/
│
├── hand_tracking.py
├── recognize_gesture.py
├── train.py
├── train_model.py
│
├── asl_knn_model.pkl
├── dataset/
│
├── requirements.txt
├── README.md
└── statement.md
```

> The exact file structure may vary depending on the files included in the submitted repository.

---

## Model

The project uses a **K-Nearest Neighbors (KNN)** classifier for gesture recognition.

The model is trained using the available ASL gesture dataset. During real-time operation, the detected hand gesture is processed and provided to the trained classifier, which predicts the corresponding ASL gesture.

### Why KNN?

KNN is a simple supervised machine learning algorithm that classifies an input based on the closest training samples. It is suitable for this project because the extracted gesture features can be compared with previously collected gesture samples.

---

## Installation

### 1. Clone the repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd ASL_visualiser
```

### 2. Install the required dependencies

```bash
pip install -r requirements.txt
```

---

## How to Run

Run the appropriate Python file used for real-time recognition:

```bash
python recognize_gesture.py
```

Allow the application to access your webcam and place your hand in front of the camera.

The system will detect the hand gesture and display the predicted ASL sign.

> If your current project uses a different file as the main entry point, replace the command above with the actual command used by your project.

---

## Dataset

The project uses a dataset containing images/samples of predefined ASL hand gestures.

The dataset is used during the training process to teach the KNN classifier how to distinguish between different hand gestures.

---

## Testing

The system can be tested by:

1. Starting the application.
2. Allowing webcam access.
3. Showing a supported ASL gesture to the camera.
4. Observing the predicted gesture displayed by the application.
5. Testing multiple supported gestures under different conditions.

Testing focuses on whether the system correctly detects the hand and recognizes the supported ASL gestures.

---

## Screenshots

Add screenshots of the working application below.

### Real-Time Gesture Recognition

![ASL Visualizer](screenshots/recognition.png)

### Gesture Prediction

![Gesture Prediction](screenshots/prediction.png)

> Replace the image paths above with the actual screenshots included in the repository.

---

## Limitations

- The system recognizes only the gestures included in the trained dataset.
- Recognition performance can be affected by lighting and background conditions.
- Hand positioning and camera quality can affect detection.
- The system is designed for predefined ASL gestures rather than complete sign-language sentences.

---

## Future Enhancements

Possible future improvements include:

- Supporting more ASL gestures.
- Improving recognition accuracy.
- Supporting continuous sign-language recognition.
- Adding sentence-level prediction.
- Improving robustness under different lighting and backgrounds.
- Developing a more comprehensive user interface.

---

## References

- OpenCV Documentation
- CVZone Documentation
- Scikit-learn Documentation
- MediaPipe Documentation

---

## Author

**Shivansh Sinha**

B.Tech Computer Science and Engineering  
Specialization: Artificial Intelligence and Machine Learning  
VIT Bhopal University
