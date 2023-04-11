# Face-detection-on-Raspberry-pi

Here's a basic face detection project using a Raspberry Pi and OpenCV library. This project will detect faces using the Pi Camera module and draw a rectangle around them.

First, make sure your Raspberry Pi is updated and has OpenCV installed:

1) sudo apt-get update
2) sudo apt-get upgrade
3) sudo apt-get install python-opencv

Then, face_detection.py loads the face detection cascade classifier, initializes the Pi Camera module, and captures frames from the camera in a loop. It then converts each frame to grayscale and applies the face detection algorithm using OpenCV's detectMultiScale() function. Finally, it draws a green rectangle around each detected face and displays the resulting frame.

Note: You need to download the "haarcascade_frontalface_default.xml" file which contains the pre-trained data for face detection from this link: https://github.com/opencv/opencv/blob/master/data/haarcascades/haarcascade_frontalface_default.xml

To run the code, save it to your Raspberry Pi and execute it using the following command:

python3 face_detection.py

This should open a window with the live camera feed and rectangles around any detected faces. You can stop the program by pressing the 'Esc' key.
