# robot-tasks-specifications
This repository has all the specifications (classes in C++ and python) needed to use a predifined industrial task.

## Typical Industrial tasks.
A typical industrial task is compose of the following elements:

> ##### Type of Task (Inspection, Transportation, Manipulation and composed).

> ##### List of Goals positions (Goal Poses).

> ##### Time at the goal position (optional).

> ##### Surface in which the object is placed. (static surface, conveyor belt, rotating surface, etc.)

> ##### Object (the object to inspect, manipulate and/or transport).

### Type of Task (Inspection, Transportation, Manipulation and composed).
Each tasks vary in complexity, this complexity depends on the elements that compose the task, the way in which those elements must interact and the objects to manipulate.

#### Inspection Task.
For this task a robot processes the information sensed with one or more peripherals wich communicate their sensed information (scene) to the robot. The robot processes/interpret the information finding the current state of the sensed scene and the state of the elements that are in the scene.

#### Transportation Task.
This type of task refers specifically to the change in the pose property of the object or objects to be transported from one position to another, The robots that performs this tasks have a surface where the objects are placed for their transportation. **A transportation task does not involve an end effector**.

#### Manipulation Task.
This type of task refers to any kind of interaction between an object and a robot end effector, in which the end effector must change the current state of the object or any property of it (pose, shape, color, etc.).
