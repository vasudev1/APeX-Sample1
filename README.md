# APeX Sample1
Sample Code utilizing APeX HDK, Raspberry Pi, and OpenCV

## Objective

This sample code illustrates a simple video analytics application utilizing the popular Raspberry Pi, a camera module, an APeX hardware kit, and a Cisco Aironet AP 3800

### Prerequisites
(1) APeX HDK plugged into Cisco Aironet AP3800 module port
(2) Aironet AP3800 connected to Wireless Lan Controller and a valid IP address
(3) Raspberry Pi connected to the APeX HDK (power and ethernet)
(4) Internet connectivity available on Raspberry Pi

### Executing sample application

Open a shell terminal on Raspberry Pi and run the following commands:
``` sh
sudo apt-get install python-wxgtk3.0 python-matplotlib python-opencv python-pip python-numpy
```
This will install a python based windowing toolkit, python bindings for OpenCV, and a Python package manager (pip)

If you are using a Raspberry Pi camera module, please ensure that it is enabled. Instructions to do so are available at the following link:
https://www.raspberrypi.org/documentation/usage/camera/README.md

Upon enabling the camera module, you can test it using the following command:
```sh
raspivid -t 0

You can also download Pi Camera python bindings by installing:
sudo apt-get install python-picamera
OR
sudo apt-get install python3-picamera (if you are using Python3)
```

If you are using a USB based webcam, you can test it by installing the guvcview tool, using the following command:
```sh
sudo apt-get guvcview
```

If you are using a DevNet Sandbox reservation instance, you can get instructions in the [Learning Lab](https://github.com/vasudev1/APeX-DevNet)

Once you have tested your camera interface on RPi, you are now ready to execute the sample application.

Log into the shell terminal of your Raspberry Pi and execute the following command to download the latest sample code:

```sh
git clone https://github.com/vasudev1/APeX-Sample1.git
cd APeX-Sample1
/// To run a script for face detection:
python facedetect.py
/// To run a script for people detection:
python peopledetect.py
```
You should see an output such as the following:
<Image coming soon> 


