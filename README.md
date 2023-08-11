
# DECA: Detailed Expression Capture and Animation

This is a fork of https://github.com/cedro3/DECA with a couple bug fixes for it to work with Google Colab running Python 3.10


## Installation
- Run the following code inside the colab notebook.
```python
!pip install pip setuptools wheel --upgrade
!pip install -r requirements.txt
!pip install 'git+https://github.com/facebookresearch/pytorch3d.git@stable'
```

- Download data
    - Register at https://flame.is.tue.mpg.de/register.php
    - Sign in and download data form [FLAME 2020 model](https://flame.is.tue.mpg.de/download.php). 
    - Unzip the file
    - Copy `generic_model.pkl` to `data` folder

## Demo

```python
!python demos/demo_reconstruct.py -i TestSamples/examples --saveDepth True --saveObj True
```

demo_reconstruct\
<p align="left"> 
<img src="TestSamples/examples/results/00_vis.jpg">
</p>
<p align="left"> 
<img src="TestSamples/examples/results/01_vis.jpg">
</p>
<p align="left"> 
<img src="TestSamples/examples/results/02_vis.jpg">
</p>

```python
!python demos/demo_teaser.py
# TODO: fix errors (not currently working in colab)
```

demo_teaser\
<p align="left"> 
<img src="TestSamples/teaser/results/teaser.gif">
</p>


