# The Devil is in the Details: Delving into Unbiased Data Processing for Human Pose Estimation

## Introduction

[ALGORITHM]

```bibtex
@InProceedings{Huang_2020_CVPR,
author = {Huang, Junjie and Zhu, Zheng and Guo, Feng and Huang, Guan},
title = {The Devil Is in the Details: Delving Into Unbiased Data Processing for Human Pose Estimation},
booktitle = {The IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
month = {June},
year = {2020}
}
```

Note that, UDP also adopts the unbiased encoding/decoding algorithm of [DARK](/configs/top_down/darkpose/README.md).

## Results and models

### 2d Human Pose Estimation

#### Results on COCO val2017 with detector having human AP of 56.4 on COCO val2017 dataset

| Arch  | Input Size | AP | AP<sup>50</sup> | AP<sup>75</sup> | AR | AR<sup>50</sup> | ckpt | log |
| :----------------- | :-----------: | :------: | :------: | :------: | :------: | :------: |:------: |:------: |
| [pose_hrnet_w32_udp](/configs/top_down/udp/coco/hrnet_w32_coco_256x192_udp.py)  | 256x192 | 0.760 | 0.907 | 0.827 | 0.811 | 0.945 | [ckpt](https://download.openmmlab.com/mmpose/top_down/udp/hrnet_w32_coco_256x192_udp-aba0be42_20210220.pth) | [log](https://download.openmmlab.com/mmpose/top_down/udp/hrnet_w32_coco_256x192_udp_20210220.log.json) |
| [pose_hrnet_w32_udp_regress](/configs/top_down/udp/coco/hrnet_w32_coco_256x192_udp_regress.py)  | 256x192 | 0.758 | 0.908 | 0.823 | 0.812 | 0.943 | [ckpt](https://download.openmmlab.com/mmpose/top_down/udp/hrnet_w32_coco_256x192_udp_regress-be2dbba4_20210222.pth) | [log](https://download.openmmlab.com/mmpose/top_down/udp/hrnet_w32_coco_256x192_udp_regress_20210222.log.json) |
