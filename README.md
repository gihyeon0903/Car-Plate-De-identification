# Car-Plate-De-identification

### Project Goal
- Car Plate De-identification

### Dependencies
- numpy 1.2+
- opencv-python 4.8+
- pytorch 2.0+

### Method

##### 1. Plate Detection
We detect car plate using yolov5<br>
<p align="center">
  <img src="./result/plate detection.png" width="300" height="200"/>
</p>

##### 2. 4-Corner Detection
We predict 4 corner of car plate using custom model<br>
<p align="center">
  <img src="./result/MNIST.webp" width="300" height="200"/>
</p>

##### 3. Classification
We classify car plate type using custom model (1996_b, 2004_n, ....)<br>
<p align="center">
  <img src="./result/MNIST.webp" width="300" height="200"/>
</p>



