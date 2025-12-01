# workshop3:-Canny Edge Detection
# Name: K Charan Teja
# Reg No: 212224040163

# AIM:
To perform Canny Edge Detection model through your laptop.

# PROGRAM:
```
import cv2
import matplotlib.pyplot as plt
```
```
img = cv2.imread('charan.jpg',cv2.IMREAD_GRAYSCALE)
```
```
blurred =cv2.GaussianBlur(img, (5,5),0)
```
```
edges = cv2.Canny(blurred, 50, 150)
```
```
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```

# OUTPUT:
<img width="1112" height="560" alt="image" src="https://github.com/user-attachments/assets/1bcac856-63f9-4621-832e-074292bf8ee9" />



 
