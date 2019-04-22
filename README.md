# WSGAN-GP for generating 3D Vertebrae masks

This codes generates 3D Vertebrae segmentation masks using 3D GANs trained on XvertSeg dataset, and another in-house dataset from rechts der Isar. 

This repo contains the WSGAN-GP model for generating 64x64x64 cubes, and the conditional 64^3 model, where the vertebrae region is used as the condition ( 0 Thoracic, 1 Lumbar, no much of Cervical vertebrae data was available so it was execluded)

## Training
Training was done on Nvidia Tesla GPU with 16 GB of memory. The convergence of the objective function is shown in the Gif included inside each model's directory. 
## Prerequisites
You need to have python 3.6 and PyTorch 0.4 or 1.0. 

## Data 

To learn more about XvertSeg please follow [this] link (http://lit.fe.uni-lj.si/xVertSeg/)

## Pre-trained model
Please feel free to contact me for the pre-trained models. 

## Acknowledgment 
Code structure is mainly from this [repo](https://github.com/rimchang/3DGAN-Pytorch) with a lot of modifications made.

This was a project at TUM that was supervised by Anjany Sekuboyina (anjany.sekuboyina@tum.de) from Image-base biomedical modelling (IBBM) group at Munich School of BIO-Engineering. 
