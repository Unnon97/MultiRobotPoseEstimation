(Unable to share implementation due to Intellectual Property Rules)
# MultiRobotPoseEstimation
This Repository describes the task of using syntethic dataset generation for a Robot pose estimator algorithm(PoseCNN) using Nvidia Isaac Sim tool. This task was a part of the CoRob-X project done by multiple EU based Space Research Groups to prove the capability of autonmous multi robot mapping on the Lunar surface.
The task involved follwing steps:
1. Creating a custom environment in Isaac Sim utilising the robots and Lunar environment for simulating the test site. Here for training, the background contained a dark brownish sand ground based on the test site on Earth.
2. Develop the dataset in the format of YCB dataset used by the official PoseCNN paper for predicting the pose of random objects from daily life.
3. Develop a docker image and container to implement the model and input the dataset to predict the object pose
4. Train the model using different datasets to obtain a robust pose prediction model that could be implemented and predict pose on real robot images obtained from test site.



## Synthetic Dataset generation using NVIDIA Isaac Sim
1. Adapted propriety space exploratory robot 3D models with distraction objects to develop synthetic dataset for Computer Vision based Pose estimation model training.
2. Developed python script for custom Offline Pose Generator code along with a customized YCB Video format script to get the datasets in specifically YCB Video format for training
3. Utilized Docker Container to input the dataset, camera properties and 3D models for PoseCNN algorithm

## PoseCNN Algorithm
1. Developed docker compose files with CUDA based GL docker image specific to the hardware of RTX 4090 architecture.
2. Utilised different version of datasets(each complex than the other) to train the model to predict Robot Pose from RGB images
3. Compared performance of the model with different hyperparameters and dataset batches to optimise training.
4. Obtained robot poses for different robots on real images captured by the cameras on robots in on-site testing
