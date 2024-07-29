# ZTunnel

The Z tunnel environment contains an obstacle in the shape of a rectangular prism with a single narrow passage removed from the obstacle in the shape of a Z. The robot (rectangular prisms of varying dimensions) must navigate through the passageway.

<!-- The robot is a stick which is considered a rigid body with 6 degrees of freedom. -->

![Ztunnel Gif](media/mygif_placeholder)

__Type__: Static 3D

__#Agents__: 1

__Difficulty__: 3/5

__Provided by__: Parasol Lab

## Running this benchmark

The ``ZTunnel.xml`` file is provided, which will generate the above solution using Rapidly-exploring Random Tree (RRT). The xml file also includes other strategies you may want to experiment with.

To run this benchmark using the open-source PPL code, after compiling the executable, run

```
<your_path_to_ppl>/build/ppl_mp -f ZTunnel.xml
```

|              |                                                               |
| ------------ | ------------------------------------------------------------- |
| Code Version | OpenPPL main, commit d4e7d44caf18ff0c9962c9a0f47e18c4220d6747 |
| MPStrategy   | RRT                                                           |
| Sampler(s)   | UniformRandomFree, ObstacleBased                              |

|          |           |
| -------- | --------- |
| Samples  | 6,875     |
| CD Calls | 1,286,308 |
| Runtime  | 8.22 sec  |

---

|              |                                                               |
| ------------ | ------------------------------------------------------------- |
| Code Version | OpenPPL main, commit 4ba6006b81a2e4a145b71fae0419ad76e187f3be |
| MPStrategy   | RRT                                                           |
| Sampler(s)   | UniformRandomFree, UniformRandom                              |

|          |           |
| -------- | --------- |
| Samples  | 6,875     |
| CD Calls | 1,286,308 |
| Runtime  | 30.1 sec  |

![Alt Text](gifs/BasicRRT3D.gif)

---

|              |                                                               |
| ------------ | ------------------------------------------------------------- |
| Code Version | OpenPPL main, commit 4ba6006b81a2e4a145b71fae0419ad76e187f3be |
| MPStrategy   | PRM                                                           |
| Sampler(s)   | UniformRandomFree, UniformRandom                              |

|          |            |
| -------- | ---------- |
| Samples  | 4,702      |
| CD Calls | 20,783,414 |
| Runtime  | 278.0 sec  |

![Alt Text](gifs/BasicPRM3D.gif)
