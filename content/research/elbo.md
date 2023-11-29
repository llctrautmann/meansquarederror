+++
title = 'Elbo'
date = 2023-11-29T15:06:38+01:00
draft = false
mathjax = true
+++

The formula for the ELBO in the context of the Variational Autoencoder is given by the following:
$$
\operatorname{ELBO}[\boldsymbol{\theta}, \boldsymbol{\phi}]=\int q(\mathbf{z} \mid \mathbf{x}, \boldsymbol{\theta}) \log [\operatorname{Pr}(\mathbf{x} \mid \mathbf{z}, \boldsymbol{\phi})] d \mathbf{z}-\mathrm{D}_{K L}[q(\mathbf{z} \mid \mathbf{x}, \boldsymbol{\theta}) \| \operatorname{Pr}(\mathbf{z})] \text {, }
$$