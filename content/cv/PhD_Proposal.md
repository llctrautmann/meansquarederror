+++
title = 'PhD Proposal'
date = 2024-03-25T11:06:17+01:00
draft = true
mathjax = true
+++

## What I plan to do in my PhD
The general reserach I am pursuing in my Phd is low-field MRI improvements with super-resolutions. models. I want to learn how we can use low-field MRI scanner data and medical grade high resolution image data to build a data pipeline across multiple models that does three things:

1) Output high resolution images that match medical grade HR images for a regualar MRI machine
2) Model the model uncertainty in across the super-resolution model and any precursor and post-processing models
3) Model the data uncertainty from the input data to the output images

This leads to the model chain outputting three images, the acutal image, an uncertainty map for the model, and an uncertainty map for the data.

The alpha prototype I am working on right now, will be a deep esemble Super-Resolution model based on the DenseSR-Net architecture. This will allow me to build a SR model and add UQ for the model pipeline.

## Hard nuts to crack
There are mulitple milestones that I want to achive:

Firstly, build a valuable dataset for publication that allows researchers to work with low-field data and provide a constrastive dataset from the same patient at the same time. This requires some work on distortions which I have not been able to delve deeper into this topic but it will definitely require some further work. 

Secondly , build the pipeline from reconstruction from k-space to the super-resolution model. I will start with the super-resolution model and then see if I can chain in other models for the reconstruction (pre-super resolution) and biomarker identification (post super-resolution).

Thirdly, current approaches are not yet able to break the assumption that pixel-values are assumed to be independent which is not true in the underlying tissue in the body. 


## Tools
The main framework I will be using is JAX. Documentation will happen on [Github](https://github.com/llctrautmann) and publications are aimed at high-impact papers.

## Roadmap & Progress
