## Versatile Conv

### 目录说明
`vcnn.py`是Versatile Conv应用于VGG-16的一个实现，其中的VConv2d可以替换任意网络中的Conv2d层

`imagenet-vcnn.py`是ImageNet训练脚本（云上训练）

`config.png`是我们在云上训练的配置

### 精度
method	top1	top5
baseline 71.5  90.1
spatial versatile	72.2	91.1
spatial+channel versatile	70.5	89.8
