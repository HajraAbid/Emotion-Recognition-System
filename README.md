# Emotion Recognition System

This **Emotion Recognition System** uses a pre-trained deep learning model to identify facial expressions from real-time webcam feed. It leverages OpenCV for face detection and Keras for emotion classification.

## Features:
- **Real-time Emotion Detection**: Identifies emotions such as Angry, Disgust, Fear, Happy, Neutral, Sad, and Surprise from the webcam feed.
- **Face Detection**: Detects faces using Haar Cascade Classifier.
- **Emotion Display**: Displays the predicted emotion label above the detected face in the webcam feed.

## Requirements:
- Python 3.x
- OpenCV (`cv2`)
- Numpy
- Keras (with TensorFlow backend)

## Installation:

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/your-username/emotion-recognition-system.git
Install the required Python libraries:

pip install opencv-python numpy tensorflow keras
Download the pre-trained model file (model_file_30epochs.h5) and Haar Cascade file (haarcascade_frontalface_default.xml) and place them in the appropriate paths in the code.

Usage:
Run the script to start the emotion recognition system:

python emotion_recognition.py
The system will use your webcam to capture video and detect faces in real-time. Once a face is detected, the system will predict the emotion of the person and display it above the face.

The following emotions will be recognized:

Angry

Disgust

Fear

Happy

Neutral

Sad

Surprise

Press the q key to exit the system.

Code Overview:
Face Detection: Uses OpenCV's CascadeClassifier to detect faces in real-time.

Emotion Recognition: Processes the face region, normalizes it, and passes it through a pre-trained Keras model for emotion classification.

Result Display: Predicted emotion is displayed on the video feed along with a bounding box around the detected face.

License:
This project is licensed under the MIT License. See the LICENSE file for more details.
