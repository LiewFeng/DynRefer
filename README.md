<div align=center>
  
# DynRefer: Delving into Region-level Multi-modality Tasks via Dynamic Resolution
</div>

This is the official implementaion of paper '[***DynRefer: Delving into Region-level Multi-modality Tasks via Dynamic Resolution***](assets/DynRefer_arxiv.pdf)'. This repository contains Pytorch training code, evaluation code.

<div align=center>

![Python 3.8](https://img.shields.io/badge/Python-3.8-green.svg?style=plastic)
![PyTorch 1.11](https://img.shields.io/badge/PyTorch-1.11-EE4C2C.svg?style=plastic)
[![LICENSE](https://img.shields.io/github/license/vasgaowei/ts-cam.svg)](LICENSE)
</div>


<div align=center>
<img src="assets/framework.png" width="90%">
</div>


## 1. Contents
- DynRefer: Delving into Region-level Multi-modality Tasks via Dynamic Resolution
  - [1. Contents](#1-contents)
  - [2. Introduction](#2-introduction)
  - [3. Results](#3-results)
  - [4. Start](#4-get-start)
  - [5. Contacts](#5-contacts)
  - [6. Acknowledgment](#6-acknowledgment)
  - [7. Citation](#7-citation)
 
## 2. Introduction

Region-level captioning is challenged by the caption degeneration issue, which refers to that pre-trained multimodal models tend to predict the most frequent captions but miss the less frequent ones. In this study, we propose a controllable region-level captioning (ControlCap) approach, which introduces control words to a multimodal model to address the caption degeneration issue. In specific, ControlCap leverages a discriminative module to generate control words within the caption space to partition it to multiple sub-spaces. The multimodal model is constrained to generate captions within a few sub-spaces containing the control words, which increases the opportunity of hitting less frequent captions, alleviating the caption degeneration issue. Furthermore, interactive control words can be given by either a human or an expert model, which enables captioning beyond the training caption space, enhancing the model’s generalization ability. Extensive experiments on Visual Genome and RefCOCOg datasets show that ControlCap respectively improves the CIDEr score by 21.6 and 2.2, outperforming the state-of-the-arts by significant margins.

## 3. Results

## 4. Start

- [**Installation**](./docs/install.md)

- [**Data**](./docs/data.md)

- [**Training and Evaluation**](./docs/train_and_eval.md)

## 5. Contacts
If you have any question about our work or this repository, please don't hesitate to contact us by emails or open an issue under this project.
- [zhaoyuzhong20@mails.ucas.ac.cn](zhaoyuzhong20@mails.ucas.ac.cn)
- [liufeng20@mails.ucas.ac.cn](liufeng20@mails.ucas.ac.cn)
- [wanfang@ucas.ac.cn](wanfang@ucas.ac.cn)

## 6. Acknowledgment

- Part of the code is borrowed from [LAVIS](https://github.com/salesforce/LAVIS), [GlaMM](https://github.com/mbzuai-oryx/groundingLMM), [Osprey](https://github.com/CircleRadon/Osprey/tree/main), [RAM](https://github.com/xinyu1205/recognize-anything), and [OVAD](), we sincerely thank them for their contributions to the community.

## 7. Citation

```text
@misc{zhao2024controlcap,
      title={ControlCap: Controllable Region-level Captioning}, 
      author={Yuzhong Zhao and Yue Liu and Zonghao Guo and Weijia Wu and Chen Gong and Fang Wan and Qixiang Ye},
      year={2024},
      eprint={2401.17910},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```

