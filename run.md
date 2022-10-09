﻿
# Usage Guide

------------------

## Prerequisites

The major libraries to run the code are as follow.

- [PyTorch==1.8.0][pytorch]
- [scikit-learn==0.24.2][sklearn]
- [scipy==1.5.2][scipy]

## Feature extraction

- Calculate vectors of the  Inception-v3-RGB and Inception-v3-Flow features according to the [URL][tsn].
- Calculate vectors of the  VGGish feature according to the [URL][VGGish].

## Data Preparation

Download the feature vectors of VideoEmotion from [Baiduyun][urldata], and the password is ``785q``. Then, extract the downloaded files to the directory ``./data``.

## Testing Provided Models

Download the trained models for VideoEmotion from [Baiduyun][urlmodel] by using the password ``umfn``, and copy the downloaded directorys to the source code directory. To evaluate the models trained on VideoEmotion, run the scripts as follows.

```
./test-VideoEmotion.sh
```

## Training Model

To train the model on VideoEmotion, run the scripts as follows.

```
./train-VideoEmotion.sh
```

## Reference

If you find the code useful, please cite the following paper:

```
@article{umfn,
author = {Yi, Yun and Wang, Hanli and Tang, Pengjie},
title = {Unified multi-stage fusion network for affective video content analysis},
journal = {Electronics Letters},
volume = {58},
number = {21},
pages = {795-797},
doi = {https://doi.org/10.1049/ell2.12605},
year = {2022}
}
```

[pytorch]:https://pytorch.org
[sklearn]:http://scikit-learn.org/stable/index.html
[scipy]:https://www.scipy.org
[tsn]:https://github.com/yjxiong/temporal-segment-networks
[VGGish]:https://github.com/tensorflow/models/tree/master/research/audioset
[urldata]:https://pan.baidu.com/s/1aRFdnJB_bRJymuHKwDNbWQ
[urlmodel]:https://pan.baidu.com/s/1GsMd7U3v18US7JZWQWLoYQ
