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
Developed By: **Shafeeq Ahamed. S**
</br>
Register Number: **212221230092**
### i) Convert BGR and RGB to HSV and GRAY
```py
img = cv2.imread('Mikasa.jpeg')
cv2.imshow('original',img)

bgr2hsv = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR To HSV',bgr2hsv)

bgr2gray = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR To GRAY',bgr2gray)

rgb2hsv = cv2.cvtColor(img_rgb,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',rgb2hsv)

rgb2gray = cv2.cvtColor(img_rgb,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',rgb2gray)

cv2.waitKey(0)
cv2.destroyAllWindows()
```
### ii) Convert HSV to RGB and BGR
```py
cv2.imshow('HSV',bgr2hsv)

hsv2rgb = cv2.cvtColor(bgr2hsv,cv2.COLOR_HSV2RGB)
cv2.imshow('HSVtoRGB',hsv2rgb)

hsv2bgr = cv2.cvtColor(bgr2hsv,cv2.COLOR_HSV2BGR)
cv2.imshow('HSVtoBGR',hsv2bgr)

cv2.waitKey(0)
cv2.destroyAllWindows()
```
### iii) Convert RGB and BGR to YCrCb
```py
cv2.imshow('RGB',img_rgb)

rgb2YcrCb = cv2.cvtColor(img_rgb,cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGBtoYCrCb',rgb2YcrCb)

bgr2YcrCb = cv2.cvtColor(img,cv2.COLOR_HSV2BGR)
cv2.imshow('BGRtoYCrCb',bgr2YcrCb)

cv2.waitKey(0)
cv2.destroyAllWindows()
```
### iv)Split and Merge RGB Image
```py
b,g,r = cv2.split(img)
cv2.imshow("RED MODEL", r)
cv2.imshow("GREEN MODEL", g)
cv2.imshow("BLUE MODEL ", b)

merger = cv2.merge([b,g,r])
cv2.imshow("MERGED IMAGE", merger)

cv2.waitKey(0)
cv2.destroyAllWindows()
```
#### v) Split and merge HSV Image
```py
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

<img height = "700" alt = "image" src="./BGRtoGRAY.png">
<img height = "700" alt = "image" src="./BGRtoHSV.png">

![BGR_Conv](https://user-images.githubusercontent.com/93427237/227734578-f05c2bb7-2b33-48ba-9008-5fada3a49771.png)

![RGB_Conv](https://user-images.githubusercontent.com/93427237/227734576-d70a773c-a512-4d33-9327-8c0164158478.png)

### ii) HSV to RGB and BGR
![HSV_Conv](https://user-images.githubusercontent.com/93427237/227734575-0986cc70-0a54-4de4-9ff1-7ca487fb2b05.png)
### iii) RGB and BGR to YCrCb
![YCrCb_Conv](https://user-images.githubusercontent.com/93427237/227734574-f593781f-b527-459d-bee8-a5e348fbe0e0.png)

### iv) Split and merge RGB Image
![RGB_Merge_Out](https://user-images.githubusercontent.com/93427237/227734572-938d83cf-a312-442d-ba43-f6f1b258e479.png)

![RGB_Split](https://user-images.githubusercontent.com/93427237/227734573-6efc275f-2a77-4c6e-93c2-60813eba092c.png)

### v) Split and merge HSV Image
![Split_HSV_Out](https://user-images.githubusercontent.com/93427237/227734569-5c9685f7-0c57-4fb3-940b-062e49e7c03e.png)

![Split_HSV](https://user-images.githubusercontent.com/93427237/227734571-7e801886-afa6-4ff4-b290-4912e38236f0.png)










## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
