# PiperFinetuneWindows

#
##

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

