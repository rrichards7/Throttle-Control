![eecs-header-mobile](https://user-images.githubusercontent.com/23239868/28728329-3dc1609e-7396-11e7-910b-6be87048d7d8.png)
# Autonomous Snowmobile Throttle Control #
*Lead Architect: Ryan J. Richards*

*The Pennsylvania State University - School of Electrical Engineering and Computer Science*

## Methodology ##

A custom servo motor horn attachment was designed with SolidWorks to attach to the throttle cable of the snowmobile. Code was developed in LabVIEW to control the servo motor via **Pulse Width Modulation** (PWM).

## MakerHub LINX ## 
LINX is a library developed by MakerHub that allows programmers to interface with the RaspberryPi, Arduino and other microcontrollers on LabVIEW. LINX has been used extensively in this project to communicate with the ArduinoMEGA, which controls each subsystem. Download and other information can be found at:

[MakerHub LINX](http://sine.ni.com/nips/cds/view/p/lang/en/nid/212478)

## LabVIEW Code ##

Since LINX already has pre-built serco motor control VIs, it makes the setup incredibly simple:

![2](https://user-images.githubusercontent.com/23239868/28730876-aaa73324-739f-11e7-8d50-749ff2350a4a.PNG)

Control instructions:

(1) on the LabVIEW Front Panel select the **Serial Port** for the ArduinoMEGA

(2) choose the **Servo PWM Channel**

(3) run the VI and change the **Pulse Width uS** dial to control the degree rotation of the servo motor

(4) click the **Stop** button when finished to ensure that the Arduino VISA resource closes correctly

![ezgif com-video-to-gif 2](https://user-images.githubusercontent.com/23239868/28730651-ff98549a-739e-11e7-9b17-23615d583ab2.gif)



## SolidWorks Throttle Assembly ##




## Mounting ##
![img_0123](https://user-images.githubusercontent.com/23239868/28730743-44dd24ae-739f-11e7-8b64-c60eab6c9a3c.JPG)
![img_0118](https://user-images.githubusercontent.com/23239868/28730745-474df10a-739f-11e7-9099-c5867ac803b1.JPG)
![img_0115](https://user-images.githubusercontent.com/23239868/28730750-4e2472ce-739f-11e7-9040-945ccccf13b2.JPG)









## Future Considerations ##

programming based on velocity indicator

