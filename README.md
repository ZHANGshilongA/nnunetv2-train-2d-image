# nnUNetv2-train-2d-image
This repo is mianly used to record how to train 2d image using nnUNetv2.
## Hardware configuration
· windows10
· NVIDIA RTX A6000
## Some things we need to know
1. nnunetv1 not supports 2d image, if u want to train 2d image, u need to transfer 2d img to fake 3d img, but now nnunetv2 supports 2d image, so we just know the training steps and can to train.
2. nnunetv2 just appects RGB 3 channels image, gray image is not appected. (it can be PNG, TIF, etc. Mine is PNG)
3. The suffix must be with '_0000'
## 4 steps of training nnunetv2
### Download code and create env
1. Download nnunetv2 [here](https://github.com/MIC-DKFZ/nnUNet "nnUNetv2")
2. Open the code u download, and create 'dataset' file. In the 'dataset' file, create 3 files.
3. create a new env, download GPU version Pytorch, and 'pip install -e .'
4. go to 'path.py' and change 3 path variables into yours
### Prepare the format dataset
use the 'Dataset_120_conversation.py'
### Preprocess the dataset
use the command
### Train model
use the command
### Predict
use the command


refer to [this website](https://zhuanlan.zhihu.com/p/633898872)
