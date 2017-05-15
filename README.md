# robot-tasks-specifications
This repository has all the specifications (classes in C++ and python) needed to use a predefined industrial task.

## Industrial tasks.
A typical industrial task is composed of the following elements:

> ##### Type of Task (Inspection, Transportation, Manipulation and Compound).

> ##### List of Goals positions (Goal Poses).

> ##### Time at the goal position (optional).

> ##### Surface to interact with. (static surface, conveyor belt, rotating surface, etc.)

> ##### Objects (the list of objects to inspect, transport and/or manipulate).

### Type of Task (Inspection, Transportation, Manipulation and Compound).
Each tasks vary in complexity, this complexity depends on the elements that compose the task, their limitations and the way in which those elements interact.

#### Inspection Task.
For this task a robot processes the information sensed with one or more peripherals which communicate their sensed information (scene) to the robot. The robot processes/interpret the information finding the current state of the perceived scene and the state of the elements found in it.

#### Transportation Task.
This type of task refers specifically to the change in the pose property of the object or objects to be transported from one position to another, The robots that performs this tasks have a surface where the objects are placed for their transportation. **A transportation task does not involve an end effector**.

#### Manipulation Task.
This type of task refers to any kind of interaction between an object and a robot end effector, in which the end effector must change either the current state of the object or any property of it (pose, shape, color, etc.). Applying glue, welding, pick and place, drilling and screwing are considered manipulation tasks.

#### Compound Task.
It is a list of tasks, where each task could be either an Inspection, a Transportation or a Manipulation. the tasks must be placed in the list in the order in which they must be performed. 
