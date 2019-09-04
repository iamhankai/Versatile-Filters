## Versatile Filters

Code for paper: [Yunhe Wang, et al. Learning Versatile Filters for Efficient Convolutional Neural Networks (NeurIPS 2018)](https://papers.nips.cc/paper/7433-learning-versatile-filters-for-efficient-convolutional-neural-networks)

### Files description
Platform: Pytorch 0.4

`vcnn.py` is the implementation of Versatile Convolution (an example of VGG-16). The `VConv2d` class can be used to replace the `nn.Conv2d` in any CNN.

`imagenet-vcnn.py` is the script for training ImageNet on Huawei Cloud DLS.

### Getting Started
Run `imagenet-vcnn.py` to train and test the model.

### Hyper-paprameters
In `VConv2d`:
- `delta`: (c-\hat{c}) in Eq.(6)
- `g`: g in Eq.(6)

### Performance
| backbone | method                    | top1 acc | top5 acc |
|--------|---------------------------|----------|----------|
| VGG-16 | spatial versatile filters        | 72.2     | 91.1     |

### Citation
If you use these models in your research, please cite:
```
@inproceedings{wang2018learning,
  title={Learning versatile filters for efficient convolutional neural networks},
  author={Wang, Yunhe and Xu, Chang and Chunjing, XU and Xu, Chao and Tao, Dacheng},
  booktitle={Advances in Neural Information Processing Systems},
  pages={1608--1618},
  year={2018}
}
```

### Contributing
We appreciate all contributions. If you are planning to contribute back bug-fixes, please do so without any further discussion.

If you plan to contribute new features, utility functions or extensions to the core, please first open an issue and discuss the feature with us. Sending a PR without discussion might end up resulting in a rejected PR, because we might be taking the core in a different direction than you might be aware of.