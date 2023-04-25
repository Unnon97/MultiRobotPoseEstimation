# MultiRobotPoseEstimation
## Synthetic Dataset generation using NVIDIA Isaac Sim
1. Adapted propriety space exploratory robot 3D models with distraction objects to develop synthetic dataset for Computer Vision based Pose estimation model training.
2. Developed python script for custom Offline Pose Generator code along with a customized YCB Video format script to get the datasets in specifically YCB Video format for training
3. Utilized Docker Container to input the dataset, camera properties and 3D models for PoseCNN algorithm

## PoseCNN Algorithm
1. Developed docker compose files with CUDA based GL docker image specific to the hardware of RTX 4090 architecture.
2. Utilised different version of datasets(each complex than the other) to train the model to predict Robot Pose from RGB images
3. Compared performance of the model with different hyperparameters and dataset batches to optimise training.
4. Obtained robot poses for different robots on real images captured by the cameras on robots in on-site testing
