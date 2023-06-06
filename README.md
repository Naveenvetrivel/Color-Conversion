# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
1.Import cv2 and save and image as filename.jpg
2.Use imread(filename, flags) to read the file.
3.Use cv2.cvtColor(src, code, dst, dstCn) to convert an image from one color space to another.
4.Split and merge the image using cv2.split and cv2.merge commands.
5.End the program and close the output image windows.
### Step1:
Import cv2 and save and image as filename.jpg

### Step2:
Use imread(filename, flags) to read the file.

### Step3:
Use cv2.cvtColor(src, code, dst, dstCn) to convert an image from one color space to another.

### Step4:
Split and merge the image using cv2.split and cv2.merge commands.

### Step5:
End the program and close the output image windows.

## Program:
# Developed By:V NAVEENKUMAR
# Register Number:212221230068
# i) Convert BGR and RGB to HSV and GRAY
# BGR TO HSV

import cv2
image =cv2.imread('ship.jpg')
cv2.imshow('original',image)
b_h=cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR_HSV',b_h)
cv2.waitKey(0)
cv2.destroyAllWindows

# BGR TO GRAY
~~~
import cv2
image =cv2.imread('ship.jpg')
cv2.imshow('original',image)
b_g=cv2.cvtColor(image,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR_GRAY',b_g)
cv2.waitKey(0)
cv2.destroyAllWindows

# RGB TO HSV

import cv2
image =cv2.imread('ship.jpg')
cv2.imshow('original',image)
r_h=cv2.cvtColor(image,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB_HSV',r_h)
cv2.waitKey(0)
cv2.destroyAllWindows

# RGB TO GRAY

import cv2
image =cv2.imread('ship.jpg')
cv2.imshow('original',image)
r_g=cv2.cvtColor(image,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB_GRAY',r_g)
cv2.waitKey(0)
cv2.destroyAllWindows




# ii)Convert HSV to RGB and BGR

# HSV TO RGB

import cv2
ori=cv2.imread('bgr2hsv.png')
cv2.imshow('hsvtorgb',ori)
h_r=cv2.cvtColor(ori,cv2.COLOR_HSV2RGB)
cv2.imshow('HSV_RGB',h_r)
cv2.waitKey(0)
cv2.destroyAllWindows

# HSV TO BGR

import cv2
ori=cv2.imread('bgr2hsv.png')
cv2.imshow('Original',ori)
h_b=cv2.cvtColor(ori,cv2.COLOR_HSV2BGR)
cv2.imshow('HSV_BGR',h_b)
cv2.waitKey(0)
cv2.destroyAllWindows




# iii)Convert RGB and BGR to YCrCb

# RGB TO YCrCb

import cv2
ori=cv2.imread('hsv2rgb.png')
YCrCb_image = cv2.cvtColor(ori, cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB_YCRCB',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows

# BGR TO YCrCb

import cv2
image1=cv2.imread('ship.jpg')
YCrCb_image = cv2.cvtColor(image1, cv2.COLOR_BGR2YCrCb)
cv2.imshow('BGR_YCRCB',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows




# iv)Split and Merge RGB Image

import cv2
img = cv2.imread("ship.jpg")
img1= cv2.resize(img, (270,180))
cv2
b,g,r = cv2.split(img1)
cv2.imshow("RED MODEL", r)
cv2.imshow("GREEN MODEL", g)
cv2.imshow("BLUE MODEL ", b)
merger = cv2.merge([b,g,r])
cv2.imshow("MERGED IMAGE", merger )
cv2.waitKey(0)
cv2.destroyAllWindows()


# v) Split and merge HSV Image

import cv2
img = cv2.imread("ship.jpg")
img1= cv2.resize(img, (270,180))
cv2
b,g,r = cv2.split(img1)
cv2.imshow("RED MODEL", r)
cv2.imshow("GREEN MODEL", g)
cv2.imshow("BLUE MODEL ", b)
merger = cv2.merge([b,g,r])
cv2.imshow("MERGED IMAGE", merger )
cv2.waitKey(0)
cv2.destroyAllWindows()
~~~
## Output:
# ORIGINAL IMAGE:
![image](https://user-images.githubusercontent.com/94165322/231366900-7756e75b-fb89-4149-b064-6460d673eae0.png)

### i) BGR and RGB to HSV and GRAY
## BGR TO HSV:
/home/sec/Downloads/ori.png
### ii) HSV to RGB and BGR
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/b8d55f4d-cad7-47e7-937e-03dda6a12cd3)
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/c9d365e2-3002-4eeb-bb90-f25a9db86453)

### iii) RGB and BGR to YCrCb
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/2b9f233e-3aea-444e-8527-6e4ea1397ae6)
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/42c64a21-fa84-408f-8a69-ffc33f1a9d09)

### iv) Split and merge RGB Image
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/afbc9e1e-b309-4353-b308-b85f76ab4925)

### v) Split and merge HSV Image
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/85309b5b-39b0-4535-b394-920ae0a196be)

## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
