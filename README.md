# Implementation-of-Erosion-and-Dilation
## Aim:
To implement Erosion and Dilation using Python and OpenCV.
## Software Required:
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.

### Step2:
Create the Text using cv2.putText.

### Step3:
Create the structuring element.

### Step4:
Erode and Dilate the image.

### Step5:
End Program.

 
## Program:

``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Load the image
img1=np.zeros((200,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL

# Create the Text using cv2.putText
cv2.putText(img1,' KRISHNA ',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1,cmap='gray')

# Create the structuring element
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))

# Erode the image
img_erode=cv2.erode(img1,kernel1)
plt.imshow(img_erode,cmap='gray')

# Dilate the image
img_dilate=cv2.dilate(img1,kernel1)
plt.imshow(img_dilate,cmap='gray')

```
## Output:

### Display the input Image
![krishna 1](https://user-images.githubusercontent.com/75241177/171628993-5821b43a-9a84-4f14-895c-c73d4abd1439.jpg)



### Display the Eroded Image
![krishna  2](https://user-images.githubusercontent.com/75241177/171629010-02ca649f-17ed-4cb0-b31d-36ef35db71dd.jpg)


### Display the Dilated Image
![krishna 1](https://user-images.githubusercontent.com/75241177/171629029-29313f7c-3962-4319-bdb5-1b4b24fa6fe8.jpg)




## Result:
Thus the generated text image is eroded and dilated using python and OpenCV.
