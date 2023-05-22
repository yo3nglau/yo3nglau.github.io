---
title: (ICCV 21') Calibrating Concepts and Operations- Towards Symbolic Reasoning on Real Images
author: yo3nglau
date: '2023-05-17'
categories:
  - Skimmed Papers
tags:
  - Neural-Symbolic
  - ICCV
toc: true
---

## Overview

![](https://s1.ax1x.com/2023/05/18/p9fBcCR.png)

Figure 1: Statistics and examples from the synthetic CLEVR dataset and the real GQA dataset. Compared to the synthetic dataset, VQA on real data needs to deal with long-tail concept distribution and uneven importance of reasoning steps.

<img src="https://s1.ax1x.com/2023/05/18/p9fBrE4.png" style="zoom:50%;">

Figure 2: A failure case that can be corrected by reweighting the operations. The *select(bag)* operation overrides *filter(not black)*, thus lead to incorrect answer. This can be corrected by scaling up the result of *filter* operation.

## Framework


![](https://s1.ax1x.com/2023/05/18/p9fBy59.png)

Figure 3: Overview of our method. We first parse the image into a symbolic scene representation in the form of objects and attributes, then parse the question into a program. In each reasoning step, a reasoning module takes in the scene representation and the instruction from the program, and outputs a distribution over objects. The Operation Weight Predictor predicts a weight for each reasoning module, which will be used to merge module outputs based on the program dependency. The final distribution is fed into the output module to predict answers.

## Unfamiliar knowledge

**Note: May include buzz word and potential literature.**

## Resources

[Paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Li_Calibrating_Concepts_and_Operations_Towards_Symbolic_Reasoning_on_Real_Images_ICCV_2021_paper.pdf), [Code](https://github.com/Lizw14/CaliCO)

## Elementary drafts

**Note: May contain Chinese. This section will disappear once all drafts are embellished.**

<details>
	<summary>collapsed contents</summary>
		something
		<br>
		一些草稿
</details>
{{< embed-pdf url="../../pdfs/Calibrating Concepts and Operations- Towards Symbolic Reasoning on Real Images.pdf" >}}
