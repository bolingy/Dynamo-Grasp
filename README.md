# DYNAMO-GRASP Project


This project introduces DYNAMO-GRASP, a novel approach to the challenge of suction grasp point detection. By leveraging the power of physics-based simulation and data-driven modeling, DYNAMO-GRASP is capable of accounting for object dynamics during the grasping process. This significantly enhances a robot's ability to handle unseen objects in real-world scenarios.
Our method was benchmarked against established approaches through comprehensive evaluations in both simulated and real-world environments. It outperformed the alternatives by achieving a success rate of 98% in diverse simulated picking tasks and 80% in real-world, adversarially-designed scenarios.
DYNAMO-GRASP demonstrates a strong ability to adapt to complex and unexpected object dynamics, offering robust generalization to real-world challenges. The results of this research pave the way for more reliable and resilient robotic manipulation in intricate real-world situations.

This repository provides the codebase for collecting data through simulation. These scripts will help users to generate their own datasets, further enhancing the extensibility and usefulness of DYNAMO-GRASP.

For more information please refer to our [project website](https://sites.google.com/view/dynamo-grasp)

## Table of Contents

1. [Installation](#installation)
2. [Running the Project](#running)

## Installation

Follow these steps for the installation:

```bash
# Import the conda environment with Python version 3.8
conda env create -f environment.yaml
```

For more details see [Installation](INSTALLATION.md)


```bash
pip install -e .

# Create a folder inside the repo for saving the data(grasp point properties, depth image, segmentation mask image),
mkdir scenario_grasp_configurations
```

## Running
To run the project, use the dynamo_grasp.sh bash script:
```bash
conda run -n dynamo-grasp ./data-collection.py --num-envs 50
```
