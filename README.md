jderobot
========

Here I have the development of several components which belong to JDErobot project [1], a SDK for robotic applications.

The components you can find here are:

basic_component: This component is a very simple tool that allows to get and reproduce image streaming from an ICE server. The main purpose of the tool is to provide a simple scheleton that can be used as a reference for future components more sofisticated.

gazeboserver: Gazeboserver acts as a middleware between Gazebo (robot simulator) and external applications using ICE as communications engine. Thanks to this component users can controll a robot simulated by Gazebo as well as get data from several sensors.

teleoperatorPC: TeleoperatorPC is a client that uses gazeboserver to send orders to a simulated robot on Gazebo. TeleoperatorPC provides a Graphical User Interface (GUI) that allows users to control a robot through simple buttons. In addition to control a robot, the user can see the robot sensors data on the GUI.

wiimote: wiimote is divided in two different proyects. In one hand a server that uses gazeboserver to operate with Gazebo and on the other hand a client that is managed using a wiimote. Therefore an user can take control of a robot using a wiimote and see what the behaviour in real time.

[1] http://jderobot.org/Main_Page
