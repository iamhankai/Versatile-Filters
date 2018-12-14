## Versatile Filters

Versatile Filters on Pytorch

Paper: [Learning Versatile Filters for Efficient Convolutional Neural Networks (NeurIPS 2018)](https://papers.nips.cc/paper/7433-learning-versatile-filters-for-efficient-convolutional-neural-networks)

### Files description
`vcnn.py` is the implementation of Versatile Convolution (an example of VGG-16). The `VConv2d` class can be used to replace the `nn.Conv2d` in any CNN.

`imagenet-vcnn.py` is the script for training ImageNet on Cloud DLS.

`config.png` is a config example on Cloud DLS.

### Hyper-paprameters
In `VConv2d`:
- `delta`: (c-\hat{c}) in Eq.(6)
- `g`: g in Eq.(6)

## Performance
| method                    | top1 acc | top5 acc |
|---------------------------|----------|----------|
| baseline                  | 71.5     | 90.1     |
| spatial versatile         | 72.2     | 91.1     |
| spatial+channel versatile | 70.4     | 89.6     |

---
Chinese:

### 目录说明
`vcnn.py`是Versatile Conv应用于VGG-16的一个实现，其中的VConv2d可以替换任意网络中的Conv2d层

`imagenet-vcnn.py`是ImageNet训练脚本（云上训练）

`config.png`是我们在云上训练的配置

### 超参
`VConv2d`类中:
- `delta`: (c-\hat{c}) in Eq.(6)
- `g`: g in Eq.(6)

### 精度
| method                    | top1 acc | top5 acc |
|---------------------------|----------|----------|
| baseline                  | 71.5     | 90.1     |
| spatial versatile         | 72.2     | 91.1     |
| spatial+channel versatile | 70.4     | 89.6     |
