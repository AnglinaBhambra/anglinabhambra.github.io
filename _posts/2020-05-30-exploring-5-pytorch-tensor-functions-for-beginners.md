---
title: Exploring 5 PyTorch Tensor Functions for Beginners
tags:
    - PyTorch
    - Jovian
categories:
    - PyTorch
---

*This post is written to allow me to share what I am learning during the 6 week course - Deep Learning with PyTorch: Zero to GANs, using Jovian.ml.*

INSERT IMAGE HERE

## Introduction

### Overview of PyTorch

The PyTorch library, developed by the Facebook AI Research lab, plays a big part in the Deep learning framework. PyTorch is very similar to another popular python library, NumPy, which uses multi-dimensional arrays. In PyTorch, we use tensors which can be a number, vector, matrix or any n-dimensional array.

The main difference between PyTorch and NumPy is that unlike PyTorch tensors, NumPy arrays cannot be used on a GPU. This means that in practice NumPy is more expensive and computationally slower.

To learn more about PyTorch tensors, I’ve included links below to the documentation and my course notebook.

[__My Jovian Notebook - Tensor Operations__](https://jovian.ml/anglinabhambra/01-tensor-operations)

[__torch.Tensor - PyTorch 1.6.0 documentation__](https://pytorch.org/docs/stable/tensors.html)

ADD PAGE SEPARATOR

## PyTorch Tensor Functions
If you’re also using PyTorch, or thinking about using it, I hope that this post encourages you to read through the documentation (linked above).

### torch.square()

`torch.square`(input, out=None) → Tensor

The torch.square() function returns a tensor with the square of every element in the input tensor.

<iframe src="https://jovian.ml/embed?url=https://jovian.ml/anglinabhambra/01-tensor-operations/v/26&cellId=3" title="Jovian Viewer" height="179" width="800" frameborder="0" scrolling="auto"></iframe>


