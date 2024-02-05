---
title: 'Dense Blocks'
date: 2024-02-05T13:18:43+01:00
draft: false
mathjax: true
---

```python
import torch
import torch.nn as nn

class DenseBlock(nn.Module):
    def __init__(self, in_channels, kernel_size=3, stride=1, padding=1, activation='relu'):
        super(DenseBlock, self).__init__()
        self.feature_maps = torch.linspace(16, 128, 8).int()
        self.layers = nn.ModuleList()

        for i in range(len(self.feature_maps)):
            self.layers.append(nn.Sequential(
                nn.Conv2d(in_channels + (i * 16), 16, kernel_size=kernel_size, stride=stride, padding=padding),
                nn.BatchNorm2d(16),
                nn.ReLU(inplace=True) if activation == 'relu' else nn.GELU(),
            ))

    def forward(self, x):
        outputs = [x]
        for layer in self.layers:
            x = layer(torch.cat(outputs, dim=1))
            outputs.append(x)
        return torch.cat(outputs, dim=1)
```
