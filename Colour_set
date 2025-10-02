import cv2
import numpy as np

def get_limit(color):
     
     c = np.uint8([[color]])  #unsigned-8 int has a range of 0 to 255 
     hsv = cv2.cvtColor(c, cv2.COLOR_BGR2HSV)
     #cv2.showcolor('hsv',hsv)
     lower = hsv[0][0][0] -10,100,100
     upper = hsv[0][0][0] +10,255,255

     lowerlimit =np.array(lower,dtype=np.uint8)
     upperlimit =np.array(upper,dtype=np.uint8)

     return lowerlimit,upperlimit 
