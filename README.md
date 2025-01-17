# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Import cv2 library and upload the image or capture an image.

### Step2:
Read the saved image using cv2.imread("filename.jpg").
### Step3:
Convert the image into the given color transformation using cv2.cvtColor(image, cv2.BGR2YCrCb) and similarly for other color formats.

### Step4:
Split and merge the image using cv2.split(hsv) and cv2.merge([h,s,v])



### Step5:
Output the image using cv2.imshow("OUTPUT", image)

## Program:
```python
# Developed By:M.Pavan kishore
# Register Number:212221230076
# i) Convert BGR and RGB to HSV and GRAY
```
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




## Output:
### i) BGR and RGB to HSV and GRAY

![f1](https://user-images.githubusercontent.com/94154941/231703767-dab356fb-2942-4f64-8769-66c4afeb4de4.png)


### ii) HSV to RGB and BGR

![f2](https://user-images.githubusercontent.com/94154941/231703789-797f87e4-a50b-4422-8ebe-cd6c360ebe7a.png)

### iii) RGB and BGR to YCrCb

![f3](https://user-images.githubusercontent.com/94154941/231703861-0fd2103c-9c56-4ef9-bca3-cdb750911cd5.png)


### iv) Split and merge RGB Image

![f4](https://user-images.githubusercontent.com/94154941/231703888-a9a7b03d-e465-4041-86a6-5e8162b50c93.png)



### v) Split and merge HSV Image
![f5](https://user-images.githubusercontent.com/94154941/231703916-d82f6392-6175-451e-b3ce-e824c3d2eea2.png)




## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
