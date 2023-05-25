---
title: (arXiv 22') SymFormer- End-to-end symbolic regression using transformer-based architecture
author: yo3nglau
date: '2023-05-25'
categories:
  - Skimmed Papers
tags:
  - Neural-Symbolic
  - arXiv
toc: true
---

## Overview

### Motivation

<img src="https://s1.ax1x.com/2023/05/24/p97B3pF.png" style="zoom:90%;" />

Many real-world problems can be naturally described by mathematical formulas. The task of finding formulas from a set of observed inputs and outputs is called *symbolic regression*.

Neural networks have been applied to symbolic regression, among which the transformer-based ones seem to be the most promising. However, the main drawback of transformers is that they generate formulas without numerical constants, which have to be optimized separately, so yielding suboptimal results.

### Resolution

This work proposes a transformer-based approach called **SymFormer**, which predicts the formula by *outputting the individual symbols and the corresponding constants simultaneously*. 

The model is trained on hundreds of millions of formulas to be able to generate a symbolic representation of a previously unseen formula given a set of input-output pairs efficiently. It jointly predicts the symbolic representation of a function and the values of all constants in a single forward pass of a neural network. A local gradient search is used to improve constants further to fit the input points better.

The model generates both the symbolic representation of the formula and the concrete values for all constants at the same time. This allows the symbolic decoder to condition on the generated constants and it improves the quality of the symbolic representation. The generated constants are used to initialize the local gradient search to fine-tune the final constants effectively and reliably.

## Framework

![](https://s1.ax1x.com/2023/05/24/p97B8l4.png)

"Figure 1: Schematic diagram of inference. The input points are passed through the transformer, generating several candidate equations using Top-K sampling. These candidates are further improved using gradient descent. The final equation is then selected by the lowest mean squared error."

## Methods

### Benchmark functions

"Table 5: Benchmark functions that we have used in our experiments. We have restricted ourselves only to the univariate and bivariate functions."

<img src="https://s1.ax1x.com/2023/05/24/p97yDUI.png" style="zoom:80%;" />

<img src="https://s1.ax1x.com/2023/05/24/p97yBVA.png" style="zoom:80%;" />

## Unfamiliar knowledge

**Note: May include buzz word and potential literature.**

local gradient search

## Resources

[Paper](), [Code]()

## Elementary drafts

**Note: May contain Chinese. This section will disappear once all drafts are embellished.**

<details>
	<summary>collapsed contents</summary>
		add more details
</details>
{{< embed-pdf url="../../pdfs/SymFormer- End-to-end symbolic regression using transformer-based architecture.pdf" >}}

