This project is based on detecting objects from picamera which is connected to raspberry pi. The model is mounted on top of a cap. Whenever an object is detected in front of the cap, buzzer will turn ON and the object is marked with a rectangular boundary along with the name of the object.
You can select objects names from the coco file attached in the code.
This project is completely based on object detection algorithm.
Future Reference: You can implement this project for detecting objects and getting a voice output using gtts python package that will speak out the detected object name.

Change the path for following variables in the code according to your need:
1. classFile
2. configPath
3. weightsPath

#Enable Pi Camera and VNC

sudo raspi-config

  Go to Interfaces->
  
	Enable PiCamera
	  
	Enable VNC
    
#Update and upgrade rapberry pi

	sudo apt-get update && sudo apt-get upgrade

#Update the firmware

	sudo rpi-update -> Press 'y' when prompted

#Reboot

	sudo reboot

#Upgrade the kernel (Use this command only for object detection projects)

	sudo apt-get dist-upgrade

#Install the following dependencies (Dude this might take a while to install. Take a break, leave it as it is and it will install)

	sudo pip3 install pillow
	sudo pip3 install lxml
	sudo pip3 install jupyter
	sudo pip3 install matplotlib
	sudo pip3 install cython

#Install OpenCV dependencies

	sudo apt-get install libjpeg-dev libtiff5-dev libjasper-dev libpng12-dev
	sudo apt-get install libavcodec-dev libavformat-dev libswscale-dev libv4l-dev
	sudo apt-get install libxvidcore-dev libx264-dev
	sudo apt-get install libatlas-base-dev
	sudo apt-get install python-tk
	sudo apt-get install qt4-dev-tools libatlas-base-dev

#Install OpenCV

	sudo pip3 install opencv-python

Note: If opencv is installed in your system but facing problem in running the code, please follow my facial recognition for installing OpenCV.
