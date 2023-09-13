# COLOR-CONVERSION
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
Split and merge the image using cv2.split(hsv) and cv2.merge([h,s,v]).

### Step5:
Output the image using cv2.imshow("OUTPUT", image).

## Program:
```python
# Developed By: JEEVITHA E
# Register Number: 212222230054
```
# i) Convert BGR and RGB to HSV and GRAY
```
import cv2
houseImage = cv2.imread('d.jpeg')
cv2.imshow('212222230054_jeevitha',houseImage)
hsvImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsvImage)
hsvImage1=cv2.cvtColor(houseImage,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsvImage1)
grayImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',grayImage)
grayImage1 = cv2.cvtColor(houseImage,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',grayImage1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```




# ii)Convert HSV to RGB and BGR
```
import cv2
houseHSVImage = cv2.imread('d.jpeg')
cv2.imshow('212222230054_jeevitha',houseHSVImage)
RGBImage = cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2RGB)
cv2.imshow('BGR2HSV',RGBImage)
BGRImage=cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',BGRImage)
cv2.waitKey(0)
cv2.destroyAllWindows()
```




# iii)Convert RGB and BGR to YCrCb
```
import cv2
houseImage = cv2.imread('d.jpeg')
cv2.imshow('212222230054_jeevitha',houseImage)
YCrCb_image = cv2.cvtColor(houseImage, cv2.COLOR_RGB2YCrCb)
cv2.imshow('BGR2HSV',YCrCb_image)
YCrCb_image1 = cv2.cvtColor(houseImage, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2HSV',YCrCb_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```



# iv)Split and Merge RGB Image
```
import cv2
image = cv2.imread('d.jpeg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('212222230054_jeevitha',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()
```



# v) Split and merge HSV Image
```

import cv2
image = cv2.imread('d.jpeg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('212222230054_jeevitha',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindow()
```



## Output:
### i) BGR and RGB to HSV and GRAY
![WhatsApp Image 2023-09-13 at 17 16 05](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/f87b1ac3-e0d8-4543-a78e-7eaf805cfb42)

![WhatsApp Image 2023-09-13 at 17 18 09](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/f5a4e93a-6cc3-4ec4-ad4b-77a1d04cc2d9)

![WhatsApp Image 2023-09-13 at 17 18 10](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/4bc79c62-fdfd-474a-bc81-9e0a43deae98)

![WhatsApp Image 2023-09-13 at 17 18 10](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/072697d2-38e0-4495-b955-bf94016049ba)

![WhatsApp Image 2023-09-13 at 17 18 10](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/e8c69361-cf3a-4ff4-a3ba-d590f4c6a3a9)


### ii) HSV to RGB and BGR
![WhatsApp Image 2023-09-13 at 17 16 27](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/7e757a10-560c-42b8-9add-f959b88e0e98)
![WhatsApp Image 2023-09-13 at 17 18 10](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/7235ebcf-5817-4849-8860-62f34bb85a04)



### iii) RGB and BGR to YCrCb
![WhatsApp Image 2023-09-13 at 17 16 27](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/1889d0ab-5a75-4405-8393-50aeb4d7eac2)
![WhatsApp Image 2023-09-13 at 17 16 27](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/079fc6eb-e846-45ee-a640-f9bed922f31d)



### iv) Split and merge RGB Image
![WhatsApp Image 2023-09-13 at 17 16 02](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/6e1295c3-188a-4166-91e5-c8bafc94e470)
![WhatsApp Image 2023-09-13 at 17 16 03](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/5d55fab7-b5f4-46bd-8154-45ae3d43c4b1)
![WhatsApp Image 2023-09-13 at 17 16 04](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/7e63b05f-ca6d-4887-9bcf-5074e3c04e5f)
![WhatsApp Image 2023-09-13 at 17 16 05](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/fda2ebae-b1d1-4691-9ad9-7b1729348e0c)
![WhatsApp Image 2023-09-13 at 21 50 52](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/44af507d-c9e4-495e-b2d9-866910ade99b)







### v) Split and merge HSV Image
![WhatsApp Image 2023-09-13 at 17 15 41](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/3d897e53-9e0b-4dc2-ae22-eab310881d01)

![WhatsApp Image 2023-09-13 at 17 15 56](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/787e8e6c-66ac-45eb-bbaa-2425a43d4949)

![WhatsApp Image 2023-09-13 at 17 16 01](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/94bb2d49-054e-4a89-ae9c-ffbfd22c30d4)

![WhatsApp Image 2023-09-13 at 17 16 01](https://github.com/Jeevithaelumalai/COLOR-CONVERSION/assets/118708245/c6ed5d5f-0869-4e52-b0bc-d2e3453b15b2)




## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
