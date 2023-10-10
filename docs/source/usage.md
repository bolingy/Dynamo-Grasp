# Getting Started

## Data Collection
Before running the dynamo_grasp.sh script, you need to create a folder in the grasp-point-selection-sim folder. This folder will be used to store the data collected from the simulation. You can create this folder using the following command:
```bash
mkdir <PATH_TO_YOUR_WORKSPACE>/grasp-point-selection-sim/scenario_grasp_configurations
```

Kickstart your experience with a basic usage example:

**Usage**:
```bash
./dynamo_grasp.sh --num-envs NUM_ENVS
```
**Parameters**:
```bash
NUM ENVS :  Integer representing the number of environments to run.
            Select this number based on your computational resources.
```