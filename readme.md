国内脑科学机构展示：https://neuspeech.github.io/awesome-brain-decoding/

具体信息：https://neuspeech.github.io/awesome-brain-decoding/国内脑机接口研究机构及公司.md

这里基本上很全，但是可能有些错误信息，欢迎大家指正。

# Awesome Brain decoding [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) 
<!-- # <p align=center>`awesome digital human`</p> -->
<!-- [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
[![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com) 
![visitors](https://visitor-badge.glitch.me/badge?style=flat-square&page_id=weihaox/awesome-clothed-human)  -->

> A curated collection of resources in brain decoding, including interaction with multi-modalities, theories, and foundation models.

## Contributing

Feedback and contributions are welcome! 
If you think I have missed out on something (or) have any suggestions (papers, implementations and other resources), 
feel free to raise issues and pull requests.

```Markdown
**Here is the Paper Name.**<br>
*[Author 1](homepage), Author 2, and Author 3.*<br>
Short description
Conference or Journal Year. [[PDF](link)] [[Project](link)] [[Code](link)] [[Data](link)]
```

## Table of Contents

- [Awesome Brain decoding ](#awesome-brain-decoding-)
  - [Contributing](#contributing)
  - [Table of Contents](#table-of-contents)
  - [Brain to text](#brain-to-text)
    - [EEG](#eeg)
    - [MEG](#meg)
    - [ECoG](#ecog)
    - [fMRI](#fmri)
  - [Brain-to-speech](#brain-to-speech)
    - [ECoG](#ecog-1)
    - [MEG](#meg-1)
    - [EMG](#emg)
    - [EEG](#eeg-1)
    - [fMRI](#fmri-1)
  - [Brain-to-music](#brain-to-music)
    - [fMRI](#fmri-2)
    - [ECoG](#ecog-2)
  - [Brain-to-image](#brain-to-image)
    - [EEG](#eeg-2)
    - [MEG](#meg-2)
    - [fMRI](#fmri-3)
  - [Brain-to-video](#brain-to-video)
  - [Foundation models](#foundation-models)
  - [theory](#theory)
  - [Team and People](#team-and-people)
  - [Dataset](#dataset)
    - [fMRI](#fmri-4)
    - [EEG](#eeg-3)
    - [MEG](#meg-3)
    - [ECoG](#ecog-3)


## Brain to text

### EEG
**Open Vocabulary Electroencephalography-to-Text Decoding and Zero-Shot Sentiment Classification**<br>
*Zhenhailong Wang, Heng Ji*<br>
AAAI 2022
. Convert EEG signal within each time frame of reading word to token, and translate tokens to text in open vocabulary condition.
The start of this open-vocabulary field.
[[PDF](https://ojs.aaai.org/index.php/AAAI/article/view/20472)]
[[ZuCo1](https://osf.io/q3zws/files/osfstorage)]
[[ZuCo2](https://osf.io/2urht/files/osfstorage)]
[[Code](https://github.com/MikeWangWZHL/EEG-To-Text)]

**Are EEG-to-Text Models Working?**<br>
*Hyejeong Jo\*, Yiqian Yang\*, Juhyeok Han, Yiqun Duan, Hui Xiong, Won Hee Lee*<br>
IJCAI workshop 2024
. Investigated major flaws in EEG-to-text models. Compared model performance on pure noise inputs.
[[PDF](https://arxiv.org/pdf/2405.06459)]
[[Data-ZuCo1](https://osf.io/q3zws/files/osfstorage)]
[[Data-ZuCo2](https://osf.io/2urht/files/osfstorage)]
[[Code](https://github.com/NeuSpeech/EEG-To-Text)]


### MEG

**NeuSpeech: Decode Neural signal as Speech**<br>
*Yiqian Yang\*, Yiqun Duan\*,  Qiang Zhang, Hyejeong Jo, Jinni Zhou, Won Hee Lee, Renjing Xu, Hui Xiong*<br>
Arxiv 2024
. 
[[PDF](https://arxiv.org/pdf/2403.01748)]
[MEG [Data-Gwilliams](https://osf.io/ag3kj/)]
[MEG [Data-Schoffelen](https://data.ru.nl/collections/di/dccn/DSC_3011020.09_236)]
[[Code](https://github.com/NeuSpeech/NeuSpeech1)]


**MAD:Multi-Alignment MEG-to-Text Decoding**<br>
*Yiqian Yang\*, Hyejeong Jo\*, Yiqun Duan\*  Qiang Zhang, Jinni Zhou, Won Hee Lee, Renjing Xu, Hui Xiong*<br>
Arxiv 2024
. 
[[PDF](https://arxiv.org/pdf/2406.01512)]
[MEG [Data-Gwilliams](https://osf.io/ag3kj/)]
[[Code](https://github.com/NeuSpeech/MAD-MEG2text)]


### ECoG


**High-performance brain-to-text communication via handwriting**<br>
*Francis R. Willett, Donald T. Avansino, Leigh R. Hochberg, Jaimie M. Henderson, Krishna V. Shenoy*<br>
Nature 2021.
[[PDF](https://www.nature.com/articles/s41586-021-03506-2)]
[[Code](https://github.com/fwillett/handwritingBCI)]
[[Data-Willett2021](https://datadryad.org/stash/dataset/doi:10.5061/dryad.wh70rxwmv)]


**A high-performance speech neuroprosthesis**<br>
*Francis R. Willett, Erin M. Kunz, Chaofei Fan, Donald T. Avansino, Guy H. Wilson, Eun Young Choi, Foram Kamdar, Matthew F. Glasser, Leigh R. Hochberg, Shaul Druckmann, Krishna V. Shenoy, Jaimie M. Henderson*<br>
Decode ecog signal with RNN network. Signal->phonemes with RNN and plus a language model to get word.
Nature 2023.
[[PDF](https://www.nature.com/articles/s41586-023-06377-x)]
[[Code](https://github.com/fwillett/speechBCI)]
[[Data-Willett2023](https://datadryad.org/stash/dataset/doi:10.5061/dryad.x69p8czpq)]

**Generalizable spelling using a speech neuroprosthesis in an individual with severe limb and vocal paralysis**<br>
*Sean L. Metzger, Jessie R. Liu, David A. Moses, Maximilian E. Dougherty, Margaret P. Seaton, Kaylo T. Littlejohn, Josh Chartier, Gopala K. Anumanchipalli, Adelyn Tu-Chan, Karunesh Ganguly & Edward F. Chang*<br>
Nature communications 2022.
[[PDF](https://www.nature.com/articles/s41467-022-33611-3)]
[[Code](https://github.com/ChangLabUcsf/silent_spelling)]
[[Data-Metzger2022 should contact edward.chang@ucsf.edu](edward.chang@ucsf.edu)]

**A high-performance neuroprosthesis for speech decoding and avatar control**<br>
*Sean L. Metzger, Kaylo T. Littlejohn, Alexander B. Silva, David A. Moses, Margaret P. Seaton, Ran Wang, Maximilian E. Dougherty, Jessie R. Liu, Peter Wu, Michael A. Berger, Inga Zhuravleva, Adelyn Tu-Chan, Karunesh Ganguly, Gopala K. Anumanchipalli, Edward F. Chang*<br>
Nature 2023. ECoG to text using bi-RNN and CTC beam search, 
to speech using hubert model and to waveform and voice-convert to target speaker, 
to articulatory gestures with bi-RNN to gesture units and to gestures and to avatar,
etc.
[[PDF](https://www.nature.com/articles/s41586-023-06443-4)]
[[Code](https://github.com/UCSF-Chang-Lab-BRAVO/multimodal-decoding)]
[[Data-Metzger2023](https://zenodo.org/records/8200782)]

**Decoding and synthesizing tonal language speech from brain activity**<br>
*YAN LIU, ZEHAO ZHAO, MINPENG XU, HAIQING YU, YANMING ZHU, JIE ZHANG, LINGHAO BU, XIAOLUO ZHANG, JUNFENG LU, JINSONG WU*<br>
SCIENCE ADVANCES
9 Jun 2023
. Chinese language decoding
[[PDF](https://www.science.org/doi/full/10.1126/sciadv.adh0478#sec-1)]

### fMRI
**Semantic reconstruction of continuous language from non-invasive brain recordings**<br>
*Jerry Tang, Amanda LeBel, Shailee Jain & Alexander G. Huth*<br>
Nature Neuroscience 2023
. brain encoding model, generate word by comparing the predicted brain signal with the original one.
[[PDF](https://www.nature.com/articles/s41593-023-01304-9)]
[[Data-LeBel2023](https://openneuro.org/datasets/ds003020)]
[[Data-Tang2023](https://openneuro.org/datasets/ds004510)]
[[Code](https://github.com/HuthLab/semantic-decoding)]

**Decoding Continuous Character-based Language from Non-invasive Brain Recordings**<br>
*Cenyuan Zhang, Xiaoqing Zheng, Ruicheng Yin, Shujie Geng, Jianhan Xu, Xuan Gao, Changze Lv, Zixuan Ling, Xuanjing Huang, Miao Cao, Jianfeng Feng*<br>
Arxiv 2024.
[[PDF](https://arxiv.org/pdf/2403.11183)]



## Brain-to-speech

### ECoG
**Speech synthesis from neural decoding of spoken sentences.**<br>
*Gopala K. Anumanchipalli\*, Josh Chartier\*, Edward F. Chang.*<br> 
Withdrawn recently.
 Nature. 2019 April 
[[PDF](https://europepmc.org/backend/ptpmcrender.fcgi?accid=PMC9714519&blobtype=pdf)] 

**Subject-Agnostic Transformer-Based Neural Speech Decoding from Surface and Depth Electrode Signals.**<br>
*Junbo Chen, Xupeng Chen, Ran Wang, Chenqian Le, Amirhossein Khalilian-Gourtani, Erika Jensen, Patricia Dugan, Werner Doyle, Orrin Devinsky, Daniel Friedman, Adeen Flinker, and Yao Wang*<br>
bioRxiv. Preprint. 2024 Mar 14.
[[PDF](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC10980022/)] 

**A neural speech decoding framework leveraging deep learning and speech synthesis.**<br>
*Xupeng Chen, Ran Wang, Amirhossein Khalilian-Gourtani, Leyao Yu, Patricia Dugan, Daniel Friedman, Werner Doyle, Orrin Devinsky, Yao Wang, Adeen Flinker*
Nature Machine Intelligence 2024
[[PDF](https://www.nature.com/articles/s42256-024-00824-8)] 
[[Data-Chen2024](https://data.mendeley.com/datasets/fp4bv9gtwk/2)]
[[Code](https://github.com/flinkerlab/neural_speech_decoding)]


**Reverse the auditory processing pathway: Coarse-to-fine audio reconstruction from fMRI.**<br>
*Che Liu, Changde Du, Xiaoyu Chen, Huiguang He*
Arxiv 2024  Short as C2F-LDM
[[PDF](https://arxiv.org/pdf/2405.18726)] 
[[Data- Brain2Sound]()]
[[Data- Brain2Music]()]
[[Data- Brain2Speech]()]
[[Data- Brain2Sound]()]


### MEG
**Decoding speech perception from non-invasive brain recordings**<br>
*Alexandre Défossez, Charlotte Caucheteux, Jérémy Rapin, Ori Kabeli, Jean-Rémi King*<br>
Nature Machine Intelligence 2023
. Decode M/EEG to speech with proposed brain module, trained with CLIP. M/EEG input to the brain module and get features, 
only choose sentence from candidates, not generate.
[[PDF](https://www.nature.com/articles/s42256-023-00714-5)]
[MEG [Data-Gwilliams](https://osf.io/ag3kj/)]
[MEG [Data-Schoffelen](https://data.ru.nl/collections/di/dccn/DSC_3011020.09_236)]
[EEG [Data-Broderick](https://datadryad.org/stash/dataset/doi:10.5061/dryad.070jc)]
[EEG [Data-Brennan](https://deepblue.lib.umich.edu/data/concern/data_sets/bg257f92t)]
[[Code](https://github.com/facebookresearch/brainmagick)]

### EMG

**A Cross-Modal Approach to Silent Speech with LLM-Enhanced Recognition**<br>
*Tyler Benster, Guy Wilson, Reshef Elisha, Francis R Willett, Shaul Druckmann*<br>
Arxiv 2024.
[[PDF](https://arxiv.org/pdf/2403.05583v1)]

### EEG

**End-to-end translation of human neural activity to speech with a dual–dual generative adversarial network**<br>
*Yina Guo\*, Ting Liu\*, Xiaofei Zhang\*, Anhong Wang, Wenwu Wang*<br>
Knowledge-Based Systems 2023.
[[PDF](https://www.sciencedirect.com/science/article/pii/S0950705123005877)]
[[Code](https://github.com/qwe1218088/dual-dualgan)]

### fMRI

**Open-vocabulary Auditory Neural Decoding Using fMRI-prompted LLM**<br>
*Xiaoyu Chen, Changde Du, Liu Che, Yizhe Wang, Huiguang He*<br>
Arxiv 2024.
[[PDF](https://arxiv.org/abs/2405.07840)]
[MEG [Data-Gwilliams](https://osf.io/ag3kj/)]

## Brain-to-music

### fMRI
**BRAIN2MUSIC: RECONSTRUCTING MUSIC FROM HUMAN BRAIN ACTIVITY**<br>
*Timo I. Denk\*, Yu Takagi\*, Takuya Matsuyama, Andrea Agostinelli, Tomoya Nakai, Christian Frank, Shinji Nishimoto*<br>
ICLR 2024.
[[PDF](https://arxiv.org/pdf/2307.11078)]
[[Data-Nakai2022](https://openneuro.org/datasets/ds003720/versions/1.0.0)]

### ECoG
**Music can be reconstructed from human auditory cortex activity using nonlinear decoding models**<br>
*Bellier, Anaïs Llorens, Déborah Marciano, Aysegul Gunduz, Gerwin Schalk, Peter Brunner, Robert T. Knight *<br>
PLOS 2023.
[[PDF](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3002176&utm_source=ASOTU&utm_medium=email&utm_campaign=483-connecting-connections)]


## Brain-to-image

### EEG
**Visual Decoding and Reconstruction via EEG Embeddings with Guided Diffusion.**<br>
*Dongyang Li, Chen Wei, Shiying Li, Jiachen Zou, Quanying Liu*<br>
Arxiv 2024.
[[PDF](https://arxiv.org/pdf/2403.07721)]
[[Code](https://github.com/dongyangli-del/EEG_Image_decode)]
[[Data-Things-EEG1](https://osf.io/3jk45/)]
[[Data-Things-EEG2](https://openneuro.org/datasets/ds003825/versions/1.1.0)]
[[Data-Things-MEG](https://openneuro.org/datasets/ds004212/versions/2.0.0)]

### MEG

**BRAIN DECODING: TOWARD REAL-TIME RECONSTRUCTION OF VISUAL PERCEPTION.**<br>
*Yohann Benchetrit\*, Hubert Banville\*, Jean-R´emi King*<br>
ICLR 2024.
[[PDF](https://openreview.net/pdf?id=3y1K6buO8c)]
[[Data-Things-MEG](https://openneuro.org/datasets/ds004212/versions/2.0.0)]


### fMRI

**Brain captioning: Decoding human brain activity into images and text.**<br>
*Matteo Ferrante, Furkan Ozcelik, Tommaso Boccato, Rufin VanRullen, Nicola Toschi*<br>
Arxiv 2023.
[[PDF](https://arxiv.org/pdf/2305.11560)]
[[Data-NSD](https://naturalscenesdataset.org/)]

**Natural scene reconstruction from fMRI signals using generative latent diffusion.**<br>
*Furkan Ozcelik, Rufin VanRullen*<br>
Nature scientific reports 2023.
[[PDF](https://www.nature.com/articles/s41598-023-42891-8)]
[[Data-NSD](https://naturalscenesdataset.org/)]


**Seeing Beyond the Brain: Conditional Diffusion Model with Sparse Masked Modeling for Vision Decoding .**<br>
*Zijiao Chen\* Jiaxin Qing\*, Tiange Xiang, Wan Lin Yue, Juan Helen Zhou*<br>
CVPR2023.
[[PDF](CVPR2023)]
[[Project](https://mind-vis.github.io/)]
[[Code](https://github.com/zjc062/mind-vis)]
[[Data-HCP Young Adult](https://www.humanconnectome.org/study/hcp-young-adult/data-releases)]
[[Data-GOD](https://github.com/KamitaniLab/GenericObjectDecoding)]
[[Data-BOLD5000](https://figshare.com/articles/dataset/BOLD5000_Release_2_0/14456124)]


**UMBRAE: Unified Multimodal Decoding of Brain Signals.**<br>
*Weihao Xia, Raoul de Charette, Cengiz Öztireli, Jing-Hao Xue*<br>
Arxiv 2024.
[[PDF](https://arxiv.org/pdf/2404.07202)]
[[Project](https://weihaox.github.io/UMBRAE/)]
[[Code](https://github.com/weihaox/UMBRAE)]
[[Data-NSD](https://naturalscenesdataset.org/)]

## Brain-to-video

**Cinematic Mindscapes: High-quality Video Reconstruction from Brain Activity.**<br>
*Zijiao Chen\*,  Jiaxin Qing\*, Juan Helen Zhou*<br>
NeurIPS 2023.
[[PDF](https://arxiv.org/pdf/2305.11675)]
[[Project](https://mind-video.com/)]
[[Code](https://github.com/jqin4749/MindVideo)]
[[Data-HCP Young Adult](https://www.humanconnectome.org/study/hcp-young-adult/data-releases)]
[[Data-Wen](https://purr.purdue.edu/publications/2809/1)]


## Foundation models

**LARGE BRAIN MODEL FOR LEARNING GENERIC REPRESENTATIONS WITH TREMENDOUS EEG DATA IN BCI.**<br>
*Wei-Bang Jiang, Li-Ming Zhao, Bao-Liang Lu*<br>
ICLR 2024.
[[PDF](https://arxiv.org/pdf/2405.18765)]
[[Code](https://github.com/935963004/LaBraM)]
[Data-BCI Competition IV-1]
[Data-Emobrain]
[Data-Grasp and Lift EEG Challenge]
[Data-Inria BCI Challenge]
[Data-EEGMotorMovement/ImageryDataset]
[Data-Raw EEG Data]
[Data-Resting State EEG Data]
[Data-SEED Series]
[Data-Siena Scalp EEG Database]
[Data-SPIS Resting State Dataset]
[Data-Target Versus Non-Target]
[Data-TUAR]
[Data-TUEP]
[Data-TUSZ]
[Data-TUSL]
[Data-Self-collected EEG Data]



## theory

**How Many Bytes Can YouTake Out Of Brain-To-Text Decoding?.**<br>
*Richard J. Antonello, Nihita Sarma, Jerry Tang, Jiaru Song, Alexander G. Huth*<br>
Arxiv 2024.
[[PDF](https://arxiv.org/pdf/2405.14055)]

**The Brain's Bitter Lesson: Scaling Speech Decoding With Self-Supervised Learning.**<br>
*Richard J. Antonello, Nihita Sarma, Jerry Tang, Jiaru Song, Alexander G. Huth*<br>
Arxiv 2024.

[[PDF](https://arxiv.org/abs/2406.04328)]

## Team and People

- [NCC lab](https://github.com/ncclab-sustech), **SUSTech**, by [Quanying Liu](https://www.sustech.edu.cn/zh/faculties/liuquanying.html).
- [Computational Cognitive and Translational Neuroscience Lab](https://yuanningli.github.io/), **ShanghaiTech**, by [Yuanning Li](https://yuanningli.github.io/).
- [Department of Linguistics and Translation](https://lt.cityu.edu.hk/), **CityU of HK**, by [Niels O. Schiller](https://scholars.cityu.edu.hk/en/person/nschille).
- [Meta/CNRS](https://ai.meta.com/), **École Normale Supérieure**, by [Jean-Remi King](https://kingjr.github.io/).
- [Neural Prosthetics Translational Laboratory](https://nptl.stanford.edu/), **Stanford University**, by [Jaimie Henderson](https://profiles.stanford.edu/jaimie-henderson).
- [HuthLab](https://www.cs.utexas.edu/~huth/), **The University of Texas at Austin**, by [Alexander G. Huth](https://www.cs.utexas.edu/people/faculty-researchers/alexander-huth).
- [Nishimoto Lab](https://nishimotolab.org/), **Osaka University**, by [Shinji Nishimoto](https://cinet.jp/english/people/20141086/).
- [Research and Development Center for Large Language Models](https://nishimotolab.org/), **National Institute of Informatics**, by [Yu Takagi](https://yu-takagi.github.io/).
- [ISTBI](https://istbi.fudan.edu.cn/), **Fudan University**, by [Jianfeng FENG](https://istbi.fudan.edu.cn/lnen/info/1157/1629.htm).
- [ZNLP](https://nlpr.ia.ac.cn/cip/introduction.htm), **CASIA**, by some researchers [Shaonan WANG](https://wangshaonan.github.io/),[Jingyuan SUN](https://openreview.net/profile?id=~Jingyuan_Sun1).
- [State Key Laboratory of Management and Control for Complex Systems](http://english.ia.cas.cn/rd/202004/t20200415_234810.html), **Chinese Academy of Sciences and ShanghaiTech University**, by [Huiguang He](https://people.ucas.ac.cn/~hehuiguang?language=en).


## Dataset

### fMRI
[[Data-NSD](https://naturalscenesdataset.org/)]
[[Data-HCP Young Adult](https://www.humanconnectome.org/study/hcp-young-adult/data-releases)]
[[Data-GOD](https://github.com/KamitaniLab/GenericObjectDecoding)]
[[Data-BOLD5000](https://figshare.com/articles/dataset/BOLD5000_Release_2_0/14456124)]
[[Data-Wen](https://purr.purdue.edu/publications/2809/1)]
[[Data-LeBel2023](https://openneuro.org/datasets/ds003020)]
[[Data-Tang2023](https://openneuro.org/datasets/ds004510)]

### EEG
[[Data-Things-EEG1](https://osf.io/3jk45/)]
[[Data-Things-EEG2](https://openneuro.org/datasets/ds003825/versions/1.1.0)]
[EEG [Data-Broderick](https://datadryad.org/stash/dataset/doi:10.5061/dryad.070jc)]
[EEG [Data-Brennan](https://deepblue.lib.umich.edu/data/concern/data_sets/bg257f92t)]
[[Data-ZuCo1](https://osf.io/q3zws/files/osfstorage)]
[[Data-ZuCo2](https://osf.io/2urht/files/osfstorage)]

### MEG

[MEG [Data-Gwilliams](https://osf.io/ag3kj/)]
[MEG [Data-Schoffelen](https://data.ru.nl/collections/di/dccn/DSC_3011020.09_236)]
[[Data-Things-MEG](https://openneuro.org/datasets/ds004212/versions/2.0.0)]

### ECoG
[[Data-Metzger2023](https://zenodo.org/records/8200782)]
[[Data-Metzger2022 should contact edward.chang@ucsf.edu](edward.chang@ucsf.edu)]
[[Data-Willett2023](https://datadryad.org/stash/dataset/doi:10.5061/dryad.x69p8czpq)]
[[Data-Willett2021](https://datadryad.org/stash/dataset/doi:10.5061/dryad.wh70rxwmv)]



