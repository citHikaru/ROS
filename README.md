# ROS
ROSとArduinoを通信してサーボモータを0~180°の範囲で制御できます。

# YouTube
・<a href="https://youtu.be/36kieCNJ7Kw" target=window>robosys2017 ArduinoとROSを通信</a>

# 必要なもの   
  * Arduino UNO   
* Servo motor  
  * Futaba S3003    
* Ubuntu 16.04  
* ROS  
  * kinetic Kame
# rosserialのインストール
```
$ sudo apt-get install ros-kinetic-rosserial ros-kinetic-rosserial-arduino
```
# 動作確認
```
$ roscore

$ rosrun rosserial_python serial_node.py _port:=/dev/ttyACM0

$ rostopic pub -1 /servo std_msgs/UInt16 0   <-- トピックに"0"を送る サーボが0度に動く
$ rostopic pub -1 /servo std_msgs/UInt16 180   <--トピックに"180"を送る サーボが180度に動く
```
