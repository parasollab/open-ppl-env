# SimpleObstacle

This is a group of three environments, each with two rectangular obstacles of varying sizes that create a simple, straightforward path that the robot can pass through. The passsage size also varies. The model is available in BYU format, with each piece represented in a separate file.

## Obstacle 1
<img src="Media/Obstacle1GIF.gif" alt="Obstacle 1" width="50%" height="50%"/>

## Obstacle 2
<img src="Media/Obstacle2GIF.gif" alt="Obstacle 2" width="50%" height="50%"/>

## Obstacle 3
<img src="Media/Obstacle3GIF.gif" alt="Obstacle 3" width="50%" height="50%"/>

__Type__: Static 2D

__#Agents__: 1

__Difficulty__: 1/5

__Provided by__: Parasol Lab, Texas A&M University

## Running this benchmark
The ```obstacle.xml``` file is provided in each obstacle directory, which will generate the above solutions using Obstacle-Based PRM (OBPRM). The xml files also include other strategies you may want to experiment with. Before running, make sure that you are in the correct directory for the obstacle that you want to run!

To run this benchmark using the open-source PPL code, after compiling the executable, run

```
<your_path_to_open-ppl>/build/ppl_mp -f obstacle.xml
```

|  |  |
| ------ | ------ |
| Code Version       |  OpenPPL main, commit 4bf4be2bba97a777aed1c10857404f88d0782e03 |
| MPStrategy       |   OBPRM     |
| Sampler(s)       |   UniformRandomFree, ObstacleBased     |

|  |  |
| ------ | ------ |
| | Obstacle 1 |
| Samples       |   42    |
| CD Calls       |   248,564   |
| Runtime       |    1.5 sec   |

|  |  |
| ------ | ------ |
| | Obstacle 2 |
| Samples       |   42    |
| CD Calls       |   172,098   |
| Runtime       |    1.08 sec   |

|  |  |
| ------ | ------ |
| | Obstacle 3 |
| Samples       |   42    |
| CD Calls       |   121,903   |
| Runtime       |    0.75 sec   |
