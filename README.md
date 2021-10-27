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

### Sensing and Actuation

1. **Sensors**: Cobot needs to sense the environment and should act according to the surrounding through numerous sensors. For the accessing of the sensors
several programming languages can be used such as C, C++, Python, Java. PLC technologies can serve the actuation process for cobots in industries.

| Sensors         | Functions | Positions |
| ------------- | ------------- | ------------ |
| Torque sensor  | Torque sensor can be integrated at each cobot joint to meet the safety requirements up to ISO standard. It increases accuracy and speed. With low susceptibility to cross load  | Each joint |
| Force-Torque/FT sensor  | FT sensor is a device that is able to feel forces exerted in all directions. FT sensor is designed to monitor, detect, record and regulate linear and rotational forces exerted upon it.  | placed between the robot wrist and the robot tool (end-effector) |
| Tactile sensor  | Tactile sensors are used for object detection. For instance, these sensors to help acquire object detection from inside a gripper.  | gripper |
| Skin sensor  | can be attached to any robot and industrial gripper and will then continuously measure pressure and pressure changes. If there is a collision, for example when touching a human, the system sends a stop signal to the controller within 9 ms and the robot stops immediately.  | whole body, gripper |
| Collision detection sensor  | Robotic end-effector or device that can detect a crash before or during a collision of the robot or its tool.  | body |
| Depth Camera  | • Read and Scan a Barcode • Categorize a Product or Item by Color, Size, or Shape • Count Items • Adjust the Path of the Machine by Providing It with Feedback from the Vision System • Inspect Components for any Defects or Issues • Identify a Component Accurately  | body |

2. **Servo Motors**: Servo motor (or servo) is a rotary actuator that allows for precise control of angular position, velocity and acceleration.

3. **Encoders**:  Encoder is an electromechanical device which generates an electrical signal depending on the position or the displacement of the measured item. In robotics, rotary encoders are used to measure the movement (direction and speed) of each of the wheels of the robot.
