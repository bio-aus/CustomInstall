# CustomInstall

sudo apt install containerd

sudo apt install docker.io

sudo apt git https://gitlab.com/nvidia/container-images/cuda/blob/master/dist/12.8.0/ubuntu2204/base/Dockerfile

reboot

docker login nvcr.io
try docker login without nvcr.io





docker pull nvidia/cuda:12.8.0-base-ubuntu22.04

docker run --rm --gpus all nvidia/cuda:12.8.0-base-ubuntu22.04 nvidia-smi
