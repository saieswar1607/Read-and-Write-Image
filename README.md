# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
```python
# Developed By: Sai Eswar Kandukuri
# Register Number: 212221240020
# To Read,display the image

import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
cv2.imshow('212221240020-Read&Display',colorImage)
cv2.waitKey(0)

# To write the image

import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
cv2.imwrite('/Users/eswar1607/Desktop/written.jpg',colorImage)
writtenImage = cv2.imread('/Users/eswar1607/Desktop/written.jpg',1)
cv2.imshow('212221240020-WrittenImage',writtenImage)
cv2.waitKey(0)

# Find the shape of the Image

import cv2
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
print(colorImage.shape)

# To access rows and columns

import cv2
import random
colorImage = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
for i in range(100):
    for j in range(colorImage.shape[1]):
        colorImage[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240020-AccessingRowsAndColumns',colorImage)
cv2.waitKey(0)

# To cut and paste portion of image

import cv2
color_img = cv2.imread('/Users/eswar1607/Desktop/flower.png',1)
tag = color_img[200:400,300:500]
color_img[300:500,200:400] = tag
cv2.imshow('212221240020-CutAndPaste',color_img)
cv2.waitKey(0)

```
## Output:

### i) Read and display the image

<br>
<img width="462" alt="Screenshot 2022-03-30 at 9 02 04 PM" src="https://user-images.githubusercontent.com/93427011/160879315-edac10a5-6080-402b-ab3e-741969d141f0.png">
<br>

### ii)Write the image

<br>
<img width="462" alt="Screenshot 2022-03-30 at 9 19 06 PM" src="https://user-images.githubusercontent.com/93427011/160879395-be65b57b-62b2-4808-b5c4-78dc682c1268.png">
<br>

### iii)Shape of the Image

<br>
<img width="810" alt="Screenshot 2022-03-30 at 9 20 47 PM" src="https://user-images.githubusercontent.com/93427011/160879778-ce4893ad-ba69-4699-8f64-cbcaa61e74ab.png">
<br>

### iv)Access rows and columns
<br>
<img width="462" alt="Screenshot 2022-03-30 at 9 21 48 PM" src="https://user-images.githubusercontent.com/93427011/160879846-6d1832d7-798f-40c2-9867-d8a5a104a6da.png">
<br>

### v)Cut and paste portion of image
<br>
<img width="462" alt="Screenshot 2022-03-30 at 9 26 06 PM" src="https://user-images.githubusercontent.com/93427011/160879886-ed512986-cbae-42e8-9e06-88599f14696d.png">
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


