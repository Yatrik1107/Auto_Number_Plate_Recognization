# Auto_Number_Plate_Recognization

## Overview 
* It detects the number plate from the picture of a car
* Numpy: It is powerful library for numerical computing, providing support for large, multidimensional array and matrices.
* OpenCV: It is a Open Source computer Vision and machine learning library that contains a  set of tools for image and video processing.
* Matplotlib: It is library for creating static, interactive and animated visualizations.
* Imutils: It provides us functions which can help us to translate, rotate and resize the photo which is present in a form of matplotlib graph
* EasyOCR: For optical character recognition to read text from an image. 


### => Reading image and converting into grayscale
* It reads an image using open CV's 'imread'  function,then converts the image to grayscale and then attempts to display the grayscale image using matplotlib's plt.show function.

![Gray_scale](https://github.com/Yatrik1107/Auto_Number_Plate_Recognization/assets/102149563/b158f628-24e4-4479-bb98-3a32aa746886)

### Reducing noise and Detecting Edge
* Then a bilateral filter is applied to the grayscale image 'ev2.bilateralFilter' for noise reduction and then canny edge detection algo to the filtered image and then then attempts to  show image using matplotlib's plt.show function.

![Edges_and_localization](https://github.com/Yatrik1107/Auto_Number_Plate_Recognization/assets/102149563/ae359024-b980-46c7-92d5-9aa71fa99d1d)

### Finding largest rectangle and applying mask
* The provided code snippet performs contour detection on an edge-detected image using OpenCV. It identifies the largest quadrilateral contour in the image, creates a mask based on this contour, and then applies the mask to the original image, effectively isolating the detected quadrilateral shape. The resulting processed image is displayed using Matplotlib.

![Number_plate](https://github.com/Yatrik1107/Auto_Number_Plate_Recognization/assets/102149563/336c326f-b24d-4e69-b315-123560a1bd45)

### Final Cropped Number Plate
* The additional code snippet extracts the bounding box coordinates of the detected quadrilateral region from the mask. Using these coordinates, it crops the original grayscale image to isolate the detected area. The resulting cropped image is displayed using Matplotlib with proper grayscale visualization, providing a focused view of the identified quadrilateral shape.

![Cropped_Numberplate](https://github.com/Yatrik1107/Auto_Number_Plate_Recognization/assets/102149563/643ac4a6-f43e-426b-9fb7-45955ef426cb)

### Final Output: 
![Final_image](https://github.com/Yatrik1107/Auto_Number_Plate_Recognization/assets/102149563/fc03376d-a2de-4c42-804b-6e8f372c482a)

