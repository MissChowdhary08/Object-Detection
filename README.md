# Object-Detection
# What is YOLO exactly?
YOLO (You Only Look Once) is a method / way to do object detection. It is the algorithm /strategy behind how the code is going to detect objects in the image.

Earlier detection frameworks, looked at different parts of the image multiple times at different scales and repurposed image classification technique to detect objects. This approach is slow and inefficient.
 
YOLO takes entirely different approach. It looks at the entire image only once and goes through the network once and detects objects. Hence the name. It is very fast. That’s the reason it has got so popular.

There are other popular object detection frameworks like Faster R-CNN and SSD that are also widely used.

# Installing dependencies
Following things are needed to execute the code we will be writing.
Python 3
Numpy
OpenCV Python bindings

# Python 3
If you are on Ubuntu, it’s most likely that Python 3 is already installed. Run python3 in terminal to check whether its installed. If its not installed use
   # sudo apt-get install python3

# Numpy
   # pip install numpy
This should install numpy. Make sure pip is linked to Python 3.x ( pip -V will show this info)
If needed use pip3. Use sudo apt-get install python3-pip to get pip3 if not already installed.

# OpenCV-Python
You need to compile OpenCV from source from the master branch on github to get the Python bindings. (recommended)
Adrian Rosebrock has written a good blog post on PyImageSearch on this. (Download the source from master branch instead of from archive)
If you are overwhelmed by the instructions to get OpenCV Python bindings from source, you can get the unofficial Python package using
  # pip install opencv-python
  
 # Pre-download requiremnts.
The script requires four input arguments.
1. input image
2. YOLO config file
3. pre-trained YOLO weights
4. text file containing class names

