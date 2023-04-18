# MultiRobotPoseEstimation
## Synthetic Dataset generation using NVIDIA Isaac Sim
1. Modified and used the 3D models of objects/robots in Universal Scene Descriptor(USD) format with distraction objects to develop synthetic dataset for Computer Vision model training
2. Developed python script for custom Offline Pose Generator code along with a customized YCBVideoWriter to get the datasets in specifically YCB Video format for training
3. Inputting the dataset, camera parameters and 3D models for PoseCNN algorithm inside its Docker Container

## PoseCNN Algorithm
1. Developed docker compose files with CUDA based GL docker image specific to the hardware of RTX 4090 architecture.
2. Utilised different version of datasets(each complex than the other) to train the model to predict Robot Pose from RGB images
3. Compared performance of the model with different hyperparameters and dataset batches to optimise training.
4. Obtained robot poses for different robots on real images captured by the cameras on robots in on-site testing
