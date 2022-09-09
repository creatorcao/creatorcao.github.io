---
layout: post
published: true
title: Untitled
subtitle: DistributedDataParallel in Pytorch
date: '2022-09-09'
tags: machine-learning
---


When I get access to the computer cluster, which provides 4 graphic cards by the department. 
1. `!python mnist.py -n 1 -g 1 -nr 0`
<img width="365" src="https://user-images.githubusercontent.com/54368185/189223116-6a2b9e1d-9ba7-4ece-89bc-0328208813ec.png">


2. `!python mnist-distributed.py.1 -n 1 -g 1 -nr 0`
<img width="361" src="https://user-images.githubusercontent.com/54368185/189223224-87184b40-2877-4ffd-864f-cf829903b01a.png">


3. `!python mnist-mixed.py -n 1 -g 1 -nr 0`
<img width="365" src="https://user-images.githubusercontent.com/54368185/189223426-2b78a6fc-b85d-4dce-a52d-0b0564faeeae.png">



transfer the code with your own data


![](https://user-images.githubusercontent.com/54368185/189344641-269ce539-9cba-4d15-b642-d82cc06814bf.png)


![](https://user-images.githubusercontent.com/54368185/189344666-ec1c7808-a949-4a10-8d3d-96e2d647c1d6.png)

![](https://user-images.githubusercontent.com/54368185/189344688-243472e2-a16c-4925-b517-9310ba36fa29.png)



![](https://user-images.githubusercontent.com/54368185/189344945-85f72dd4-8b24-4916-918e-ecfe9a995111.png)
