# Hand Gesture Volume Control 

![Hand Gesture Volume Control Example]

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [How It Works](#how-it-works)

## Introduction

Hand Gesture Volume Control is a Computer Vision project that allows you to control the system's audio volume using hand gestures detected from a webcam input. The project uses the [Mediapipe Hands]solution to detect hand landmarks in real-time and calculates the distance between the thumb and index finger tips. This distance is then mapped to the system's volume range to control the volume level based on specific hand gestures.

## Features

- Real-time hand gesture recognition for volume control
- Webcam feed with hand landmarks and volume control bar display
- Audio volume control using hand gestures
- Hand gesture feedback on successful volume control

## Requirements

To run this project, you need the following dependencies:

- Python (>= 3.6)
- OpenCV (cv2)
- Mediapipe
- NumPy
- Pycaw

## How It Works

The project uses the Mediapipe Hands solution to detect hand landmarks in the webcam feed. The distance between the thumb and index finger tips is calculated using the `math.hypot()` function. The calculated distance is then mapped to the system's volume range using `np.interp()` to control the volume level. The `pycaw` library is used to interact with the system's audio volume interface and set the volume level.