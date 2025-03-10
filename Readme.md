# Diffusion Models Tutorial (Python)

This repository shows you the implementation of representative diffusion model (DM) algorithms from scratch in Python (PyTorch), with theoretical aspects behind code.

## Table of Contents

- [Variational Auto-Encoder (VAE)](01-vae.ipynb)
- [Denoising Diffusion Probabilistic Models (DDPM)](02-ddpm.ipynb)
- [Score Matching with Langevin Dynamics (SMLD)](03-smld.ipynb)
- [Score-based generative modeling with Stochastic Differential Equation (SDE)](04-sde.ipynb)

Historically image generation (including text-to-image models) has been developed and improved by adopting GAN-based methods and autoregressive methods in 2014 - 2021.<br>
In recent works, diffusion models have achieved great success, outperforming these previous approaches in the quality of image generation. (GAN-based approach, however, still has its own beneficial aspects. See the below note.)

In this repository, I'll focus on implementing diffusion model's algorithms.<br>
To focus on diffusion algorithms, all experiments use unconditional (plain) diffusion models. (Class-conditional models and diffusion guidances are out of scope.)

> Note : The drawback of diffusion models (compared to GAN) is the computational efficiency. As you will see in the examples in this repository, diffusion models requires hundreds or thousands of iterations to generate an image - i.e., slow speed for image generation.<br>
> There exist works and challenges to improve the sampling speed in diffusion models. (See DDIM in [this notebook](./02-ddpm.ipynb).)

*Tsuyoshi Matsuzaki @ Microsoft*
