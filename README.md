# Finger Count with OpenCV

This project implements a real-time finger counting system using OpenCV. It captures hand gestures from a webcam, segments the hand region, and uses contour analysis with convexity defects to estimate the number of extended fingers.

## Features
- ROI-based hand detection
- Background subtraction and thresholding
- Contour and convex hull extraction
- Convexity defect-based finger counting
- Real-time webcam interface

## Dependencies
- Python
- OpenCV
- NumPy
- scikit-learn

## How It Works
1. A region of interest (ROI) is defined in the camera frame.
2. The background is averaged over time to allow hand segmentation.
3. The segmented hand contour is processed using convex hulls and convexity defects.
4. Valleys between fingers (defects) are counted to estimate the number of fingers shown.
