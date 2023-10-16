# EROSION-AND-DILATION

## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary libraries (OpenCV and NumPy).
<br>
### Step2:
Use cv2.putText to add the text to the img1 image at specific coordinates.
<br>

### Step3:
Define two kernels (kernel and kernel1) for morphological operations.
<br>

### Step4:
Display the eroded image using cv2.imshow.
<br>

### Step5:
Use cv2.waitKey(0) to wait for a key press indefinitely.
<br>

## Program:
```
Developed by:ROSHINI R K
Register Number:212222230123
```
### Import the necessary packages
``` Python
import cv2
import numpy as np
```
### Create the Text using cv2.putText
```python
img1=np.zeros((100,400),dtype="uint8")
font=cv2.FONT_HERSHEY_PLAIN
cv2.putText(img1,"ROSHINI.R.K",(5,70),font,2,(255),5,cv2.LINE_AA)
cv2.imshow("image",img1)
cv2.waitKey(0)
```
### Create the structuring element
```python
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
```


### Erode the image
```python
cv2.erode(img1, kernel)
image_erode = cv2.erode(img1,kernel1)
cv2.imshow("ROSHINI.R.K-212222230123",image_erode)
cv2.waitKey(0)
```
### Dilate the image
```python
image_dilatel=cv2.dilate(img1,kernel1)
cv2.imshow("ROSHINI-212222230123",image_dilatel)
cv2.waitKey(0)
```
## Output:

### Display the input Image
<br>

![image](https://github.com/roshiniRK/EROSION-AND-DILATION/assets/118956165/73fd4424-707f-4eca-b192-4239687eff8b)


<br>

### Display the Eroded Image
<br>

![image](https://github.com/roshiniRK/EROSION-AND-DILATION/assets/118956165/d71a0705-e79b-4043-be1a-da70d6a796ce)


<br>


### Display the Dilated Image
<br>

![image](https://github.com/roshiniRK/EROSION-AND-DILATION/assets/118956165/e9ad1182-754a-4be2-8b7b-cf168a659bc8)


<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
