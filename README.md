# Vehicle-Detection
Machine learning project for 18CSE392T

Data: [Source](https://drive.google.com/file/d/1P0yiO5KlnU8dGgB_L68KB_hjIvUec55f/view)

### Looking at the Frame
* 8th frame from a collection of frames

![Frame 8](https://github.com/sidthakur08/Vehicle-Detection/blob/main/plots/frame8.png)

* 10th frame from a collection of frames

![Frame 10](https://github.com/sidthakur08/Vehicle-Detection/blob/main/plots/frame10.png)

### Difference between two images
A video is a set of frames stacked together in the right sequence. So, when we see an object moving in a video, it means that the object is at a different location at every consecutive frame.
* Grayscale representation of the difference between the 8th and 10th frame.

![Difference](https://github.com/sidthakur08/Vehicle-Detection/blob/main/plots/diff_grayscale.png)

### Images Thresholding
In this method, the pixel values of a grayscale image are assigned one of the two values representing black and white colors based on a threshold. So, if the value of a pixel is greater than a threshold value, it is assigned one value, else it is assigned the other value.

![Thresholding](https://github.com/sidthakur08/Vehicle-Detection/blob/main/plots/image_thresholding.png)

### Image Dilation
This is a convolution operation on an image wherein a kernel (a matrix) is passed over the entire image.

![Dilation](https://github.com/sidthakur08/Vehicle-Detection/blob/main/plots/image_dilation_default.png)

### Finding Contours
The contours are used to identify the shape of an area in the image having the same color or intensity. Contours are like boundaries around regions of interest. So, if we apply contours on the image after the thresholding step, we would get the following result:

![Contour](https://github.com/sidthakur08/Vehicle-Detection/blob/main/plots/contour.png)

### Vehicle Detection Video

![Video](https://github.com/sidthakur08/Vehicle-Detection/blob/main/detection_video/vehicle_detection.gif)


Made using the Article: [Vehicle Detection using Image Processing](https://www.analyticsvidhya.com/blog/2020/04/vehicle-detection-opencv-python/)
