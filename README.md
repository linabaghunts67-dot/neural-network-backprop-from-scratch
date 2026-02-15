# neural-network-backprop-from-scratch
Mini deep learning framework built from scratch in NumPy with manual backpropagation and MNIST training.


Mini PyTorch from Scratch (NumPy)

This project is my implementation of a small deep learning framework built entirely with NumPy.
The goal was to truly understand what happens inside loss.backward() instead of relying on PyTorch or TensorFlow.

I implemented:

Linear (Fully Connected) layer

ReLU activation

SoftMax activation

Cross-Entropy (Negative Log Likelihood) loss

Manual backpropagation

SGD training loop

The model is trained on the MNIST digits dataset (sklearn.datasets.load_digits) and successfully learns to classify handwritten digits.

Why I Built This

While modern frameworks make deep learning easy, I wanted to deeply understand:

How gradients flow through layers

How parameter updates actually work

How matrix calculus connects to backpropagation

Why SoftMax + CrossEntropy simplifies gradients

This project helped me connect theory (matrix derivatives) with implementation.

Technologies Used

Python

NumPy

Scikit-learn (for dataset loading only)

Matplotlib (for plotting loss)

No autograd. No deep learning frameworks.

What I Learned

Backpropagation is just repeated application of the chain rule

Linear layers are simple matrix multiplications with structured gradients

SoftMax gradients are more complex unless combined with CrossEntropy

Numerical stability matters (log(0), overflow in exp)
