# WRO-Speed_Warrios

Speed Warriors
Robot: EcoSight
Robotic Solution

We are a member of the Speed ​​Warriors team and part of the engineering team that has developed an "EcoSight" autonomous vehicle model to compete in the exciting 2023 WRO Future Engineers season. This repository is home to a wide range of engineering resources related to our autonomous vehicle, designed to meet challenging tests of speed and skill.
The Speed Warriors team has introduced an innovative robotic solution called EcoSight, which is based on a robot that utilizes various sensors to navigate and make decisions in the face of obstacles on the game track. This revolutionary approach relies on two key concepts: "Echolocation" and "Computer Vision," which are implemented through a combination of ultrasonic sensors and the OV7670 camera. In this way, the robot can obtain accurate information about its surroundings and effectively and strategically use it during the competition.


## Content

* `Team Photo`
In this section, we present an official photo of our talented Speed Warriors team. This image captures the spirit of collaboration and dedication that has led us to develop a high-performance autonomous vehicle for the WRO Future Engineers competition. Get to know the faces behind the project and discover the collective effort we have invested to achieve our goals.

* `Diagrams`
Here we present 4 comprehensive diagrams that showcase the internal workings and structure of our autonomous robot. These diagrams will provide you with a clear understanding of how we have designed and assembled each essential part of our vehicle, including the sensor system, control unit, actuators, and overall component arrangement.

* `Robot Photos`
In this section, you will find a variety of 6 detailed photos of our impressive robot. You will be able to closely explore its innovative design, components, and standout features. These images will allow you to appreciate the quality and precision with which we have built our autonomous vehicle for the WRO Future Engineers competition.

* `Programming`
In this section, you will find a wide range of programs and codes that we have developed for the operation of our autonomous robot. These programming files will provide you with detailed information on how we have programmed the navigation algorithms, obstacle detection, and decision-making capabilities of our vehicle. Additionally, you will find a special programming specifically designed for the WRO Future Engineers competition called "EcoSight - Program".

* `3D Model`
Here you can explore our 3D model of our autonomous vehicle in all its glory. This file will allow you to visualize our robot from different angles and perspectives, giving you a clear idea of its aesthetic design and functionality. You will be able to examine every detail and appreciate how we have optimized space and efficiency in our model.

* `3D Images`
Here you will find 6 impressive 3D images of our autonomous vehicle. These images will allow you to explore our robot from different angles and perspectives, appreciating how we have designed each component to optimize performance and efficiency. Admire the sophistication and elegance of our autonomous vehicle through these captivating 3D images.

* `Robot Video`
In this section, we provide a link to a video where you can witness our robot in action. 


## Introduction
To optimize the design, the solution was modeled in 3D and utilized a minimal number of components, allowing for space-saving. Additionally, simulations were conducted in virtual simulators like Tinkercad or Wokwi to validate its functionality. Great effort was dedicated to optimizing the size of the robot while also aiming to reduce the consumption of printing materials.

The components used in our prototype are as follows:
Microcontroller:
ESP-32 (1)
Sensors:
Ultrasonic sensors (4)
OV7670 Camera (1)
Motors:
12V Motor (2)
Servomotor (1)
Other components:
18650 Batteries (3)
LN298 Module (1)
Jumpers
LEDs

Functioning:
The starting point of the robotic prototype's journey involves the utilization of the four strategically placed sensors at its cardinal points. These sensors capture and provide accurate information about the distance between the robot and the surrounding objects. Once this data is obtained, the robot enters a second conditional processing phase that enables it to determine its precise location on the game track.

Based on this information, the prototype can take two distinct approaches to act accordingly. On one hand, it can choose to follow a predefined or previously programmed route, using sensor data to adjust its trajectory and avoid obstacles. This strategy is based on prior planning and precise execution to achieve the desired objective.

On the other hand, the prototype can also employ a more dynamic and adaptive approach. By utilizing sensor information, the robot can continuously assess its environment and make real-time decisions to avoid obstacles and reach its goal in the most efficient manner possible. This entails a higher capacity for reaction and adaptation to the changing conditions of the game environment.

First option: The robotic prototype extensively validates the data from the ultrasonic sensors to determine its exact position on the game track. It uses this information to follow a predetermined, optimized path that ensures a smooth, fast, and precise journey. The robot maintains a constant and safe pace by utilizing distance data recorded by the ultrasonic sensors, avoiding unnecessary stops to check for obstacles in its path.

