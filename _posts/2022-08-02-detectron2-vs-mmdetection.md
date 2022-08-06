---
layout: post
published: true
title: Detectron2 vs MMDetection
date: '2022-08-02'
tags: machine-learning
---

![](https://raw.githubusercontent.com/facebookresearch/detectron2/main/.github/Detectron2-Logo-Horz.svg)(https://github.com/facebookresearch/detectron2)

**Steps** [(demo)](https://github.com/creatorcao/mask-rcnn/blob/main/Detectron2_tutorial.ipynb)
- install Detectron2 
- configs: pretrained models 
- dataset registration: custom dataset 
- trainer and predictor

Pros:
- modular, flexible, and extensible for efficient training on single or multiple GPUs
- the successor of Detectron and maskrcnn-benchmark includes state-of-the-art object detection algorithms such as DensePose, panoptic feature pyramid networks, and numerous variants of the pioneering Mask R-CNN
- developed by Facebook AI Research, using PyTorch

Cons:
- limited state-of-the-art models
- good at detection and segmentation but not classification
- difficult to modify the deep learning model

&nbsp;<br>

![](https://raw.githubusercontent.com/open-mmlab/mmdetection/master/resources/mmdet-logo.png)(https://github.com/open-mmlab/mmdetection)

**Steps** [(demo)](https://github.com/open-mmlab/mmdetection/blob/master/demo/MMDet_InstanceSeg_Tutorial.ipynb)
- install MMDetection
- configs: pretrained models 
- custom dataset
- modify the configs
- train_detector and inference_detector

Pros: 
- fast 
- multiple state-of-the-art object detection models
- also includes scripts for model conversion, benchmarking, hyper-parameter optimization

Cons:
- restricted to some object detection and instance segmentation models  
- not support image classification

&nbsp;<br>
&nbsp;<br>
I choose Detectron2 because of the [First Impression](https://en.wikipedia.org/wiki/First_impression_(psychology)) effect. I saw one or two posts, implemted it, and was attracted by the colorful masks and easy steps. Actually, the relative fast speed of **MMDetection** does not have large advantage.

&nbsp;<br>
&nbsp;<br>

### Reference
1. [https://mmdetection.readthedocs.io/en/latest/model_zoo.html#comparison-with-detectron2](https://mmdetection.readthedocs.io/en/latest/model_zoo.html#comparison-with-detectron2)
2. [https://www.libhunt.com/compare-mmdetection-vs-detectron2?ref=compare](https://www.libhunt.com/compare-mmdetection-vs-detectron2?ref=compare)


&nbsp;<br>
&nbsp;<br>
&nbsp;<br>
&nbsp;<br>
