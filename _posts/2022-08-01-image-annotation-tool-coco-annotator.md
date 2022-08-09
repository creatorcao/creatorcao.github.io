---
layout: post
published: true
title: 'Image annotation tool '
date: '2022-08-01'
tags: machine-learning
subtitle: COCO Annotator vs LabelMe
---

<p align="center">
<a href="https://github.com/facebookresearch/detectron2">
    <img src="https://camo.githubusercontent.com/69ce7a40db8bdee3e2a292950b5d84cd3f60cc8ac32bdce3316e40ca4130a71d/68747470733a2f2f692e696d6775722e636f6d2f414137496462512e706e67" 
         width="500" height="200" />
</a>
</p>


This post is the trouble-shooting for installing [COCO Annotator](https://github.com/jsbroks/coco-annotator) on Macbook M1.

If you have the following issues when installing, please use the solutions below. 

After these steps, you can register an account by opening `http://localhost:5000` in your browser.

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
&nbsp;<br>
&nbsp;<br>
