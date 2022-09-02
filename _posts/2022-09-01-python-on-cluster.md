---
layout: post
published: true
title: python-on-cluster
date: '2022-09-01'
tags: machine-learning
subtitle: Deep learning setup on computer cluster
---

**1. access cluster**

`ssh yourusername@hostname`, then input your password 

**2. check cpu and gpu **

`scontrol show nodes`

**3. show available software **

`module avail`

**4. setup your custom environment**

`module load anaconda` # check the absolute path and available conda

`conda create -n cp` # create a new environment called cp

`pip install matplotlib` # install packages

**5. transfer data**

Terminal: `sftp yourusername@hostname`

The remote path: `pwd` 

The local path: `lpwd`

Transfer from local to remote folder: `put file.py`

Transfer from remote folder to local: `get file.py`

**6. creating a job**

`touch submit.sh` # create a command file

`vi submit.sh` # edit 

```
#!/bin/bash

#SBATCH —job-name=test
 
module load anaconda

source activate cp

python run.py
```

then press **ESC**, type `:exit` and press **ENTER**

`sbatch submit.sh` # submit this command to cluster



&nbsp;<br>
&nbsp;<br>

#### Run Jupyter Lab

1. On cluster input: `jupyter notebook --no-browser --port=9999`

2. On local Terminal input: `ssh -NfL localhost:9999:localhost:9999 yourusername@hostname`

3. On local browser open: `http://localhost:9999`


&nbsp;<br>
&nbsp;<br>
&nbsp;<br>

