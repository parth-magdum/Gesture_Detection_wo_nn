# Gesture Detection Assignment

This project aims to detect a specific gesture in a video stream using the MediaPipe library for pose estimation.

## Introduction

Gesture detection is an important task in computer vision, with applications ranging from human-computer interaction to sign language recognition. In this assignment, we use the MediaPipe library, which provides robust pose estimation functionality, to detect a specific gesture in a video stream.

## Project Overview

The project consists of the following components:

1. **Pose Detection**: Utilizes the MediaPipe library for real-time pose estimation, detecting key landmarks on the human body.
2. **Gesture Detection**: Analyzes the pose landmarks to detect a specific gesture, such as waving or pointing.
3. **Video Processing**: Processes input video frames, applies pose and gesture detection algorithms, and generates an output video with detected gestures highlighted.

## Features

- Detects a specific gesture in a video stream.
- Utilizes pose estimation for landmark detection.
- Allows for customization of the gesture and detection threshold.

## MediaPipe Pose Detection

MediaPipe is an open-source, cross-platform library developed by Google that offers ready-to-use, high-performance AI solutions for various tasks, including pose estimation. The pose estimation model provided by MediaPipe detects key landmarks on a human body, such as the nose, eyes, shoulders, elbows, wrists, hips, knees, and ankles, in real-time.

## Customization

To customize the gesture detection process, follow these steps:

1. **Gesture Representation**: Modify the `gesture_image.png` file to represent the gesture you want to detect.

2. **Adjust Landmark Focus**: Modify the `extract_landmarks_from_frame` function to focus on specific body parts for detection. You can adjust the indices to prioritize certain landmarks over others. For example, I've cleverly increased the weights of coordinates for hands and legs by multiplying their x and y values by 5, providing more emphasis on these body parts for better gesture detection.

3. **Threshold Configuration**: Set the detection threshold according to your requirements. The threshold determines the similarity level required for a gesture to be detected.

4. **Record Test Video**: You have the option to record your own test video by running the script and following the prompts. This allows you to test the gesture detection algorithm on real-time video input.

## Functionality Provided

- **Recording Test Video**: The script prompts the user to record a test video if desired. This feature allows for easy testing and validation of the gesture detection algorithm on custom input.
  
- **Adjustment of Landmark Weights**: By increasing the weights of coordinates for hands and legs in the `extract_landmarks_from_frame` function, the algorithm gives more importance to these body parts, enhancing the accuracy of gesture detection.



## Requirements

- Python 3.x
- OpenCV (cv2)
- MediaPipe
- NumPy

## Installation

1. Clone the repository:

```bash
https://github.com/parth-magdum/Gesture_Detection_wo_nn.git
