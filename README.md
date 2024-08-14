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
    - [Intermediate Networks](#Intermediate-Networks)
    - [Feature-level Fusion](#Feature-level-Fusion)
    - [Linear Layers Projection](#Linear-Layers-Projection)
    - [Prompt Tuning](#Prompt-Tuning)
    - [Preference Alignment](#Preference-Alignment)
  - [Contrastive Language-Image Pre-Training](#Contrastive-Language-Image-Pre-Training)
    - [Intermediate Networks](#Intermediate-Networks)
    - [Simple Contrastive Learning Paradigms](#Simple-Contrastive-Learning-Paradigms)
  - [Universal Embedding Space](#Universal-Embedding-Space)
  - [Training Recipes](#Training-Recipes)
- [Acknowledgement](#Acknowledgement)

# Presentations
**From Multimodal LLM to Human-level AI: Modality, Instruction, Reasoning, Efficiency and Beyond**\
_Hao Fei, Yuan Yao, Zhuosheng Zhang, Fuxiao Liu, Ao Zhang, Tat-Seng Chua_\
LREC-COLING 2024, [[Paper](https://aclanthology.org/2024.lrec-tutorials.1/)] [[Webpage](https://mllm2024.github.io/COLING2024/)]\
20 May 2024

**Recent Advances in Vision Foundation Models**\
_Chunyuan Li, Zhe Gan, Zhengyuan Yang, Jianwei Yang, Linjie Li, Lijuan Wang, Jianfeng Gao_\
CVPR 2023 Tutorial, [[Paper](https://arxiv.org/abs/2309.10020)] [[Webpage](https://vlp-tutorial.github.io/2023/)]\
18 Sep 2023

**A Vision-and-Language Approach to Computer Vision in the Wild: Building a General-Purpose Assistant in the Visual World Towards Building and Surpassing Multimodal GPT-4**\
_Chunyuan Li_\
Deep Learning Team, Microsoft Research, Redmond, [[Presentations](https://chunyuan.li/doc/talk_cvinw_instruction_june2.pdf)]\
1 May 2023

**Flamingo 🦩: A Visual Language Model for Few-Shot Learning**\
_Andrea Wynn, Xindi Wu_\
Princeton University, [[Presentations](https://www.cs.princeton.edu/courses/archive/fall22/cos597G/lectures/lec20.pdf)]\
21 November 2022

# Books
**Foundation Models for Natural Language Processing: Pre-trained Language Models Integrating Media**\
*Gerhard Paaß, Sven Giesselbach*\
Artificial Intelligence: Foundations, Theory, and Algorithms (Springer Nature), [[Link](https://link.springer.com/book/10.1007/978-3-031-23190-2)]\
16 Feb 2023

# Benchmarks
**IconQA: A New Benchmark for Abstract Diagram Understanding and Visual Language Reasoning**\
_Pan Lu, Liang Qiu, Jiaqi Chen, Tony Xia, Yizhou Zhao, Wei Zhang, Zhou Yu, Xiaodan Liang, Song-Chun Zhu_\
NeurIPS 2021, [[Paper](https://arxiv.org/abs/2110.13214)] [[Webpage](https://iconqa.github.io/)]\
Note: abstract diagram comprehension and holistic cognitive reasoning in real-world diagram-based word problems, requiring both perceptual acumen and versatile cognitive reasoning\
25 Jul 2022

**OK-VQA: A Visual Question Answering Benchmark Requiring External Knowledge**\
_Kenneth Marino, Mohammad Rastegari, Ali Farhadi, Roozbeh Mottaghi_\
CVPR 2019, [[Paper](https://arxiv.org/abs/1906.00067)] [[Webpage](https://okvqa.allenai.org/)]\
Note: questions requiring reasoning with a variety of knowledge types such as commonsense, world knowledge, and visual knowledge\
4 Sep 2019

**GQA: A New Dataset for Real-World Visual Reasoning and Compositional Question Answering**\
_Drew A. Hudson, Christopher D. Manning_\
CVPR 2019, [[Paper](https://arxiv.org/abs/1902.09506)] [[Webpage](https://cs.stanford.edu/people/dorarad/gqa/)]\
Note: image scene graphs reasoning, offering impartial compositional questions derived from real-world images.\
10 May 2019

**VQA v2 & Making the V in VQA Matter: Elevating the Role of Image Understanding in Visual Question Answering**\
_Yash Goyal, Tejas Khot, Douglas Summers-Stay, Dhruv Batra, Devi Parikh_\
CVPR 2017, [[Paper](https://arxiv.org/abs/1612.00837)] [[Webpage](https://visualqa.org/)]\
Note: every question is associated with a pair of similar images that result in two different answers to the question.\
15 May 2017

# Papers
## Survey
**The Revolution of Multimodal Large Language Models: A Survey**\
_Davide Caffagni, Federico Cocchi, Luca Barsellotti, Nicholas Moratelli, Sara Sarto, Lorenzo Baraldi, Lorenzo Baraldi, Marcella Cornia, Rita Cucchiara_\
ACL 2024, [[Paper](https://arxiv.org/abs/2402.12451)]\
6 Jun 2024

**MM-LLMs: Recent Advances in MultiModal Large Language Models**\
_Duzhen Zhang, Yahan Yu, Jiahua Dong, Chenxing Li, Dan Su, Chenhui Chu, Dong Yu_\
ACL 2024, [[Paper](https://arxiv.org/abs/2401.13601)] [[Webpage](https://mm-llms.github.io/archives/)]\
Note: Categorize MM-LLMs by Modality Encoder, Input Projector, LLM Backbone, Output Projector, Modality Generator, Training Pipeline, SoTA MM-LLMs, and Benchmarks & Performance\
28 May 2024

**A Survey on Multimodal Large Language Models**\
_Shukang Yin, Chaoyou Fu, Sirui Zhao, Ke Li, Xing Sun, Tong Xu, Enhong Chen_\
arXiv, [[Paper](https://arxiv.org/abs/2306.13549)] [[GitHub](https://github.com/BradyFU/Awesome-Multimodal-Large-Language-Models)]\
Note: The Section 3: Training Strategy and Data is a good reference.\
1 Apr 2024

## Multimodal Large Language Models
### Alignment Before Projection
**Video-LLaVA: Learning United Visual Representation by Alignment Before Projection**\
_Bin Lin, Yang Ye, Bin Zhu, Jiaxi Cui, Munan Ning, Peng Jin, Li Yuan_\
arXiv, [[Paper](https://arxiv.org/abs/2311.10122)] [[Codes](https://github.com/PKU-YuanGroup/Video-LLaVA)]\
21 Nov 2023

### Intermediate Networks
Note: including _Q-Former + linear layer(s) projection_

**NExT-GPT: Any-to-Any Multimodal LLM**\
*Shengqiong Wu, Hao Fei, Leigang Qu, Wei Ji, Tat-Seng Chua*\
ICML 2024, [[Paper](https://arxiv.org/abs/2309.05519)] [[Codes and Dataset](https://github.com/NExT-GPT/NExT-GPT)] [[Webpage](https://next-gpt.github.io/)]\
25 Jun 2024

**mPLUG-Owl: Modularization Empowers Large Language Models with Multimodality**\
_Qinghao Ye, Haiyang Xu, Guohai Xu, Jiabo Ye, Ming Yan, Yiyang Zhou, Junyang Wang, Anwen Hu, Pengcheng Shi, Yaya Shi, Chenliang Li, Yuanhong Xu, Hehong Chen, Junfeng Tian, Qi Qian, Ji Zhang, Fei Huang, Jingren Zhou_\
arXiv, [[Paper](https://arxiv.org/abs/2304.14178)] [[Codes](https://github.com/X-PLUG/mPLUG-Owl)] [[Webpage](https://www.modelscope.cn/studios/iic/mPLUG-Owl)]\
29 Mar 2024

**MiniGPT-5: Interleaved Vision-and-Language Generation via Generative Vokens**\
_Kaizhi Zheng, Xuehai He, Xin Eric Wang_\
arXiv, [[Paper](https://arxiv.org/abs/2310.02239)] [[Codes](https://github.com/eric-ai-lab/MiniGPT-5)] [[Webpage](https://eric-ai-lab.github.io/minigpt-5.github.io/)]\
29 Mar 2024

**Video-LLaMA: An Instruction-tuned Audio-Visual Language Model for Video Understanding**\
_Hang Zhang, Xin Li, Lidong Bing_\
EMNLP 2023, [[Paper](https://arxiv.org/abs/2306.02858)] [[Codes](https://github.com/DAMO-NLP-SG/Video-LLaMA)] [[Video](https://www.youtube.com/watch?v=RDNYs3Rswhc)]\
25 Oct 2023

**MiniGPT-4: Enhancing Vision-Language Understanding with Advanced Large Language Models**\
_Deyao Zhu, Jun Chen, Xiaoqian Shen, Xiang Li, Mohamed Elhoseiny_\
arXiv, [[Paper](https://arxiv.org/abs/2304.10592)] [[Codes](https://github.com/Vision-CAIR/MiniGPT-4)] [[Dataset](https://huggingface.co/datasets/Vision-CAIR/cc_sbu_align)] [[Webpage](https://minigpt-4.github.io/)]\
25 Oct 2023

**ImageBind-LLM: Multi-modality Instruction Tuning**\
_Jiaming Han, Renrui Zhang, Wenqi Shao, Peng Gao, Peng Xu, Han Xiao, Kaipeng Zhang, Chris Liu, Song Wen, Ziyu Guo, Xudong Lu, Shuai Ren, Yafei Wen, Xiaoxin Chen, Xiangyu Yue, Hongsheng Li, Yu Qiao_\
arXiv, [[Paper](https://arxiv.org/abs/2309.03905)] [[Codes](https://github.com/OpenGVLab/LLaMA-Adapter)]\
11 Sep 2023

**BuboGPT: Enabling Visual Grounding in Multi-Modal LLMs**\
_Yang Zhao, Zhijie Lin, Daquan Zhou, Zilong Huang, Jiashi Feng, Bingyi Kang_\
arXiv, [[Paper](https://arxiv.org/abs/2307.08581)] [[Codes](https://github.com/magic-research/bubogpt)] [[Webpage](https://bubo-gpt.github.io/)]\
17 Jul 2023

**InstructBLIP: Towards General-purpose Vision-Language Models with Instruction Tuning**\
_Wenliang Dai, Junnan Li, Dongxu Li, Anthony Meng Huat Tiong, Junqi Zhao, Weisheng Wang, Boyang Li, Pascale Fung, Steven Hoi_\
arXiv, [[Paper](https://arxiv.org/abs/2305.06500)] [[Codes](https://github.com/salesforce/LAVIS/tree/main/projects/instructblip)]\
15 Jun 2023

**X-LLM: Bootstrapping Advanced Large Language Models by Treating Multi-Modalities as Foreign Languages**\
_Feilong Chen, Minglun Han, Haozhi Zhao, Qingyang Zhang, Jing Shi, Shuang Xu, Bo Xu_\
arXiv, [[Paper](https://arxiv.org/abs/2305.04160)] [[Codes](https://github.com/phellonchen/X-LLM)] [[Webpage](https://x-llm.github.io/)]\
22 May 2023

### Feature-level Fusion
Note: These methods can also be categorized in other perspectives. 

**CogVLM: Visual Expert for Pretrained Language Models**\
_Weihan Wang, Qingsong Lv, Wenmeng Yu, Wenyi Hong, Ji Qi, Yan Wang, Junhui Ji, Zhuoyi Yang, Lei Zhao, Xixuan Song, Jiazheng Xu, Bin Xu, Juanzi Li, Yuxiao Dong, Ming Ding, Jie Tang_\
arXiv, [[Paper](https://arxiv.org/abs/2311.03079)] [[Codes](https://github.com/THUDM/CogVLM)]\
4 Feb 2024

**LLaMA-Adapter: Efficient Fine-tuning of Language Models with Zero-init Attention**\
_Renrui Zhang, Jiaming Han, Chris Liu, Peng Gao, Aojun Zhou, Xiangfei Hu, Shilin Yan, Pan Lu, Hongsheng Li, Yu Qiao_\
ICLR 2024, [[Paper](https://arxiv.org/abs/2303.16199)] [[Codes](https://github.com/OpenGVLab/LLaMA-Adapter)]\
14 Jun 2023

**Flamingo 🦩 & Cross-attention (Perceiver Resampler): a Visual Language Model for Few-Shot Learning**\
_Jean-Baptiste Alayrac, Jeff Donahue, Pauline Luc, Antoine Miech, Iain Barr, Yana Hasson, Karel Lenc, Arthur Mensch, Katie Millican, Malcolm Reynolds, Roman Ring, Eliza Rutherford, Serkan Cabi, Tengda Han, Zhitao Gong, Sina Samangooei, Marianne Monteiro, Jacob Menick, Sebastian Borgeaud, Andrew Brock, Aida Nematzadeh, Sahand Sharifzadeh, Mikolaj Binkowski, Ricardo Barreira, Oriol Vinyals, Andrew Zisserman, Karen Simonyan_\
NeurIPS 2022, [[Paper](https://arxiv.org/abs/2301.12597)] [[Codes](https://github.com/lucidrains/flamingo-pytorch)] [[Video](https://www.youtube.com/watch?v=smUHQndcmOY)] \
15 Nov 2022

### Linear Layers Projection
**LLaVA-OneVision: Easy Visual Task Transfer**\
_Bo Li, Yuanhan Zhang, Dong Guo, Renrui Zhang, Feng Li, Hao Zhang, Kaichen Zhang, Yanwei Li, Ziwei Liu, Chunyuan Li_\
arXiv, [[Paper](https://arxiv.org/abs/2408.03326)] [[Codes](https://github.com/LLaVA-VL/LLaVA-NeXT)] [[Webpage](https://next-gpt.github.io/)]\
6 Aug 2024

**LLaVA-NeXT-Interleave: Tackling Multi-image, Video, and 3D in Large Multimodal Models**\
_Feng Li, Renrui Zhang, Hao Zhang, Yuanhan Zhang, Bo Li, Wei Li, Zejun Ma, Chunyuan Li_\
arXiv, [[Paper](https://arxiv.org/abs/2407.07895)] [[Codes](https://github.com/LLaVA-VL/LLaVA-NeXT)] [[Webpage](https://llava-vl.github.io/blog/2024-06-16-llava-next-interleave/)]\
28 Jul 2024

**Video-ChatGPT: Towards Detailed Video Understanding via Large Vision and Language Models**\
_Muhammad Maaz, Hanoona Rasheed, Salman Khan, Fahad Shahbaz Khan_\
ACL 2024, [[Paper](https://arxiv.org/abs/2306.05424)] [[Codes](https://github.com/mbzuai-oryx/Video-ChatGPT)] [[Webpage](https://mbzuai-oryx.github.io/Video-ChatGPT/)]\
10 Jun 2024

**LLaVA-1.5: Improved Baselines with Visual Instruction Tuning**\
_Haotian Liu, Chunyuan Li, Yuheng Li, Yong Jae Lee_\
CVPR 2024, [[Paper](https://arxiv.org/abs/2310.03744)] [[Codes](https://github.com/haotian-liu/LLaVA)] [[Webpage](https://llava-vl.github.io/)]\
15 May 2024

**LLaVA: Visual Instruction Tuning**\
_Haotian Liu, Chunyuan Li, Qingyang Wu, Yong Jae Lee_\
NeurIPS 2023, [[Paper](https://arxiv.org/abs/2304.08485)] [[Codes](https://github.com/haotian-liu/LLaVA)] [[Webpage](https://llava-vl.github.io/)]\
11 Dec 2023

**CoDi-2: In-Context, Interleaved, and Interactive Any-to-Any Generation**\
_Zineng Tang, Ziyi Yang, Mahmoud Khademi, Yang Liu, Chenguang Zhu, Mohit Bansal_\
arXiv, [[Paper](https://arxiv.org/abs/2311.18775)] [[Codes](https://github.com/microsoft/i-Code/tree/main/CoDi-2)] [[Webpage](https://codi-2.github.io/)]\
30 Nov 2023

**X-InstructBLIP: A Framework for aligning X-Modal instruction-aware representations to LLMs and Emergent Cross-modal Reasoning**\
_Artemis Panagopoulou, Le Xue, Ning Yu, Junnan Li, Dongxu Li, Shafiq Joty, Ran Xu, Silvio Savarese, Caiming Xiong, Juan Carlos Niebles_\
arXiv, [[Paper](https://arxiv.org/abs/2311.18799)] [[Codes](https://github.com/artemisp/LAVIS-XInstructBLIP)] [[Webpage](https://artemisp.github.io/X-InstructBLIP-page/)]\
30 Nov 2023

**GILL: Generating Images with Multimodal Language Models**\
*Jing Yu Koh, Daniel Fried, Ruslan Salakhutdinov*\
NeurIPS 2023, [[Paper](https://arxiv.org/abs/2305.17216)] [[Codes](https://github.com/kohjingyu/gill)] [[Webpage](https://jykoh.com/gill)]\
13 Oct 2023

**MiniGPT-v2: large language model as a unified interface for vision-language multi-task learning**\
_Jun Chen, Deyao Zhu, Xiaoqian Shen, Xiang Li, Zechun Liu, Pengchuan Zhang, Raghuraman Krishnamoorthi, Vikas Chandra, Yunyang Xiong, Mohamed Elhoseiny_\
arXiv, [[Paper](https://arxiv.org/abs/2310.09478)] [[Codes](https://github.com/Vision-CAIR/MiniGPT-4)] [[Webpage](https://minigpt-v2.github.io/)]\
7 Nov 2023

**Qwen-VL: A Versatile Vision-Language Model for Understanding, Localization, Text Reading, and Beyond**\
_Jinze Bai, Shuai Bai, Shusheng Yang, Shijie Wang, Sinan Tan, Peng Wang, Junyang Lin, Chang Zhou, Jingren Zhou_\
arXiv, [[Paper](https://arxiv.org/abs/2308.12966)] [[Codes](https://github.com/QwenLM/Qwen-VL)] [[Webpage](https://qianwen.aliyun.com/)]\
13 Oct 2023

**ChatSpot: Bootstrapping Multimodal LLMs via Precise Referring Instruction Tuning**\
_Liang Zhao, En Yu, Zheng Ge, Jinrong Yang, Haoran Wei, Hongyu Zhou, Jianjian Sun, Yuang Peng, Runpei Dong, Chunrui Han, Xiangyu Zhang_\
arXiv, [[Paper](https://arxiv.org/abs/2307.09474)]\
18 Jul 2023

**Shikra: Unleashing Multimodal LLM's Referential Dialogue Magic**\
_Keqin Chen, Zhao Zhang, Weili Zeng, Richong Zhang, Feng Zhu, Rui Zhao_\
arXiv, [[Paper](https://arxiv.org/abs/2306.15195)] [[Codes](https://github.com/shikras/shikra)]\
3 Jul 2023

**FROMAGe: Grounding Language Models to Images for Multimodal Inputs and Outputs**\
_Jing Yu Koh, Ruslan Salakhutdinov, Daniel Fried_\
ICML 2023, [[Paper](https://arxiv.org/abs/2301.13823)] [[Codes](https://github.com/kohjingyu/fromage)] [[Webpage](https://jykoh.com/fromage)]\
13 Jun 2023

**PaLI-X: On Scaling up a Multilingual Vision and Language Model**\
_Xi Chen, Josip Djolonga, Piotr Padlewski, Basil Mustafa, Soravit Changpinyo, Jialin Wu, Carlos Riquelme Ruiz, Sebastian Goodman, Xiao Wang, Yi Tay, Siamak Shakeri, Mostafa Dehghani, Daniel Salz, Mario Lucic, Michael Tschannen, Arsha Nagrani, Hexiang Hu, Mandar Joshi, Bo Pang, Ceslee Montgomery, Paulina Pietrzyk, Marvin Ritter, AJ Piergiovanni, Matthias Minderer, Filip Pavetic, Austin Waters, Gang Li, Ibrahim Alabdulmohsin, Lucas Beyer, Julien Amelot, Kenton Lee, Andreas Peter Steiner, Yang Li, Daniel Keysers, Anurag Arnab, Yuanzhong Xu, Keran Rong, Alexander Kolesnikov, Mojtaba Seyedhosseini, Anelia Angelova, Xiaohua Zhai, Neil Houlsby, Radu Soricut_\
arXiv, [[Paper](https://arxiv.org/abs/2305.18565)]\
29 May 2023

**PandaGPT: One Model To Instruction-Follow Them All**\
_Yixuan Su, Tian Lan, Huayang Li, Jialu Xu, Yan Wang, Deng Cai_\
TLLM 2023, [[Paper](https://arxiv.org/abs/2305.16355)] [[Codes](https://github.com/yxuansu/PandaGPT)] [[Webpage](https://panda-gpt.github.io/)]\
25 May 2023

**VideoLLM: Modeling Video Sequence with Large Language Models**\
_Guo Chen, Yin-Dong Zheng, Jiahao Wang, Jilan Xu, Yifei Huang, Junting Pan, Yi Wang, Yali Wang, Yu Qiao, Tong Lu, Limin Wang_\
arXiv, [[Paper](https://arxiv.org/abs/2305.13292)] [[Codes](https://github.com/cg1177/VideoLLM)]\
23 May 2023

### Prompt Tuning
**Prompt-Transformer (P-Former) & DLP: Bootstrapping Vision-Language Learning with Decoupled Language Pre-training**\
_Yiren Jian, Chongyang Gao, Soroush Vosoughi_\
NeurIPS 2023, [[Paper](https://arxiv.org/abs/2307.07063)] [[Codes](https://github.com/yiren-jian/BLIText)]\
19 Dec 2023

**LLaMA-Adapter: Efficient Fine-tuning of Language Models with Zero-init Attention**\
_Renrui Zhang, Jiaming Han, Chris Liu, Peng Gao, Aojun Zhou, Xiangfei Hu, Shilin Yan, Pan Lu, Hongsheng Li, Yu Qiao_\
ICLR 2024, [[Paper](https://arxiv.org/abs/2303.16199)] [[Codes](https://github.com/OpenGVLab/LLaMA-Adapter)]\
14 Jun 2023

## Contrastive Language-Image Pre-Training
### Intermediate Networks
**Lyrics & Multi-scale Querying Transformer (MQ-Former): Boosting Fine-grained Language-Vision Alignment and Comprehension via Semantic-aware Visual Objects**\
_Junyu Lu, Dixiang Zhang, Songxin Zhang, Zejian Xie, Zhuoyang Song, Cong Lin, Jiaxing Zhang, Bingyi Jing, Pingjian Zhang_\
arXiv, [[Paper](https://arxiv.org/abs/2312.05278)]\
12 Apr 2024

**BLIP-2 & Query-Transformer (Q-Former): Bootstrapping Language-Image Pre-training with Frozen Image Encoders and Large Language Models**\
_Junnan Li, Dongxu Li, Silvio Savarese, Steven Hoi_\
ICML 2023, [[Paper](https://arxiv.org/abs/2301.12597)] [[Codes](https://github.com/salesforce/LAVIS/tree/main/projects/blip2)]\
15 Jun 2023

**Flamingo 🦩 & Cross-attention (Perceiver Resampler): a Visual Language Model for Few-Shot Learning**\
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
ICML 2021, [[Paper](https://arxiv.org/abs/2103.00020)] [[Codes](https://github.com/OpenAI/CLIP)] [[Webpage](https://openai.com/index/clip/)]\
26 Feb 2021

### Preference Alignment
**Aligning Large Multimodal Models with Factually Augmented RLHF**\
_Zhiqing Sun, Sheng Shen, Shengcao Cao, Haotian Liu, Chunyuan Li, Yikang Shen, Chuang Gan, Liang-Yan Gui, Yu-Xiong Wang, Yiming Yang, Kurt Keutzer, Trevor Darrell_\
arXiv, [[Paper](https://arxiv.org/abs/2309.14525)] [[Codes](https://github.com/llava-rlhf/LLaVA-RLHF)] [[Webpage](https://llava-rlhf.github.io/)]\
25 Sep 2023

## Universal Embedding Space
**Point-Bind & Point-LLM: Aligning Point Cloud with Multi-modality for 3D Understanding, Generation, and Instruction Following**\
_Ziyu Guo, Renrui Zhang, Xiangyang Zhu, Yiwen Tang, Xianzheng Ma, Jiaming Han, Kexin Chen, Peng Gao, Xianzhi Li, Hongsheng Li, Pheng-Ann Heng_\
arXiv, [[Paper](https://arxiv.org/abs/2309.00615)] [[Codes](https://github.com/ZiyuGuo99/Point-Bind_Point-LLM)]\
1 Sep 2023

**ImageBind: One Embedding Space To Bind Them All**\
_Rohit Girdhar, Alaaeldin El-Nouby, Zhuang Liu, Mannat Singh, Kalyan Vasudev Alwala, Armand Joulin, Ishan Misra_\
CVPR 2023, [[Paper](https://arxiv.org/abs/2305.05665)] [[Codes](https://github.com/facebookresearch/ImageBind)] [[Webpage](https://imagebind.metademolab.com/)]\
31 May 2023

## Training Recipes
**VILA: On Pre-training for Visual Language Models**\
_Ji Lin, Hongxu Yin, Wei Ping, Yao Lu, Pavlo Molchanov, Andrew Tao, Huizi Mao, Jan Kautz, Mohammad Shoeybi, Song Han_\
CVPR 2024, [[Paper](https://arxiv.org/abs/2312.07533)] [[Codes](https://github.com/NVlabs/VILA)] [[Webpage](https://vila-demo.hanlab.ai/)]\
16 May 2024

# Acknowledgement
This project is sponsored by the [MedPodGPT](https://medpodgpt.org/) group, Kolachalama Laboratory at Boston University.

<a href="https://medpodgpt.org/"> <img width="500" src="https://github.com/user-attachments/assets/234af688-d099-4c51-9122-09b9cff17ac4"></a>
