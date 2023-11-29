+++
title = 'Init'
date = 2023-11-29T15:00:19+01:00
draft = false
mathjax = true
+++

We need more opinions.


$$
\begin{aligned}
\mathrm{ELBO}[\mathbf{\theta}, \mathbf{\phi}] & =\int q(\mathbf{z} \mid \mathbf{\theta}) \log \left[\frac{\operatorname{Pr}(\mathbf{x}, \mathbf{z} \mid \mathbf{\phi})}{q(\mathbf{z} \mid \mathbf{\theta})}\right] d \mathbf{z} \\
& =\int q(\mathbf{z} \mid \mathbf{\theta}) \log \left[\frac{\operatorname{Pr}(\mathbf{x} \mid \mathbf{z}, \mathbf{\phi}) \operatorname{Pr}(\mathbf{z})}{q(\mathbf{z} \mid \mathbf{\theta})}\right] d \mathbf{z} \\
& =\int q(\mathbf{z} \mid \mathbf{\theta}) \log [\operatorname{Pr}(\mathbf{x} \mid \mathbf{z}, \mathbf{\phi})] d \mathbf{z}+\int q(\mathbf{z} \mid \mathbf{\theta}) \log \left[\frac{\operatorname{Pr}(\mathbf{z})}{q(\mathbf{z} \mid \mathbf{\theta})}\right] d \mathbf{z} \\
& =\int q(\mathbf{z} \mid \mathbf{\theta}) \log [\operatorname{Pr}(\mathbf{x} \mid \mathbf{z}, \mathbf{\phi})] d \mathbf{z}-\mathrm{D}_{K L}[q(\mathbf{z} \mid \mathbf{\theta}) \| \operatorname{Pr}(\mathbf{z})],
\end{aligned}
$$