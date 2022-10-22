## Hyperparameter Tuning with sweep

One of the first and best known convolutional neural networks is LeNet-5, described by Yann LeCun, et al. in their 1998 paper titled [Gradient-Based Learning Applied to Document Recognition](https://ieeexplore.ieee.org/document/726791). The system was developed for use in a handwritten character recognition problem and demonstrated on the MNIST standard dataset, achieving approximately 99.2% classification accuracy (or a 0.8% error rate). The network was then described as the central technique in a wider system referred to as Graph Transformer Networks.

With that in mind, we performed hyperparameter tuning using [Weights and Biases](https://wandb.ai) for three models based on LeNet5:

* __Model 1__: From the architecture of the original paper, a sweep was performed with other activation functions, more convolutional layers, other filter sizes, batch sizes etc.
* __Model 2__: Another sweep was performed using data augmentation by varying parameters such as zoom, shear, among others, and also testing techniques such as dropout, batchnormalization, etc.
* __Model 3__: to write

It is important to highlight that this work was carried out in a group, the first part being responsible for [Mariana Brito](https://github.com/marianabritoazevedo), the second part for 

[Morsinaldo Medeiros](https://github.com/Morsinaldo) [![Repository](https://img.shields.io/badge/-Repo-191A1B?style=flat-square&logo=github)](https://github.com/Morsinaldo/embedded_artificial_intelligence/tree/main/projects/lenet5) and the third part for

[Thaís Araújo](https://github.com/thaisaraujo2000?tab=repositories) [![Repository](https://img.shields.io/badge/-Repo-191A1B?style=flat-square&logo=github)](https://github.com/thaisaraujo2000/embedded_artificial_intelligence/tree/main/projects). (Ajeitar o link de Thaís quando ela fizer o push)

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

### :chart_with_upwards_trend: Metrics

The table below shows the metrics obtained in all 10 different configurations tested. We can see that only one configuration obtained bad results, but the other 9 configurations reached an accuracy over 80%.

Model                         |Accuracy|Precision|Recall|F1-Score
------------------------------|:--------:|:---------:|:------:|:--------:
earnest-sweep-9               | 0.9882   | 0.9882    | 0.9882 | 0.9882
sandy-sweep-3                 | 0.9864   | 0.9864    | 0.9864 | 0.9864 
faithful-sweep-6              | 0.9761   | 0.9761    | 0.9761 | 0.9761 
worldly-sweep-7               | 0.961    | 0.9611    | 0.961  | 0.961
denim-sweep-2                 | 0.9481   | 0.9481    | 0.9481 | 0.948
vocal-sweep-10                | 0.9374   | 0.9373    | 0.9374 | 0.9373
usual-sweep-1                 | 0.9119   | 0.9123    | 0.9119 | 0.9119
wild-sweep-8                  | 0.8667   | 0.867     | 0.8667 | 0.8663
summer-sweep-4                | 0.8284   | 0.8277    | 0.8284 | 0.8254
legendary-sweep-5             | 0.4834   | 0.4557    | 0.4834 | 0.433

The image below shows the results reached according to the parameters of each sweep.

![image info](./images/sweep-lenet.png)
