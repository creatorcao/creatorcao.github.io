---
layout: post
published: true
title: 'Training Time '
date: '2022-08-30'
tag: machine-learning
subtitle: Apple M1 vs Google Colab
---

&nbsp;<br>
&nbsp;<br>

**PyTorch Metal Performance Shaders (MPS)**

1. setup GPU-acceleration 

2. check gpu: `import torch` `torch.backends.mps.is_available()`
   ```
      └> True
   ```
3. show CPU and GPU activity

   <img width="500" src="https://user-images.githubusercontent.com/54368185/187384477-6205a359-8e6b-4de0-95e2-099d7d77c946.png">

4. runtime 

   <img width = "300" src="https://user-images.githubusercontent.com/54368185/187384603-d3539b6a-6a99-42f9-bb67-eed27c9c3e89.png">


&nbsp;<br>
&nbsp;<br>
&nbsp;<br>


**Google Colab**

1. check GPU version: `!nvidia-smi -L`
   ```
     └> GPU 0: Tesla T4 (UUID: GPU-ceabb2dd-24b5-a045-1e0d-9d69acd13a7c)
   ```

2. show CPU and GPU activity

   <img width="500" alt="Screen Shot 2022-08-30 at 09 54 12" src="https://user-images.githubusercontent.com/54368185/187384599-96c2ce19-57f1-4aee-ab1a-12b0ba97b0d6.png">

3. runtime 

   <img width = "300" src="https://user-images.githubusercontent.com/54368185/187384580-b0cbea36-ee2b-4f4a-bb6e-e0f16a26c7b3.png">

&nbsp;<br>
&nbsp;<br>
The results shown above is by running the same script with 3366 images.
&nbsp;<br>
&nbsp;<br>

**Read more**
1. [Apple's M1 Pro Chip: Everything You Need to Know](https://www.macrumors.com/guide/m1-pro/#:~:text=as%20the%20%E2%80%8CM1%E2%80%8C.-,CPU,and%20two%20high%20efficiency%20cores.)
2. [Setup GPU-acceleration to PyTorch on Apple M1](https://towardsdatascience.com/gpu-acceleration-comes-to-pytorch-on-m1-macs-195c399efcc1)

&nbsp;<br>
&nbsp;<br>
&nbsp;<br>
&nbsp;<br>

