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
### Developed By: Charumathi R
### Register Number: 212222240021

i) #To Read,display the image
```python3
import cv2
color_img=cv2.imread('qoutes2.jpeg',1)
cv2.imshow('212222240021_CHARUMATHI',color_img)
cv2.waitKey(0)

```
ii) #To write the image
```python3
import cv2
color_img=cv2.imread('qoutes2.jpeg',1)
w=cv2.imwrite('2.png',color_img)
cv2.imshow('212222240021_CHARUMATHI',color_img)
cv2.waitKey(0)

```
iii) #Find the shape of the Image
```python3
import cv2
import random
color_img=cv2.imread('qoutes2.jpeg',1)
print(color_img.shape)

```
iv) #To access rows and columns
```python3
import cv2
import random
color_img=cv2.imread('qoutes2.jpeg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222240021_CHARUMATHI',color_img)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```python3
import cv2
color_image=cv2.imread('qoutes2.jpeg',-1)
tag=color_image[300:400,300:400]
color_image[50:150,50:150]=tag
cv2.imshow('212222240021_CHARUMATHI',color_image)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image
![DIPT_1](https://user-images.githubusercontent.com/120204455/224645761-38dc42ee-bfec-4e25-8945-8c51918e8810.png)



### ii)Write the image
![DIPT_2](https://user-images.githubusercontent.com/120204455/224645869-e1f1c27c-0a81-48a5-999c-fbbb75df7799.png)


### iii)Shape of the Image
![DIPT_3](https://user-images.githubusercontent.com/120204455/224645922-7474cb8b-717d-4d7b-8b47-7990ed975107.png)


### iv)Access rows and columns
![DIPT_4](https://user-images.githubusercontent.com/120204455/224645938-00e1b2ea-9d66-4605-aead-c536eed1d18a.png)


### v)Cut and paste portion of image
![DIPT_5](https://user-images.githubusercontent.com/120204455/224645993-8dd24ed1-a063-48b1-89d8-6892af2dea78.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


