# Eclipse-Kuksa
Eclipse Kuksa Ide support deals with the creation of Yocto-based SDK and then integrating it with the Eclipse Che application tools.
Yocto based SDK-
Yocto helps to create embedded linux distributions.Yocto has a build system which uses openembedded project,which uses the bitbake tool .These two are combinedly used to form poky,a reference build system.
This  project uses Krogoth master branch.
The Image (Software Development Kit(SDK)) is generated by using bitbake tool. 
The image is then transferred to a SD card.The SD card is then partitioned using a Gparted Editor .The SD card is then implemented on Raspberrypi target.This leads to the building of Automated Grade Linux in form of Yocto distro(2.1.3).
The image (SDK) also contains various packages such as dpkg,apt,git,opk and rpm. 
The Eclipse Kuksa IDE support  is made to be implemented in vehicles so this project also aims at monitoring vehicle pollution by using MQ-7 sensor(CO sensor).This is done by including wiringpi or I2C tools in the raspberrypi to take MQ-7 sensor data.
The built SDK is then included with Eclipse Che .Eclipse Che is a web based IDE based on docker container.Eclipse Che tools are later used to monitor pollution and build Eclipse Kuksa Ide support.
