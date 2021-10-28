# kEffNet
This repository contains the source code for the paper [Grouped Pointwise Convolutions Significantly Reduces Parameters in EfficientNet](https://www.researchgate.net/publication/355214501_Grouped_Pointwise_Convolutions_Significantly_Reduces_Parameters_in_EfficientNet) [(PDF)](https://github.com/joaopauloschuler/kEffNet/blob/main/Grouped%20Pointwise%20Convolutions%20Significantly%20Reduces%20Parameters%20in%20EfficientNet.pdf) by Joao Paulo Schwarz Schuler, Santiago Romani, Mohamed Abdel-Nasser, Hatem Rashwan and Domenec Puig.

## Abstract
EfficientNet is a recent Deep Convolutional Neural Network (DCNN) architecture intended to be proportionally extendible in depth, width and resolution. Through its variants, it can achieve state of the art accuracy on the ImageNet classification task as well as on other classical challenges. Although its name refers to its efficiency with respect to the ratio between outcome (accuracy) and needed resources (number of parameters, flops), we are studying a method to reduce the original number of trainable parameters by more than 84\% while keeping a very similar degree of accuracy. Our proposal is to improve the pointwise (1x1) convolutions, whose number of parameters rapidly grows due to the multiplication of the number of filters by the number of input channels that come from the previous layer. Basically, our tweak consists in grouping filters into parallel branches, where each branch processes a fraction of the input channels. However, by doing so, the learning capability of the DCNN is degraded. To avoid this effect, we suggest interleaving the output of filters from different branches at intermediate layers of consecutive pointwise convolutions. Our experiments with the CIFAR-10 dataset show that our optimized EfficientNet has similar learning capacity to the original layout when training from scratch.

## Citing this Paper 
Bibtex:
```
@inbook{inbook,
author = {Schuler, Joao and Romaní, Santiago and Abdel-nasser, Mohamed and Rashwan, Hatem and Puig, Domenec},
year = {2021},
month = {10},
pages = {383-391},
title = {Grouped Pointwise Convolutions Significantly Reduces Parameters in EfficientNet},
isbn = {9781643682105},
doi = {10.3233/FAIA210158}
}
```
