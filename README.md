# feature-detection-opencv
Implementation of keypoint detection and matching using SIFT, SURF, and Corner Detection algorithms with OpenCV for feature extraction and comparison.

🔍 Feature Detection using SIFT, SURF & Corner Detection | OpenCV


This project demonstrates the use of feature detection algorithms—SIFT, SURF, and Harris Corner Detection—to extract and compare key points across images for various computer vision tasks like matching, registration, and motion tracking.



📌 Objective


Detect and visualize important features in images

Match features between image pairs

Compare the behavior and performance of SIFT, SURF, and Harris Corner Detector



📚 Theoretical Overview


🔹 1. SIFT (Scale-Invariant Feature Transform)

Detects keypoints invariant to scale, rotation, and illumination.

Computes a 128-dimensional descriptor for each keypoint.

Uses Difference of Gaussians for scale-space extrema detection.



🔹 2. SURF (Speeded-Up Robust Features)

Faster alternative to SIFT, based on Hessian matrix approximation.

Uses integral images for rapid computation.

Good for real-time applications.


🔹 3. Harris Corner Detection

Classical method for detecting corners based on eigenvalues of the gradient matrix.

Best suited for static, grayscale images with sharp features.



📁 Project Structure

sift-surf-corner-detection/
├── sift_feature_matching.ipynb
├── surf_feature_matching.ipynb
├── harris_corner_detection.ipynb
├── images/
│   ├── Optimus.jpg
│   ├── Car.jpg
├── README.md
└── requirements.txt


🎯 Features

📸 Load and preprocess grayscale images

🧠 Detect keypoints using:

cv2.SIFT_create()

cv2.xfeatures2d.SURF_create() (requires opencv-contrib)

cv2.cornerHarris()


🎯 Match keypoints using BFMatcher (for SIFT & SURF)


🖼️ Visualize:

Detected keypoints

Matched keypoints between two images

Corner points on grayscale image

