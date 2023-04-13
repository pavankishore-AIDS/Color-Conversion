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
# Developed By:M.Pavan kishore
# Register Number:212221230076
# i) Convert BGR and RGB to HSV and GRAY
```
import cv2
img = cv2.imread('th.jpeg')
cv2.imshow('original',img)

bgr2hsv = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR To HSV',bgr2hsv)

bgr2gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR To GRAY',bgr2gray)

rgb2hsv = cv2.cvtColor(img,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',rgb2hsv)

rgb2gray = cv2.cvtColor(img,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',rgb2gray)

cv2.waitKey(0)
cv2.destroyAllWindows()
```




# ii)Convert HSV to RGB and BGR
```
cv2.imshow('HSV',bgr2hsv)

hsv2rgb = cv2.cvtColor(bgr2hsv,cv2.COLOR_HSV2RGB)
cv2.imshow('HSVtoRGB',hsv2rgb)

hsv2bgr = cv2.cvtColor(bgr2hsv,cv2.COLOR_HSV2BGR)
cv2.imshow('HSVtoBGR',hsv2bgr)

cv2.waitKey(0)
cv2.destroyAllWindows()
```




# iii)Convert RGB and BGR to YCrCb
```
cv2.imshow('RGB',img)

rgb2YcrCb = cv2.cvtColor(img,cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGBtoYCrCb',rgb2YcrCb)

bgr2YcrCb = cv2.cvtColor(img,cv2.COLOR_HSV2BGR)
cv2.imshow('BGRtoYCrCb',bgr2YcrCb)

cv2.waitKey(0)
cv2.destroyAllWindows()
```



# iv)Split and Merge RGB Image
```
b,g,r = cv2.split(img)
cv2.imshow("RED MODEL", r)
cv2.imshow("GREEN MODEL", g)
cv2.imshow("BLUE MODEL ", b)

merger = cv2.merge([b,g,r])
cv2.imshow("MERGED IMAGE", merger)

cv2.waitKey(0)
cv2.destroyAllWindows()
```



# v) Split and merge HSV Image
```

cv2.imshow("INITIAL_HSV ", bgr2hsv)

h,s,v = cv2.split(bgr2hsv)
cv2.imshow("RED MODEL", h)
cv2.imshow("GREEN MODEL", s)
cv2.imshow("BLUE MODEL ", v)

merger = cv2.merge([h,s,v])
cv2.imshow("MERGED IMAGE", merger)

cv2.waitKey(0)
cv2.destroyAllWindows()
```



```
## Output:
### i) BGR and RGB to HSV and GRAY
<br>
![f1](https://user-images.githubusercontent.com/94154941/231702201-8e486982-a38a-43fa-b81e-717fd96a8812.png)

<br>

### ii) HSV to RGB and BGR
<br>
![f2](https://user-images.githubusercontent.com/94154941/231702173-39d2cca3-7a67-4d9e-9d6a-176da889327a.png)

<br>

### iii) RGB and BGR to YCrCb
<br>
![f3](https://user-images.githubusercontent.com/94154941/231702149-1e6dc25d-b60d-45c7-99a4-91adc2dc03f6.png)
<br>

### iv) Split and merge RGB Image
<br>
![f4](https://user-images.githubusercontent.com/94154941/231702034-43cf3b69-4e2d-4b3f-8593-f68af7347c5d.png)
<br>


### v) Split and merge HSV Image
<br>
![f5](https://user-images.githubusercontent.com/94154941/231701911-4b89f86c-ec6f-42b7-8afa-3d99e3dd8823.png)
<br>


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
