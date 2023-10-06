# NASA EELS Locomotion Simulation in Unity

## Introduction
Welcome to the NASA EELS Locomotion Simulation repository. This project aims to recreate the locomotion types demonstrated by NASA's EELS robot that one day should venture into the oceans of Encaldus, on of Saturns moons. We use Unity as the simulation environment and make extensive use of Unity's ML-Agents toolkit for the machine learning components. Additionally, we utilize reinforcement learning algorithms provided by OpenAI APO for this research.

We have provided two different types of environments for testing and training the model:

1. **Simple Environment (EEL folder)**: A simpler, less cluttered version for initial tests and quicker results.
2. **Complex Environment (EEL_Complex folder)**: A more intricate setup with diverse obstacles and parameters for testing the limits of the model.

![image](https://github.com/MarnixMeersman/EEL_Embodied_Intelligence/assets/57674797/d654cd11-aabb-4d21-9638-5658251d0b84)


## Acknowledgment
This project is largely build upon the [Unity ML-Agents Toolkit](https://github.com/Unity-Technologies/ml-agents). Also thanks to the community behind this toolkit.

## Configuration
The `Config` folder contains various configuration files for hyperparameters that the model uses for training. Feel free to tweak these parameters to suit your particular needs. Note that in order to reproduce any of these results, you should clone the ml agents toolkit repo, download unity hub and the latest version of unity editor.
![image](https://github.com/MarnixMeersman/EEL_Embodied_Intelligence/assets/57674797/7fb08f89-e98c-4700-b4d1-3c2e5c2e4d3a)


## Results
The training and test results can be found on the [public tensorboard](https://tensorboard.dev/experiment/oKkN7ge1QjSlHY9vKnE77Q/#scalars). They can be 'downloaded' from there anf you can also visualize the metrics using TensorBoard locally by running the following command in your terminal:
```
tensorboard --logdir results
```

## Folders
- **EEL**: Contains the simpler environment.
- **EEL_Complex**: Contains the more complex environment with diverse obstacles.

Feel free to explore, contribute, and create issues. Thank you for visiting!
