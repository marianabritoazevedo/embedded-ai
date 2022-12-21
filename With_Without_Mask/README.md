# With or Without a mask

## About this project

write

## How to run

It is important to know that these steps on how to run take into account that the entire model creation process has already been carried out on the [Edge Impulse](https://www.edgeimpulse.com/) platform.

1- Clone this repository 

```
git clone https://github.com/marianabritoazevedo/embedded-ai.git
```

2- Download Arduino IDE, you can check it [here](https://www.arduino.cc/en/software)

3- Install the libraries necessary to run this project. They are: `Arduino Mbed OS Nano Boards`, `Harvard_TinyMLx`, `Arduino_TensorFlowLite` and `Arduino_OV767X`.
To install the libraries, you can follow these steps:

```
Tools >> Manage libraries
```

:heavy_exclamation_mark: Attention: to install `Arduino_TensorFlowLite`, it is necessary to use this [repository](https://github.com/tensorflow/tflite-micro-arduino-examples)

4- Take the file `ei-face_mask_detection_2-arduino-1.0.5.zip` in the folder `library_zip` and add as a library in Arduino IDE. This can be done by following the sequence:

```
Sketch >> Include library >> Add .zip library
```

5- Connect your Arduino Nano 33 BLE sense in the Arduino IDE. 
```
Tools >> Board >> Arduino Mbed OS Nano Boads >> Arduino Nano 22 BLE
```

6- Connect the port
```
Tools >> Port >> COM4 (this may change)
```

7- Run the project
```
Verify >> Upload
```
