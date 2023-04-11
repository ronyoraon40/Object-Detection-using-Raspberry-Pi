Change the path for following variables in the code according to your need:
1. classFile
2. configPath
3. weightsPath

Steps to operate and prepare Pi:
1. Enable Pi Camera and VNC
2. Update and Upgrade Raspberry pi
3. Update the formware and reboot
4. Upgrade the kernel
5. Install the dependencies
6. Install OpenCV using PIP

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
