# Towards semantic consistency: Dirichlet energy driven robust multi-modal entity alignment
This repository is the code of method, DESAlign, proposed in our paper: ["Towards Semantic Consistency: Dirichlet Energy Driven Robust Multi-Modal Entity Alignment"](https://arxiv.org/abs/2401.17859), which has been accepted by ICDE 2024.

## Introduction
Multi-Modal Entity Alignment (MMEA) is a pivotal task in Multi-Modal Knowledge Graphs (MMKGs), seeking to identify identical entities by leveraging associated modal attributes. However, real-world MMKGs confront the challenges of semantic inconsistency arising from diverse and incomplete data sources. This inconsistency is predominantly caused by the absence of specific modal attributes, manifesting in two distinct forms: disparities in attribute counts or the absence of certain modalities. Current methods address these issues through attribute interpolation, but their reliance on predefined distributions introduces modality noise, compromising original semantic information. Furthermore, the absence of a generalizable theoretical principle hampers progress towards achieving semantic consistency. In this work, we propose a generalizable theoretical principle by examining semantic consistency from the perspective of Dirichlet energy. Our research reveals that, in the presence of semantic inconsistency, models tend to overfit to modality noise, leading to over-smoothing and performance oscillations or declines, particularly in scenarios with a high rate of missing modality. To overcome these challenges, we propose DESAlign, a robust method addressing the over-smoothing caused by semantic inconsistency and interpolating missing semantics using existing modalities. Specifically, we devise a training strategy for multi-modal knowledge graph learning based on our proposed principle. Then, we introduce a propagation strategy that utilizes existing features to provide interpolation solutions for missing semantic features. DESAlign outperforms existing approaches across 60 benchmark splits, encompassing both monolingual and bilingual scenarios, achieving state-of-the-art performance. Experiments on splits with high missing modal attributes demonstrate its effectiveness, providing a robust MMEA solution to semantic inconsistency in real-world MMKGs.

## Dataset
The dataset we processed can be downloaded at [GoogleDrive](https://drive.google.com/file/d/1xYgXv8n1F8CBSNmYs5f3GfdJmrWHpxDJ/view?usp=drive_link)

## Environment
* Python = 3.7
* PyTorch = 1.6.0
* numpy = 1.19.2
* Transformers = 4.21.3
* easydict = 1.10
* unidecode = 1.3.6
* tensorboard = 2.11.0

## Cite
Please consider citing this paper if you find the code or data useful. Thanks a lot ~


```bigquery
@article{wang2024towards,
  title={Towards semantic consistency: Dirichlet energy driven robust multi-modal entity alignment},
  author={Wang, Yuanyi and Sun, Haifeng and Wang, Jiabo and Wang, Jingyu and Tang, Wei and Qi, Qi and Sun, Shaoling and Liao, Jianxin},
  journal={arXiv preprint arXiv:2401.17859},
  year={2024}
}
```
