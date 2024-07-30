# Periscope
The periscope folding problem is a motion planning problem containing a narrow passage. The objective is to fold the articulated model into its final periscope shape. There are no external obstacles in the enviroment, but self-collision among the links (connected by revolute joints) must be avoided.

The model consists of 12 parts, each of which is a rectangular piece. One is considered the fixed base, and 11 are considered links. The model is available in BYU format, with each piece (1 fixed base and 11 links) represented in a separate file. The linkage information is contained in an environment file, which is in our env format. The environment file gives the pieces in the start configuration.
We solved this problem using our OBPRM planner.

![Alt Text](media/pariscope.gif)

__Type__: Static 3D

__#Agents__: 1

__Difficulty__: 3/5

__Provided by__: Guang Song, Parasol Lab, Texas A&M University

## Running this benchmark
The ```periscope.xml``` file is provided, which will generate the above solution using Obstacle-Based PRM (OBPRM). The xml file also includes other strategies you may want to experiment with.

To run this benchmark using the open-source PPL code, after compiling the executable, run

```
<your_path_to_open-ppl>/build/ppl_mp -f periscope.xml
```

|  |  |
| ------ | ------ |
| Code Version       |  OpenPPL main, commit 22988962e56db93ed68a0e6b7acc7ac952f73434 |
| MPStrategy       |   OBPRM     |
| Sampler(s)       |   UniformRandomFree, ObstacleBased     |

|  |  |
| ------ | ------ |
| Samples       |   1,319    |
| CD Calls       |   967,227   |
| Runtime       |    674 sec   |