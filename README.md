# Facial Emotion Detector

Real-time facial emotion detection from webcam using DeepFace and OpenCV.

## What it does
Analyzes a webcam feed frame by frame and detects the dominant emotion
(happy, sad, angry, neutral, surprise, fear, disgust) with a confidence
score, displayed live on screen.

## Tech Stack
- Python
- OpenCV — webcam capture and frame display
- DeepFace (VGG-Face) — pretrained CNN for face and emotion analysis

## How to run
pip install opencv-python deepface tf-keras
python app.py
Press q to quit.

## How it works
Each webcam frame is passed to DeepFace which runs a pretrained CNN
(VGG-Face) to detect faces and classify emotions. The model outputs
probability scores for 7 emotions based on Ekman's universal emotion
theory. Dominant emotion is overlaid on the live video feed.

## Next steps
- Add speech tone analysis for multimodal emotion detection
- Log emotions over time and plot a graph
- Extend to video file input for post-processed interview analysis
- Fine-tune model on interview-specific data
