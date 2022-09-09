## Assignment 2
### Q1: Linear Classifiers
The notebook linear_classifier.ipynb will walk you through implmenting SVM and Softmax classifier. You are required to write code on linear_classifier.py.
### Q2: Two-layer Neural Network
The notebook two_layer_net.ipynb will walk you through implementing a two-layer neural network-based classifier. Your implementation will go to two_layer_net.py.

## Note
### Gradient of SVM loss function
* [cs231n - Computing the gradient analytically with Calculus](https://cs231n.github.io/optimization-1/#analytic)
  * ...when you’re implementing this in code you’d simply count the number of classes that didn’t meet the desired margin (and hence contributed to the loss function) and then the data vector xi scaled by this number is the gradient.
* [Vectorized Implementation of SVM Loss and Gradient Update](https://mlxai.github.io/2017/01/06/vectorized-implementation-of-svm-loss-and-gradient-update.html)
  * some corrections
    * The coefficent of xi1 is the number of classes that **didn't** meet the desire margin.
    * this single class yi requires us to count the number of classes that **didn't** satisfy the margin condition
    * 2.jpg: sum along col -> **N**x1    
* [Derivation of gradient of SVM loss](https://math.stackexchange.com/questions/2572318/derivation-of-gradient-of-svm-loss/2572319)

### Gradient of Softmax loss function
* [cs231n - Computing the Analytic Gradient with Backpropagation](https://cs231n.github.io/neural-networks-case-study/#grad)
* [Logistic classification with cross-entropy](https://peterroelants.github.io/posts/cross-entropy-logistic/)
* [Classification and Loss Evaluation - Softmax and Cross Entropy Loss](https://deepnotes.io/softmax-crossentropy)
