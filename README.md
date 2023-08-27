# Time-of-Flight-ToF-Point-Cloud-Processing

The *Time-of-Flight (ToF)* camera operates based on the principle of measuring the time taken by light to travel from the camera to an object and back. This measurement allows the camera to calculate the distance between itself and the object, enabling the creation of a depth map that represents the spatial layout of the scene. Here's a concise breakdown of its working principle:

**1. Light Emission:** The ToF camera emits short bursts of light, often in the form of *infrared (IR) pulses*, toward the scene being captured. These light pulses are emitted at a rapid rate.

**2. Reflection:** When these light pulses encounter objects in the scene, they reflect off those objects and return to the camera.

**3. Time Measurement:** The camera's sensor measures the time it takes for each emitted light pulse to travel to the object and then return to the camera. This measurement is typically done in nanoseconds or picoseconds.

**4. Distance Calculation:** Using the constant speed of light, the camera calculates the distance between itself and the object. The formula ***Distance = Speed of Light × Time of Flight / 2*** is applied. The division by 2 accounts for the round trip of the light pulse.

**5. Depth Mapping:** By repeating this process for numerous light pulses emitted at different intervals, the camera generates a series of distance measurements. These measurements are used to construct a depth map, where each pixel corresponds to a distance measurement.

**6. Depth Interpretation:** The depth map enables the ToF camera to create a three-dimensional representation of the scene. Darker areas in the depth map correspond to objects closer to the camera, while lighter areas represent objects farther away.

**7. Applications:** *Time-of-Flight cameras* find applications in various fields, including *robotics*, *Quality Control*, *augmented reality*, *gesture recognition*, and *3D scanning*. Their ability to rapidly capture depth information in real-time makes them valuable tools for tasks requiring spatial understanding and interaction.

So In this Grand Project Named ***Safe Rail*** I am using [Basler Blaze 101 - Time of Flight Camera](https://www.baslerweb.com/en/products/cameras/3d-cameras/basler-blaze/blaze-101/) manufactured by a german company named [Basler AG - Computer Vision Expert](https://www.baslerweb.com/en/). 

Balser Blaze 101 - Time of Flight Sensor:

![image-blaze-101](https://github.com/SamiUddin-tech/Time-of-Flight-ToF-Point-Cloud-Processing/assets/81253183/65382601-424b-43d7-9a95-865ebd5bd013)![machinevision-basler-3d-tof_cameras-blaze-101-1-1](https://github.com/SamiUddin-tech/Time-of-Flight-ToF-Point-Cloud-Processing/assets/81253183/2cd51403-e5f8-47e5-b917-5659c9b975fb)

## Calibration of Balser Ace2 1920-160ucPro along with Basler Blaze 101 - 160ucPro

Setting Up Environemnt For Calibration 

![1692431724815](https://github.com/SamiUddin-tech/Time-of-Flight-ToF-Point-Cloud-Processing/assets/81253183/f7357cc5-e46e-4086-a787-bf6f57817611)

## Real Time Point Cloud Accquisition from Real TOF Sesnor: Point Cloud Accquisition from Balser Blaze 101 Time of Flight Sensor at 30 FPS

## VISUAL FUSION: Merging Color Data of Basler 2D Camera Balser Ace2 1920-160ucPro with Basler Blaze Depth Data

## Real Time Point Cloud Registeration: Stiching of RGBD Point Cloud from 2 different fused pairs of Balser Blaze 101 and Balser Ace2 1920-160ucPro

## Real Time Point Cloud Segemntation: Segmentation of RGBD Point Cloud generated from a pair of Balser Blaze 101 and Balser Ace2 1920-160ucPro
