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

### i) BGR and RGB to HSV and GRAY
## BGR TO HSV:
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/bfc83df5-2b3e-4407-936c-b5e25c3b3d29)
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/8a4f2802-f150-4ecc-a8ba-903f1aece449)
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/26f77fde-66ef-4463-a531-27776c8c21a3)
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/80b39dfa-f533-4e3c-8287-335b9a698c35)

### ii) HSV to RGB and BGR
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/c14cd787-aa84-4b3a-8457-d6e96319f5b2)
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/c7f86530-9f63-49b8-8b55-f969eafe34fc)


### iii) RGB and BGR to YCrCb
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/59a279f0-cf26-40cd-9e4c-19e7c7a29fbc)
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/1da5eed4-8f14-48eb-b9f6-bcd93c44147e)


### iv) Split and merge RGB Image

![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/cca28656-6f8a-4d56-9bc1-59c21cac3a64)

### v) Split and merge HSV Image
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/8524c316-46a0-4878-b293-5aaf7932b336)


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
