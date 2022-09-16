---
layout: post
published: true
title: Run Python on computer cluster
date: '2022-09-01'
tags: machine-learning
subtitle: Deep learning setup on high performance computing (HPC) systems
---

**1. Access cluster**

`ssh yourusername@hostname`, then input your password 

**2. Check cpu and gpu**

`scontrol show nodes`

**3. Show available software**

`module avail`

**4. Setup your custom environment**

`module load anaconda` # check the absolute path and available version

`conda create -n cp` # create a new environment called cp

`pip install matplotlib` # install packages

**5. Transfer data**

Terminal: `sftp yourusername@hostname`

The remote path: `pwd` 

The local path: `lpwd`

Transfer from local to remote folder: `put file.py`

Transfer from remote folder to local: `get file.py`

**6. Creating a job**

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

**Read More**

1. [Slurm CheatSheet](https://slurm.schedmd.com/pdfs/summary.pdf)

2. [Use SFTP transfer files with a remote server](https://www.digitalocean.com/community/tutorials/how-to-use-sftp-to-securely-transfer-files-with-a-remote-server)

&nbsp;<br>
&nbsp;<br>
&nbsp;<br>
