# ROS
ROSとArduinoを通信してサーボモータを0~180°の範囲で制御できます。

# YouTube
・<a href="https://youtu.be/36kieCNJ7Kw" target=window>robosys2017 ArduinoとROSを通信</a>

# 必要なもの   
  Arduino UNO   
* Servo motor  
  *Futaba S3003    
* Ubuntu 16.04  
* ROS  
  *kinetic Kame

```
sudo apt install ros-kinetic-urg-node
cd ~/catkin_ws/src
git clone https://github.com/zaki0929/navigation.git
git clone https://github.com/AtsushiSaito/lab_usb_9axisimu_driver.git
git clone https://github.com/zaki0929/raspimouse_navigation_2.git
```
