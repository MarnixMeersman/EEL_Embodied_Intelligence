# NASA EELS Locomotion Simulation in Unity

Before diving in, please [read and download the full report](https://github.com/MarnixMeersman/EEL_Embodied_Intelligence/blob/main/Embodied_Intelligence_NASA_EELS_robot.pdf) for comprehensive background, detailed results, and an in-depth discussion of our methodology.

An advanced simulation project that models the locomotion of NASA’s EELS robot using Unity. This project utilizes the ML-Agents toolkit and reinforcement learning algorithms (PPO and SAC) to recreate and analyze complex movement behaviors in environments inspired by Enceladus, one of Saturn’s moons.

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

Welcome to the NASA EELS Locomotion Simulation repository. This simulation project recreates the locomotion strategies of the NASA EELS robot—designed for exploring challenging terrains like those on Enceladus. Built in Unity, the project leverages both the [Unity ML-Agents Toolkit](https://github.com/Unity-Technologies/ml-agents) and cutting-edge reinforcement learning techniques (PPO and SAC) to train and evaluate robot behavior.

![image](https://github.com/MarnixMeersman/EEL_Embodied_Intelligence/assets/57674797/d654cd11-aabb-4d21-9638-5658251d0b84)

---

## Background & Project Sketch

### Project Background

NASA’s EELS robot is engineered to traverse extreme environments with its segmented, snake-like design, capable of “screw locomotion” for maneuvering over irregular terrain. The goal of this simulation is to validate these locomotion strategies in a realistic, physics-based environment using reinforcement learning.

### Project Sketch

Below is a simplified visual diagram of the project’s main components:

```
       +------------------------------------+
       |          NASA EELS Robot           |
       |  (Segmented & Screw Locomotion)    |
       +----------------+-------------------+
                        |
                        v
       +------------------------------------+
       |      Simulation Environment        |
       |         (Unity & ML-Agents)        |
       +----------------+-------------------+
                        |
                        v
       +------------------------------------+
       |   Reinforcement Learning (PPO/SAC) |
       +----------------+-------------------+
                        |
                        v
       +------------------------------------+
       |       Performance Metrics          |
       | (TensorBoard, YouTube, Logs)       |
       +------------------------------------+
```

---

## Key Features

- **Dual Training Environments:**  
  - **Simple Environment (EEL folder):** A flat terrain ideal for initial tests and rapid prototyping.
  - **Complex Environment (EEL_Complex folder):** An enriched setting with diverse obstacles, replicating the conditions on Enceladus.
  
- **Reinforcement Learning Integration:**  
  Utilizes Unity’s ML-Agents with PPO and SAC to develop robust locomotion strategies.
  
- **Configurable Hyperparameters:**  
  Modify training settings (learning rate, batch size, network architecture) through the configuration files in the `Config` folder.
  
- **Detailed Documentation:**  
  For an in-depth analysis of the simulation’s design, methodology, and performance, refer to the accompanying **Embodied_Intelligence_NASA_EELS_robot.pdf** located at the repository root.

- **Visual Assets:**  
  All original image references are preserved for clear visual guidance:
  - Environment visualization:
    ![image](https://github.com/MarnixMeersman/EEL_Embodied_Intelligence/assets/57674797/d654cd11-aabb-4d21-9638-5658251d0b84)
  - Configuration overview:
    ![image](https://github.com/MarnixMeersman/EEL_Embodied_Intelligence/assets/57674797/7fb08f89-e98c-4700-b4d1-3c2e5c2e4d3a)

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
   - For running the OpenAI Gym API, install Python 3.x and required packages:
     ```bash
     pip install mlagents gym
     ```

---

## Configuration

The `Config` folder contains files with hyperparameters and training settings. Key aspects include:

- **Learning Rate & Schedule:**  
  PPO employs a linear decay schedule while SAC uses a constant rate.
  
- **Batch & Buffer Sizes:**  
  Tweak these parameters to optimize training speed based on your hardware.
  
- **Neural Network Architecture:**  
  Adjust the number of layers and hidden units to experiment with the agent's learning capacity.

Refer to inline comments within the configuration files for detailed explanations.

![image](https://github.com/MarnixMeersman/EEL_Embodied_Intelligence/assets/57674797/7fb08f89-e98c-4700-b4d1-3c2e5c2e4d3a)

---

## Results & Performance

Training outcomes can be tracked using TensorBoard. Explore the performance metrics and experiment logs at:

- [Public TensorBoard Experiment](https://tensorboard.dev/experiment/oKkN7ge1QjSlHY9vKnE77Q/#scalars)

A demonstration video showcasing the simulation in action is available on YouTube:

- [EELS Simulation Demo](https://youtu.be/LdKwgdQfkKw)

Run TensorBoard locally with:
```bash
tensorboard --logdir results
```

---

## Repository Structure

- **EEL:**  
  Contains the simple training environment.
- **EEL_Complex:**  
  Houses the complex environment with additional obstacles.
- **Config:**  
  Configuration files for hyperparameters and training setups.
- **Embodied_Intelligence_NASA_EELS_robot.pdf:**  
  Detailed project report/documentation covering methodology, experiments, and analysis.

---

## Documentation & Further Reading

For a comprehensive understanding of the project’s background, methodology, and future recommendations, please refer to the **Embodied_Intelligence_NASA_EELS_robot.pdf** document located at the repository root. You can also [read and download the report online](https://github.com/MarnixMeersman/EEL_Embodied_Intelligence/blob/main/Embodied_Intelligence_NASA_EELS_robot.pdf).

---

## Acknowledgments

This project is built on the contributions of the [Unity ML-Agents Toolkit](https://github.com/Unity-Technologies/ml-agents) and the supportive community behind it. Special thanks to all researchers and engineers advancing embodied intelligence and reinforcement learning.

---

## Contributing

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature
   ```
3. Commit your changes:
   ```bash
   git commit -am 'Add new feature'
   ```
4. Push your branch:
   ```bash
   git push origin feature/your-feature
   ```
5. Open a pull request.

Please adhere to our coding and documentation guidelines.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

Feel free to explore, contribute, and share your feedback. Thank you for your interest in the NASA EELS Locomotion Simulation project!
