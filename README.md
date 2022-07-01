## 第二届清华人工智能挑战赛A赛（LGGAN）
成员：华东理工大学 梁磊、俞贤康、何旭峰
指导教师：华东理工大学 陈志华教授；上海交通大学 盛斌教授

## Contents
  - [Introduce](#Introduce)
  - [Requirement](#Requirement)
  - [Dataset Preparation](#Dataset-Preparation)
  - [Pretrained](Pretrained)
  - [Trainset](#trainset)
  
## Introduce
This is the LGGAN of jittor edition, which for a competition of Jittor AI

## Requirement
  - python>=3.7
  - jittor>=1.3.4
  - dominate>=2.3.1
  - dill
  - scikit-image

## Dataset Preparation
You can use the custom.py to load your own dataset for training,you can refer [this](https://cloud.tsinghua.edu.cn/f/1d734cbb68b545d6bdf2/?dl=1) to download the dataset

## Pretrained
The Pretrained model is already open,you can refer [this](https://pan.baidu.com/s/1Cncz5dS_0CRG_n-AHSOJWQ?pwd=acmz) to get it

## Trainset
1. Prepare dataset.
2. Change several parameters and then run `train.py` for training.
There are many options you can specify. To specify the number of GPUs to utilize, use `--gpu_ids`. If you want to use the second and third GPUs for example, use `--gpu_ids 1,2`.
3. Due to the limit of GPU memory,we set batchsize =1.If you have enough computing resource,you can set batchsize=2 or other.
4. Testing is similar to testing pretrained models. Use `--results_dir` to specify the output directory. `--how_many` will specify the maximum number of images to generate. By default, it loads the latest checkpoint. It can be changed using `--which_epoch`.

