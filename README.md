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
~~~
# displaying original pic
import cv2
img=cv2.imread('doraemon.jpg')
# Original image
cv2.imshow('Original Image',img)
cv2.waitKey(0)
cv2.destroyAllWindows()
~~~
~~~~
# i) Convert BGR and RGB to HSV and GRAY
# BGR2HSV
hsv_img=cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsv_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

# RGB2HSV
hsv_img1=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsv_img1)
cv2.waitKey(0)
cv2.destroyAllWindows()

# BGR2GRAY
gray_img=cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',gray_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

# RGB2GRAY
gray_img1=cv2.cvtColor(img,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',gray_img1)
cv2.waitKey(0)
cv2.destroyAllWindows()
~~~



~~~
# ii)Convert HSV to RGB and BGR
# HSV TO RGB
rgb_img=cv2.cvtColor(hsv_img,cv2.COLOR_HSV2RGB)
cv2.imshow('HSV TO RGB',rgb_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

# HSV TO BGR
bgr_img=cv2.cvtColor(hsv_img1,cv2.COLOR_HSV2BGR)
cv2.imshow('HSV TO BGR',bgr_img)
cv2.waitKey(0)
cv2.destroyAllWindows()


~~~

~~~
# iii)Convert RGB and BGR to YCrCb
# RGB to YCrCb
YCrCb_img=cv2.cvtColor(img,cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb',YCrCb_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

# BGR TO YCrCb
YCrCb_img1=cv2.cvtColor(img,cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2YCrCb',YCrCb_img1)
cv2.waitKey(0)
cv2.destroyAllWindows()


~~~
~~~
# iv)Split and Merge RGB Image
blue=img[:,:,0]
green=img[:,:,1]
red=img[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
merged_BGR=cv2.merge((blue,green,red))
cv2.imshow('Merged BGR Image',merged_BGR)
cv2.waitKey(0)
cv2.destoryAllWindows()
~~~

~~~
# v) Split and merge HSV Image
#Split:
hsv = cv2.cvtColor(img, cv2.COLOR_BGR2HSV)
h,s,v=cv2.split(hsv)
cv2.imshow("Hue-image",h)
cv2.imshow("Saturation-image",s)
cv2.imshow("Gray-image",v)
#Merge:
Merged_HSV=cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',Merged_HSV)
cv2.waitKey(0)
cv2.destoryAllWindows()
~~~
## Output:
# ORIGINAL IMAGE:
![image](https://user-images.githubusercontent.com/94165322/231366900-7756e75b-fb89-4149-b064-6460d673eae0.png)

### i) BGR and RGB to HSV and GRAY
## BGR TO HSV:
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/cd486bae-ce2b-406e-9487-7adb1e3fff0a)
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/2c2ed10f-c79e-400a-aee3-b0449c25199c)
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/062c3ad4-1454-4d5a-9f5b-0a5646668442)
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/10ee451a-00e3-4abc-a006-b9535d2cda10)
![image](https://github.com/Naveenvetrivel/Color-Conversion/assets/94165322/5524f7fa-a7b3-4aff-b7d6-e3598a1e0fe3)

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
