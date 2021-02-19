<h1 align="center">
  <br>
  <img src="https://github.com/Reagan1947/STOI-Enhance-Net/blob/main/README_source/STOI-Enhance-Net_icon.png?raw=true" alt="STOI-Enhance-Net_icon" width="170">
  <br>
  STOI-Enhance-Net
  <br>
</h1>
<h4 align="center" font-weight:bold;">Speech Enhancement Network Based On STOI Score Loss Function<br>基于STOI语音评价指标损失函数的语音增强网络</h4>
<p align="center">
<img src="https://img.shields.io/badge/license-MIT-%23373737">
<img src="https://img.shields.io/badge/plantform-Tensorflow-lightgrey">
</p>


<p align="center">
<img src="https://github.com/Reagan1947/latex2word/blob/master/exp_pic.png">
</p>

## 1. Dataset 数据集

##### Microsoft Scalable Noisy Speech Dataset (MS-SNSD)

- This dataset contains a large collection of clean speech files and variety of environmental noise files in .wav format sampled at 16 kHz.

- The main application of this dataset is to train Deep Neural Network (DNN) models to suppress background noise. But it can be used for other audio and speech applications.

- We provide the recipe to mix clean speech and noise at various signal to noise ratio (SNR) conditions to generate large noisy speech dataset.

- The SNR conditions and the number of hours of data required can be configured depending on the application requirements.
- More Infor: https://github.com/microsoft/MS-SNSD



## 2. Based on 基于

##### STOI 

> Existing objective speech-intelligibility measures are suitable for several types of degradation, however, it turns out that they are less appropriate for methods where noisy speech is processed by a time-frequency (TF) weighting, e.g., noise reduction and speech separation. In this paper, we present an objective intelligibility measure, which shows high correlation (rho=0.95) with the intelligibility of both noisy, and TF-weighted noisy speech. The proposed method shows significantly better performance than three other, more sophisticated, objective measures. Furthermore, it is based on an intermediate intelligibility measure for short-time (approximately 400 ms) TF-regions, and uses a simple DFT-based TF-decomposition. In addition, a free Matlab implementation is provided. 
>
> More Infor: https://ieeexplore.ieee.org/document/5495701

##### IDSEGAN

> This is the repository of the DSEGAN, ISEGAN, (and the baseline SEGAN) in our original paper:
>
> H. Phan, I. V. McLoughlin, L. Pham, O. Y. Chén, P. Koch, M. De Vos, and A. Mertins, "[*Improving GANs for Speech Enhancement*](https://arxiv.org/pdf/2001.05532.pdf)," IEEE Signal Processing Letters, 2020. *(accepted)*
>
> More Infor: https://github.com/pquochuy/idsegan



## 3. Statue 项目进度

1. Dataset Preparation 数据集准备



## 4. Dependencies 依赖

- tensorflow_gpu == 1.9
- numpy== 1.1.3
- scipy== 1.0.0