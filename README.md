# Car-Plate-De-identification

### Project Goal
- Car Plate De-identification
--------------

### Dependencies
- numpy 1.2+
- opencv-python 4.8+
- pytorch 2.0+
--------------

### Method
#### 1. Plate Detection
We detect car plate using yolov5.<br>
<p align="center">
  <img src="./results/plate detection.jpg" width="300" height="350"/>
</p>

#### 2. 4-Corner Detection
We predict 4 corner of car plate using custom model.<br>
<p align="center">
  <img src="./results/4 corner detection.png" width="700" height="90"/>
</p>

#### 3. Classification
We classify car plate type using custom model. (1996_b, 2004_n, ....)<br>
<p align="center">
  <img src="./results/classification.png" width="500" height="120"/>
</p>

#### 4. De-Identification
We make natural car plate using De-Identification technique in three steps below.<br>
- 1. Generate artificial plate
- 2. Transfer style of original plate to artificial plate
- 3. Synthesize plate

<br>

> #### i. Generate artificial plate
> - Define Position of {Digit(숫자), Word(문자), Region(지역)} in plate (fig.i-1)<br>
> - Randomly generates characters that may appear depending on the type of license plate<br>
> - Sampling image matching Generated characters from DataBase(fig.i-2)<br>
> - Attach image to car plat frame(fig.i-3)
<p align="center">
  <img src="./results/de identification1.png" width="300" height="110"/>
  <img src="./results/de identification2.png" width="300" height="80"/>
  <img src="./results/de identification3.png" width="270" height="150"/>
</p>

