## Assignment 4
### Q1: PyTorch Autograd
The notebook pytorch_autograd_and_nn.ipynb will introduce you to the different levels of abstraction that PyTorch provides for building neural network models. You will use this knowledge to implement and train Residual Networks for image classification.
### Q2: Image Captioning with Recurrent Neural Networks
The notebook rnn_lstm_attention_captioning.ipynb will walk you through the implementation of vanilla recurrent neural networks (RNN) and Long Short Term Memory (LSTM) RNNs. You will use these networks to train an image captioning model. You will then augment your implementation to perform spatial attention over image regions while generating captions.
### Q3: Network Visualization
The notebook network_visualization.ipynb will walk you through the use of image gradients for generating saliency maps, adversarial examples, and class visualizations.
### Q4: Style Transfer
In the notebook style_transfer.ipynb, you will learn how to create images with the artistic style of one image and the content of another image.

## Notes
### Attention for RNN
The [lecture] already explained the evolution of attention for RNN in detail; just note some other introduction of applications:
* [Attention and Augmented Recurrent Neural Networks]
* [Attention? Attention!]

### Adversarial Attack
* [Know your enemy]
* [Chapter 1 - Introduction to adversarial robustness]
* https://github.com/Harry24k/adversarial-attacks-pytorch

### CNN Visualization
* [Understanding Neural Networks Through Deep Visualization]
* https://github.com/utkuozbulak/pytorch-cnn-visualizations

### Style Transfer
* [Neural Transfer Using PyTorch]



[lecture]: https://www.youtube.com/watch?v=YAgjfMR9R_M&list=PL5-TkQAfAZFbzxjBHtzdVCWE0Zbhomg7r&index=13
[Attention and Augmented Recurrent Neural Networks]: https://distill.pub/2016/augmented-rnns/
[Attention? Attention!]: https://lilianweng.github.io/lil-log/2018/06/24/attention-attention.html
[Know your enemy]: https://towardsdatascience.com/know-your-enemy-7f7c5038bdf3
[Chapter 1 - Introduction to adversarial robustness]: https://adversarial-ml-tutorial.org/introduction/
[Understanding Neural Networks Through Deep Visualization]: https://yosinski.com/deepvis
[Neural Transfer Using PyTorch]: https://pytorch.org/tutorials/advanced/neural_style_tutorial.html
