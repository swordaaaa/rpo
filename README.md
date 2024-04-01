# [NeurIPS 2023] Reduced Policy Optimization for Continuous Control with Hard Constraints

## **Note!!!**
**We apologize for uploading an incorrect version of the EVOPF-v0 environment. Concretely, the ```step``` function of the EVOPF-v0 environment returns the current state rather than the next state incorrectly. So, if you are using the code before, please modify this bug, or delete it and clone the newest version. You can reproduce the result reported in our paper with this modification. Apologize again!!!**

Code release for **Reduced Policy Optimization for Continuous Control with Hard Constraints (NeurIPS 2023)**.

[[paper]](#) [[project page]](#)

![](./img/RPO_pipeline.jpg)

## Requirements
```
numpy                         1.21.6
torch                         1.13.1
gym                           0.19.0
matplotlib                    3.5.2
scipy                         1.9.1
scikit-learn                  1.0.2
pandas                        1.4.4
pygame                        2.1.0
pycairo                       1.11.0
igraph                        0.10.8
```
## Preparation

To run the experiments, you need to first install the python package rpo via running `pip install -e .` in the current directory.

## Getting started
Then, you can simply 

run `python scripts/cart_exp.py` to re-implement our experiments on the Safe Cartpole environment using RPODDPG algorithm.

run `python scripts/pen_exp.py` to re-implement our experiments on the Spring Pendulum environment using RPODDPG algorithm.

run `python scripts/evopf_exp.py` to re-implement our experiments on the OPF with Battery Energy Storage environment using RPODDPG algorithm.

run `python scripts/cart_exp_sac.py` to re-implement our experiments on the Safe Cartpole environment using RPOSAC algorithm.

run `python scripts/pen_exp_sac.py` to re-implement our experiments on the Spring Pendulum environment using RPOSAC algorithm.

run `python scripts/evopf_exp_sac.py` to re-implement our experiments on the OPF with Battery Energy Storage environment using RPOSAC algorithm.

## Citation
If you find this repository useful in your research, please consider citing:

```
@inproceedings{
ding2023reduced,
title={Reduced Policy Optimization for Continuous Control with Hard Constraints},
author={Shutong Ding and Jingya Wang and Yali Du and Ye Shi},
booktitle={Thirty-seventh Conference on Neural Information Processing Systems},
year={2023},
url={https://openreview.net/forum?id=fKVEMNmWqU}
}
