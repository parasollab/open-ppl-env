# Serial Walls
The Serial Walls environment consists of a set of walls (with openings) that the stick (the robot) has to traverse.
The robot is a stick which is considered a rigid body with 6 degrees of freedom.

![Alt Text](media/serial-walls.gif)

__Difficulty__: 3/5

__Provided by__: Parasol Lab

The ```serial_walls.xml``` file is provided, which will generate the above solution using Obstacle-Based PRM (OBPRM). The xml file also includes other strategies you may want to experiment with.

To run this benchmark using the open-source PPL code, after compiling the executable, run 

```
<your_path_to_ppl>/build/ppl_mp -f serial_walls.xml
```
