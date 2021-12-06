## Assignment 3
### Q1: Fully-Connected Neural Network
The notebook fully_connected_networks.ipynb will walk you through implementing Fully-Connected Neural Networks.
### Q2: Convolutional Neural Network 
The notebook convolutional_networks.ipynb will walk you through implementing Convolutional Neural Networks.

## Notes
### Nesterov Momentum
> ```python
> x_ahead = x + mu * v
> # evaluate dx_ahead (the gradient at x_ahead instead of at x)
> v = mu * v - learning_rate * dx_ahead
> x += v
> ```
> 
> However, in practice people prefer to express the update to look as similar to vanilla SGD or to the previous momentum update as possible. This is possible to achieve by manipulating the update above with a variable transform `x_ahead = x + mu * v`, and then expressing the update in terms of `x_ahead` instead of `x`. That is, the parameter vector we are actually storing is always the ahead version. The equations in terms of `x_ahead` (but renaming it back to `x`) then become:
> 
> ```python
> v_prev = v # back this up
> v = mu * v - learning_rate * dx # velocity update stays the same
> x += -mu * v_prev + (1 + mu) * v # position update changes form
> ```

Paragraph of Nesterov Momentum from [cs231n], in fact, it skips a lot details,
* to see the detailed derivation of Nesterov Momentum: 
  * [Nesterov Accelerated Gradient and Momentum]
* to see why it's coded in this way (it actually takes a detour route): 
  * [Momentum & Nesterov momentum]
  * [What's the difference between momentum based gradient descent and Nesterov's accelerated gradient descent?]
* although the assignment only asks us to implement vanilla Momentum rather than Nesterov Momentum, I'd like to take a note.：) 

### Backpropagation of CNN
* [Convolutional Neural Networks(CNN) #4 卷積核的Back propagation] (backpropagation of kernel)
* [Convolutional Neural Networks(CNN) #5 特徵圖&偏差值的導數] (backpropagation of feature map & bias)
* [Convolutional Neural Networks(CNN) #6 Pooling in Backward pass] (backpropagation of pooling)

### Backpropagation of Batch Normalization
The assignment asks us to implement backpropagation of batch normalization in two ways: (1) write out a computation graph for batch normalization on paper and propagate gradients backward through intermediate nodes, and (2) work out the derivatives for the batch normalizaton backward pass on paper and simplify as much as possible.
1. Things become easy after drawing out the computation graph. ([source])  
![computation graph]
2. The [paper] provided the derivatives for the batch normalizaton backward pass though, to see further simplification: [Deriving the Gradient for the Backward Pass of Batch Normalization]  
![BN derivatives]



[cs231n]: https://cs231n.github.io/neural-networks-3/#sgd
[Nesterov Accelerated Gradient and Momentum]: https://jlmelville.github.io/mize/nesterov.html
[Momentum & Nesterov momentum]: https://tensorflow.blog/2017/03/22/momentum-nesterov-momentum/
[What's the difference between momentum based gradient descent and Nesterov's accelerated gradient descent?]: https://stats.stackexchange.com/questions/179915/whats-the-difference-between-momentum-based-gradient-descent-and-nesterovs-acc
[Convolutional Neural Networks(CNN) #4 卷積核的Back propagation]: https://www.brilliantcode.net/1670/convolutional-neural-networks-4-backpropagation-in-kernels-of-cnns/
[Convolutional Neural Networks(CNN) #5 特徵圖&偏差值的導數]: https://www.brilliantcode.net/1748/convolutional-neural-networks-5-backpropagation-in-feature-maps-biases-of-cnns/
[Convolutional Neural Networks(CNN) #6 Pooling in Backward pass]: https://www.brilliantcode.net/1781/convolutional-neural-networks-6-backpropagation-in-pooling-layers-of-cnns/
[source]: https://kratzert.github.io/2016/02/12/understanding-the-gradient-flow-through-the-batch-normalization-layer.html
[computation graph]: img/BNcircuit.png 
[paper]: https://arxiv.org/abs/1502.03167
[Deriving the Gradient for the Backward Pass of Batch Normalization]: https://kevinzakka.github.io/2016/09/14/batch_normalization/
[BN derivatives]: img/BNderi.png
