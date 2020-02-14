# cloud_faceswap
Sets up deepfake/Faceswap for cloud machines and executes training script with telegram notifications

# Installation

## Bootstrap: Optimized for Vast.ai (non root user)

'''
#!/bin/bash

# this script downloads and installs the faceswap program 

# make user (optional) - uncomment if your user is non-root already
useradd -m deepfake
# NOT safe - change passwd if instance is public or is supposed to be in operation for a long time
echo deepfake:deeper721 | chpasswd
usermod -aG sudo deepfake
su - deepfake


git clone https://github.com/JustinGuese/cloud_faceswap.git
cd ~/cloud_faceswap
chmod +x faceswap_setup_x64.sh
./faceswap_setup_x64.sh -y 
'''
