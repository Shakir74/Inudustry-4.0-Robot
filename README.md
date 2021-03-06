# Title
Collaborative Robots in the Industrial Internet of Things (IIoT)

## Collaborative Robots (Cobots)
Industrial robots can be defined as a programmable, self-controlled device consisting of electronic, electrical, or mechanical units which can perform a complex series of actions. 
Normally, industrial robots are defined as application specific, isolated from human workforce and possess their own working space. In contrast, collaborative robots are robots, that are designed to figure along their human counterparts and share an equivalent working space as human co-workers. Compared to industrial robots, cobots have advantages of mobility, flexibility, light weight, multi tasker, easier programmable and better computing. In industry cobots applications can be specified such as:
1. Pick and Place
2. Packaging and Palletizing
3. Quality Control
4. Finishing tasks (polishing, grinding, deburring, gluing, dispensing, welding)
5. CNC Machine Tending

![alt text](https://github.com/Shakir74/Inudustry-4.0-Robot/blob/main/cobots.jpg)

## Industry 4.0
Industrial Internet of Things or IIoT is defined as machines, sensors, actuators, edges, computers and people enabling smart industrial operations using advanced data analytics for transformational business outcomes. With the advent of Internet of Things (IoT), cyber-physical systems and cloud computing, Industry 4.0 facilitates and induces advanced concepts based on the aforementioned technology to create "Smart Factories". cobots play a vital role in enabling process automation that continue evolving though software updates and their own programmability. With the advantages of Interoperability, Information Transparency, Technical assistance, Predictive capacity, and Adaptability Industry 4.0 and cobots are cruicial parts of Smart Factories.

![alt text](https://github.com/Shakir74/Inudustry-4.0-Robot/blob/main/industry%204.0.jpg)

## Objectives
1. Literature research on cobots and data interfaces to the Industrial IT and IIoT.
2. Development of concepts for cobots in IIoT.
3. Design and develop cobot Digital Twin for Industry 4.0.
4. Long period data customization with CODESYS PLC control unit. 
5. Develop cobot prototype for Industry 4.0.

## Requirements

1. **Sensors**: Cobot needs to sense the environment and should act according to the surrounding through numerous sensors. For the accessing of the sensors
several programming languages can be used such as C, C++, Python, Java. PLC technologies can serve the actuation process for cobots in industries.

| Sensors         | Functions | Positions |
| ------------- | ------------- | ------------ |
| Torque sensor  | Torque sensor can be integrated at each cobot joint to meet the safety requirements up to ISO standard. It increases accuracy and speed with low susceptibility to cross load  | Each joint |
| Force-Torque/FT sensor  | FT sensor is a device that is able to feel forces exerted in all directions. FT sensor is designed to monitor, detect, record and regulate linear and rotational forces exerted upon it.  | placed between the robot wrist and the robot tool (end-effector) |
| Tactile sensor  | Tactile sensors are used for object detection. For instance, these sensors to help acquire object detection from inside a gripper.  | gripper |
| Skin sensor  | can be attached to any robot and industrial gripper and will then continuously measure pressure and pressure changes. If there is a collision, for example when touching a human, the system sends a stop signal to the controller within 9 ms and the robot stops immediately.  | whole body, gripper |
| Collision detection sensor  | Robotic end-effector or device that can detect a crash before or during a collision of the robot or its tool.  | body |
| Depth Camera  | ??? Read and Scan a Barcode ??? Categorize a Product or Item by Color, Size, or Shape ??? Count Items ??? Adjust the Path of the Machine by Providing It with Feedback from the Vision System ??? Inspect Components for any Defects or Issues ??? Identify a Component Accurately  | body |

2. **Servo Motors**: Servo motor is a rotary actuator that allows for precise control of angular position, velocity and acceleration of robot arms.

3. **Encoders**:  Encoder is an electromechanical device which generates an electrical signal depending on the position or the displacement of the measured item. In robotics, rotary encoders are used to measure the movement (direction and speed) of each of the wheels of the robot.

4. **Industrial Communication**:

| Industrial Ethernet         | Fieldbus |
| ------------- | ------------- |
| ModBus-TCP, EtherCAT, EtherNet/IP, Profinet  | ModBus-RTU, Profibus, Interbus, CC-Link, DeviceNet  |

5. **Networking Protocol**: Protocol is the reason behind cobots can communicate through IIoT. In industry 4.0 there are some networking technologies for cobot integration including MQTT, CoAP, OPC UA.

6. **Data Science**: Data science performs with Big data analytics of volume, variety, velocity including industrial automation, predictive maintenance and Artificial Intellegence (AI) including Deep learing and Machine Learning.

7. **Cloud Computing**: After the encryption of cobot variables data by networking protocol, through cloud computing those variables data can be stored through IIoT process.

## Set-Up

![alt text](https://github.com/Shakir74/Inudustry-4.0-Robot/blob/main/physical%20setup.jpg)

## Control Unit

### CODESYS PLC
CODESYS is an IDE for soft PLC programming that implements to a great extent the IEC 61131-3 standard. CODESYS is hardware-independent and more than 250 hardware manufacturers use CODESYS for industrial equipments. 

**Graphical languages**: Ladder Diagrams, Function Block Diagrams, Instruction List, Structured Text.

**CODESYS Communication Protocols**: CODESYS has numerous conveniences and add-on functions which can facilitate immediately in I 4.0 applications for peripheral connectivity. Communication can be established with proprietary protocols via standard interfaces such as Ethernet/CAN/serial, with standard web protocols or with fieldbuses, with OPC UA, as well as with special industrial protocols. From CODESYS store \IIoT Libraries SL" contains various libraries to support different communication protocols like MQTT, HTTPS
including tools for encoding and decoding data structures.

**Berghof Controller**: Berghof Automation and Control offers the unique flexibility and functionality of the CODESYS software platform and it enables programmable visualization as well as programmable safety and motion control. Berghof controllers use Linux as a platform, so that a wide variety of software modules can be easily combined.

Cobots control unit can be summarized with following figure.

![alt text](https://github.com/Shakir74/Inudustry-4.0-Robot/blob/main/Untitled3.jpg)

## Digital Twin

Digital Twin as a virtual representation technology with lots of advanced benefits in contrast to industry 4.0 and it can be described as a digital replica of a physical cobot including data about this systems interaction with its environment. 

1. **Design**: From AutoCAD robot model I designed 6DoF cobot model in Digital Twin simulation software following Python kinematics, Articulated Kinematics, Kinematics Adjustment and Joints adjustment and developed following 6DoF cobot model. 

![alt text](https://github.com/Shakir74/Inudustry-4.0-Robot/blob/main/DTw.jpg)

2. **Coomunication**: OPC Ua communication functions with server-client communication and in this project, robot controller CODESYS PLC works as a server and DTw works as a client for real-time communication of physical and virtual robot.

3. **Virtual Representation**: after setting the communication in between physical and virtual robot, I got following Digital Twin real time virtual representation of my project's 6axis robot.

![alt text](https://github.com/Shakir74/Inudustry-4.0-Robot/blob/main/Untitled17(2).gif)

## MySQL Database

For cobot real time data customization after having neccessary communication setup using OPC UA, I stored the required cobot's PLC data in Microsoft Excel server using MySQL. 

![alt text](https://github.com/Shakir74/Inudustry-4.0-Robot/blob/main/MySQL.jpg)

## Features

1. Remote Robot monitoring with digital visualization.
2. Robotic Arm status monitoring with real-time update.
3. avoid any unnecessary or unwanted production loss with updated status of preventive maintenance.
4. Securing highly Safety Measurements in production areas.
5. Sequential Cobots Functionalities in a large production line.
6. Green cobot to avoid unwanted energy consumption.

The cobot was designed and functioned for Industry 3.0. In this project I developed the cobot prototype with requirements, control, communication, IT seup for Industry 4.0. Here are some used cases of this cobot prototype in Industry 4.0. I have also worked on another embedded IoT drone project which is available here https://github.com/Shakir74/IoT_Drone

