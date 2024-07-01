# Media Player using Hand Gesture


## Overview
This project implements a real-time hand gesture recognition system using deep learning techniques. The system allows users to control media playback and other actions through intuitive hand gestures captured by a webcam.

## Description
The Hand Gesture Recognition System utilizes a Convolutional Neural Network (CNN) to classify hand gestures from live video streams. It preprocesses video frames, extracts regions of interest (ROI), and predicts gestures based on a trained model. Actions corresponding to recognized gestures are performed using `pyautogui`, enabling seamless interaction with media playback and other applications.

## Features
- Real-time hand gesture recognition from webcam feed.
- Supports gestures like palm, fist, thumbs-up, thumbs-down, and directional gestures (index pointing left/right).
- Integration with `pyautogui` for controlling media playback (play/pause, volume control) and seeking.
- Easily extendable to include additional gestures or actions.

## Steps for Approach
1. **Data Collection and Preprocessing:** Gathered and preprocessed a dataset of hand gesture images, including augmentation to enhance model robustness.
   
2. **Model Architecture:** Designed a CNN architecture consisting of 4 convolutional layers followed by fully connected layers for gesture classification. Used ReLU activations, dropout for regularization, and batch normalization to improve training stability.

3. **Training Details:**
   - **Loss Function:** Cross-entropy loss function used for multi-class classification.
   - **Optimizer:** Adam optimizer with an initial learning rate of 0.001, adjusted dynamically using learning rate scheduling (`StepLR`) to optimize convergence.
   - **Early Stopping:** Implemented early stopping based on validation accuracy to prevent overfitting and improve generalization.

4. **Model Evaluation:** Evaluated the model using a separate validation dataset to ensure generalization and optimized hyperparameters using techniques like learning rate scheduling.
   
5. **Real-time Inference:** Developed a script to capture live video frames, preprocess them for model input, and perform real-time inference using the trained CNN model.
   
6. **Integration with `pyautogui`:** Mapped predicted gestures to corresponding actions (e.g., media control commands) using the `pyautogui` library for seamless interaction.

## KPIs (Key Performance Indicators)
- **Accuracy:** Achieved an accuracy of 98% on the validation dataset for gesture classification.
- **Real-time Performance:** System operates at an average of 30 frames per second (FPS) on standard hardware, ensuring smooth real-time interaction.
- **User Interaction:** Recognizes gestures with minimal latency, enabling responsive control of media playback and other applications.

## Implementation
The implementation involves:
- Training and saving the CNN model for gesture recognition.
- Developing a Python script to capture webcam frames, preprocess them, and perform gesture classification using the trained model.
- Integrating `pyautogui` to execute actions based on recognized gestures.

## Photos: 
**Code Snapshot:**
![Code Snapshot](https://github.com/jainam0037/Media-Player-with-Hand-Gesture/blob/main/code%20.png)

**Move Backwards:**
![Move Backwards](https://github.com/jainam0037/Media-Player-with-Hand-Gesture/blob/main/move%20backwards.png)


**Move Forward:**
![Move Forward](https://github.com/jainam0037/Media-Player-with-Hand-Gesture/blob/main/move%20forward.png)


**Volume Down:**
![Volume Down](https://github.com/jainam0037/Media-Player-with-Hand-Gesture/blob/main/volume%20down.png)


**Volume Up:**
![Volume Up](https://github.com/jainam0037/Media-Player-with-Hand-Gesture/blob/main/volume%20up.png)




## Conclusion
The Hand Gesture Recognition System enhances user interaction with digital devices by providing a hands-free, intuitive control mechanism. Future enhancements could include expanding gesture vocabulary, improving model robustness, and integrating with broader applications beyond media control.
