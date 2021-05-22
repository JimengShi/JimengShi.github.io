---
layout:     post
title:      Difference between epoch and iteration
subtitle:   Introduce the difference between epoch, iteration and batch size
date:       2021-05-22
author:     Jimeng
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - Machine Learning
---


## Epoch

> One Epoch is when an ENTIRE dataset is passed forward and backward through the neural network only ONCE.


#### Why we use more than one Epoch?

I know it doesn’t make sense in the starting that — passing the entire dataset through a neural network is not enough.
And we need to pass the full dataset multiple times to the same neural network. 
But keep in mind that we are using a limited dataset and to optimize the learning using Gradient Descent which is an iterative process. 
So, updating the weights with single pass or one epoch is not enough.


## Iteration

Since one epoch is too big to feed to the computer at once we divide it in several smaller batches. 

> Batch size is the total number of training examples present in a single batch.
> Iteration is the number of batches needed to complete one epoch.


## Example
> Let’s say we have 2000 training examples that we are going to use. We divide the dataset of 2000 examples into batches of 500.
 
In the above example, we can get that it take 4 iterations to complete 1 epoch.
Where Batch Size is 500 and Iterations is 4, for 1 complete epoch.

