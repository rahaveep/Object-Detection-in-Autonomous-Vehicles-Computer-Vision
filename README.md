# Object-Detection-in-Autonomous-Vehicles-Computer-Vision
In Ubuntu 18.04
1. Install Docker
2. Install NVIDIA GPU drivers
3. Install NVIDIA toolkit container
4. Run the following commands on Terminal Window
5. Download code from https://github.com/tianweiy/CenterPoint.git
6. Open the Centerpoint directory
7. Create a folder called data and download data from 
https://s3.amazonaws.com/data.nuscenes.org/public/v1.0/v1.0-
mini.tgz?AWSAccessKeyId=AKIA6RIK4RRMFUKM7AM2&Signature=IV8aYbYiTwSxtJrC6ppB403Es
5c%3D&Expires=1652210730
8. Organize as shown in 
https://github.com/tianweiy/CenterPoint/blob/master/docs/GETTING_START.md
9. Download nvidia/cuda:11.1-cudnn8-devel-ubuntu18.04 docker from 
https://hub.docker.com/layers/cuda/nvidia/cuda/11.1.1-cudnn8-develubuntu18.04/images/sha256-
0272ed266b68a3673663bdac5d28506844da9e29ebe986bf9c8b7feaf147720c?context=explore
10. Sudo docker run -it –gpus all –shm-size 16G nvidia/cuda:11.1-cudnn8-devel-ubuntu18.04
11. After docker container is created copy the Centerpoint directory into the container
12. After entering docker use Dockerfile as reference to install the required packages
13. All the train and test commands can be found in 
https://github.com/tianweiy/CenterPoint/blob/master/docs/NUSC.md
