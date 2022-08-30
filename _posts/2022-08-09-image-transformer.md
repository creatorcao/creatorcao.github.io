---
layout: post
published: true
title: Image Transformer
date: '2022-08-09'
tags: machine-learning
subtitle: Convolutional Neural Network (CNN) vs Vision Transformer (ViT)
---
<p align="left">
    <img src="/images/ML/image-transformer/no_padding_strides.gif" 
         width="300px" />
</p>


# CNN
**Pros**

CNN has inductive biases like translation invariance and locally restricted receptive field. Translational invariance recognizes an object even when its appearance varies, like changing orientation or zoom in or zoom out.

**Cons**
1. Specifically designed for images.
2. It has a domain-specific design and is not scalable for it to be domain agnostic. CNN uses pixel arrays where each pixel represents varying importance and is domain-specific.
3. It lacks a global understanding of the images. It only looks for the presence of the image's features and does not understand the structural dependency between its features.
4. Computationally expensive: each pixel bears varying importance for the target task, which causes redundancy in both computation and representations.

&nbsp;<br>

<p align="left">
    <img src="/images/ML/image-transformer/vit.gif" 
         width="600px" />
</p>

# [Vision Transformer](https://github.com/google-research/vision_transformer)

Transformers have great success with NLP and are now applied to images. CNN uses pixel arrays, whereas Visual Transformer(ViT) divides the image into visual tokens.

**Steps**
  
1. Split an image into patches (fixed sizes)
2. Flatten the image patches
3. Create lower-dimensional linear embeddings from these flattened image patches
4. Include positional embeddings
5. Feed the sequence as an input to a state-of-the-art transformer encoder
6. Pre-train the ViT model with image labels, which is then fully supervised on a big dataset
7. Fine-tune the downstream dataset for image classification

&nbsp;<br>
&nbsp;<br>

**Read more**
1. [Vision transformer tutorial notebooks](https://uvadlc-notebooks.readthedocs.io/en/latest/tutorial_notebooks/tutorial15/Vision_Transformer.html)
2. [Are Pre-trained Convolutions Better than Pre-trained Transformers?](https://arxiv.org/pdf/2105.03322.pdf)
3. [Implementation of vision transformer](https://github.com/lucidrains/vit-pytorch)

&nbsp;<br>
&nbsp;<br>
&nbsp;<br>
&nbsp;<br>

