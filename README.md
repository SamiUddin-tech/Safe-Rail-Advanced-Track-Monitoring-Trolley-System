# Time-of-Flight-ToF-Point-Cloud-Processing

## Time of Flight Working Principle

![20200501_Time_of_flight svg](https://github.com/SamiUddin-tech/Time-of-Flight-ToF-Point-Cloud-Processing/assets/81253183/2be4ca21-a279-421b-8ae3-9488fc117181)

Image Source: [Wikipedia](https://en.wikipedia.org/wiki/Time_of_flight)

The *Time-of-Flight (ToF)* camera operates based on the principle of measuring the time taken by light to travel from the camera to an object and back. This measurement allows the camera to calculate the distance between itself and the object, enabling the creation of a depth map that represents the spatial layout of the scene. Here's a concise breakdown of its working principle:

**1. Light Emission:** The ToF camera emits short bursts of light, often in the form of *infrared (IR) pulses*, toward the scene being captured. These light pulses are emitted at a rapid rate.

**2. Reflection:** When these light pulses encounter objects in the scene, they reflect off those objects and return to the camera.

**3. Time Measurement:** The camera's sensor measures the time it takes for each emitted light pulse to travel to the object and then return to the camera. This measurement is typically done in nanoseconds or picoseconds.

**4. Distance Calculation:** Using the constant speed of light, the camera calculates the distance between itself and the object. The formula ***Distance = Speed of Light × Time of Flight / 2*** is applied. The division by 2 accounts for the round trip of the light pulse.

**5. Depth Mapping:** By repeating this process for numerous light pulses emitted at different intervals, the camera generates a series of distance measurements. These measurements are used to construct a depth map, where each pixel corresponds to a distance measurement.

**6. Depth Interpretation:** The depth map enables the ToF camera to create a three-dimensional representation of the scene. Darker areas in the depth map correspond to objects closer to the camera, while lighter areas represent objects farther away.

**7. Applications:** *Time-of-Flight cameras* find applications in various fields, including *robotics*, *Quality Control*, *augmented reality*, *gesture recognition*, and *3D scanning*. Their ability to rapidly capture depth information in real-time makes them valuable tools for tasks requiring spatial understanding and interaction.

# Project: Safe Rail - Development of Advanced Rail Track Inpsection and Monitoring Trolley system using High Speed RGB Cameras and Time of Flight Sensor.

![Rail_v4](https://github.com/SamiUddin-tech/Time-of-Flight-ToF-Point-Cloud-Processing/assets/81253183/d4df7086-458a-45fe-8d57-ebf16c340b6b)

## Bill of Materials (BOM):
1. [Basler Blaze 101 - Time of Flight Camera](https://www.baslerweb.com/en/products/cameras/3d-cameras/basler-blaze/blaze-101/)
2. [ a2A1920-160ucPRO - Basler ace 2](https://www.baslerweb.com/en/products/cameras/area-scan-cameras/ace2/a2a1920-160ucpro/)
3. [Ace 2 to blaze mounting bracket - Mounting](https://www.baslerweb.com/en/products/accessories-and-bundles/ace-2-to-blaze-mounting-bracket/)
4. [Cable GigE M12, M, 8P/RJ45, 10 m - Data Cable](https://www.baslerweb.com/en/products/cable/cable-gige-m12-m-8p-rj45-10-m/)
5. [Power-I/O Cable M12, M, 8P/Open,10 m - I/O / Power Cables](https://www.baslerweb.com/en/products/cable/power-i-o-cable-m12-m-8p-open-10-m/)
6. [ Power Cable M12 8-pin, DC Jack 5.5/2.1mm - Adapter Cable](https://www.baslerweb.com/en/products/cable/power-cable-m12-8-pin-dc-jack-5-5-2-1mm/)
7. Camera Mounts are designed and manufactured by [Zambeel Machine Craft](https://www.zambeel.ltd/)
8. [WitMotion WTGAHRS2 10 Axis GPS Navigation Position Speed Tracker Sensor Accelerometer + Gyro + Angle + Magnetometer + Barometer](https://www.wit-motion.com/10-axis/witmotion-wtgahrs2-10-axis.html)
9. [OAK - D - POE](https://shop.luxonis.com/products/oak-d-poe)
10. [USW-Lite-8-POE (52W)](https://store.ui.com/us/en/products/usw-lite-8-poe)
11. [POE Injector](https://shop.luxonis.com/products/poe-injector?variant=43731965673695)

So In this Grand Project Named ***Safe Rail*** I am using [Basler Blaze 101 - Time of Flight Camera](https://www.baslerweb.com/en/products/cameras/3d-cameras/basler-blaze/blaze-101/) manufactured by a german company named [Basler AG - Computer Vision Expert](https://www.baslerweb.com/en/). 

### 1. Balser Blaze 101 - Time of Flight Sensor
1. Basler Blaze 101 - Time of Flight (ToF) Camera
![image-6](https://github.com/SamiUddin-tech/Time-of-Flight-ToF-Point-Cloud-Processing/assets/81253183/b8ed3293-5770-43fc-83ac-414e8339c92a)

### 2. a2A1920-160ucPRO - Basler ace 2

![Untitled](https://github.com/SamiUddin-tech/Safe-Rail-Advanced-Track-Monitoring-Trolley-System/assets/81253183/23483572-eae2-43e7-8264-4607c82f213b)

### Rail Inspection Vehicle

![IMG_20230607_102546](https://github.com/SamiUddin-tech/Safe-Rail-Advanced-Track-Monitoring-Trolley-System/assets/81253183/6830cabc-94f1-4f8d-be74-171986f1c262)

### Camera Mounts

![imgonline-com-ua-twotoone-KYenDHiK1T0](https://github.com/SamiUddin-tech/Safe-Rail-Advanced-Track-Monitoring-Trolley-System/assets/81253183/1f0665af-e336-4874-8692-49c161615302)



## Calibration of Balser Ace2 1920-160ucPro along with Basler Blaze 101 - 160ucPro

Setting Up Environemnt For Calibration 

[LinkedIn Highlights](https://www.linkedin.com/posts/sami-uddin-a6b40b20a_computervision-cameracalibration-camras-activity-7098573158764490752-0OX7?utm_source=share&utm_medium=member_desktop)

![1692431724815](https://github.com/SamiUddin-tech/Time-of-Flight-ToF-Point-Cloud-Processing/assets/81253183/f7357cc5-e46e-4086-a787-bf6f57817611)

*Here is an interesting observation: As of today, there has not been an individual in my country, Pakistan, who possesses hands-on experience with **Basler Blaze 101 Time of Flight Sensors** in the field of Computer Vision.*

## Real Time Point Cloud Accquisition from Real TOF Sesnor: Point Cloud Accquisition from Balser Blaze 101 Time of Flight Sensor at 30 FPS

## VISUAL FUSION: Merging Color Data of Basler 2D Camera Balser Ace2 1920-160ucPro with Basler Blaze Depth Data

## Real Time Point Cloud Registeration: Stiching of RGBD Point Cloud from 2 different fused pairs of Balser Blaze 101 and Balser Ace2 1920-160ucPro

## Real Time Point Cloud Segemntation: Segmentation of RGBD Point Cloud generated from a pair of Balser Blaze 101 and Balser Ace2 1920-160ucPro
