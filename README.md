# Awesome Large Vision-Language Model
Awesome Large Vision-Language Model: A Curated List of Large Vision-Language Model

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/SuperBruceJia/Awesome-Large-Vision-Language-Model) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Made With Love](https://img.shields.io/badge/Made%20With-Love-red.svg)](https://github.com/SuperBruceJia/Awesome-Large-Vision-Language-Model)

This repository, called **Large Vision-Language Model**, contains a collection of resources and papers on **Large Vision-Language Models** and **Medical Foundation Models**. 

*Welcome to share your papers, thoughts, and ideas by [submitting an issue](https://github.com/SuperBruceJia/Awesome-Large-Vision-Language-Model/issues/new)!* 

## Contents
- [Presentations](#Presentations)
- [Books](#Books)
- [Benchmarks](#Benchmarks)
- [Papers](#Papers)
  - [Survey](#Survey)
  - [Multimodal Large Language Models (MM-LLMs)](#Multimodal-Large-Language-Models)
    - [Alignment Before Projection](#Alignment-Before-Projection)
    - [Linear Layer Projection](#Linear-Layer-Projection)
    - [Intermediate Networks](##Intermediate-Networks)
    - [Prompt Tuning](#Prompt-Tuning)
  - [Contrastive Language-Image Pre-Training](#Contrastive-Language-Image-Pre-Training)
    - [Intermediate Networks](#Intermediate-Networks)
    - [Simple Contrastive Learning Paradigms](#Simple-Contrastive-Learning-Paradigms)
  - [Universal Embedding Space](#Universal-Embedding-Space)

# Presentations
**Recent Advances in Vision Foundation Models**\
_Chunyuan Li, Zhe Gan, Zhengyuan Yang, Jianwei Yang, Linjie Li, Lijuan Wang, Jianfeng Gao_\
CVPR 2023 Tutorial, [[Paper](https://arxiv.org/abs/2309.10020)] [[Webpage](https://vlp-tutorial.github.io/2023/)]\
18 Sep 2023

**A Vision-and-Language Approach to Computer Vision in the Wild: Building a General-Purpose Assistant in the Visual World Towards Building and Surpassing Multimodal GPT-4**\
_Chunyuan Li_\
Deep Learning Team, Microsoft Research, Redmond, [[Presentations](https://chunyuan.li/doc/talk_cvinw_instruction_june2.pdf)]\
01 May 2023

# Books
**Foundation Models for Natural Language Processing - Pre-trained Language Models Integrating Media**\
*Gerhard Paaß, Sven Giesselbach*\
Artificial Intelligence: Foundations, Theory, and Algorithms (Springer Nature), [[Link](https://link.springer.com/book/10.1007/978-3-031-23190-2)]\
16 Feb 2023

# Benchmarks

# Papers
## Survey
**MM-LLMs: Recent Advances in MultiModal Large Language Models**\
_Duzhen Zhang, Yahan Yu, Jiahua Dong, Chenxing Li, Dan Su, Chenhui Chu, Dong Yu_\
ACL 2024, [[Paper](https://arxiv.org/abs/2401.13601)] [[Webpage](https://mm-llms.github.io/archives/)]\
Note: Categorize MM-LLMs by Modality Encoder, Input Projector, LLM Backbone, Output Projector, and Modality Generator\
28 May 2024

## Multimodal Large Language Models
### Alignment Before Projection
**Video-LLaVA: Learning United Visual Representation by Alignment Before Projection**\
_Bin Lin, Yang Ye, Bin Zhu, Jiaxi Cui, Munan Ning, Peng Jin, Li Yuan_\
arXiv, [[Paper](https://arxiv.org/abs/2311.10122)] [[Codes](https://github.com/PKU-YuanGroup/Video-LLaVA)]\
21 Nov 2023

### Intermediate Networks
**NExT-GPT: Any-to-Any Multimodal LLM**\
*Shengqiong Wu, Hao Fei, Leigang Qu, Wei Ji, Tat-Seng Chua*\
ICML 2024, [[Paper](https://arxiv.org/abs/2309.05519)] [[Codes and Dataset](https://github.com/NExT-GPT/NExT-GPT)] [[Webpage](https://next-gpt.github.io/)]\
25 Jun 2024

**ImageBind-LLM: Multi-modality Instruction Tuning**\
_Jiaming Han, Renrui Zhang, Wenqi Shao, Peng Gao, Peng Xu, Han Xiao, Kaipeng Zhang, Chris Liu, Song Wen, Ziyu Guo, Xudong Lu, Shuai Ren, Yafei Wen, Xiaoxin Chen, Xiangyu Yue, Hongsheng Li, Yu Qiao_\
arXiv, [[Paper](https://arxiv.org/abs/2309.03905)] [[Codes](https://github.com/OpenGVLab/LLaMA-Adapter)]\
11 Sep 2023

### Linear Layer Projection
**LLaVA-OneVision: Easy Visual Task Transfer**\
_Bo Li, Yuanhan Zhang, Dong Guo, Renrui Zhang, Feng Li, Hao Zhang, Kaichen Zhang, Yanwei Li, Ziwei Liu, Chunyuan Li_\
arXiv, [[Paper](https://arxiv.org/abs/2408.03326)] [[Codes](https://github.com/LLaVA-VL/LLaVA-NeXT)] [[Webpage](https://next-gpt.github.io/)]\
6 Aug 2024

**LLaVA-NeXT-Interleave: Tackling Multi-image, Video, and 3D in Large Multimodal Models**\
_Feng Li, Renrui Zhang, Hao Zhang, Yuanhan Zhang, Bo Li, Wei Li, Zejun Ma, Chunyuan Li_\
arXiv, [[Paper](https://arxiv.org/abs/2407.07895)] [[Codes](https://github.com/LLaVA-VL/LLaVA-NeXT)] [[Webpage](https://llava-vl.github.io/blog/2024-06-16-llava-next-interleave/)]\
28 Jul 2024

**LLaVA-1.5: Improved Baselines with Visual Instruction Tuning**\
_Haotian Liu, Chunyuan Li, Yuheng Li, Yong Jae Lee_\
CVPR 2024, [[Paper](https://arxiv.org/abs/2310.03744)] [[Codes](https://github.com/haotian-liu/LLaVA)] [[Webpage](https://llava-vl.github.io/)]\
15 May 2024

**LLaVA: Visual Instruction Tuning**\
_Haotian Liu, Chunyuan Li, Qingyang Wu, Yong Jae Lee_\
NeurIPS 2023, [[Paper](https://arxiv.org/abs/2304.08485)] [[Codes](https://github.com/haotian-liu/LLaVA)] [[Webpage](https://llava-vl.github.io/)]\
11 Dec 2023

**Video-LLaMA: An Instruction-tuned Audio-Visual Language Model for Video Understanding**\
_Hang Zhang, Xin Li, Lidong Bing_\
EMNLP 2023, [[Paper](https://arxiv.org/abs/2306.02858)] [[Codes](https://github.com/DAMO-NLP-SG/Video-LLaMA)] [[Video](https://www.youtube.com/watch?v=RDNYs3Rswhc)]\
25 Oct 2023

**GILL: Generating Images with Multimodal Language Models**\
*Jing Yu Koh, Daniel Fried, Ruslan Salakhutdinov*\
NeurIPS 2023, [[Paper](https://arxiv.org/abs/2305.17216)] [[Codes](https://github.com/kohjingyu/gill)] [[Webpage](https://jykoh.com/gill)]\
13 Oct 2023

**PandaGPT: One Model To Instruction-Follow Them All**\
_Yixuan Su, Tian Lan, Huayang Li, Jialu Xu, Yan Wang, Deng Cai_\
TLLM 2023, [[Paper](https://arxiv.org/abs/2305.16355)] [[Codes](https://github.com/yxuansu/PandaGPT)] [[Webpage](https://panda-gpt.github.io/)]\
25 May 2023

**VideoLLM: Modeling Video Sequence with Large Language Models**\
_Guo Chen, Yin-Dong Zheng, Jiahao Wang, Jilan Xu, Yifei Huang, Junting Pan, Yi Wang, Yali Wang, Yu Qiao, Tong Lu, Limin Wang_\
arXiv, [[Paper](https://arxiv.org/abs/2305.13292)] [[Codes](https://github.com/cg1177/VideoLLM)]\
23 May 2023

### Prompt Tuning
**LLaMA-Adapter: Efficient Fine-tuning of Language Models with Zero-init Attention**\
_Renrui Zhang, Jiaming Han, Chris Liu, Peng Gao, Aojun Zhou, Xiangfei Hu, Shilin Yan, Pan Lu, Hongsheng Li, Yu Qiao_\
ICLR 2024, [[Paper](https://arxiv.org/abs/2303.16199)] [[Codes](https://github.com/OpenGVLab/LLaMA-Adapter)]\
14 Jun 2023

## Contrastive Language-Image Pre-Training
### Intermediate Networks
**BLIP-2 & Q-Former: Bootstrapping Language-Image Pre-training with Frozen Image Encoders and Large Language Models**\
_Junnan Li, Dongxu Li, Silvio Savarese, Steven Hoi_\
ICML 2023, [[Paper](https://arxiv.org/abs/2301.12597)] [[Codes](https://github.com/salesforce/LAVIS/tree/main/projects/blip2)]\
15 Jun 2023

**Flamingo: a Visual Language Model for Few-Shot Learning**\
_Jean-Baptiste Alayrac, Jeff Donahue, Pauline Luc, Antoine Miech, Iain Barr, Yana Hasson, Karel Lenc, Arthur Mensch, Katie Millican, Malcolm Reynolds, Roman Ring, Eliza Rutherford, Serkan Cabi, Tengda Han, Zhitao Gong, Sina Samangooei, Marianne Monteiro, Jacob Menick, Sebastian Borgeaud, Andrew Brock, Aida Nematzadeh, Sahand Sharifzadeh, Mikolaj Binkowski, Ricardo Barreira, Oriol Vinyals, Andrew Zisserman, Karen Simonyan_\
NeurIPS 2022, [[Paper](https://arxiv.org/abs/2301.12597)] [[Codes](https://github.com/lucidrains/flamingo-pytorch)] [[Video](https://www.youtube.com/watch?v=smUHQndcmOY)] \
15 Nov 2022

**BLIP: Bootstrapping Language-Image Pre-training for Unified Vision-Language Understanding and Generation**\
_Junnan Li, Dongxu Li, Caiming Xiong, Steven Hoi_\
ICML 2022, [[Paper](https://arxiv.org/abs/2204.14198)] [[Codes and Dataset](https://github.com/salesforce/BLIP)]\
15 Feb 2022

### Simple Contrastive Learning Paradigms
**CLIP: Learning Transferable Visual Models From Natural Language Supervision**\
_Alec Radford, Jong Wook Kim, Chris Hallacy, Aditya Ramesh, Gabriel Goh, Sandhini Agarwal, Girish Sastry, Amanda Askell, Pamela Mishkin, Jack Clark, Gretchen Krueger, Ilya Sutskever_\
ICML'21, [[Paper](https://arxiv.org/abs/2103.00020)] [[Codes](https://github.com/OpenAI/CLIP)] [[Webpage](https://openai.com/index/clip/)]\
26 Feb 2021

## Universal Embedding Space
**Point-Bind & Point-LLM: Aligning Point Cloud with Multi-modality for 3D Understanding, Generation, and Instruction Following**\
_Ziyu Guo, Renrui Zhang, Xiangyang Zhu, Yiwen Tang, Xianzheng Ma, Jiaming Han, Kexin Chen, Peng Gao, Xianzhi Li, Hongsheng Li, Pheng-Ann Heng_\
arXiv, [[Paper](https://arxiv.org/abs/2309.00615)] [[Codes](https://github.com/ZiyuGuo99/Point-Bind_Point-LLM)]\
1 Sep 2023

**ImageBind: One Embedding Space To Bind Them All**\
_Rohit Girdhar, Alaaeldin El-Nouby, Zhuang Liu, Mannat Singh, Kalyan Vasudev Alwala, Armand Joulin, Ishan Misra_\
CVPR 2023, [[Paper](https://arxiv.org/abs/2305.05665)] [[Codes](https://github.com/facebookresearch/ImageBind)] [[Webpage](https://imagebind.metademolab.com/)]\
31 May 2023
