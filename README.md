jderobot
========

Here you can find the development of several components which belong to JDErobot project [1], a SDK for robotic applications.

The components you can find here are:

basic_component: basic_compoment is the simplest component JDErobot consists of. The main purpose of this tool is to provide a simple code scheleton that can be used as a pattern in more sofisticated components. The component is able to connect to an ICE server and it gets images by streaming from it. The images are shown on a Graphical User Interface (GUI). Each process runs on a different thread and is handled by a common controller.

gazeboserver: Gazeboserver acts as an interface between Gazebo [2] (robot simulator) and other JDErobot components by using ICE as communications engine. Thanks to gazeboserver the funcionality of the JDErobot components as well as the robot artificial intelligence can be developed and tested on a robot simulated before setting them up on a real robot.

teleoperatorPC: TeleoperatorPC is a component that uses gazeboserver to send orders to a simulated robot on Gazebo as well as to request the robot's sensors data. TeleoperatorPC provides a Graphical User Interface (GUI) that allows users to control the robot by using virtual joysticks and buttons. In addition to control the robot, the user can see the robot sensors data, which are updated in real time, on the GUI.

wiimote: wiimote is a tool divided in two different components. A server that makes use of gazeboserver to communicate with Gazebo and a client that implements a driver that allows the communication with the wiimote device. Together both components brings to the user the possibility to control a simulated robot by using a wiimote. In addition to control the robot the user also can see the wiimote sensors data such as infrared and accelerometer information.

[1] http://jderobot.org/Main_Page
[2] http://gazebosim.org/
