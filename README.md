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
Developed by: Pooja A
Register No: 212222240072
```

```python
# Import the necessary packages
import cv2
import numpy as np

# Create the Text using cv2.putText

IMg= np.zeros((350,1400),dtype ='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'poo',(15,200),font,5,(255),10,cv2.LINE_AA)
cv2.imshow('created_text',img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

```python
# Create the structuring element

# Erode the image

erode1= np.ones((5,5),np.uint8)
erode2 = cv2.getStructuringElement(cv2.MORPH_CROSS,(12,12))

image_erode1 = cv2.erode(img,erode1)
cv2.imshow('Eroded_image_1',image_erode1)
cv2.waitKey(0)
cv2.destroyAllWindows()
image_erode2 = cv2.erode(img,erode2)
cv2.imshow('Eroded_image_2',image_erode2)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

```python
# Dilate the image

dilate1= np.ones((5,5),np.uint8)
dilate2 = cv2.getStructuringElement(cv2.MORPH_CROSS,(12,12))

image_dilate1 = cv2.dilate(img,dilate1)
cv2.imshow('Dilated_image_1',image_dilate1)
cv2.waitKey(0)
cv2.destroyAllWindows()
image_dilated2 = cv2.dilate(img,dilate2)
cv2.imshow('Dilated_image_2',image_dilated2)
cv2.waitKey(0)
cv2.destroyAllWindows()
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
