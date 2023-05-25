<div align="center">
<h1> ViTMatte🐒</h1>
<h3> Boosting Image Matting with Pretrained Plain Vision Transformers</h3>

[Jingfeng Yao](https://github.com/JingfengYao)<sup>1</sup>, [Xinggang Wang](https://xinggangw.info/)<sup>1 📧</sup>, [Shusheng Yang](https://github.com/vealocia)<sup>1</sup>, [Baoyuan Wang](https://sites.google.com/site/zjuwby/)<sup>2</sup>

<sup>1</sup> School of EIC, HUST, <sup>2</sup> Xiaobing.AI

(<sup>📧</sup>) corresponding author.

[arxiv Preprint](https://arxiv.org/abs/2305.15272)

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/vitmatte-boosting-image-matting-with/image-matting-on-composition-1k-1)](https://paperswithcode.com/sota/image-matting-on-composition-1k-1?p=vitmatte-boosting-image-matting-with)

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/vitmatte-boosting-image-matting-with/image-matting-on-distinctions-646)](https://paperswithcode.com/sota/image-matting-on-distinctions-646?p=vitmatte-boosting-image-matting-with)

</div>

#

## News
* **`May 25th, 2023`:** We released codes of ViTMatte. The pretrained models will be coming soon!
* **`May 24th, 2023`:** We released our paper on [arxiv](https://arxiv.org/abs/2305.15272). 

## Introduction
<div align="center"><h4>Plain Vision Transformer could also do image matting with simple ViTMatte framework!</h4></div>

![avatar](figs/vitmatte.png)

Recently, plain vision Transformers (ViTs) have shown impressive performance on various computer vision tasks, thanks to their strong modeling capacity and large-scale pretraining. However, they have not yet conquered the problem of image matting. We hypothesize that image matting could also be boosted by ViTs and present a new efficient and robust ViT-based matting system, named ViTMatte. Our method utilizes (i) a hybrid attention mechanism combined with a convolution neck to help ViTs achieve an excellent performance-computation trade-off in matting tasks. (ii) Additionally, we introduce the detail capture module, which just consists of simple lightweight convolutions to complement the detailed information required by matting. To the best of our knowledge, ViTMatte is the first work to unleash the potential of ViT on image matting with concise adaptation. It inherits many superior properties from ViT to matting, including various pretraining strategies, concise architecture design, and flexible inference strategies. We evaluate ViTMatte on Composition-1k and Distinctions-646, the most commonly used benchmark for image matting, our method achieves state-of-the-art performance and outperforms prior matting works by a large margin.

## Results

Quantitative Results on [Composition-1k](https://paperswithcode.com/dataset/composition-1k)
| Model      | SAD   | MSE | Grad | Conn  | checkpoints |
| ---------- | ----- | --- | ---- | ----- | ----------- |
| ViTMatte-S | 21.46 | 3.3 | 7.24 | 16.21 | coming soon |
| ViTMatte-B | 20.33 | 3.0 | 6.74 | 14.78 | coming soon |

Quantitative Results on [Distinctions-646](https://paperswithcode.com/dataset/distinctions-646)
| Model      | SAD   | MSE | Grad | Conn  | checkpoints |
| ---------- | ----- | --- | ---- | ----- | ----------- |
| ViTMatte-S | 21.22 | 2.1 | 8.78 | 17.55 | coming soon |
| ViTMatte-B | 17.05 | 1.5 | 7.03 | 12.95 | coming soon |


## Get Started

* [Installation](docs/installation.md)
* [Train](docs/train.md)
* [Test](docs/test.md)

## Citation
```
@article{vitmatte,
      title={ViTMatte: Boosting Image Matting with Pretrained Plain Vision Transformers}, 
      author={Jingfeng Yao and Xinggang Wang and Shusheng Yang and Baoyuan Wang},
      journal={arXiv preprint arXiv:2305.15272},
      year={2023}
}
```