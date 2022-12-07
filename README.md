# Face-Recognition-With-HaarCasCade
## Goal
* learn the basics of face detection using Haar Feature-based Cascade Classifiers
* extend the same for eye detection etc.
## Basics

##Haar-cascade Detection in OpenCV
Here we will deal with detection. OpenCV already contains many pre-trained classifiers for face, eyes, smile etc. Those XML files are stored in opencv/data/haarcascades/ folder. Let's create a face and eye detector with OpenCV.

We use the function: detectMultiScale (image, objects, scaleFactor = 1.1, minNeighbors = 3, flags = 0, minSize = new cv.Size(0, 0), maxSize = new cv.Size(0, 0))

## Parameters
image	matrix of the type CV_8U containing an image where objects are detected.
objects	vector of rectangles where each rectangle contains the detected object. The rectangles may be partially outside the original image.
scaleFactor	parameter specifying how much the image size is reduced at each image scale.
minNeighbors	parameter specifying how many neighbors each candidate rectangle should have to retain it.
flags	parameter with the same meaning for an old cascade as in the function cvHaarDetectObjects. It is not used for a new cascade.
minSize	minimum possible object size. Objects smaller than this are ignored.
maxSize	maximum possible object size. Objects larger than this are ignored. If maxSize == minSize model is evaluated on single scale.
