# Install

This guide will walk you through the installation process.


## Download the URDF models

## Download the GQCNN model

## Creating a new conda environment


```bash
conda create -n dynamo-grasp python=3.8
conda activate dynamo-grasp

pip install -U pip poetry
conda install pytorch torchvision torchaudio pytorch-cuda=11.8 cudatoolkit=11.8 cudnn -c pytorch -c nvidia
poetry install
```
