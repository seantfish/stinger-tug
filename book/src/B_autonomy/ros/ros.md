The Robot Operating System (ROS) is a common middleware enabling communication between different software processes for robots. In robotics, there are many different problems which must be solved to enable complex behavior, and various programs have been written to solve the independent problems. ROS was created to enable people to use various independently developed programs together in one system. The first generation of ROS will soon be deprecated and is being replaced by ROS 2. Of course, software needs to be able to communicate with actuators or else the robot will not be able to do much at all!

## A Brief Introduction to ROS

ROS has several key concepts which describe how programs communicate:

- **Topics:** A topic is a virtual bus for data which can be thought of as similar to a shared variable between programs. It has a pre-defined format or data structure called a **message type**, and any data that is sent to the topic must be the correct message type.

- **Nodes:** A node in ROS is a program (executable) which may execute some action or behavior, such as converting an image from color to greyscale. A node can **publish** data to a topic and **subscribe** to retrieve the latest data from a topic.

- **Publisher:** A publisher is a process that can be created inside of a node to push data to a topic

- **Subscriber:** A subscriber is a process that can be created inside of a node to retrieve the latest data from a topic automatically and execute a callback function to handle that data.

There are also more advanced concepts such as services and actions which are used in more specific situations.
