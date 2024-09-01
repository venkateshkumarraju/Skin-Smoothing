# Facial Skin Smoothing with Bilateral Filtering
This project demonstrates two methods for applying bilateral filtering to smoothen facial skin in images.

# Purpose
This code aims to reduce noise and blemishes from facial skin in images while preserving sharp edges. It achieves this by utilizing the bilateral filter, which combines spatial and intensity similarity for smoothing.

# Key Features
Detects faces in an image using the Haar cascade classifier.
Applies bilateral filtering for skin smoothing.
Compares two approaches for applying bilateral filtering.

# Dependencies
 OpenCV  
 
 NumPy
 
 Matplotlib  

Installation:

You can install these dependencies using pip:

```
pip install opencv-python numpy matplotlib
```
# Usage
Make sure you have OpenCV, NumPy, and Matplotlib installed.
Place the haarcascade_frontalface_default.xml file in the same directory as your Python script. This file is a pre-trained Haar cascade classifier for face detection. You can download it from the OpenCV website.
Save the provided code as notebook
Run the notebook

# Explanation of the Code:

The notebook  first imports the necessary libraries.
It then reads the image using OpenCV and displays it using Matplotlib.
The script uses a Haar cascade classifier to detect faces in the image.
For each detected face, two functions are defined for skin smoothing:
smooth_skin_1: This function converts the image to LAB color space, applies bilateral filtering to the L channel (brightness), and then merges it back with the original A and B channels.
smooth_skin_2: This function directly applies bilateral filtering to the BGR image with user-defined parameters for diameter, sigmaColor, and sigmaSpace.
Finally, the script displays the original and smoothed versions of the face region for both methods.
# Experimenting with Parameters:

You can experiment with the parameters of the bilateral filter (diameter, sigmaColor, and sigmaSpace) in the smooth_skin_2 function to achieve different levels of smoothing and edge preservation.

# Input image 
![input](https://github.com/venkateshkumarraju/Skin-Smoothing/blob/main/venkatesh.jpg)
# Output for method 1
![output1](https://github.com/venkateshkumarraju/Skin-Smoothing/blob/main/op%201.PNG)
# Output for method 2
![output2](https://github.com/venkateshkumarraju/Skin-Smoothing/blob/main/op2.PNG)
