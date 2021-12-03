# EECS 498-007 / 598-005 Deep Learning for Computer Vision
My implementation for the assignments from the course of Michigan University EECS 498-007 / 598-005 Deep Learning for Computer Vision Fall 2020.

## Information
* Instructor: Justin Johnson
* [Course Description](https://web.eecs.umich.edu/~justincj/teaching/eecs498/FA2020/)
* [Schedule](https://web.eecs.umich.edu/~justincj/teaching/eecs498/FA2020/schedule.html)
* [Lecture videos](https://www.youtube.com/playlist?list=PL5-TkQAfAZFbzxjBHtzdVCWE0Zbhomg7r) (2019)

## Goals
### [Assignment 1](https://web.eecs.umich.edu/~justincj/teaching/eecs498/FA2020/assignment1.html)
In this assignment, you will first learn how to use PyTorch on Google Colab environment. You will then practice putting together a simple image classification pipeline, based on the k-Nearest Neighbor, and finally will learn how to use Autograder for evaluating what you implement. The goals of this assignment are as follows:

* Develop proficiency with PyTorch tensors
* Gain experience using notebooks on Google Colab
* Understand the basic Image Classification pipeline and the data-driven approach (train/predict stages)
* Understand the train/val/test splits and the use of validation data for hyperparameter tuning
* Implement and apply a k-Nearest Neighbor (kNN) classifier
* Learn how to test your implementation on Autograder

### [Assignment 2](https://web.eecs.umich.edu/~justincj/teaching/eecs498/FA2020/assignment2.html)
In this assignment, you will implement various image classification models, based on the SVM / Softmax / Two-layer Neural Network. The goals of this assignment are as follows:

* Implement and apply a Multiclass Support Vector Machine (SVM) classifier
* Implement and apply a Softmax classifier
* Implement and apply a Two-layer Neural Network classifier
* Understand the differences and tradeoffs between these classifiers
* Practice implementing vectorized gradient code by checking against naive implementations, and using numeric gradient checking

### [Assignment 3](https://web.eecs.umich.edu/~justincj/teaching/eecs498/FA2020/assignment3.html)
In this assignment, you will implement Fully-Connected Neural Networks and Convolutional Neural Networks for image classification models. The goals of this assignment are as follows:

* Understand Neural Networks and how they are arranged in layered architectures
* Understand and be able to implement modular backpropagation
* Implement various update rules used to optimize Neural Networks
* Implement Batch Normalization for training deep networks
* Implement Dropout to regularize networks
* Understand the architecture of Convolutional Neural Networks and get practice with training these models on data

### [Assignment 4](https://web.eecs.umich.edu/~justincj/teaching/eecs498/FA2020/assignment4.html)
From this assignment forward, you will use autograd in PyTorch to perform backpropgation for you. This will enable you to easily build complex models without worrying about writing code for the backward pass by hand. The goals of this assignment are:

* Understand how autograd can help automate gradient computation
* See how to use PyTorch Modules to build up complex neural network architectures
* Understand and implement recurrent neural networks
* See how recurrent neural networks can be used for image captioning
* Understand how to augment recurrent neural networks with attention
* Use image gradients to synthesize saliency maps, adversarial examples, and perform class visualizations
* Combine content and style losses to perform artistic style transfer

### [Assignment 5](https://web.eecs.umich.edu/~justincj/teaching/eecs498/FA2020/assignment5.html)
In this assignment you will implement two different object detection systems. The goals of this assignment are:

* Learn about the object detection pipeline
* Understand how to build an anchor-based single-stage object detectors
* Understand how to build a two-stage object detector that combines a region proposal network with a recognition network

### [Assignment 6](https://web.eecs.umich.edu/~justincj/teaching/eecs498/FA2020/assignment6.html)
In this assignment you will implement two different kinds of generative models: Variational Autoencoders (VAEs) and Generative Adversarial Networks (GANs).
