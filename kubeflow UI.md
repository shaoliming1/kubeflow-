# kubeflow UI
本小节主要来源于[官网教程](https://www.kubeflow.org/docs/other-guides/accessing-uis/). 

kubeflow包括许多web UIs. 本文档重点关于如何连接使用这些UI.


## Kubeflow UIs概览

* central **Kubeflow** UIs : 用于在kubeflow 应用中导航.
* **Pipelines**: kubeflow piplines dashboad
* **Notebook Servers**: 用于管理jupyter notebooks.
* **Kartib**: 用于调节超参数
* **Artifact Store**: for tracking of artifact metadata.

我们在172.16.215.116上的central Kubeflow UIs访问地址:http://172.16.215.116:31380, 如下图:

![avatar](./images/kubeflow_central_dashboard.png)

# [Set Up Your Notebooks](https://www.kubeflow.org/docs/notebooks/setup/)

This guide shows you how to set up a notebook server for your Jupyter notebooks in Kubeflow.

## Quick guide

1. 打开central Kubeflow UI,我们的地址为: http://172.16.215.116:31380
1. 在Kubeflow UI左边的面板上点击 **Notebook Servers**
1. 点击**NEW SERVER** 来创建notebook server.
1. 



## TroubleShouting
1. /api/workgroup/existing报错403
1. js库无法从google上拉取下来

![avatar](./images/workgroup_jquery.png)

问题1: 看着像$(namespace)这个没有替换成该变量的值的造成,将 **$(namespace)** 改成 **kubeflow**

