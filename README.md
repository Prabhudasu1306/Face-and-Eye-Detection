AIM:
The aim of this project is to create a real-time face and eye detection web application using Flask, OpenCV, and Haarcascade classifiers. The application accesses the user's webcam, 
processes the video feed to detect faces and eyes, and displays the live video stream in a browser with rectangles drawn around detected facial features.

Tools and Technologies:
Flask:

Flask is a lightweight Python web framework that is used to create the web interface for this project. Flask handles the routing and serves the video feed to the browser.
Flask provides the following key functionalities:
Routes and views: It defines the endpoints for displaying the home page and streaming the video feed.
HTML rendering: Flask renders an HTML page that serves as the user interface (UI) to display the webcam feed.
Response object: It streams video frames in real time using Response.
OpenCV:

OpenCV (Open Source Computer Vision Library) is a powerful computer vision library that provides tools to process images and video in real time.
Key functions in OpenCV:
cv2.VideoCapture(): Captures live video from the webcam.
cv2.CascadeClassifier(): Loads the pre-trained Haarcascade models to detect objects (like faces and eyes) in video frames.
cv2.rectangle(): Draws rectangles around detected faces and eyes.
cv2.imencode(): Encodes the video frame as a JPEG image to be served via the web application.
cv2.cvtColor(): Converts the video frame to grayscale to help in the detection process (as Haarcascade classifiers work better on grayscale images).
Haarcascade Classifiers:

Haarcascade classifiers are machine learning-based classifiers used to detect objects in images, like faces and eyes. These classifiers are pre-trained on large datasets of images.
Files used:
haarcascade_frontalface_default.xml: Detects faces.
haarcascade_eye.xml: Detects eyes.
