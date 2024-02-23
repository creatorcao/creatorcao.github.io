---
layout: post
published: false
title: Distributed Data Parallel
subtitle: DistributedDataParallel in Pytorch
date: '2022-09-09'
tag: machine-learning
---
I run the same scripts on Google Colab (1 GPU node, 1 graphic card, white) and a computer cluster (1 GPU node, 4 graphic cards, black) to compare the training speed.

**1. regular run**

```
!python mnist.py -n 1 -g 1 -nr 0  # 1 node, 1 gpu, node_rank 0
```
<p align="left">
    <img src="https://user-images.githubusercontent.com/54368185/189223116-6a2b9e1d-9ba7-4ece-89bc-0328208813ec.png" 
         width="385" />
</p>

```
python mnist.py -n 1 -g 1 -nr 0  # 1 node, 1 gpu, node_rank 0  
```
<p align="left">
    <img src="https://user-images.githubusercontent.com/54368185/189344945-85f72dd4-8b24-4916-918e-ecfe9a995111.png" 
         width="340" />
</p>

&nbsp;<br>

**2. distributed run**

```
!python mnist-distributed.py.1 -n 1 -g 1 -nr 0  # 1 node, 1 gpu, node_rank 0
```

<p align="left">
    <img src="https://user-images.githubusercontent.com/54368185/189223224-87184b40-2877-4ffd-864f-cf829903b01a.png" 
         width="385" />
</p>

```
python mnist-distributed.py.1 -n 1 -g 4 -nr 0  # 1 node, 4-gpu, node_rank 0
```

<p align="left">
    <img src="https://user-images.githubusercontent.com/54368185/189344688-243472e2-a16c-4925-b517-9310ba36fa29.png" 
         width="340" />
</p>

&nbsp;<br>

**3. mixed-precision run**

```
!python mnist-mixed.py -n 1 -g 1 -nr 0  # 1 node, 1 gpu, node_rank 0
```

<p align="left">
    <img src="https://user-images.githubusercontent.com/54368185/189223426-2b78a6fc-b85d-4dce-a52d-0b0564faeeae.png" 
         width="385" /> 
</p>

```
python mnist-mixed.py -n 1 -g 4 -nr 0  # 1 node, 4-gpu, node_rank 0
```

<p align="left">
<img src="https://user-images.githubusercontent.com/54368185/189344666-ec1c7808-a949-4a10-8d3d-96e2d647c1d6.png" 
         width="340" />
</p>


&nbsp;<br>
&nbsp;<br>
&nbsp;<br>

**Read More**
1. [Training script on mnist data](https://github.com/yangkky/distributed_tutorial/blob/master/src/mnist-distributed.py)
2. [Training script on cifar10 data](https://github.com/Taited/DistributedTutorial/blob/master/cifar10_ddp.py)
3. [Distributed data parallel training in Pytorch](https://yangkky.github.io/2019/07/08/distributed-pytorch-tutorial.html)

&nbsp;<br>
&nbsp;<br>
&nbsp;<br>
    
    
    
    