By employing this predefined navigation system, the prototype achieves a significant reduction in travel time by avoiding unnecessary interruptions. Its ultimate goal is to efficiently and accurately complete the round, following an optimal route and effectively avoiding obstacles.

The strategy is based on maximizing the performance and effectiveness of the prototype during the competition by optimizing the planning and execution of the trajectory based on ultrasonic sensor data. Through thorough data validation and a predefined path, a smooth, fast, and safe journey is sought for the robot, enhancing its overall performance in the competition.

Second option: When the EcoSight system detects obstacles through the camera, a conditional logic is activated in program number 2. This program encodes variables and actions for the prototype to make dynamic decisions and adapt its trajectory to avoid obstacles. If an obstacle is detected, the prototype efficiently turns left or right.

The prototype utilizes camera data to identify the location and nature of the obstacles, determining the optimal direction to avoid them and encoding the necessary instructions for the corresponding turn. This real-time responsiveness and adaptation to obstacles are crucial for the prototype's success.

The combination of obstacle detection through the camera and appropriate programming allows the robot to make intelligent and agile decisions, ensuring smooth

 and safe movement during the competition.

Action-Reaction
Our action-reaction principle is based on the idea that all components of the vehicle must work in perfect harmony to achieve optimal performance. The following are the components and actions required to generate a reaction based on the received data.

1. When the vehicle is turned on, the first action is to activate the ultrasonic sensors, which will provide distance data to locate the prototype at a specific point on the track. These sensors are crucial for obstacle detection and proper positioning of the vehicle.

2. Once the prototype's location is known, the next action is to determine if there are any obstacles present. To achieve this, we have proposed the implementation of artificial intelligence (AI) capable of detecting such obstacles. Our team has decided to develop this AI using freely accessible and user-friendly tools like Teachable Machine. This way, we can leverage machine learning capabilities to train the system in obstacle detection.

3. Once the prototype knows its location and the presence of obstacles on the track, two possible reactions are triggered:

3.1. The first reaction is to act as if the prototype is in a round 1, meaning a track free of obstacles. To achieve this, we utilize known data such as the initial position, robot's speed, track size, robot's size, and turning angles. By using mathematical and physical principles, we can calculate a predefined route based on this data, thus avoiding the need to constantly read and analyze the known data, saving time and improving efficiency.

3.2. In the case that the prototype detects an obstacle, indicating a round 2, a second reaction takes place. Since round 2 features obstacles, it is necessary to reduce the speed of the motors to avoid errors due to excessive velocity.

3.2.1. The next action would be to monitor the color of the obstacles. This way, we can predefine the vehicle's reaction, which consists of reducing the speed of the DC motors and turning the servomotor in the appropriate direction to provide an optimal direction for the robot. This approach allows us to safely and efficiently navigate around obstacles.

In summary, the action-reaction principle of our robotics project is based on a systematic and precise approach to address various situations on the track. The combination of sensors, artificial intelligence, and mathematical algorithms enables us to make informed decisions and generate the appropriate responses to the received data.

Analyzable Information
To ensure the success of our robot's mission, it is crucial to implement an efficient system for data storage and analysis. This involves capturing and processing both physical variables obtained from sensors and virtual variables, which are internal counters defined in the code.

Regarding physical variables, the robot utilizes an ultrasonic sensor to gather data about the distance between the robot and nearby objects. The information captured by this sensor is sent to the ESP-32 board. Additionally, we have an OV7670 camera that provides visual data that can be analyzed for various purposes.

Regarding the connection and wiring of the sensors, the ultrasonic sensors are connected to the ESP-32 board. The Trig pin of the sensor is connected to an input port of the board, while the Echo pin is connected to an output port of the board. This allows the sensor data to be properly received and processed.

The power supply for the device is based on 18650 batteries, which act as the main power source. To ensure proper power supply to the board, a voltage regulator is used to reduce the 11.1V voltage from the batteries to the required 5V for the board's proper operation.

Additionally, the 18650 batteries also supply power to the robot's motors. For this purpose, an LN298 H-bridge is used, which allows controlling the flow of power to the motors and providing them with sufficient power for their

 operation.

In summary, to achieve the success of the robot's mission, it is essential to capture, store, and analyze both physical variables (ultrasonic sensor data and OV7670 camera) and virtual variables (internal counters). Additionally, proper connection of the sensors to the ESP-32 board and efficient power supply through 18650 batteries and an LN298 H-bridge are required to power both the board and the motors.
