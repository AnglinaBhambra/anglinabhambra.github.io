---
title: Exploring 5 PyTorch Tensor Functions for Beginners
header:
    overlay_image: /images/andrew-neel-course-unsplash.jpg
    overlay_filler: 0.5
    caption: Photo by [**Andrew Neel on Unsplash**](https://unsplash.com/@andrewtneel)
classes: wide
tags:
    - PyTorch
    - Jovian
excerpt: This post is written to allow me to share what I am learning during the 6 week course - Deep Learning with PyTorch Zero to GANs, using Jovian.ml.
---

*This post is written to allow me to share what I am learning during the 6 week course - Deep Learning with PyTorch: Zero to GANs, using Jovian.ml.*


# Introduction

### Overview of PyTorch

The PyTorch library, developed by the Facebook AI Research lab, plays a big part in the Deep learning framework. PyTorch is very similar to another popular python library, NumPy, which uses multi-dimensional arrays. In PyTorch, we use tensors which can be a number, vector, matrix or any n-dimensional array.

The main difference between PyTorch and NumPy is that unlike PyTorch tensors, NumPy arrays cannot be used on a GPU. This means that in practice NumPy is more expensive and computationally slower.

To learn more about PyTorch tensors, I’ve included links below to the documentation and my course notebook.

> [__My Jovian Notebook - Tensor Operations__](https://jovian.ml/anglinabhambra/01-tensor-operations)
>
>[__torch.Tensor - PyTorch 1.6.0 documentation__](https://pytorch.org/docs/stable/tensors.html)


# PyTorch Tensor Functions
If you’re also using PyTorch, or thinking about using it, I hope that this post encourages you to read through the documentation (linked above).

### torch.square()

`torch.square`(input, out=None) → Tensor

The torch.square() function returns a tensor with the square of every element in the input tensor.

<iframe src="https://jovian.ml/embed?url=https://jovian.ml/anglinabhambra/01-tensor-operations/v/26&cellId=3" title="Jovian Viewer" height="179" width="800" frameborder="0" scrolling="auto"></iframe>

Here we have created a tensor, x, and squared every element in x.

### torch.squeeze()

`torch.sqeeze`(input, dim=None) → Tensor

The torch.squeeze() function returns a tensor with all the dimensions of input of size 1 removed, where dim is dimension.

<iframe src="https://jovian.ml/embed?url=https://jovian.ml/anglinabhambra/01-tensor-operations/v/26&cellId=11" title="Jovian Viewer" height="800" width="800" frameborder="0" scrolling="auto"></iframe>

Here we have created a tensor, x, with dimensions (4 x 3 x 1 x 4 x 1) filled with random elements.  
We can see that the torch.squeeze() function has removed all dimensions that have a size of 1, as y.size() shows that tensor y has dimensions (4 x 3 x 4).

<iframe src="https://jovian.ml/embed?url=https://jovian.ml/anglinabhambra/01-tensor-operations/v/26&cellId=13" title="Jovian Viewer" height="410" width="800" frameborder="0" scrolling="auto"></iframe>

In the previous example, the torch.squeeze() function’s dim value is set to None (dim=None) as this is the default. This meant that all dimensions of size 1 was removed.  
In this example, y.size() is the same as x.size(), as we set dim to 0. The ‘0’ (in dim=0) is referring to the ‘3’ (in x.size() # torch.Size(3, 1, 2)). As this is a 3, and not a 1, the tensor remains the same. However is we set dim=1, then y.size() would be torch.Size(3, 2).

### torch.round_()

`torch.round_`(input) → Tensor

The torch.round_() function returns the same tensor with each of the elements of the input rounded to the closest integer, as the underscore denotes __in place__.
The torch.round() function would otherwise return a new tensor with each of the elements of the input rounded to the closest integer.

<iframe src="https://jovian.ml/embed?url=https://jovian.ml/anglinabhambra/01-tensor-operations/v/26&cellId=19" title="Jovian Viewer" height="300" width="800" frameborder="0" scrolling="auto"></iframe>

In this example we can see that the output is the same tensor, where all of the elements in the tensor have been rounded to the closest integer.

<iframe src="https://jovian.ml/embed?url=https://jovian.ml/anglinabhambra/01-tensor-operations/v/26&cellId=21" title="Jovian Viewer" height="255" width="800" frameborder="0" scrolling="auto"></iframe>

Here we have created a tensor, x, to have 4 floating numbers. PyTorch knows that if one of the values is a float, then the rest of the elements will also be floating numbers.  
We can see that the elements have been rounded to the closest integer, and that the data type of all of the elements are floats.

### torch.neg()

`torch.neg`(input) → Tensor

The torch.neg() function returns a new tensor with the negative of the elements of the input.

<iframe src="https://jovian.ml/embed?url=https://jovian.ml/anglinabhambra/01-tensor-operations/v/26&cellId=27" title="Jovian Viewer" height="230" width="800" frameborder="0" scrolling="auto"></iframe>

Here we can see that the elements in the new tensor, y, are the same as -1 multiplied by the elements in the input tensor, x.

### torch.min()

`torch.min`(input, dim, keepdim=False) → Tensor

The torch.min() function returns the minimum value out of all the elements in the input tensor.  
‘dim’ refers to the dimension to reduce, and ‘keepdim’ is fed a boolean which determines whether the output tensor has dim retained or not.

<iframe src="https://jovian.ml/embed?url=https://jovian.ml/anglinabhambra/01-tensor-operations/v/26&cellId=35" title="Jovian Viewer" height="254" width="800" frameborder="0" scrolling="auto"></iframe>

In this example, we can see that without including any of the other parameters, the torch.min() function returns the the smallest element out of all of the elements in tensor x.

<iframe src="https://jovian.ml/embed?url=https://jovian.ml/anglinabhambra/01-tensor-operations/v/26&cellId=37" title="Jovian Viewer" height="608" width="800" frameborder="0" scrolling="auto"></iframe>

As explained in the PyTorch documentation, if keepdim=True, the output tensor will be of the same size as input except in the dimension dim where they are of size 1. Otherwise, dim is squeezed (see above) resulting in the output tensor having 1 fewer dimension than the input.  
This example shows that the output is a ___namedtuple___ __(values, indices)__.  
__values__: the minimum value of each row of the input tensor in the given dimension dim.  
__indices__: the index location of each minimum value found (argmin).



# Final Remarks

It’s worth mentioning here that we were also asked to explore ways in which these functions wouldn’t work, which is a great learning technique. I have done this in my notebook (linked in the intro and [here](https://jovian.ml/anglinabhambra/01-tensor-operations)).  
One thing that could improve this post would be to include when these functions would be most useful.

A big Thank You to Aakash and the Jovian.ml team. I would highly recommend following along if you can. To do so, use the Jovian.ml link or simply watch the first video linked [here](https://www.youtube.com/watch?v=vo_fUOk-IKk).