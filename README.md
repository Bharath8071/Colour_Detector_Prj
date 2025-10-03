# Object Detection using colour with OpenCV
A simple and extensible Python project to **detect the object based on the colour** from an image or pixel value using OpenCV and NumPy.


## Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Working](#project-working)
- [Installation](#installation)
- [Future Enhancements](#future-enhancements)
- [License](#license)


## Features

- Detects objects from images or pixel values  
- Built with **Python + OpenCV**  
- Easily extendable to include more colors  
- Lightweight and beginner-friendly  

## Tech Stack

- Python 3.9+  
- OpenCV  
- NumPy

## Project Working

This project detects objects **based on their color** using your webcam in real-time.  

1. **Set Color**  
   - Open the `set_colour` module and define the target color by updating the color code (RGB/HSV).  

2. **Live Camera Input**  
   - The program uses your webcam to capture video frames continuously.  

3. **Color Detection**  
   - Each frame is analyzed to find pixels matching the target color.  
   - A mask is applied to isolate the colored regions.  

4. **Object Highlighting**  
   - Detected objects are outlined with bounding boxes or highlighted in the frame.  

5. **Real-Time Output**  
   - The processed video is displayed live with the detected colored objects.  
   - You can change the target color anytime by updating the `getcolour` module.


## Installation

 1. Clone the repository: git clone https://github.com/Bharath8071/Colour_Detector_Prj.git
 2. Navigate to the project directory: `cd Colour_Detector_Prj`


## Future Enhancements

-Expand color dataset (more shades, custom colors)
-Build a GUI or web interface
-Support clustering for dominant color detection

## License

This project is licensed under the MIT License. See the LICENSE file for details.
