---
title: Machine Learning 01
categories: [Machine Learning]
tags: [Machine Learning]
---

### Introduction

Some examples used in Machine Learning:

- Database mining
- Applications can't program by hand
- Self-customizing programs
- Understanding human learning

### What is Machine Learning?

Task, Experience, Performance

`A computer program is said to learn from experience E with respect to some class of tasks T and performance measure P, if its performance at tasks in T, as measured by P, improves with experience E."`  *by* Tom Mitchell

Classification
- Supervised learning

- Unsupervised learning

- Reinforcement learning

  ​

### Supervised Learning

we are given a data set and know what correct output should look like

- Regression -- Continuous output

- Classification -- Discrete output

many features

### Unsupervised Learning

little or no idea about what our results should look like, no feedback

Examples:

- news grouping 
- social network analysis
- market segmentation

Cocktail party Problem Algorithm

```matlab
[W, s, v] = svd((repmat(sum(x.x, 1), size(x, 1), 1).x)*x');
```

<font color=red>Is it an unsupervised learning problem or not?</font>



### After Class

What is svd?



###  Model and Cost Function



### Gradient descent algorithm

repeat until convergence {

​	$\theta_j := \theta_j - \alpha \frac{\partial}{\partial\theta_j} J(\theta_0, \theta_1)$

}

$\alpha$ : learning rate

- too small - slow
- too big - fail to converge, or even diverge


update $\theta_j$ simultaneously

convex function - bowl shape, always converge to global optimum

"Batch" : Each step of gradient descent uses all the training examples

