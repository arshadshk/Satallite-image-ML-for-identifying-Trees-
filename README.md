# Deep Learning - Custom Aerial Image Recognition 

This repository contains a set of python scripts for creating a list of annotations(in xml) based on the user defined bounding box on multiple set of aerial images and the visualization of the detection accuracy. This list of annotation files can thus be used for the training purpose using Deep-Neural-Networks (YOLO v.2 neural detectors) based on Darknet( A custom GPU-accelerated Framework) for near real time aerial object detection and classification. After labelling, the set of images with their accurate bounding box were trained on GPU accelerated server with NVIDIA Tesla P100 SMI 16 GB for nearly an hour. The resulting weights and configuration files were then loaded on the script (visualization.py) to visualize the detection accuracy.

Dependencies: 

1. OpenCV 3
2. Python 3, Matplotlib, Numpy
3. Darkflow(Open Source Neural Network Darknet in C translated to tensorflow) 
4. CUDA 
5. Tensorflow 1.0 

## Results

![unnamed](https://user-images.githubusercontent.com/7304644/38349784-cfc08a0e-38d2-11e8-9f86-401ba5a57dbe.png)

<img width="777" alt="screen shot 2018-04-05 at 12 52 09 pm" src="https://user-images.githubusercontent.com/7304644/38350048-d7231c3e-38d3-11e8-9b77-defd13cb1222.png">

<img width="871" alt="screen shot 2018-04-05 at 12 52 44 pm" src="https://user-images.githubusercontent.com/7304644/38350183-65f72522-38d4-11e8-8351-eaeeca4d7dd5.png">


## FUTURE WORKS

These initial results demonstrate that provided a large training dataset (approx. 5 times more than current ) with good quality labeled images and intensive training time, YOLO v2 net can accurately detect palm trees in our project area. As for now, the training spends more time per epoch resizing than training due to large resolution images, therefore, to increase performance the future prospects of our work would focus on cutting each images into 36 different images making 666x500 pixel blocks. 



ENJOY
Thank you 
