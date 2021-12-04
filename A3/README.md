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

Paragraph of Nesterov Momentum from [cs231n](https://cs231n.github.io/neural-networks-3/#sgd), in fact, it skipped a lot details,
* to see the detail derivation of Nesterov Momentum: 
  * [Nesterov Accelerated Gradient and Momentum](https://jlmelville.github.io/mize/nesterov.html)
* to see why it coded in this way (it actually takes a detour route): 
  *
  *
* although the assignment only asks us to implement vanilla Momentum rather than Nesterov Momentum, I'd like to take a note.：) 


### Backproprogation of CNN
* [Convolutional Neural Networks(CNN) #4 卷積核的Back propagation](https://www.brilliantcode.net/1670/convolutional-neural-networks-4-backpropagation-in-kernels-of-cnns/)
* [Convolutional Neural Networks(CNN) #5 特徵圖&偏差值的導數](https://www.brilliantcode.net/1748/convolutional-neural-networks-5-backpropagation-in-feature-maps-biases-of-cnns/)
* [Convolutional Neural Networks(CNN) #6 Pooling in Backward pass](https://www.brilliantcode.net/1781/convolutional-neural-networks-6-backpropagation-in-pooling-layers-of-cnns/)
