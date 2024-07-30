# Box Folding Problem

The box folding problem is a motion planning problem containing a narrow passage. 

The objective is to fold the articulated model into its final box shape. 

There are no external obstacles in the enviroment, but self-collision among the links (connected by revolute joints) must be avoided. The model consists of 11 parts, each of which is a rectangular piece.

One is considered the fixed base, and 10 are considered links. However, taking advantage of symmetry conditions, we can reduce the number of parts by half (1 fixed base and 5 links). 

The model is available in BYU format, with each piece (base and links) represented in a separate file. 

The linkage information is contained in an environment file, which is in our env format. The environment file gives the pieces in the start configuration shown below.

We solved this problem using our OBPRM planner. 

![box_folding_problem_gif](media/box.gif)

__Type__: Static 3D

__#Agents__: 1

__Difficulty__: 5/5

__Provided by__: Guang Song, Parasol Lab, Texas A&M University

## Running this benchmark
The ```box.xml``` file is provided, which will generate the above solution using Obstacle-Based PRM (OBPRM). The xml file also includes other strategies you may want to experiment with.

To run this benchmark using the open-source PPL code, after compiling the executable, run

```
<your_path_to_open-ppl>/build/ppl_mp -f box.xml
```

|  |  |
| ------ | ------ |
| Code Version       |  OpenPPL main, commit  |
| MPStrategy       |   OBPRM     |
| Sampler(s)       |   UniformRandomFree, ObstacleBased     |

|  |  |
| ------ | ------ |
| Samples       |   24,993    |
| CD Calls       |   9,224,856   |
| Runtime       |    967 sec   |
