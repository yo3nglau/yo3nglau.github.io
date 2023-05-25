---
title: (ICLR 19' oral) THE NEURO-SYMBOLIC CONCEPT LEARNER- INTERPRETING SCENES, WORDS, AND SENTENCES FROM NATURAL SUPERVISION
author: yo3nglau
date: '2023-05-17'
categories:
  - Skimmed Papers
tags:
  - Neural-Symbolic
  - ICLR
toc: true
---

## Overview

<img src="https://s1.ax1x.com/2023/05/24/p97R59I.png" style="zoom:60%;" />

"Figure 7: An example image-question pair from the VQS dataset and the corresponding execution trace of NS-CL."

This work proposes the Neuro-Symbolic Concept Learner (**NS-CL**), a model that learns visual concepts, words, and semantic parsing of sentences *without explicit supervision* on any of them; instead, the model *learns by simply looking at images and reading paired questions and answers*. The proposed model builds an **object-based scene representation** and **translates sentences into executable, symbolic programs**. To bridge the learning of two modules, it uses a neuro-symbolic reasoning module that executes these programs on the latent scene representation.

### Learning pattern of human

![](https://s1.ax1x.com/2023/05/24/p97RWAH.png)

"Figure 1: Humans learn visual concepts, words, and semantic parsing jointly and incrementally. **I.** Learning visual concepts (red vs. green) starts from looking at simple scenes, reading simple questions, and reasoning over contrastive examples (Fazly et al., 2010). **II.** Afterwards, we can interpret referential expressions based on the learned object-based concepts, and learn relational concepts (e.g., on the right of, the same material as). **III.** Finally, we can interpret complex questions from visual cues by exploiting the compositional structure."

## Framework

![](https://s1.ax1x.com/2023/05/24/p97RogP.png)

"Figure 2: We propose to use neural symbolic reasoning as a bridge to jointly learn visual concepts, words, and semantic parsing of sentences."

![](https://s1.ax1x.com/2023/05/24/p97R2He.png)

"Figure 3: We treat attributes such as Shape and Color as neural operators. The operators map object representations into a visual-semantic space. We use similarity-based metric to classify objects."

### Curriculum concept learning

![](https://s1.ax1x.com/2023/05/24/p97Rh4A.png)

"Figure 4: **A.** Demonstration of the curriculum learning of visual concepts, words, and semantic parsing of sentences by watching images and reading paired questions and answers. Scenes and questions of different complexities are illustrated to the learner in an incremental manner. **B.** Illustration of our neuro-symbolic inference model for VQA. The perception module begins with parsing visual scenes into object-based deep representations, while the semantic parser parse sentences into executable programs. A symbolic execution process bridges two modules."

## Methods

The work first introduces the domain-specific language (DSL) designed for the CLEVR VQA dataset.

"Table 6: All operations in the domain-specific language for CLEVR VQA."

<img src="https://s1.ax1x.com/2023/05/24/p97RfNd.png" style="zoom:80%;" />

"Table 7: The type system of the domain-specific language for CLEVR VQA.  "

<img src="https://s1.ax1x.com/2023/05/24/p97RI3t.png" style="zoom: 60%;" />

## Unfamiliar knowledge

**Note: May include buzz word and potential literature.**

## Resources

[Paper](), [Code]()

## Elementary drafts

**Note: May contain Chinese. This section will disappear once all drafts are embellished.**

<details>
	<summary>collapsed contents</summary>
		something
		<br>
		一些草稿
</details>
{{< embed-pdf url="../../pdfs/THE NEURO-SYMBOLIC CONCEPT LEARNER- INTERPRETING SCENES, WORDS, AND SENTENCES FROM NATURAL SUPERVISION.pdf" >}}

