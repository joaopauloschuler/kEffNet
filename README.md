# kEffNet
This repository contains the source code for the paper [Grouped Pointwise Convolutions Significantly Reduces Parameters in EfficientNet](https://www.researchgate.net/publication/355214501_Grouped_Pointwise_Convolutions_Significantly_Reduces_Parameters_in_EfficientNet) [(PDF)](https://github.com/joaopauloschuler/kEffNet/blob/main/Grouped%20Pointwise%20Convolutions%20Significantly%20Reduces%20Parameters%20in%20EfficientNet.pdf) by Joao Paulo Schwarz Schuler, Santiago Romani, Mohamed Abdel-Nasser, Hatem Rashwan and Domenec Puig.

## Abstract
EfficientNet is a recent Deep Convolutional Neural Network (DCNN) architecture intended to be proportionally extendible in depth, width and resolution. Through its variants, it can achieve state of the art accuracy on the ImageNet classification task as well as on other classical challenges. Although its name refers to its efficiency with respect to the ratio between outcome (accuracy) and needed resources (number of parameters, flops), we are studying a method to reduce the original number of trainable parameters by more than 84\% while keeping a very similar degree of accuracy. Our proposal is to improve the pointwise (1x1) convolutions, whose number of parameters rapidly grows due to the multiplication of the number of filters by the number of input channels that come from the previous layer. Basically, our tweak consists in grouping filters into parallel branches, where each branch processes a fraction of the input channels. However, by doing so, the learning capability of the DCNN is degraded. To avoid this effect, we suggest interleaving the output of filters from different branches at intermediate layers of consecutive pointwise convolutions. Our experiments with the CIFAR-10 dataset show that our optimized EfficientNet has similar learning capacity to the original layout when training from scratch.

## Test on Colab
You can test kEffNet on Google Colab:
* [kEffNet v1.](https://colab.research.google.com/github/joaopauloschuler/k-neural-api/blob/master/examples/jupyter/kEffNet_v1.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/joaopauloschuler/k-neural-api/blob/master/examples/jupyter/kEffNet_v1.ipynb)

## Prerequisites
All examples in this project require importing the [K-CAI Neural API](https://github.com/joaopauloschuler/k-neural-api).

## Give this Project a Star
This project is an open source project. If you like what you see, please give it a star on github.

## Further Parameter and Floating-point Computation Savings
The following papers also deal about parameters and floating-point computation savings:
- [Grouped Pointwise Convolutions Reduce Parameters in Convolutional Neural Networks.](https://www.researchgate.net/publication/360226228_Grouped_Pointwise_Convolutions_Reduce_Parameters_in_Convolutional_Neural_Networks)
- [An Enhanced Scheme for Reducing the Complexity of Pointwise Convolutions in CNNs for Image Classification Based on Interleaved Grouped Filters without Divisibility Constraints.](https://www.researchgate.net/publication/363413038_An_Enhanced_Scheme_for_Reducing_the_Complexity_of_Pointwise_Convolutions_in_CNNs_for_Image_Classification_Based_on_Interleaved_Grouped_Filters_without_Divisibility_Constraints)
- [Reliable Deep Learning Plant Leaf Disease Classification Based on Light-Chroma Separated Branches.](https://www.researchgate.net/publication/355215213_Reliable_Deep_Learning_Plant_Leaf_Disease_Classification_Based_on_Light-Chroma_Separated_Branches)
- [Color-aware two-branch DCNN for efficient plant disease classification.](https://www.researchgate.net/publication/361511874_Color-Aware_Two-Branch_DCNN_for_Efficient_Plant_Disease_Classification)

## Citing this Paper 
Bibtex:
```
@inbook{Schuler2021k01,
author = {Schuler, Joao and Romaní, Santiago and Abdel-nasser, Mohamed and Rashwan, Hatem and Puig, Domenec},
year = {2021},
month = {10},
pages = {383-391},
title = {Grouped Pointwise Convolutions Significantly Reduces Parameters in EfficientNet},
booktitle = {Artificial Intelligence Research and Development},
publisher = {IOS Press},
isbn = {9781643682105},
doi = {10.3233/FAIA210158}
}
```





