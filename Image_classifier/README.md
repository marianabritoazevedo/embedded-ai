## :camera: Image classifier: dog, cat or panda
This project aims to create different models of Machine Learning (ML) to solve the following problem: given an image, classify it as an image that contains a dog, a cat or a panda. For this project, three ML models will be used for the image classification:
- __K-nearest neighbors__ (KNN) algorithm, from the library scikit-learn;
- __Multi-layer perceptron classifier__ (MLPClassifier), from the library scikit-learn;
- __Convolucional neural network__ (CNN), from the library TensorFlow.

## :bulb: Project flow
For this project, it was also used the tool named Weights & Biases (also known as Wandb) to make the model management. Based on its operation, the big-picture of the data pipeline used in this project can be seen in the figure below.

![image info](./images/img-modelo-com-fundo.png)

In general, for each stage of the data pipeline it was created a notebook in Google Colaboratory, containing five stages: `fetch data`, `preprocessing`, `data segregation`, `train`, `test`. It is important to know that the `fetch data` stage it was executed just once, because the same dataset will be used for the three ML models that will be implemented. Also, in the last ML model (CNN), two more artifacts were generated: `validation_x` and `validation_y`. 
