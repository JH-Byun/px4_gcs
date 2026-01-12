# PX4_GCS #

## System ##
**Ubuntu**: 18.04, 20.04 <br>
**ROS**: ROS melodic, ROS noetic

## Updates ##
* Can be also utilized with Qt5

## Contributors ##
* #### *Hoseong Seo* (hosung9009@gmail.com) ####
* #### *Clark Youngdong Son* (clark.y.d.son@gmail.com) ####
* #### *Dongjae Lee* (dongjae713@gmail.com) ####
* #### *Jeonghyun Byun* (quswjdgus97@snu.ac.kr) ####

## Installation Guide ##
* #### Dependencies ####
1. ros-keyboard: https://github.com/lrse/ros-keyboard/tree/master 
* #### QtCreator ####
```
$ sudo apt-get install qtcreator
```
* #### ros-qt dependancies ####
```
$ sudo apt-get install ros-indigo-qt-build ros-indigo-qt-create
```

## Make ##
* #### package ####
In 'px4\_gcs' folder,
```
$ catkin_make
```
## Push button function ##
* #### add a push button ####
In Qtcreator with 'icsl\_gcs.ui' file, add an additional push button.
* #### define a slot function ####
Add an additional slot function in main\_window.hpp file with the name `on_NAMEOFPUSHBUTTON_clicked()` (e.g. `on_pushButton_connect_ros_clicked()`).
* #### fill content of the slot function ####
Write content in main\_window.cpp file.
