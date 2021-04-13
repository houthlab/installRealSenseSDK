# installLibrealsense
This project is cloned from jetsonhacks/installRealSenseSDK
> https://github.com/jetsonhacks/installRealSenseSDK
## Introduction
This source code is used to build python3 environment by cmake.
## Test environment
* Nvidia Jetson xavier NX Developer KIT
* JetPack 4.5.1 from Jetson NX Developer Kit SD Card Image 
* intel REALSENSE D435i
## Building From Source
```
$ git clone https://github.com/jetsonhacksnano/installLibrealsense  
$ cd installLibrealsense  
$ ./installLibrealsense.sh  
$ ./buildLibrealsense.sh  
$ sudo apt-get install libcanberra-gtk-module libcanberra-gtk3-module  
$ sudo reboot  
```
### Test RealSense viewer
```
realsense-viewer
```
### copy the build output 
* search two files
  * librealsense2.so  (cd librealsense/build)
  * pyrealsense2.cpython-35m-arm-linux-gnueabihf.so (cd librealsense/build/wrappers/python)
* copy these files and paste on librealsense/build/wrappers/python
### test python examples
```
$ cd librealsense/build/wrappers/python/examples
$ python3 opencv_viewer_example.py 
```

