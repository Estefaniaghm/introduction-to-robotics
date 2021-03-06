# Pose-to-Pose Control

The objective of this laboratory exercise is to study feedforward or open-loop pose-to-pose motion control of the robot. In particular:

* To study pose-to-pose control using a straight-line path
* To study pose-to-pose control using waypoints with straight-line segments
* To study pose-to-pose control using curved paths

For the purposes of this lab, the robot can be modeled as an “unicycle,” whose pose is given by three degrees of freedom: x, y and θ, as measured in a global reference frame. In short, **x** = [x y θ] with x, y in units of cm and θ in degrees. 

## Task 1: Pose-to-Pose Locomotion Using a Straight-Line Path
To demonstrate the basics of locomotion, the robot is commanded to move from a start pose **x**<sub>Start</sub> to a goal pose **x**<sub>Goal</sub>, with **x**<sub>Start</sub> = [0 0 0<sup>◦</sup>] and **x**<sub>Goal</sub> = [200 cm 50 cm 135<sup>◦</sup>]. The most direct way is to plan a straight-line path from the start to the goal and have the robot follow it.

## Task 2: Pose-to-Pose Locomotion Via Waypoints
In this demonstration, the robot is moved through a square path, defined by waypoints A, B, C, back to its original pose. That is, let **x**<sub>Start</sub> = [0 0 0<sup>◦</sup>], **x**<sub>A</sub> = [100 cm 0 90<sup>◦</sup>], **x**<sub>B</sub> = [100 cm 100 cm 180<sup>◦</sup>], **x**<sub>C</sub> = [0 100 cm 270<sup>◦</sup>] and **x**<sub>Goal</sub> = **x**<sub>Start</sub>. 

## Task 3: Pose-to-Pose Locomotion Along a Curved Path
Unfortunately, some robots may not be capable of pivoting on the spot. In this case, it would be necessary to design a curved path for the robot to follow. Assuming that the minimum turning radius for the robot is 25 cm, a path is designed that will take the robot from start to goal as given in Task 1. This task is demonstrated in `lab2.py`. 
