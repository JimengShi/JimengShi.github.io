---
layout:     post
title:      Introduction to Machine Learning
subtitle:   Definition and Classification of Machine Learning
date:       2020-01-01
author:     Jimeng
header-img: img/post-bg-BJJ.jpg
catalog: true
tags:
    - Machine Learning
---
 
## What is Machine Learning?

Arthur Samuel (1959): "Field of study that gives computers the ability to learn without being explicitly programmed.

Tom Michel (1999): "A computer program is said to learn from experience (E) with respect to some class of tasks (T) and performance measure (P), if its performance at tasks in T, as measured by P, improves with experience E." 

The checkers example, E = 10000s games, T is playing checkers, P if you win or not.

## Several types of learning algorithms

##### Supervised learning
You first have a data set and know what the correct output is. You can consider it as supervised learning if its corresponding dataset has the exact labels. The supervised learning problem is classified into a Regression problem and a Classification problem.

- Regression problem
In a regression problem, we try to predict the outcome in a continuous output, which means we try to map the input variable to a continuous function. For example, given a photo of a person, predicting age based on the photo, this is a regression problem.

<div align="center">
<img src="https://github.com/JimengShi/JimengShi.github.io/blob/master/img/Regressioni.png" alt="Regression" >
</div>

![images](https://github.com/JimengShi/JimengShi.github.io/blob/master/img/Regressioni.png)

[![](http://upload-images.jianshu.io/upload_images/2178672-d58bb45f9faedb70.jpg)](http://qiubaiying.github.io/)


- Classification problem
In the classification problem, we try to predict the outcome in the discrete output which means we try to map input variables into discrete categories. For example, given to a patient with a tumor, we have to predict whether the tumor is malignant or benign. 

<div align="center">
<img src="https://github.com/JimengShi/JimengShi.github.io/blob/master/img/Classification.png" alt="Classification" >
</div>

##### Unsupervised learning
Unsupervised learning allows us to have little or no idea what our results should look like. You can consider it as supervised learning if its corresponding dataset has the exact labels. In the unsupervised learning, there is no feedback based on predicted results. Unsupervised learning can be divided into "clustering" and "non-clustering". 

- Clustering: taking a collection of 1,000,000 different genes and finding a way to automatically group them into similar or related groups of different variables. In this situation, you have no idea about labels in the dataset.
<div align="center">
<img src="https://github.com/JimengShi/JimengShi.github.io/blob/master/img/post_clustering.png" alt="post_clustering" >
</div>


##### Reforcement learning
A computer program interacts with a dynamic environment in which it must perform a certain goal (such as driving a vehicle or playing a game against an opponent). The program is provided feedback in terms of rewards and punishments as it navigates its problem space.

<div align="center">
<img src="https://github.com/JimengShi/JimengShi.github.io/blob/master/img/post_reforcement.png" width=50% alt="post_reforcement" >
</div>

##### Recommendation systems
