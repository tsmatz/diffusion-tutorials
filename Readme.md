# Diffusion Models Tutorial (Python)

This repository shows you the implementation of representative diffusion model algorithms and its guidance techniques from scratch in Python (PyTorch), with theoretical aspects behind code.

## Table of Contents

- [Variational Auto-Encoder (VAE)](01-vae.ipynb)
- [Denoising Diffusion Probabilistic Models (DDPM)](02-ddpm.ipynb)
- [Score Matching with Langevin Dynamics (SMLD)](03-smld.ipynb)
- [Score-based generative modeling with Stochastic Differential Equation (SDE)](04-sde.ipynb)
- [Conditional Diffusion Models](05-class-conditional.ipynb)
- [Classifier Diffusion Guidance](06-classifier-guidance.ipynb)
- [Classifier-free Diffusion Guidance](07-classifier-free-guidance.ipynb)

In the former part in this repository (tutorial 1 - 4), I'll focus on diffusion model's algorithms.<br>
In the latter part (tutorial 5 - 7), we proceed to steer diffusion models with external knowledge (such as, a class or a generic text prompt) and learn the fundamental of diffusion guidance.

Historically image generation (including text-to-image models) has been developed and improved by adopting GAN-based methods and autoregressive methods in 2014 - 2021.<br>
In recent works, diffusion models have achieved great success, outperforming these previous approaches in the quality of image generation. (GAN-based approach, however, still has its own beneficial aspects. See below note.)

> Note : The drawback of diffusion models (compared to GAN) is the computational efficiency. As you will see in the examples in this repository, diffusion models requires hundreds or thousands of iterations to generate an image - i.e., slow speed for image generation.<br>
> There exist works and challenges to improve the sampling speed in diffusion models. (See note for DDIM in [this notebook](./02-ddpm.ipynb).)

*Tsuyoshi Matsuzaki @ Microsoft*
