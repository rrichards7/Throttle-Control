![eecs-header-mobile](https://user-images.githubusercontent.com/23239868/28728329-3dc1609e-7396-11e7-910b-6be87048d7d8.png)
# Autonomous Snowmobile Throttle Control #
*Lead Architect: Ryan J. Richards*

*The Pennsylvania State University - School of Electrical Engineering and Computer Science*

## Methodology ##

A custom servo motor [1] horn attachment was designed with SolidWorks to attach to the throttle cable of the snowmobile. Code was developed in LabVIEW to control the servo motor via **Pulse Width Modulation** (PWM).

## MakerHub LINX ## 
LINX is a library developed by MakerHub that allows programmers to interface with the RaspberryPi, Arduino and other microcontrollers on LabVIEW. LINX has been used extensively in this project to communicate with the ArduinoMEGA, which controls each subsystem. Download and other information can be found at:

[MakerHub LINX](http://sine.ni.com/nips/cds/view/p/lang/en/nid/212478)

## LabVIEW Code ##

Since LINX already has pre-built serco motor control VIs, it makes the setup incredibly simple:

![2](https://user-images.githubusercontent.com/23239868/28730876-aaa73324-739f-11e7-8d50-749ff2350a4a.PNG)

*Control instructions:*

(1) on the LabVIEW Front Panel select the **Serial Port** for the ArduinoMEGA

(2) choose the **Servo PWM Channel**

(3) run the VI and change the **Pulse Width uS** dial to control the degree rotation of the servo motor

(4) click the **Stop** button when finished to ensure that the Arduino VISA resource closes correctly

![ezgif com-crop](https://user-images.githubusercontent.com/23239868/28731039-5b8aecc6-73a0-11e7-9ec8-676900ab4153.gif)
![1](https://user-images.githubusercontent.com/23239868/28731081-7de710a6-73a0-11e7-9177-cf22d2c64da4.PNG)


## SolidWorks Throttle Assembly ##

The servo motor must connect to the snowmobile's throttle cable in order to push/release it - giving the motor more/less gas respectively. A simple solution has been designed and created in SolidWorks - which consists of two pieces (1) servo motor attachment and (2) cable lock. These parts were printed at Penn State's Makerbot Commons [2].

The servo motor attachment connects and locks onto a 4-way servo horn (to evenly distribute the torque). The attachment allows for the extension piece to move freely while the servo turns, which allows the cable to be pulled in a unique way (outward at an angle rather than a direct angle).

The cable lock connects to the throttle cable and the servo extension piece.

## Mounting ##

Mounting this throttle control is rather straight-forward. Two metal, industrial clamps are used to fix the servo motor itself to the snowmobile handlebar. The cable then is snapped into the cable lock piece. Follow the setup shown in the pictures below:

<img src="https://user-images.githubusercontent.com/23239868/28730743-44dd24ae-739f-11e7-8b64-c60eab6c9a3c.JPG" height="480" width="640">
<img src="https://user-images.githubusercontent.com/23239868/28730745-474df10a-739f-11e7-9099-c5867ac803b1.JPG" height="480" width="640">
<img src="https://user-images.githubusercontent.com/23239868/28730750-4e2472ce-739f-11e7-9040-945ccccf13b2.JPG" height="480" width="450">

## Appendix ##

[1] [Servo Motor](http://hitecrcd.com/products/servos/waterproof-servos-2/hs-5646wp-high-voltage-high-torque-programmable-digital-waterproof-servo/product)

[2] [Penn State Makerbot Commons](https://makercommons.psu.edu/)


