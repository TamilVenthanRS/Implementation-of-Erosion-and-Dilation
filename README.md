# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:
### Step 1:
Import the necessary packages.
### Step 2:
Create the Text using cv2.putText
### Step 3:
Create the structuring element.
### Step 4:
Erode the image.
### Step 5:
Dilate the image. 
## Program:
```
/*
Developed by   : Tamil venthan R S
Register Number: 212220230054
*/
```
``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt
# Create the Text using cv2.putText
img1=np.zeros((300,500),dtype='uint8')
font=cv2.FONT_ITALIC=3
img2=cv2.putText(img1,"Kumaran",(5,70),font,3,(255),5,cv2.LINE_AA)
cv2.imshow("Original",img2)
cv2.waitKey(0)
cv2.destroyAllWindows()
# Create the structuring element
kernel1=np.ones((5,5),np.uint8)
# Erode the image
erode=cv2.erode(img2,kernel1)
cv2.imshow("Erosion1",erode)
cv2.waitKey(0)
cv2.destroyAllWindows()
# Dilate the image
dilute=cv2.dilate(img2,kernel2)
cv2.imshow("Dilution",dilute)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## Output:

### Display the input Image
![Screenshot (151)](https://user-images.githubusercontent.com/75235477/171098017-a4988fa3-b05c-4a29-8dbc-da12996e7ae8.png)

### Display the Eroded Image
![Screenshot (152)](https://user-images.githubusercontent.com/75235477/171098058-b30c505c-9765-44c6-8357-eb5c5721011e.png)

### Display the Dilated Image
![Screenshot (153)](https://user-images.githubusercontent.com/75235477/171098071-6d6c823b-ea0b-40c7-a72f-993525d15498.png)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
