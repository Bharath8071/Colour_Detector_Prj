# python --version[3.12.1]
import cv2
from PIL import Image
from colour_dect_set import get_limit

yellows =[0,255,0]

webcam = cv2.VideoCapture(0) 

while True:
    ret, frame = webcam.read()                # ret is a boolean variable that returns true if the frame is available
                                              #frame is an image array vector captured based on the default frames per second defined explicitly or implicitly

    hsvImage =cv2.cvtColor(frame,cv2.COLOR_BGR2HSV)
    cv2.imshow('hsv_frame',hsvImage)    #for debugging

    lowerlimit,upperlimit = get_limit(color=yellows)
    mask =cv2.inRange(hsvImage,lowerlimit,upperlimit )
    mask_=Image.fromarray(mask)
    cv2.imshow('mask',mask)
    #mask_.show()


    bbox=mask_.getbbox()
    #print(bbox) #for debugging 
    if bbox is not None: 
        x1,y1,x2,y2 =bbox
        frame=cv2.rectangle(frame,(x1,y1),(x2,y2),(0,255,0),3)
    
    cv2.imshow('final_frame',frame)
    if cv2.waitKey(1) & 0xFF == ord('q'):
        break

webcam.release()
cv2.destroyAllWindows()
