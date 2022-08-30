---
layout: post
published: true
title: 'Image Annotator'
date: '2022-08-01'
tags: machine-learning
subtitle: COCO Annotator vs LabelMe
---

<p align="left">
<a href="https://github.com/facebookresearch/detectron2">
    <img src="https://camo.githubusercontent.com/69ce7a40db8bdee3e2a292950b5d84cd3f60cc8ac32bdce3316e40ca4130a71d/68747470733a2f2f692e696d6775722e636f6d2f414137496462512e706e67" 
         width="300" height="130" />
</a>
</p>

**[COCO Annotator](https://github.com/jsbroks/coco-annotator)** is in **[COCO](https://cocodataset.org/#home)** format, which can be used directly for training and validation for object detection tasks. It is safe, flexible and with multi-colored masks.

Following is the trouble-shooting for installing it on **Macbook M1**. After these steps, you can register an account by opening `http://localhost:5000` in your browser.

1. `brew install docker` or `docker -v`
   ```
	└> Cannot find docker.
   ``` 
     Try `brew install --cask docker` 
&nbsp;<br>
&nbsp;<br>

2. `docker-compose up`        
   ```
	└> Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running? 
   ```
    Manually start **Application** -> **Docker.app** 
&nbsp;<br>
&nbsp;<br>
 
3. `docker-compose up`     
   ```
	└> Worker fail to boot. 
   ``` 
    In the git repo folder, modify the _docker-compose.yml_ file -> - FILE_WATCHER=  (remove **True**) 
&nbsp;<br>
&nbsp;<br>
     
4. `docker-compose up`  
   ```
	└> Cannot host...  
   ```     
    **System Preferences** -> **Sharing** ->  
    - [x] **AirPlay Receiver** (uncheck this)


&nbsp;<br>
&nbsp;<br>

<p align="left">
<a href="https://github.com/wkentaro/labelme">
    <img src="https://raw.githubusercontent.com/wkentaro/labelme/main/labelme/icons/icon.png" 
         width="200" height="200" />
</a>
</p>

**[LabelMe](https://github.com/wkentaro/labelme)** is beginner-friendly and quick for rectangle boundary box drawing. You can download it with _.app_ or in 
_Python_. Please following the **[steps](https://github.com/creatorcao/mask-rcnn/blob/main/README.md)** after annotation to change the _.json_ format. 

&nbsp;<br>
&nbsp;<br>
&nbsp;<br>
&nbsp;<br>
