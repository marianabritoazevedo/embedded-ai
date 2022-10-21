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
*  `learn_rate`: the step size at each iteration while moving toward a minimum of a loss function. The possibilities are: 0.01 or 0.001;
*  `epoch`: the number of epochs which the CNN will be trained. The possibilities are: 20 or 40;
*  `batch_size`: the size of the batch. The possibilities are: 32 or 64.

### :trophy: Best configuration

The parameters for the sweep were chosen randomly, and there were tested 10 different types of configuration for the LeNet-5.

The best configuration can be seen in the image below, which has __4__ convolutional layers with __16__ filters __5x5__, the pooling layer using __AveragePooling__, and it has the number __0.01__ as learning rate and __32__ as the dize of the batch. This configuration achieved an accuracy of 98.82%.

![image info](./images/lenet-modelo.png)

:chart_with_upwards_trend: Metrics

The table below shows the metrics obtained in all 10 different configurations tested.
