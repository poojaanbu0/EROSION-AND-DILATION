# EXP-10 -Record-Implementation of Erosion and Dilation
## Aim:
To implement Erosion and Dilation using Python and OpenCV.

## Software Required:
1.Anaconda - Python 3.7

2.OpenCV.

## Algorithm:
### Step 1:
Load the necessary packages requiured for the implemtation of erosion and dilation on an image.

### Step 2:
Create the text image for the implemtation of erosion and dilation using cv2.putText function.

### Step 3:
Create the structuring image for the implemtation of erosion and dilation on the text image.

### Step 4:
Apply the erosion and dilation to the text image using cv2.erode and cv2.dilate.

### Step 5:
Display the images of the erosion and dilation applied using the plt.imshow.

### Step 6:
End the program.

## Program:
```
Program to implement Erosion and Dilation using Python and OpenCV.
Developed by : Pooja A
Register No : 212222240072
```

```python
# Import the necessary packages:

import cv2
import numpy as np
import matplotlib.pyplot as plt
```
```python
# Create the Text using cv2.putText:

text_image = np.zeros((100,300),dtype = 'uint8')
font = cv2.FONT_HERSHEY_SCRIPT_COMPLEX = 7
cv2.putText(text_image,"Javith",(5,70),font,2,(255),5,cv2.LINE_AA)
plt.title("Original Text Image")
plt.imshow('created_text',img)
plt.axis('off')
```
```python
# Create the structuring element:

kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
```
```python
# Erode the image:

image_erode = cv2.erode(text_image,kernel)
plt.title("Eroded Text Image")
plt.imshow(image_erode,'bone')
plt.axis('off')
```
```python
# Dilate the image:

image_dilate = cv2.dilate(text_image,kernel)
plt.title("Dilated Text Image")
plt.imshow(image_dilate,'bone')
plt.axis('off')
```

## Output:
### Display the input text Image:
![10 input](https://github.com/poojaanbu0/EROSION-AND-DILATION/assets/119390329/25160446-ca54-4621-b26e-f77a61070791)

### Display the Eroded text Image:
![10 eroded img1](https://github.com/poojaanbu0/EROSION-AND-DILATION/assets/119390329/41a820c0-eb7d-4aec-b00c-775308c44425)
![10 eroded img 2](https://github.com/poojaanbu0/EROSION-AND-DILATION/assets/119390329/43de7ac6-b828-43fe-b171-22da0e5940ca)

### Display the Dilated text Image:
![10 dilated img 1](https://github.com/poojaanbu0/EROSION-AND-DILATION/assets/119390329/c5a7206a-884f-4a1b-91b2-d3a75a0084e1)
![10 dilated img 2](https://github.com/poojaanbu0/EROSION-AND-DILATION/assets/119390329/09d47463-39d8-461e-9fc7-76bd0f2dd254)


## Result:
Thus the generated text image is eroded and dilated using python and OpenCV.
