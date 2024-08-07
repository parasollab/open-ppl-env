# ZigZag

The Zig-Zag environment represents an easy winding narrow passage which fools many sampling-based planners. It is a nice 2D problem, to study qualities of various planners.
The model is available in BYU format, with each piece represented in a separate file.

<img src="Media/ZigZag.gif" alt="ZigZag Solution" width="50%" height="50%"/>

__Type__: Static 2D

__#Agents__: 1

__Difficulty__: 1/5

__Provided by__: Parasol Lab, Texas A&M University

## Running this benchmark
The ```zigzag.xml``` file is provided, which will generate the above solution using Basic Rapidly exploring Random Tree (RRT). The xml file also includes other strategies you may want to experiment with.

To run this benchmark using the open-source PPL code, after compiling the executable, run

```
<your_path_to_open-ppl>/build/ppl_mp -f zigzag.xml
```

|  |  |
| ------ | ------ |
| Code Version       |  OpenPPL main, commit cfff4de05e333f76f805bcead1f60fac9d73bc5a |
| MPStrategy       |   RRT     |
| Sampler(s)       |   UniformRandom, ObstacleBased     |

|  |  |
| ------ | ------ |
| Samples       |   151    |
| CD Calls       |   0   |
| Runtime       |    0.4263 sec   |
