# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
<br>

### Step2:
<br>

### Step3:
<br>

### Step4:
<br>

### Step5:
<br>

## Program:
```python
# Developed By:
# Register Number:
# i) Convert BGR and RGB to HSV and GRAY

import cv2
house_color_image= cv2.imread('house.jpeg')
cv2.imshow ('Original image', house_color_image)
hsv_image= cv2.cvtColor (house_color_image, cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV', hsv_image)
hsv_image1 = cv2.cvtColor (house_color_image, cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV', hsv_image1)
gray_image= cv2.cvtColor (house_color_image, cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY', gray_image)
gray_image1 = cv2.cvtColor (house_color_image, cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY', gray_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()

# ii)Convert HSV to RGB and BGR

import cv2
house_HSV_image= cv2.imread('house.jpeg')
cv2.imshow('Original HSV image',house_HSV_image)
RGB_image = cv2.cvtColor(house_HSV_image, cv2.COLOR_HSV2RGB)
cv2.imshow('HSV to RGB',RGB_image )
BGR_image = cv2.cvtColor(house_HSV_image, cv2.COLOR_HSV2BGR)
cv2.imshow('HSV to BGR',BGR_image)
cv2.waitKey(0)
cv2.destroyAllwindows()

# iii)Convert RGB and BGR to YCrCb

import cv2
house_HSV_image= cv2.imread('house.jpeg')
cv2.imshow('Original HSV image',house_HSV_image)
RGB_image = cv2.cvtColor(house_HSV_image, cv2.COLOR_HSV2RGB)
cv2.imshow('HSV to RGB',RGB_image )
BGR_image = cv2.cvtColor(house_HSV_image, cv2.COLOR_HSV2BGR)
cv2.imshow('HSV to BGR',BGR_image)
cv2.waitKey(0)
cv2.destroyAllwindows()

# iv)Split and Merge RGB Image

import cv2
image = cv2.imread('house.jpeg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('Merged BGR image',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()

# v) Split and merge HSV Image

import cv2
image = cv2.imread('house.jpeg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
## Output:
### i) BGR and RGB to HSV and GRAY
<br>
<img width="1440" alt="1M" src="https://user-images.githubusercontent.com/93427286/162482650-6bbac3a9-f649-4cfe-b6e1-3e4cc40fdb8e.png">
<br>

### ii) HSV to RGB and BGR
<br>
<img width="1440" alt="2M" src="https://user-images.githubusercontent.com/93427286/162482678-0afc8761-212f-4697-9f5a-be78aa2290a4.png">
<br>

### iii) RGB and BGR to YCrCb
<br>
<img width="1440" alt="3M" src="https://user-images.githubusercontent.com/93427286/162482709-28d966eb-e7fa-4e85-b9d2-350f4160fb0a.png">
<br>

### iv) Split and merge RGB Image
<br>
<img width="1440" alt="4M" src="https://user-images.githubusercontent.com/93427286/162482745-af6bf53f-ee57-4bb0-90c8-98b50e594e58.png">
<br>

### v) Split and merge HSV Image
<br>
<img width="1440" alt="5M" src="https://user-images.githubusercontent.com/93427286/162482762-401858a1-c6c0-4c75-9d62-f4a22e5f8a81.png">
<br>


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
