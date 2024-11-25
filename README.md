# Multimodal Synthetic Accident Dataset (MSAD)

## Overview

The **Multimodal Synthetic Accident Dataset (MSAD)** is an open-source repository containing 83 accident scenarios generated using reinforcement learning (RL) agents in the CARLA simulator. This dataset addresses the scarcity of real-world accident data by focusing on synthetic accident scenarios, which are crucial for testing autonomous systems in diverse and safety-critical situations.

The dataset provides **multimodal data** for each scenario:
- **LiDAR Point Clouds**
- **Depth Images**
- **RGB Camera Feeds**

Additionally, it includes **human-verified accident reports** generated with assistance from large language models (LLMs), ensuring detailed analysis and interpretability of the accident scenarios.

---

## Key Features

### Diverse Accident Scenarios
- **Environments**: Scenarios span urban intersections, highway merges, and rural roads.
- **Agent Configurations**: Simulated behaviors include abrupt stops, lane changes, and intersection navigation.
- **Dynamic Conditions**: Accidents occur under varying weather, traffic densities, and road geometries.

### Multimodal Sensor Data
Each scenario includes synchronized sensor outputs:
- **LiDAR Point Clouds**: 3D spatial data for mapping and obstacle detection.
- **Depth Images**: Visual depth data for scene reconstruction.
- **RGB Camera Feeds**: High-resolution imagery for semantic understanding.

### Detailed Accident Reports
- Resimulated from multiple perspectives in CARLA.
- Verified by human annotators to ensure accurate interpretations.
- Reports include key information on accident causality, agents involved, and post-collision dynamics.

---

## Dataset Structure

The dataset is organized as follows:
- **`/scenarios/`**: CARLA-compatible `.xosc` scenario files.
- **`/multimodal_data/`**: Organized by scenario ID:
  - `lidar/`: LiDAR point cloud frames.
  - `depth/`: Depth image sequences.
  - `rgb/`: RGB video sequences.
- **`/reports/`**: Human-annotated accident reports in JSON and PDF formats.
- **`/metadata/`**: Scenario metadata (location, weather, agents, etc.).

---

## Installation & Usage

### Prerequisites
- **CARLA Simulator** (version ≥ 0.9.13 recommended).
- Python environment with CARLA API and dependencies installed.


## Novelty

- **Synthetic Accident Generation**: Unlike traditional datasets, MSAD emphasizes rare and complex accident scenarios, addressing gaps in real-world datasets.
- **Post-Accident Analysis**: Includes post-collision effects, offering insights into the aftermath and secondary risks.
- **Human-in-the-Loop Annotation**: Combines AI and human expertise for accurate and interpretable accident narratives.

---

## Use Cases

- **Autonomous Driving Testing**: Evaluate safety-critical scenarios for decision-making systems.
- **Simulation Research**: Develop scenario-based evaluations and models.
- **Safety Benchmarking**: Create baselines for accident prediction and impact analysis.

---

## License

This dataset is distributed under the **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**.

---

## Citation

If you use MSAD in your research, please cite: LINK

## Contributing
We welcome contributions to expand the dataset or improve existing scenarios. Please create a pull request or contact us at <email>.

## Acknowledgments
This work builds upon insights from state-of-the-art simulation frameworks like CARLA, OpenCDA, and ScenarioNet. We thank our collaborators for their invaluable contributions to annotating and validating accident scenarios.






