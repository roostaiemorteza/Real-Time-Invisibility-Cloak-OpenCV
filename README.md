# Real-Time Invisibility Cloak with OpenCV

A real-time computer vision project that creates an invisibility cloak effect using Python and OpenCV.

The application detects a configurable color range in the webcam feed and replaces the detected region with a previously captured background, creating the illusion of invisibility.

## Overview

The project uses OpenCV to process webcam frames in real time.

Before the main loop starts, a background frame is captured. During operation, the program detects the selected color using HSV thresholds and combines the background with the live video to create the cloak effect.

## Features

- Real-time webcam processing
- HSV-based color segmentation
- Interactive HSV threshold controls
- Background capture
- Morphological mask processing
- Real-time invisibility effect
- Original frame and mask preview
- Adjustable color detection using OpenCV trackbars

## How It Works

1. Open the OpenCV HSV control window.
2. Capture the initial background.
3. Read frames from the webcam.
4. Convert each frame from BGR to HSV.
5. Apply the configured lower and upper HSV thresholds.
6. Reduce noise and improve the mask using image processing operations.
7. Combine the detected region with the stored background.
8. Display the final invisibility effect.

## Requirements

Python 3.x with:

```bash
pip install opencv-python
pip install numpy
Project Structure
.
├── Harry_Potter_cloak.py
├── LICENSE
├── README.md
└── .gitignore
Notes

The quality of the invisibility effect depends on lighting conditions, camera position, background stability, and accurate HSV threshold selection.

The background should remain relatively unchanged after capture for the visual effect to work properly.

Author

Morteza Roostaie

GitHub: https://github.com/roostaiemorteza



