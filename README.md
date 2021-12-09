# NICF
Instruction for environment configuration:

- Install docker, relevant info: 
https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository

- Pull the legacy tensorflow 1.15 image: 
docker pull tensorflow/tensorflow:1.15.2-py3-jupyter

- Spin up a bash terminal in docker container: 
docker run -it --rm tensorflow/tensorflow:1.15.2-py3-jupyter bash 

- Inside the docker bash terminal, install git, and other modules using the following:
apt-get update \\
apt-get install git \\
pip install ipdb \\ 
pip install sklearn \\

- Clone the Repo:
git clone https://github.com/JiamoLiu/NICF_Jiamo.git
cd NICF_Jiamo

- Train the model using bash script:
bash model_train.sh
