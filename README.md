Hand Tracking and Volume/Brightness Control System

Overview

This project is a hand tracking and volume/brightness control system using OpenCV, MediaPipe, and PyCAW. It allows users to control their system's volume and brightness using hand gestures.

Features

Hand tracking using MediaPipe's Hand Landmark Model
Volume control using PyCAW
Brightness control using screen_brightness_control library
Real-time hand gesture recognition
Volume and brightness bars displayed on the video stream
How it Works

The system captures video from the default camera using OpenCV.
MediaPipe's Hand Landmark Model is used to detect and track hand landmarks in the video stream.
The hand landmarks are drawn on the video stream using MediaPipe's drawing utilities.
The system recognizes hand gestures by tracking the distance between the thumb and index finger.
The volume and brightness are controlled based on the distance between the thumb and index finger.
The volume and brightness bars are displayed on the video stream, and updated in real-time based on the current volume and brightness levels.
Code Structure

The code is divided into two main parts:

Volume Control: This part of the code uses PyCAW to control the system's volume. It gets the current speaker device, activates the IAudioEndpointVolume interface, and controls the volume based on the hand gesture.
Brightness Control: This part of the code uses the screen_brightness_control library to control the system's brightness. It creates a trackbar for brightness control, and sets the brightness based on the hand gesture.
Requirements

OpenCV
MediaPipe
PyCAW
screen_brightness_control library
Python 3.x
Usage

Run the code using Python 3.x.
The system will capture video from the default camera and display it on the screen.
Move your hand in front of the camera to control the volume and brightness.
Press the 'q' key to exit the program.
