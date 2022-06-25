# Image-Colorization-Using-GAN
VLG Summer Open Project Submission 2022

## Table of Contents: 
* Project Overview
* Prerequisite Theory
* Data Description 
* Libraries used
* Steps followed
* Conclusion
* How to replicate on your device

## Overview of Project:
Colorizing black and white images has always been a difficult task which required a lot of human input and hardcoding. But this gruesome task could be automated with the use of an end-to-end deep learning pipeline. The network can take a black and white image as an input, then produce a fully colored image as output.
Therefore, the final goal of this project is to colorize black and white images with the help of Conditional Generative Adversarial Networks (or CGANs). 

Colorizing black and white images could be broadly categorized as an image to image translation task. Similar to language translation, we can have two different images relay the same information, hence one could be "translated" to the other. This image to image translation task has already been researched in a paper called <a href=https://arxiv.org/pdf/1611.07004.pdf>pix2pix Paper</a>, which again, uses Conditional GAN to fulfil the requirement.

## Prerequisite Theory
Before moving on to the description of model and results, let's first understand some basic things that are used throughout the project.

### Image Spaces
Since we are gonna be working with Black and white images, it is better to move the color space to L\*a\*b from RGB. This is because of two reasons:
* L\*a\*b space requires us to generate only two channels (*a and *b) using the L channel. Compare that with an RGB image, we can see that we are required to generate all three channels. This reduces the complexity of the network, hence reducing the training and testing time drastically.
* Also, it is easier to work with L\*a\*b images, simply because the input and output are very clearly divided where L is the input and \*a\*b is the output, which could be concatencated to produce the final image. No extra conversions are required, as compared to working with RGB image space.

Read more on <a href="https://en.wikipedia.org/wiki/CIELAB_color_space">L\*a\*b here</a>

### Conditional GANs


## Data Description:  
We are given the COCO image dataset which contains various different images and our task is to use the black and white version of validation images, and produce a colorized version that is decently similar to the original image.
## Libraries used:
* Numpy
* Matplotlib
* torch
* torchvision<br>
* PIL
* os module of python
* tqdm
* shutil

## Steps Followed

## Conclusion

## How to replicate on your device
