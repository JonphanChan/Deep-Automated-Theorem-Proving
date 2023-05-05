# Predicting One-step Proofs in Formal Mathematics using Transformer-based Neural Networks
## Deep Automated Theorem Proving

**Xiao Wang** | xwang99@syr.edu   
**Junfan Chen** | jchen269@syr.edu

This project aims to investigate the potential of transformer models in mathematical proof verifica-
tion, address the challenges associated with utilizing transformer models in the field of mathematics,
and provide insights into the methodology and techniques employed in developing the transformer
model for Set.mm

### Preparation
The model is built with PyTorch, so we need to make sure the environment is built up sucessfully, here is a link about PyTorch: https://pytorch.org/docs/stable/index.html

After that, we would need to get all the packages prepared by running the following code:

```python
import matplotlib.pyplot as pt
import numpy as np
import torch as tr
import random
import requests
import math
import torch.nn.functional as F
from time import perf_counter
```

Here are all the packages we would need for the model, if the package is not able to import, try install it first, here is a link about how to install python package: https://packaging.python.org/en/latest/tutorials/installing-packages/

Before we run the model, we would need to get the data prepare. 

```python
!wget https://github.com/metamath/set.mm/raw/develop/set.mm
```

After runnning this code, we would have the dataset in our local environment.

### Model
We build two models for this project and each of them is a seq2seq architecure Transformer. Here are the structure of the two models:

#### Junfan's Architecture:

<p align="center">
  <img width="460" height="440" src=>
</p>


#### Xioa's Architecture:

<p align="center">
  <img width="460" height="440" src=>
</p>

With all the preparation steps get ready, we can run the code as these two workflow shown. And here are some sample of the output:

#### A glance at the prediction for each step:

<p align="center">
  <img width="470" height="180" src="https://user-images.githubusercontent.com/39479326/236565473-61032834-93e0-4dd3-a393-25bda158bac4.png">
</p>

#### The overall model performance (plots):

<p align="center">
  <img width="460" height="440" src="https://user-images.githubusercontent.com/39479326/236564850-e3a26494-4ef6-47c2-9ec5-1b445de8b6b3.png">
</p>

#### The overall model performance (avg accuracy):

<p align="center">
  <img width="460" height="440" src=>
</p>

#### Model evaluation:

<p align="center">
  <img width="470" height="160" src="https://user-images.githubusercontent.com/39479326/236565360-bf03a6b8-23c1-42d9-86a7-98159e6a8d4e.png">
</p>


