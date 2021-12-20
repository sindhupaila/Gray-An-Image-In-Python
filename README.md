# Gray-An-Image-In-Python

from google.colab import drive
import numpy as np
drive.mount("/content/drive")
import cv2
from google.colab.patches import cv2_imshow
img=cv2.imread("/content/drive/My Drive/Colab Notebooks/kenny-timmer--j1ljVSEGpY-unsplash.jpg",cv2.IMREAD_UNCHANGED)
print(img)
print('numpy and cv2 packages imported')
cv2.waitKey(1000)
gray_img=cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
cv2_imshow(gray_img)
