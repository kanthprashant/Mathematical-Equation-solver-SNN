# Mathematical-Equation-solver-SNN

We present supervised learning in Spiking Neural Network for the problem of handwritten digit equation solving using the Gradient Descent algorithm. The entire application is divided into 
two phases, phase 1 being image segmentation and preprocessing. Phase 2 is the classification part. We present several insights from extensive numerical experiments regarding optimizing 
learning parameters and network configuration to improve its accuracy. The network uses biologically plausible neural and learning mechanisms and is applied to a subset of the MNIST 
dataset of handwritten digits and basic mathematical operations. The research aims to assess the classification power of a straightforward biologically motivated mechanism and develop an 
application to solve the handwritten equations. The network architecture is primarily a feedforward spiking neural network (SNN) composed of Leaky Integrated and Fire neurons and Voltage-based 
synapses

## Installation

```sh
pip install nengo-dl
pip install nengo

```
![image](https://user-images.githubusercontent.com/88501367/167888317-383347e0-a649-4141-a125-54c18d553746.png)

## Experimental Design 

As illustrated in figure 3, we designed a six-layer Spiking Convolutional Neural Network to 
classify handwritten digits from the Customized digits, operators' database. The challenge was to 
get a good dataset and various instances of each digit as well as operators. We made use of a 
Kaggle dataset to train our model [4]. The sizes of the images in our dataset had varying lengths 
(mostly 155*135), so we had to resize them to a particular size to retain the uniformity in training 
data. In the train-test split, all images were resized to (128*128). These were then flattened to one 
dimension and then sent to the network

![image](https://user-images.githubusercontent.com/88501367/167888488-2e7cbf68-bee7-4736-9286-b69e6c555073.png)
