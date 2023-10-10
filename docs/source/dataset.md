# Dataset

Link to the dataset: [Prcessed_Data.zip](https://drive.google.com/file/d/16CvCuETpmtBYbqEcMIOIJCxDMaO8c4Uu/view?usp=sharing) <br/>
This dataset consists of inputs that include 4 channels: 3D point clouds and a segmentation mask. Grasp labels consist of a zero-background image with float values at each sampled point.

The dataset is organized as follows:

```bash
*_input_data_*.npy - Input data and corresponding label image is *_label_*.npy
*_input_augment1_*.npy - Augmented input data (adding noise to point cloud) and corresponding label image is *_label_*.npy
*_input_augment2_*.npy - Augmented input data (flipping the input image), corresponding flipped label image is *_label_flip_*.npy
```

The naming of the files is as follows:<br/>
<**file_order**>_input_data\_<**env_id**>\_<**config_count**>.npy <br/>
Here `file_order` is the order of the paths added in the `process_raw_files.py` file. `env_id` is the environment id and `config_count` is the number of configurations for that environment.

`Processed_Data.zip` dataset is obtained by running `pre_processing` file after collecting raw data from the simulation.

In our simulation setup, we have two cameras: one for main sampling points and the other is embedded in the suction to measure suction deformation score more accurately. We utilize images from the back camera for our dataset collection.

