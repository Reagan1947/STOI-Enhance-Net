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

> Existing objective speech-intelligibility measures are suitable for several types of degradation, however, it turns out that they are less appropriate for methods where noisy speech is processed by a time-frequency (TF) weighting, e.g., noise reduction and speech separation. In this paper, we present an objective intelligibility measure, which shows high correlation (rho=0.95) with the intelligibility of both noisy, and TF-weighted noisy speech. The proposed method shows significantly better performance than three other, more sophisticated, objective measures. Furthermore, it is based on an intermediate intelligibility measure for short-time (approximately 400 ms) TF-regions, and uses a simple DFT-based TF-decomposition. In addition, a free Matlab implementation is provided. More Infor: https://ieeexplore.ieee.org/document/5495701

##### Idsegan

> This is the repository of the DSEGAN, ISEGAN, (and the baseline SEGAN) in our original paper:
>
> H. Phan, I. V. McLoughlin, L. Pham, O. Y. Chén, P. Koch, M. De Vos, and A. Mertins, "[*Improving GANs for Speech Enhancement*](https://arxiv.org/pdf/2001.05532.pdf)," IEEE Signal Processing Letters, 2020. *(accepted)*
>
> ISEGAN (Iterated SEGAN) and DSEGAN (Deep SEGAN) were built upon the SEGAN proposed by [Pascual *et al.*](https://arxiv.org/abs/1703.09452) and SEGAN repository from [santi-pdp](https://github.com/santi-pdp/segan). Different from SEGAN with a single generator, ISEGAN and DSEGAN have multiple generators which are chained to perform multi-stage enhancement mapping:
>
> [![idsegan.png](https://github.com/pquochuy/idsegan/raw/6cc2320339f2f0781caceb4a912c77401fdd9471/assets/idsegan.png)](https://github.com/pquochuy/idsegan/blob/6cc2320339f2f0781caceb4a912c77401fdd9471/assets/idsegan.png)
>
> The enhacement result of one generator is supposed to be further enhanced/corrected by the next generator in the chain. DSEGAN's generators are independent while ISEGAN's generators share parameters. Similar to SEGAN, the generators are based on fully convolutional architecture and receive raw speech waveforms to accomplish speech enhancement:
>
> [![generator](https://github.com/pquochuy/idsegan/raw/6cc2320339f2f0781caceb4a912c77401fdd9471/assets/generator.png)](https://github.com/pquochuy/idsegan/blob/6cc2320339f2f0781caceb4a912c77401fdd9471/assets/generator.png)

## Getting Started

This program is crate base on electron. You could try to build by the sorce file which I have puted in code.

这个小程序基于npm上的electron开发，你可以尝试使用[code](https://github.com/Reagan1947/latex2word)中的源文件基于electron进行运行。

## Dependency

This program id build base other githubprogram, based program is here:

这个小程序的开发参考了一些其他的github项目，如下是参考的项目：

1. [Latex2Equation](https://github.com/idf/LaTeX2Word-Equation)
2. [MathJax](https://www.mathjax.org/)

## Note&BUG

The source file does not include the required parts such as fontawesome mathjax.

At present, there are the following bugs:

源文件中并没有包括需要的部分例如fontawesome MathJax的源文件。

目前存在如下的Bug：

1. Window cannot be enlarged or set at the top   //无法放大或置顶窗口

2. RAM memory utilization is too high   //RAM内存使用率过高

3. The installation package did not delete unnecessary support files. The files are too large after electronic packaging   //安装包没有删除不需要的支持文件，electron打包以后文件过大

## To Do List

- [ ]  Finish mini and top window function.
- [ ] Rebuild it by VUE

## Versioning

- 2020/03/13  v1.0-beta 

## Authors

* **Reagan**  *China Student* - [Reagan1947](https://github.com/Reagan1947)

Like this program give me a star ⭐！Danke！

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

项目许可证为MIT许可证，你可以在[LICENSE](LICENSE)文件中查看。
