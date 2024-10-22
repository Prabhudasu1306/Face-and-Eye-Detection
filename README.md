Real-Time Face and Eye Detection Web Application

AIM:
The aim of this project is to create a real-time face and eye detection web application using Flask, OpenCV, and Haarcascade classifiers. The application accesses the user's webcam, processes the video feed to detect faces and eyes, and displays the live video stream in a browser with rectangles drawn around detected facial features.

Tools and Technologies:
Flask:

A lightweight Python web framework used for creating the web interface and routing video feed to the browser.
Key functionalities:
1.Routes and views: Defines endpoints for the home page and streaming the video feed.
2.HTML rendering: Renders an HTML page to display the webcam feed.
3.Response object: Streams the video frames in real time using Response.

OpenCV:

An open-source library that processes images and video in real time.
Key OpenCV functions:
1.cv2.VideoCapture(): Captures live video from the webcam.
2.cv2.CascadeClassifier(): Loads pre-trained Haarcascade models to detect objects like faces and eyes.
3.cv2.rectangle(): Draws rectangles around detected faces and eyes.
4.cv2.imencode(): Encodes the video frame into JPEG format for the web application.
5.cv2.cvtColor(): Converts the video frame to grayscale, aiding the detection process.

Haarcascade Classifiers:

1.Pre-trained classifiers that use machine learning to detect objects (faces and eyes) in images.
Files used:
1.haarcascade_frontalface_default.xml: Detects faces.
2.haarcascade_eye.xml: Detects eyes.


Output:
This project outputs a live video stream displayed in a web browser where:

1.Faces are detected and highlighted with blue rectangles.

2.Eyes within the detected face region are highlighted with green rectangles.
