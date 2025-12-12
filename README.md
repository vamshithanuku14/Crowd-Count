# Crowd Counting using OpenCV and Dlib

This project detects and counts the number of faces in real-time using your computer's webcam. It leverages **Dlib's frontal face detector** along with **OpenCV** for image processing.

---

## Features

- Real-time face detection using a webcam.
- Counts the number of faces present in the frame.
- Draws bounding boxes around detected faces.
- Displays the face number for each detected face.
- Press `q` to quit the application.

---

## Requirements

- Python 3.x
- OpenCV
- Dlib
- NumPy

---

## Installation

1. Clone this repository:

```bash
git clone <repository-url>
cd <repository-folder>
```
2.Install the required packages:
```
pip install opencv-python dlib numpy
```
Usage:
1.Run the Python script:
```python crowd_count.py```
2.The webcam will open, and faces will be detected in real-time.
3.Each face will be highlighted with a green rectangle and labeled as face numX.
4.The total number of faces detected in each frame will be printed in the console.
5.Press q to quit the application.
How It Works
1.Capture Frames:
The program captures video frames from the webcam continuously using OpenCV.
2.Convert to Grayscale:
Each frame is converted to grayscale because Dlib's face detector works more efficiently with grayscale images.
3.Face Detection:
Dlib's get_frontal_face_detector is used to detect faces in the grayscale image.
4.Draw Bounding Boxes:
For each detected face, a green rectangle is drawn, and the face number is displayed.
5.Display and Count:
The frame with annotated faces is displayed in a window, and the number of detected faces is printed in the console.

**Notes
Ensure your webcam is working before running the script.
Detection may vary depending on lighting conditions and camera quality.
You can adjust the frame size and detection parameters for better accuracy.
