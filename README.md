# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.
### Step2:
Create the Text using cv2.putText.
### Step3:
Use Opening operation.
### Step4:
Use Opening operation.
### Step5:
Use Closing Operation.
## Program:

Developed by:M.CHANDRU

Register No: 212222230026

# Import the necessary packages
```python
import numpy as np
import cv2
import matplotlib.pyplot as plt
```
# Create the Text using cv2.putText
```python
img1=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL
im=cv2.putText(img1,'sameer',(5,70),font,2,(255),5,cv2.LINE_AA)
cv2.imshow ("image",im)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# Create the structuring element
```python
Kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(11,11))
```
# Use Opening operation
```python
image1=cv2.morphologyEx(im,cv2.MORPH_OPEN,Kernel)
cv2.imshow("opening image",image1)
cv2.waitKey(0)
cv2.DestroyAllWindows()
```
# Use Closing Operation
```python
image1=cv2.morphologyEx(im,cv2.MORPH_CLOSE,Kernel)
cv2.imshow("closeing image",image1)
cv2.waitKey(0)
cv2.DestroyAllWindows()
```
## Output:

### Display the input Image
![Screenshot from 2023-10-11 16-06-30](https://github.com/chandrumathiyazhagan/OPENING--CLOSING/assets/119393023/df7aa885-7e79-4629-a04a-255a0952e1c8)

### Display the result of Opening
![Screenshot from 2023-10-11 16-08-00](https://github.com/chandrumathiyazhagan/OPENING--CLOSING/assets/119393023/36bfba35-bca8-4913-a228-492c9ae4c939)
### Display the result of Closing
![Screenshot from 2023-10-11 16-08-52](https://github.com/chandrumathiyazhagan/OPENING--CLOSING/assets/119393023/9de2ed45-9841-434e-b686-605e186ac7d7)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
