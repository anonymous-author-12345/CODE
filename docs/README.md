# CODE : Confident Ordinary Differential Editing
<br>

<p align="center">
<img src="https://github.com/" width="320"/>
</p>

[**Project**](https://anonymous-author-12345.github.io/CODE/) | [**Paper**]() | [**Colab**]()

PyTorch implementation of **CODE: Confident Ordinary Differential Editing** (2024).

## Overview
CODE aims to handle guidance image that are Out-of-Distribution in a systematic manner. The key idea is to reverse stochastic process of SDE-based generative models, using the associated Probability Flow ODE in combination with a Confidence Based Clipping, and to make score-based updates in the latent spaces, method as illustrated in the figure below. Given an input image for editing, such as a stroke painting or a corrupted low-quality image, we can make the artifacts undetectable, while preserving the semantic of the image. CODE offers a natural and grounded method to balance the trade-off realism-fidelity of the generated outputs. The user can arbitrarily choose to increase realism in the image or to conserve more of the image guidance. 

<p align="center">
<img src="https://github.com/" />
</p>


## Getting Started


To generate images, please update the .yaml config file according to your needs, then run

```
python -m code.main.py --trainer=
```
