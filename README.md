# Awesome Parameter-Efficient Fine-Tuning [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

This is a curated list of research resources in `Parameter-Efficient Fine-tuning` (**PEFT**), which also goes by other names, such as `Parameter-Efficient Transfer Learning` (**PETL**). 

The repository is actively maintained. Pull requests or direct messages are welcome.

**Visual PEFT Library/Benchmark is coming soon...**

## Table of Contents
- [Introduction](#introduction)

- [Keywords](#keywords)

- [Papers](#papers)

  - [Overeview](#overeview)
  
  - [Addition-based Tuning](#addition-based-tuning)
    - [Adapter Tuning](#adapter-tuning)
  
    - [Prompt Tuning](#prompt-tuning)
  
    - [Prefix Tuning](#prefix-tuning)
  
    - [Side Tuning](#side-tuning)
  
  - [Partial-based Tuning](#partial-based-tuning)
    - [Specification Tuning](#specification-tuning)
    
    - [Repatameter Tuning](#repatameter-tuning)
  
  - [Unified Tuning](#unified-tuning)

- [Applications](#applications)

- [Contribution](#contribution)

## Introduction
Pre-trained vision models (PVMs) have shown great potential for adaptability across various downstream vision tasks. However, with state-of-the-art PVMs growing to billions or even trillions of parameters, the standard full fine-tuning paradigm is becoming unsustainable due to high computational and storage demands. In response, researchers are exploring **Parameter-Efficient Fine-Tuning (PEFT)**, which seeks to exceed the performance of full fine-tuning with minimal parameter modifications. This repository provides a comprehensive overview and offer a systematic review of the latest advancements. It introduces a categorization criterion that classifies existing methods into three categories: **Addition-based Tuning, Partial-based Tuning, and Unified-based Tuning**. This repository also introduces commonly used datasets and applications.

## Keywords
![](https://img.shields.io/badge/Abbreviation-blue) The abbreviation of the work.

![](https://img.shields.io/badge/Application-green) The main explored task/application of the work.

![](https://img.shields.io/badge/Other-orange) Other important information of the work.

## Papers
### Overeview
![avatar](Overeview.png)
### Addition-based Tuning
### Adapter Tuning
- **[1] AdaptFormer: Adapting Vision Transformers for Scalable Visual Recognition,** NeurIPS 2022.
  
  *Shoufa Chen, Chongjian Ge, Zhan Tong, Jiangliu Wang, Yibing Song, Jue Wang, Ping Luo.*

  [[Paper](https://arxiv.org/abs/2205.13535)][[Code](https://github.com/ShoufaChen/AdaptFormer)]

- **[2] Convolutional Bypasses are Better Vision Transformer Adapters,** Arxiv 2022.
  
  *Jie, Shibo and Deng, Zhi-Hong.*

  [[Paper](https://arxiv.org/abs/2207.07039)][[Code](https://github.com/JieShibo/PETL-ViT)]

- **[3] ST-Adapter: Parameter-Efficient Image-to-Video Transfer Learning,** NeurIPS 2022.
  
  *Pan, Junting and Lin, Ziyi and Zhu, Xiatian and Shao, Jing and Li, Hongsheng.*

  [[Paper](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a92e9165b22d4456fc6d87236e04c266-Abstract-Conference.html)][[Code](https://github.com/linziyi96/st-adapter)]

- **AIM: Adapting Image Models for Efficient Video Action Recognition,** ICLR 2023.
  
  *Yang, Taojiannan and Zhu, Yi and Xie, Yusheng and Zhang, Aston and Chen, Chen and Li, Mu.*

  [[Paper](https://arxiv.org/abs/2302.03024)][[Code](https://adapt-image-models.github.io/)]

- **Lossless Adaptation of Pretrained Vision Models For Robotic Manipulation,** ICLR 2023.
  
  *Sharma, Mohit and Fantacci, Claudio and Zhou, Yuxiang and Koppula, Skanda and others.*

  [[Paper](https://arxiv.org/abs/2304.06600)][[Code](https://sites.google.com/view/robo-adapters/)]

- **1% VS 100%: Parameter-Efficient Low Rank Adapter for Dense Predictions,** CVPR 2023.
  
  *Yin, Dongshuo and Yang, Yiran and Wang, Zhechao and Yu, Hongfeng and Wei, Kaiwen and Sun, Xian.*

  [[Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Yin_1_VS_100_Parameter-Efficient_Low_Rank_Adapter_for_Dense_Predictions_CVPR_2023_paper.html)][Code]

- **Polyhistor: Parameter-Efficient Multi-Task Adaptation for Dense Vision Tasks,** NeurIPS 2022.
  
  *Yen-Cheng Liu, Chih-Yao Ma, Junjiao Tian, Zijian He, Zsolt Kira.*

  [[Paper](https://arxiv.org/abs/2210.03265)][Code]

- **VMT-Adapter: Parameter-Efficient Transfer Learning for Multi-Task Dense Scene Understanding,** AAAI 2024.

  *Yi Xin, Junlong Du, Qiang Wang, Zhiwen Lin, Ke Yan.*

  [[Paper](https://arxiv.org/abs/2312.08733)][[Code]()]

- **SCT: A Simple Baseline for Parameter-Efficient Fine-Tuning via Salient Channels,** IJCV 2023.

  *Henry Hengyuan Zhao, Pichao Wang, Yuyang Zhao, Hao Luo, Fan Wang, Mike Zheng Shou.*

  [[Paper](https://arxiv.org/abs/2303.07910)][[Code](https://github.com/showlab/SCT)]

- **Important Channel Tuning,** Openreview 2023.

  *Hengyuan Zhao, Pichao WANG, Yuyang Zhao, Fan Wang, Mike Zheng Shou.*

  [[Paper](https://openreview.net/forum?id=TTMyoOdB9hZ)][Code]

- **Revisit Parameter-Efficient Transfer Learning: A Two-Stage Paradigm,** Arxiv 2023.

  *Zhao, Hengyuan and Luo, Hao and Zhao, Yuyang and Wang, Pichao and Wang, Fan and Shou, Mike Zheng.*

  [[Paper](https://arxiv.org/abs/2303.07910)][Code]

- **Compacter: Efficient Low-Rank Hypercomplex Adapter Layer,** NeurIPS 2021.
  
  *Karimi Mahabadi, Rabeeh and Henderson, James and Ruder, Sebastian.*

  [[Paper](https://arxiv.org/abs/2106.04647)][[Code](https://github.com/rabeehk/compacter)]

- **Parameter-efficient and student-friendly knowledge distillation,** NeurIPS 2022.
  
  *Rao, Jun and Meng, Xv and Ding, Liang and Qi, Shuhan and Tao, Dacheng.*

  [[Paper](https://arxiv.org/abs/2205.15308)][Code]

- **VL-adapter: Parameter-efficient transfer learning for vision-and-language tasks,** CVPR 2022.
  
  *Sung, Yi-Lin and Cho, Jaemin and Bansal, Mohit.*

  [[Paper](https://arxiv.org/abs/2112.06825)][[Code](https://github.com/ylsung/VL_adapter)]
  
- **UniAdapter: Unified Parameter-Efficient Transfer Learning for Cross-modal Modeling,** AAAI 2024.
  
  *Haoyu Lu, Mingyu Ding, Yuqi Huo, Guoxing Yang, Zhiwu Lu, Masayoshi Tomizuka, Wei Zhan.*

  [[Paper](https://arxiv.org/abs/2302.06605)][[Code](https://github.com/RERV/UniAdapter)]

- **Parameter Efficient Fine-tuning via Cross Block Orchestration for Segment Anything Model,** Arxiv 2023.

  *Zelin Peng, Zhengqin Xu, Zhilin Zeng, Lingxi Xie, Qi Tian, and Wei Shen.*
  
  [[Paper](https://arxiv.org/pdf/2311.17112.pdf)][Code]

- **Hydra: Multi-head Low-rank Adaptation for Parameter Efficient Fine-tuning,** Arxiv 2023.

  *Sanghyeon Kim, Hyunmo Yang, Younghyun Kim, Youngjoon Hong, Eunbyung Park.*
  
  [[Paper](https://arxiv.org/abs/2309.06922)][[Code](https://github.com/extremebird/Hydra/tree/main)]

- **MixPHM: Redundancy-Aware Parameter-Efficient Tuning for Low-Resource Visual Question Answering,** CVPR 2023.

  *Jingjing Jiang, Nanning Zheng.*
  
  [[Paper](https://web3.arxiv.org/abs/2303.01239)][[Code](https://github.com/jingjing12110/MixPHM)]

- **Vision Transformers are Parameter-Efficient Audio-Visual Learners,** CVPR 2023.

  *Yan-Bo Lin, Yi-Lin Sung, Jie Lei, Mohit Bansal, Gedas Bertasius.*
  
  [[Paper](https://arxiv.org/abs/2212.07983)][[Code](https://genjib.github.io/project_page/LAVISH/)]

- **T2I-Adapter: Learning Adapters to Dig out More Controllable Ability for Text-to-Image Diffusion Models,** Arxiv 2023.

  *Mou, Chong and Wang, Xintao and Xie, Liangbin and Zhang, Jian and Qi, Zhongang and others.*
  
  [[Paper](https://arxiv.org/abs/2302.08453)][[Code](https://github.com/TencentARC/T2I-Adapter)]

- **I2V-Adapter: A General Image-to-Video Adapter for Video Diffusion Models,** Arxiv 2023.

  *Guo, Xun and Zheng, Mingwu and Hou, Liang and Gao, Yuan and Deng, Yufan and others.*
  
  [[Paper](https://arxiv.org/abs/2312.16693)][[Code](https://github.com/I2V-Adapter/I2V-Adapter-repo)]

### Prompt Tuning
- **Visual Prompt Tuning,** ECCV 2022.
  
  *Menglin Jia, Luming Tang, Bor-Chun Chen, Claire Cardie, Serge Belongie, Bharath Hariharan, Ser-Nam Lim.*

  [[Paper](https://arxiv.org/abs/2203.12119)][[Code](https://github.com/kmnp/vpt)]

- **Visual Prompt Tuning for Test-time Domain Adaptation,** Arxiv 2022.
  
  *Gao, Yunhe and Shi, Xingjian and Zhu, Yi and Wang, Hao and Tang, Zhiqiang and Zhou, Xiong and others.*

  [[Paper](https://arxiv.org/abs/2203.12119)][Code]

- **LPT: Long-tailed Prompt Tuning for Image Classification,** ICLR 2023.
  
  *Dong, Bowen and Zhou, Pan and Yan, Shuicheng and Zuo, Wangmeng.*

  [[Paper](https://arxiv.org/abs/2210.01033)][[Code](https://github.com/DongSky/LPT)]

- **Pro-tuning: Unified Prompt Tuning for Vision Tasks,** TCSVT 2023.
  
  *Nie, Xing and Ni, Bolin and Chang, Jianlong and Meng, Gaofeng and Huo, Chunlei and others.*

  [[Paper](https://arxiv.org/abs/2207.14381)][Code]

- **Instance-aware Dynamic Prompt Tuning for Pre-trained Point Cloud Models,** ICCV 2023.
  
  *Zha, Yaohua and Wang, Jinpeng and Dai, Tao and Chen, Bin and Wang, Zhi and Xia, Shu-Tao.*

  [[Paper](https://arxiv.org/pdf/2304.07221.pdf)][[Code](https://github.com/zyh16143998882/ICCV23-IDPT)]

- **Visual Prompt Multi-Modal Tracking,** CVPR 2023.
  
  *Zhu, Jiawen and Lai, Simiao and Chen, Xin and Wang, Dong and Lu, Huchuan.*

  [[Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Zhu_Visual_Prompt_Multi-Modal_Tracking_CVPR_2023_paper.html)][[Code](https://github.com/jiawen-zhu/ViPT)]

- **LION: Implicit Vision Prompt Tuning,** AAAI 2024.
  
  *Wang, Haixin and Chang, Jianlong and Luo, Xiao and Sun, Jinan and Lin, Zhouchen and Tian, Qi.*

  [[Paper](https://arxiv.org/abs/2303.09992)][Code]


- **Convolutional Visual Prompt for Robust Visual Perception,** NeurIPS 2023.
  
  *Tsai, Yun-Yun and Mao, Chengzhi and Yang, Junfeng.*

  [[Paper](https://openreview.net/forum?id=qgmrC8jhCo)][Code]


- **ProSFDA: Prompt Learning based Source-free Domain Adaptation for Medical Image Segmentation,** Arxiv 2023.
  
  *Hu, Shishuai and Liao, Zehui and Xia, Yong.*

  [[Paper](https://arxiv.org/abs/2211.11514)][[Code](https://github.com/ShishuaiHu/ProSFDA)]

- **Explicit Visual Prompting for Low-Level Structure Segmentations,** CVPR 2023.
  
  *Liu, Weihuang and Shen, Xi and Pun, Chi-Man and Cun, Xiaodong.*

  [[Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Liu_Explicit_Visual_Prompting_for_Low-Level_Structure_Segmentations_CVPR_2023_paper.html)][[Code](https://github.com/NiFangBaAGe/Explicit-Visual-Prompt)]

- **P2P: Tuning Pre-trained Image Models for Point Cloud Analysis with Point-to-Pixel Prompting,** NeurIPS 2022.
  
  *Wang, Ziyi and Yu, Xumin and Rao, Yongming and Zhou, Jie and Lu, Jiwen.*

  [[Paper](https://proceedings.neurips.cc/paper_files/paper/2022/hash/5cd6dc946ccc37ae6c9f4fc6b6181e1d-Abstract-Conference.html)][[Code](https://github.com/wangzy22/P2P)]

- **Exploring Visual Prompts for Adapting Large-Scale Models,** Arxiv 2022.
  
  *Bahng, Hyojin and Jahanian, Ali and Sankaranarayanan, Swami and Isola, Phillip.*

  [[Paper](https://arxiv.org/abs/2203.17274)][[Code](https://hjbahng.github.io/visual_prompting/)]

- **Unleashing the Power of Visual Prompting At the Pixel Level,** Arxiv 2023.
  
  *Wu, Junyang and Li, Xianhang and Wei, Chen and Wang, Huiyu and Yuille, Alan and Zhou, Yuyin and Xie, Cihang.*

  [[Paper](https://arxiv.org/abs/2212.10556)][[Code](https://github.com/UCSC-VLAA/EVP)]

- **Understanding and Improving Visual Prompting: A Label-Mapping Perspective,** CVPR 2023.
  
  *Chen, Aochuan and Yao, Yuguang and Chen, Pin-Yu and Zhang, Yihua and Liu, Sijia.*

  [[Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Chen_Understanding_and_Improving_Visual_Prompting_A_Label-Mapping_Perspective_CVPR_2023_paper.html)][[Code](https://github.com/OPTML-Group/ILM-VP)]

- **Learning to Prompt for Vision-Language Models,** IJCV 2022.
  
  *Kaiyang Zhou, Jingkang Yang, Chen Change Loy, Ziwei Liu.*

  [[Paper](https://arxiv.org/abs/2109.01134)][[Code](https://github.com/KaiyangZhou/CoOp)]

- **Hyperprompt: Prompt-based task-conditioning of transformers,** ICML 2022.
  
  *He, Yun and Zheng, Steven and Tay, Yi and Gupta, Jai and Du, Yu and Aribandi, Vamsi and others.*

  [[Paper](https://proceedings.mlr.press/v162/he22f.html)][Code]

- **MaPLe: Multi-modal Prompt Learning,** CVPR 2023.
  
  *Khattak, Muhammad Uzair and Rasheed, Hanoona and Maaz, Muhammad and others.*

  [[Paper](https://arxiv.org/abs/2210.03117)][[Code](https://github.com/muzairkhattak/multimodal-prompt-learning)]

- **Hierarchical Prompt Learning for Multi-Task Learning,** CVPR 2023.
  
  *Liu, Yajing and Lu, Yuning and Liu, Hao and An, Yaozu and Xu, Zhuoran and Yao, Zhuokun and others.*

  [[Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Liu_Hierarchical_Prompt_Learning_for_Multi-Task_Learning_CVPR_2023_paper.html)][Code]

- **Visual Exemplar Driven Task-Prompting for Unified Perception in Autonomous Driving,** CVPR 2023.
  
  *Liang, Xiwen and Niu, Minzhe and Han, Jianhua and Xu, Hang and Xu, Chunjing and Liang, Xiaodan.*

  [[Paper](https://arxiv.org/abs/2303.01788)][Code]

- **Dual Modality Prompt Tuning for Vision-Language Pre-Trained Model,** TMM 2023.
  
  *Xing, Yinghui and Wu, Qirui and Cheng, De and Zhang, Shizhou and Liang, Guoqiang and others.*

  [[Paper](https://ieeexplore.ieee.org/abstract/document/10171397/)][[Code](https://github.com/fanrena/DPT)]

- **Tokenize Anything via Prompting,** Arxiv 2023.
  
  *Pan, Ting and Tang, Lulu and Wang, Xinlong and Shan, Shiguang.*

  [[Paper](https://arxiv.org/pdf/2312.09128.pdf)][[Code](https://github.com/baaivision/tokenize-anything)]

- **MmAP : Multi-modal Alignment Prompt for Cross-domain Multi-task Learning,** AAAI 2024.
  
  *Yi Xin, Junlong Du, Qiang Wang, Ke Yan, Shouhong Ding.*

  [[Paper](https://arxiv.org/abs/2312.08636)][Code]

- **Diversity-Aware Meta Visual Prompting,** CVPR 2023.
  
  *Qidong Huang, Xiaoyi Dong, Dongdong Chen, Weiming Zhang, Feifei Wang, Gang Hua, Nenghai Yu.*

  [[Paper](https://arxiv.org/abs/2303.08138)][[Code](https://arxiv.org/abs/2303.08138)]


### Prefix Tuning
- **Prefix-Tuning: Optimizing Continuous Prompts for Generation,** ACL 2021.
  
  *Li, Xiang Lisa and Liang, Percy.*

  [[Paper](https://arxiv.org/abs/2101.00190)][[Code](https://github.com/XiangLi1999/PrefixTuning)]

- **Towards a Unified View on Visual Parameter-Efficient Transfer Learning,** Arxiv 2023.
  
  *Yu, Bruce XB and Chang, Jianlong and Liu, Lingbo and Tian, Qi and Chen, Chang Wen.*

  [[Paper](https://arxiv.org/abs/2210.00788)][[Code](https://github.com/bruceyo/V-PETL)]

- **Exploring Efficient Few-shot Adaptation for Vision Transformers,** TMLR 2023.
  
  *Xu, Chengming and Yang, Siqian and Wang, Yabiao and Wang, Zhanxiong and Fu, Yanwei and Xue, Xiangyang.*

  [[Paper](https://arxiv.org/pdf/2301.02419.pdf)][[Code](https://github.com/chmxu/eTT_TMLR2022)]

- **Visual Query Tuning: Towards Effective Usage of Intermediate Representations for Parameter and Memory Efficient Transfer Learning,** CVPR 2023.
  
  *Tu, Cheng-Hao and Mai, Zheda and Chao, Wei-Lun.*

  [[Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Tu_Visual_Query_Tuning_Towards_Effective_Usage_of_Intermediate_Representations_for_CVPR_2023_paper.html)][[Code](https://github.com/andytu28/VQT)]


### Side Tuning
- **Side-Tuning: A Baseline for Network Adaptation via Additive Side Networks,** ECCV 2020.
  
  *Zhang, Jeffrey O and Sax, Alexander and Zamir, Amir and Guibas, Leonidas and Malik, Jitendra.*

  [[Paper](https://arxiv.org/pdf/1912.13503.pdf)][Code]

- **LST: Ladder Side-Tuning for Parameter and Memory Efficient Transfer Learning,** NeurIPS 2022.

  *Sung, Yi-Lin and Cho, Jaemin and Bansal, Mohit.*

  [[Paper](https://arxiv.org/abs/2206.06522)][[Code](https://github.com/ylsung/Ladder-Side-Tuning)]

- **Vision transformer adapter for dense predictions.** ICLR 2023.

  *Chen, Zhe and Duan, Yuchen and Wang, Wenhai and He, Junjun and Lu, Tong and Dai, Jifeng and Qiao, Yu.*

  [[Paper](https://arxiv.org/abs/2205.08534)][[Code](https://github.com/czczup/ViT-Adapter)]

- **Side Adapter Network for Open-Vocabulary Semantic Segmentation,** CVPR 2023.
  
  *Xu, Mengde and Zhang, Zheng and Wei, Fangyun and Hu, Han and Bai, Xiang.*

  [[Paper](https://openaccess.thecvf.com/content/CVPR2023/html/Xu_Side_Adapter_Network_for_Open-Vocabulary_Semantic_Segmentation_CVPR_2023_paper.html)][[Code](https://mendelxu.github.io/SAN/)]

- **DTL: Disentangled Transfer Learning for Visual Recognition,** AAAI 2024.
  
  *Fu, Minghao and Zhu, Ke and Wu, Jianxin.*

  [[Paper](https://arxiv.org/abs/2312.07856)][Code]

- **Parameter-efficient is not sufficient: Exploring Parameter, Memory, and Time Efficient Adapter Tuning for Dense Predictions,** NeurIPS 2023.
  
  *Yin, Dongshuo and Han, Xueting and Li, Bin and Feng, Hao and Bai, Jing.*

  [[Paper](https://arxiv.org/abs/2306.09729)][Code]

- **Ladder Fine-tuning approach for SAM integrating complementary network,** Arxiv 2023.
  
  *Chai, Shurong and Jain, Rahul Kumar and Teng, Shiyu and Liu, Jiaqing and Li, Yinhao and others.*

  [[Paper](https://arxiv.org/abs/2306.12737)][[Code](https://github.com/11yxk/SAM-LST)]



### Partial-based Tuning
### Specification Tuning
- **Do Better ImageNet Models Transfer Better?,** CVPR 2019.
  
  *Kornblith, Simon and Shlens, Jonathon and Le, Quoc V.*

  [[Paper](https://openaccess.thecvf.com/content_CVPR_2019/html/Kornblith_Do_Better_ImageNet_Models_Transfer_Better_CVPR_2019_paper.html)][[Code](https://github.com/lsh3163/Imagenet-Better)]

- **BitFit: Simple Parameter-efficient Fine-tuning for Transformer-based Masked Language-models.** ACL 2022.

  *Zaken, Elad Ben and Ravfogel, Shauli and Goldberg, Yoav.*

  [[Paper](https://arxiv.org/pdf/2106.10199.pdf)][[Code](https://github.com/benzakenelad/BitFit)]
  
- **AdapterBias: Parameter-efficient Token-dependent Representation Shift for Adapters in NLP Tasks,** NAACL 2022.
  
  *Fu, Chin-Lun and Chen, Zih-Ching and Lee, Yun-Ru and Lee, Hung-yi.*

  [[Paper](https://arxiv.org/abs/2205.00305)][[Code](https://github.com/Allen0307/AdapterBias)]

- **Differentially Private Bias-Term only Fine-tuning of Foundation Models,** Arxiv 2022.
  
  *Bu, Zhiqi and Wang, Yu-Xiang and Zha, Sheng and Karypis, George.*

  [[Paper](https://arxiv.org/abs/2210.00036)][Code]

- **Strong Baselines for Parameter Efficient Few-Shot Fine-tuning,** AAAI 2024.
  
  *Basu, Samyadeep and Massiceti, Daniela and Hu, Shell Xu and Feizi, Soheil.*

  [[Paper](https://arxiv.org/abs/2304.01917)][Code]

- **DiffFit: Unlocking Transferability of Large Diffusion Models via Simple Parameter-Efficient Fine-Tuning,** ICCV 2023.
  
  *Enze Xie, Lewei Yao, Han Shi, Zhili Liu, Daquan Zhou, Zhaoqiang Liu, Jiawei Li, Zhenguo Li.*

  [[Paper](https://arxiv.org/abs/2304.06648)][[Code](https://github.com/mkshing/DiffFit-pytorch)]

### Reparameter Tuning
- **LoRA: Low-Rank Adaptation of Large Language Models.** NeurIPS 2021.

  *Hu, Edward J and Shen, Yelong and Wallis, Phillip and Allen-Zhu, Zeyuan and Li, Yuanzhi and others.*

  [[Paper](https://arxiv.org/pdf/2106.09685.pdf)][[Code](https://github.com/microsoft/LoRA)]

- **Scaling & Shifting Your Features: A New Baseline for Efficient Model Tuning,** NeurIPS 2022.
  
  *Dongze Lian, Daquan Zhou, Jiashi Feng, Xinchao Wang.*

  [[Paper](https://arxiv.org/abs/2210.08823)][[Code](https://github.com/dongzelian/SSF)]

- **KronA: Parameter Efficient Tuning with Kronecker Adapter,** Arxiv 2023.
  
  *Ali Edalati, Marzieh Tahaei, Ivan Kobyzev, Vahid Partovi Nia, James J. Clark, Mehdi Rezagholizadeh.*

  [[Paper](https://arxiv.org/abs/2212.10650))][Code]

- **FacT: Factor-Tuning for Lightweight Adaptation on Vision Transformer,** AAAI 2023.
  
  *Jie, Shibo and Deng, Zhi-Hong.*

  [[Paper](https://ojs.aaai.org/index.php/AAAI/article/view/25187)][Code]

- **Aggregate, Decompose, and Fine-Tune: A Simple Yet Effective Factor-Tuning Method for Vision Transformer,** Arxiv 2023.
  
  *Chen, Dongping.*

  [[Paper](https://arxiv.org/abs/2311.06749)][Code]

- **Strong Baselines for Parameter Efficient Few-Shot Fine-tuning,** AAAI 2024.
  
  *Basu, Samyadeep and Massiceti, Daniela and Hu, Shell Xu and Feizi, Soheil.*

  [[Paper](https://arxiv.org/abs/2304.01917)][Code]

- **Parameter-efficient Model Adaptation for Vision Transformers,** AAAI 2023.
  
  *He, Xuehai and Li, Chunyuan and Zhang, Pengchuan and Yang, Jianwei and Wang, Xin Eric.*

  [[Paper](https://arxiv.org/abs/2203.16329)][[Code](https://github.com/eric-ai-lab/PEViT)]

- **DnA: Improving Few-Shot Transfer Learning with Low-Rank Decomposition and Alignment,** ECCV 2022.
  
  *Jiang, Ziyu and Chen, Tianlong and Chen, Xuxi and Cheng, Yu and Zhou, Luowei and Yuan, Lu and others.*

  [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-20044-1_14)][[Code](https://github.com/VITA-Group/DnA)]

- **Towards Efficient Visual Adaption via Structural Re-parameterization,** Arxiv 2023.
  
  *Luo, Gen and Huang, Minglang and Zhou, Yiyi and Sun, Xiaoshuai and Jiang, Guannan and Wang, Zhiyu and Ji, Rongrong.*

  [[Paper](https://arxiv.org/abs/2302.08106)][[Code](https://github.com/luogen1996/RepAdapter)]

- **SAM-PARSER: Fine-tuning SAM Efficiently by Parameter Space Reconstruction,** AAAI 2024.
  
  *Zelin Peng, Zhengqin Xu, Zhilin Zeng, Xiaokang Yang, Wei Shen.*

  [[Paper](https://arxiv.org/abs/2308.14604)][[Code]()]

### Unified Tuning
- **Towards a Unified View of Parameter-Efficient Transfer Learning,** ICLR 2022.

  *Junxian He, Chunting Zhou, Xuezhe Ma, Taylor Berg-Kirkpatrick, Graham Neubig.*

  [[Paper](https://arxiv.org/abs/2110.04366)][[Code](https://github.com/jxhe/unify-parameter-efficient-tuning)]

- **Towards a Unified View on Visual Parameter-Efficient Transfer Learning,** Arxiv 2023.

  *Yu, Bruce XB and Chang, Jianlong and Liu, Lingbo and Tian, Qi and Chen, Chang Wen.*

  [[Paper](https://arxiv.org/abs/2210.00788)][[Code](https://github.com/bruceyo/V-PETL)]

- **Neural Prompt Search,** Arxiv 2022.
  
  *Zhang, Yuanhan and Zhou, Kaiyang and Liu, Ziwei.*

  [[Paper](https://arxiv.org/abs/2206.04673)][[Code](https://github.com/Davidzhangyuanhan/NOAH)]

- **Rethinking Efficient Tuning Methods from a Unified Perspective,** Arxiv 2023.
  
  *Jiang, Zeyinzi and Mao, Chaojie and Huang, Ziyuan and Lv, Yiliang and Zhao, Deli and Zhou, Jingren.*

  [[Paper](https://arxiv.org/pdf/2303.00690.pdf)][Code]

- **A Unified Continual Learning Framework with General Parameter-Efficient Tuning,** ICCV 2023.
  
  *Gao, Qiankun and Zhao, Chen and Sun, Yifan and Xi, Teng and Zhang, Gang and Ghanem, Bernard and Zhang, Jian.*

  [[Paper](https://arxiv.org/abs/2303.10070)][[Code](https://github.com/gqk/LAE)]


### Others
- **Parameter-efficient Model Adaptation for Vision Transformers.** AAAI 2023.

  *He, Xuehai and Li, Chunyuan and Zhang, Pengchuan and Yang, Jianwei and Wang, Xin Eric.*

  [[Paper](https://arxiv.org/abs/2203.16329)][[Code](https://github.com/eric-ai-lab/PEViT)]

- **Gradient-based Parameter Selection for Efficient Fine-Tuning,** Arxiv 2023.
  
  *Zhi Zhang, Qizhe Zhang, Zijun Gao, Renrui Zhang, Ekaterina Shutova, Shiji Zhou, Shanghang Zhang.*

  [[Paper](https://arxiv.org/abs/2312.10136)][[Code]()]

- **Three things everyone should know about Vision Transformers,** ECCV 2022.
  
  *Hugo Touvron, Matthieu Cord, Alaaeldin El-Nouby, Jakob Verbeek, Hervé Jégou.*

  [[Paper](https://arxiv.org/abs/2203.09795)][[Code]()]

- **Sensitivity-Aware Visual Parameter-Efficient Fine-Tuning,** ICCV 2023.
  
  *Haoyu He, Jianfei Cai, Jing Zhang, Dacheng Tao, Bohan Zhuang.*

  [[Paper](https://arxiv.org/abs/2303.08566)][[Code](https://github.com/ziplab/SPT)]

- **GIST: Improving Parameter Efficient Fine Tuning via Knowledge Interaction,** Arxiv 2023.

  *Jiacheng Ruan, Jingsheng Gao, Mingye Xie, Suncheng Xiang, Zefang Yu, Ting Liu, Yuzhuo Fu.*

  [[Paper](https://arxiv.org/pdf/2312.07255.pdf)][Code]

- **Point-PEFT: Parameter-Efficient Fine-Tuning for 3D Pre-trained Models,** AAAI 2024.

  *Yiwen Tang, Ray Zhang, Zoey Guo, Xianzheng Ma, Dong Wang, Zhigang Wang, Bin Zhao, Xuelong Li.*

  [[Paper](https://arxiv.org/abs/2310.03059)][Code]

- **AdaptIR: Parameter Efficient Multi-task Adaptation for Pre-trained Image Restoration Models,** Arxiv 2023.

  *Hang Guo, Tao Dai, Yuanchao Bai, Bin Chen, Shu-Tao Xia, Zexuan Zhu.*

  [[Paper](https://arxiv.org/pdf/2312.08881.pdf)][[Code](https://github.com/csguoh/AdaptIR)]

- **A Closer Look at Parameter-Efficient Tuning in Diffusion Models,** Arxiv 2023.

  *Chendong Xiang, Fan Bao, Chongxuan Li, Hang Su, Jun Zhu.*
  
  [[Paper](https://arxiv.org/abs/2303.18181)][[Code](https://github.com/Xiang-cd/unet-finetune)]

## Applications

## Contributors

<!-- Copy-paste in your Readme.md file -->

<a href="https://github.com/synbol/Awesome-Parameter-Efficient-Transfer-Learning/graphs/contributors">
  <img src="" />
</a>

## Citation
If you find our survey and repository useful for your research, please consider citing our paper:
```bibtex
@article{,
  title={Parameter-Efficient Fine-Tuning for Pre-Trained Vision Models: A Survey},
  author={Yi Xin, Siqi Luo, Haodi Zhou, Junlong Du, Xiaohong Liu, Yue Fan, Qing Li, Yuntao Du},
  journal={Arxiv},
  year={2024}
}
```
