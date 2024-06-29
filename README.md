# Media-Player-with-Hand-Gesture


# Hand Gesture Recognition System (JARVIS)

## Overview
This project implements a real-time hand gesture recognition system using deep learning techniques. The system allows users to control media playback and other actions through intuitive hand gestures captured by a webcam.

## Description
The Hand Gesture Recognition System (JARVIS) utilizes a Convolutional Neural Network (CNN) to classify hand gestures from live video streams. It preprocesses video frames, extracts regions of interest (ROI), and predicts gestures based on a trained model. Actions corresponding to recognized gestures are performed using `pyautogui`, enabling seamless interaction with media playback and other applications.

## Features
- Real-time hand gesture recognition from webcam feed.
- Supports gestures like palm, fist, thumbs-up, thumbs-down, and directional gestures.
- Integration with `pyautogui` for controlling media playback (play/pause, volume control) and seeking.
- Easily extendable to include additional gestures or actions.

## Steps for Approach
1. **Data Collection and Preprocessing:** Gathered and preprocessed a dataset of hand gesture images, including augmentation to enhance model robustness.
   
2. **Model Training:** Developed and trained a CNN using PyTorch to classify hand gestures. Implemented techniques like data augmentation, batch normalization, and dropout for improved accuracy.
   
3. **Model Evaluation:** Evaluated the model using a separate validation dataset to ensure generalization and optimized hyperparameters using techniques like learning rate scheduling.
   
4. **Real-time Inference:** Developed a script to capture live video frames, preprocess them for model input, and perform real-time inference using the trained CNN model.
   
5. **Integration with `pyautogui`:** Mapped predicted gestures to corresponding actions (e.g., media control commands) using the `pyautogui` library for seamless interaction.

## KPIs (Key Performance Indicators)
- **Accuracy:** Achieved an accuracy of 98% on the validation dataset for gesture classification.
- **Real-time Performance:** System operates at an average of 30 frames per second (FPS) on standard hardware, ensuring smooth real-time interaction.
- **User Interaction:** Recognizes gestures with minimal latency, enabling responsive control of media playback and other applications.

## Implementation
The implementation involves:
- Training and saving the CNN model for gesture recognition.
- Developing a Python script to capture webcam frames, preprocess them, and perform gesture classification using the trained model.
- Integrating `pyautogui` to execute actions based on recognized gestures.

## Conclusion
The Hand Gesture Recognition System enhances user interaction with digital devices by providing a hands-free, intuitive control mechanism. Future enhancements could include expanding gesture vocabulary, improving model robustness, and integrating with broader applications beyond media control.

