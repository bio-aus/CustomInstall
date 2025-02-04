# CustomInstall

sudo apt install containerd

sudo apt install docker.io

docker login nvcr.io
try docker login without nvcr.io





docker pull nvidia/cuda:12.8.0-base-ubuntu22.04

docker run --rm --gpus all nvidia/cuda:12.8.0-base-ubuntu22.04 nvidia-smi

git clone https://github.com/deepmind/alphafold.git
#cd into this new repository---->
cd ./alphafold
#On all these purple popups tab to ok and hit enter
sudo apt update
sudo apt upgrade
sudo apt install aria2

cd
mkdir dd_alphafold
cd alphafold
scripts/download_all_data.sh /home/ubuntu/dd_alphafold > download.log 2> download_all.log &

docker build -f docker/Dockerfile -t alphafold .
