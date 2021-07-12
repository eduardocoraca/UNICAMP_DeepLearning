# Deep Learning for Image Segmentation of Flame Front Propagation
Files for the final project of Deep Learning discipline (IA376 - 1s2021) at [FEEC/UNICAMP](https://www.fee.unicamp.br/?language=en).

The [U-Net](https://arxiv.org/abs/1505.04597), [HRNet](https://arxiv.org/abs/1908.07919) and [DeepLab v3](https://arxiv.org/abs/1706.05587) models were trained for two data configurations:
*  __Mixed dataset__: in this case, image from Ethanol, Gasoline and Hydrogen combustion flame front propagation were ramdomly chosen as Train/Validation/Test datasets.
*  __Zero-shot dataset__: in this case, images from Ethanol and Gasoline were used as Train/Validation datasets and Hydrogen data was used for Testing.

File [FinalProject_PT.pdf](https://github.com/eduardocoraca/UNICAMP_DeepLearning/blob/main/FinalProject_PT.pdf) contains a detailed report of this project (in portuguese).

## U-Net Network:
The notebooks for the U-Net implementations are  [*UNET_Mixed.ipynb*](https://github.com/eduardocoraca/UNICAMP_DeepLearning/blob/main/UNET_Mixed.ipynb) and [*UNET_ZeroShot.ipynb*](https://github.com/eduardocoraca/UNICAMP_DeepLearning/blob/main/UNET_ZeroShot.ipynb).
The model is an implementation for semantic segmentation of brain MRI images and can be found [here](https://pytorch.org/hub/mateuszbuda_brain-segmentation-pytorch_unet/).

## HRNet Network:
The notebooks for the HRNet implementations are [*HRNet_Mixed.ipynb*](https://github.com/eduardocoraca/UNICAMP_DeepLearning/blob/main/HRNet_Mixed.ipynb) and [*HRNet_ZeroShot.ipynb*](https://github.com/eduardocoraca/UNICAMP_DeepLearning/blob/main/HRNet_ZeroShot.ipynb). The model files can be found [here](https://github.com/HRNet/HRNet-Semantic-Segmentation).
For this project, an adaptation of these files was used according to what was described [here](https://www.kaggle.com/bibek777/try-hrnet-semantic-segmentation). 

## DeepLab Network:
The notebooks for the DeepLab v3 implementations are [*DeepLab_Mixed.ipynb*](https://github.com/eduardocoraca/UNICAMP_DeepLearning/blob/main/DeepLab_Mixed.ipynb) and [*DeepLab_ZeroShot.ipynb*](https://github.com/eduardocoraca/UNICAMP_DeepLearning/blob/main/DeepLab_ZeroShot.ipynb).
A pre-trained model was used, which can be found [here](https://pytorch.org/hub/pytorch_vision_deeplabv3_resnet101/), which was trained on the *COCO* dataset.


All models were implemented in PyTorch.
