Below is an updated version of your README with enhanced documentation, a clearer project background, and explicit reference to the PDF file in the repository root.

---

# NASA EELS Locomotion Simulation in Unity

An advanced simulation project to model the locomotion of NASA’s EELS robot in environments inspired by Enceladus, one of Saturn’s moons. This project uses Unity with the ML-Agents toolkit and state‐of‐the‐art reinforcement learning algorithms to recreate and analyze complex movement behaviors.

---

## Table of Contents

- [Introduction](#introduction)
- [Background & Project Sketch](#background--project-sketch)
- [Key Features](#key-features)
- [Installation & Prerequisites](#installation--prerequisites)
- [Configuration](#configuration)
- [Results & Performance](#results--performance)
- [Repository Structure](#repository-structure)
- [Documentation & Further Reading](#documentation--further-reading)
- [Acknowledgments](#acknowledgments)
- [Contributing](#contributing)
- [License](#license)

---

## Introduction

This repository hosts the simulation for the NASA EELS Locomotion project, where we aim to emulate the snake-like movement of the EELS robot. The simulation is built in Unity and leverages both the [Unity ML-Agents Toolkit](https://github.com/Unity-Technologies/ml-agents) and reinforcement learning algorithms—namely Proximal Policy Optimization (PPO) and Soft Actor-Critic (SAC)—to evaluate locomotion strategies. The primary objective is to provide a reproducible environment where machine learning agents can learn efficient navigation over varied terrains, from simple flat surfaces to complex, obstacle-laden settings inspired by Enceladus.

---

## Background & Project Sketch

### Project Background

NASA’s EELS robot is designed for exploring challenging terrains, such as the icy and uneven surfaces of Enceladus. With its modular, segmented body, the robot is capable of “screw locomotion,” a unique movement method that enables it to traverse narrow passages and irregular terrain. This simulation seeks to validate the locomotion strategies through embodied intelligence—where the interaction between the robot’s physical structure and its environment plays a crucial role.

### Project Sketch

Below is a simplified visual sketch of the project’s core components and data flow:

```
       +------------------------------------+
       |          NASA EELS Robot           |
       |  (Segmented & Screw Locomotion)    |
       +----------------+-------------------+
                        |
                        v
       +------------------------------------+
       |         Simulation Environment     |
       |          (Unity & ML-Agents)         |
       +----------------+-------------------+
                        |
                        v
       +------------------------------------+
       |      Reinforcement Learning        |
       |      (PPO / SAC Algorithms)        |
       +----------------+-------------------+
                        |
                        v
       +------------------------------------+
       |         Performance Metrics        |
       |   (TensorBoard, YouTube, Logs)       |
       +------------------------------------+
```

This diagram summarizes the overall architecture—from the physical design of the EELS robot, through its simulation and learning, to the analysis of its performance.

---

## Key Features

- **Dual Training Environments:**  
  - **Simple Environment (EEL folder):** A flat terrain for initial tests and faster prototyping.  
  - **Complex Environment (EEL_Complex folder):** An enriched environment with diverse obstacles to simulate Enceladus-like conditions.

- **Reinforcement Learning:**  
  Uses Unity’s ML-Agents toolkit to implement PPO and SAC algorithms for training robust locomotion behaviors.

- **Configurable Hyperparameters:**  
  Easily tweak training configurations through files in the `Config` folder to experiment with different learning rates, batch sizes, and neural network architectures.

- **Detailed Documentation:**  
  Complete documentation is provided in the accompanying PDF file, **Embodied_Intelligence_NASA_EELS_robot.pdf**, located in the repository root.

---

## Installation & Prerequisites

To run the simulation and training scripts, ensure you have the following installed:

1. **Unity Hub & Unity Editor:**  
   - Install the latest Unity Editor version compatible with the ML-Agents Toolkit.
2. **Git:**  
   - Clone the repository using:
     ```bash
     git clone https://github.com/MarnixMeersman/EEL_Embodied_Intelligence.git
     ```
3. **Unity ML-Agents Toolkit:**  
   - Follow the [official installation guide](https://github.com/Unity-Technologies/ml-agents) to set up dependencies.
4. **Python & Required Libraries:**  
   - For running the OpenAI Gym API, install Python 3.x along with necessary packages:
     ```bash
     pip install mlagents gym
     ```

---

## Configuration

The `Config` folder contains all the configuration files for the simulation’s hyperparameters and training settings. Key parameters include:

- **Learning Rate & Schedule:**  
  Configure different learning rate settings for PPO (linear decay) and SAC (constant).
  
- **Batch Size & Buffer Size:**  
  Adjust these to optimize training performance based on your computational resources.
  
- **Neural Network Architecture:**  
  Modify the number of layers and hidden units to experiment with the learning capacity of your model.

Refer to the comments in each configuration file for further details on the parameters.

---

## Results & Performance

Training results are visualized using TensorBoard. For a comprehensive view of performance metrics, visit our public TensorBoard page:

- [Public TensorBoard Experiment](https://tensorboard.dev/experiment/oKkN7ge1QjSlHY9vKnE77Q/#scalars)

Additionally, a demonstration video is available on YouTube:

- [EELS Simulation Demo](https://youtu.be/LdKwgdQfkKw)

Use the following command to run TensorBoard locally:
```bash
tensorboard --logdir results
```

---

## Repository Structure

- **EEL:**  
  Contains the simple training environment with minimal obstacles.
- **EEL_Complex:**  
  Hosts the complex training environment with enriched physics and multiple obstacles.
- **Config:**  
  Configuration files for hyperparameters and training setups.
- **Embodied_Intelligence_NASA_EELS_robot.pdf:**  
  Detailed report/documentation on the project, including methodology, experiments, and analysis.

---

## Documentation & Further Reading

For a detailed overview of the project’s background, methodology, results, and future work recommendations, please refer to the **Embodied_Intelligence_NASA_EELS_robot.pdf** document in the repository root. This report provides comprehensive insights into the design choices, simulation setup, and experimental outcomes.

---

## Acknowledgments

This project is built upon the contributions of the [Unity ML-Agents Toolkit](https://github.com/Unity-Technologies/ml-agents) and its community. Special thanks to the researchers, engineers, and educators who have advanced the fields of embodied intelligence and reinforcement learning.

---

## Contributing

We welcome contributions to further improve the simulation and documentation. To contribute:

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

Please follow our code style guidelines and provide detailed documentation with your contributions.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

Feel free to explore, contribute, and provide feedback. Thank you for your interest in the NASA EELS Locomotion Simulation project!

