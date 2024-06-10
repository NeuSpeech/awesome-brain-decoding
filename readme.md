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

<details><summary>Table of Contents</summary><p>	

- [Brain to text](#brain-to-text)
- [Brain-to-image](#brain-to-image)
- [Foundation models](#foundation-models)
- [Theories](#theory)
- [Team and People](#team-and-people)
- [Datasets](#dataset)
</p></details><p></p>

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

**Speech synthesis from neural decoding of spoken sentences.**<br>
*Gopala K. Anumanchipalli\*, Josh Chartier\*, Edward F. Chang.*<br> 
Withdrawn recently.
 Nature. 2019 April 
[[PDF](https://europepmc.org/backend/ptpmcrender.fcgi?accid=PMC9714519&blobtype=pdf)] 

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

**Cinematic Mindscapes: High-quality Video Reconstruction from Brain Activity.**<br>
*Zijiao Chen\*,  Jiaxin Qing\*, Juan Helen Zhou*<br>
NeurIPS 2023.
[[PDF](https://www.nature.com/articles/s41598-023-42891-8)]
[[Project](https://mind-video.com/)]
[[Code](https://github.com/jqin4749/MindVideo)]
[[Data-HCP Young Adult](https://www.humanconnectome.org/study/hcp-young-adult/data-releases)]
[[Data-Wen](https://purr.purdue.edu/publications/2809/1)]


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

## Team and People

- [NCC lab](https://github.com/ncclab-sustech), **SUSTech**, by [Quanying Liu](https://www.sustech.edu.cn/zh/faculties/liuquanying.html).
- [Computational Cognitive and Translational Neuroscience Lab](https://yuanningli.github.io/), **ShanghaiTech**, by [Yuanning Li](https://yuanningli.github.io/).
- [Department of Linguistics and Translation](https://lt.cityu.edu.hk/), **CityU of HK**, by [Niels O. Schiller](https://scholars.cityu.edu.hk/en/person/nschille).
- [Meta/CNRS](https://ai.meta.com/), **École Normale Supérieure**, by [Jean-Remi King](https://kingjr.github.io/).
- [Neural Prosthetics Translational Laboratory](https://nptl.stanford.edu/), **Stanford University**, by [Jaimie Henderson](https://profiles.stanford.edu/jaimie-henderson).
- [HuthLab](https://www.cs.utexas.edu/~huth/), **The University of Texas at Austin**, by [Alexander G. Huth](https://www.cs.utexas.edu/people/faculty-researchers/alexander-huth).


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



