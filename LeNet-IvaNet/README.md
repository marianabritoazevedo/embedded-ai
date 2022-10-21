## Hyperparameter Tuning with sweep

Adicionar texto ainda

## Model 1: LeNet-5

This architecture of this Convolutional Neural Network (CNN) was described by Yann LeCun, et al. in their 1998 paper titled [Gradient-Based Learning Applied to Document Recognition](https://ieeexplore.ieee.org/document/726791) and it was one of the first successful applications of CNNs.

In this first part of the project, the goal was make the hyperparameter tuning using the sweep from [Wandb](https://wandb.ai) and see which is the best configuration for LeNet-5

### :mag: Settings for hyperparameter tuning 

The configurations of the sweep to make the hyperparameter tuning for the CNN LeNet-5 are described below:
*  `conv_layer`: number of convolutional layers. The possibilities are: 2, 3 or 4;
*  `pooling`: the type of technique used in pooling layer. The possibilities are: 0 (max pooling) or 1 (average pooling);
*  `qtd_filters`: the number of filters used at the convolutional layers. The possibilities are: 4, 8, 16 or 32;
*  `filter_size`: the size of the filters used at the convolutional layers. The possibilities are: 2 (2x2), 3 (3x3), 4 (4x4) or 5 (5x5);
*  `learn_rate`
