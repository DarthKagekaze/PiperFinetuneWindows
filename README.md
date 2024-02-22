# PiperFinetuneWindows

#
##


# pip Installs needed

```
### I dont know what is best for torch, but this worked for me

pip install torch==1.13.1+cu116 --extra-index-url https://download.pytorch.org/whl/cu116

pip install pytorch-lightning==1.7.7

pip install torchmetrics==0.11.4

pip install gruut==

pip install gruut_ipa==

pip install numpy==1.26.4

pip install librosa==0.10.1

pip install onnxruntime

pip install onnxruntime-gpu

pip install Cython==0.29.36

pip install torchaudio==

pip install torchvision==


```






# Changes you must make

## Add this to the top of __ main __.py file to allow os/path to understand your PC locations

import os

import path

import platform 

import pathlib

plt = platform.system()

if plt == 'Linux': 

    pathlib.WindowsPath = pathlib.PosixPath



pathlib.PosixPath = pathlib.WindowsPath



## Go into the pytorch-lightning venv files, and add this to trainer.py


<br />
<br />
<br />
<br />

# monotonic_align
## To build monotonic_align for windows do...
## Also
## Comment out this line from the monotonic_align's __ init __.py file, like so?:

```

#maximum_path_c(path, neg_cent, t_t_max, t_s_max)

```
