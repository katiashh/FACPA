Fast Adversarial CNN-based Perturbation Attack on No-Reference Image Quality Metrics (ICLR Tiny Papers 2023)
==============

[[OpenReview.net](https://openreview.net/forum?id=xKf-LSD2-Jg)] [[ArXiv](https://arxiv.org/abs/2305.15544)]


Modern neural-network-based no-reference image- and video-quality metrics exhibit performance as high as full-reference metrics. These metrics are widely
used to improve visual quality in computer vision methods and compare video processing methods. However, these metrics are not stable to traditional adversarial attacks, which can cause incorrect results. Our goal is to investigate the boundaries of no-reference metrics applicability, and in this paper, we propose a
fast adversarial perturbation attack on no-reference quality metrics. The proposed attack (FACPA) can be exploited as a preprocessing step in real-time video processing and compression algorithms. This research can yield insights to further
aid in designing of stable neural-network-based no-reference quality metrics.

![image](https://drive.google.com/uc?export=view&id=1ym97ObrVcL-Ak9NdpE5OCNXJK7of6Y3o)

## Code

FACPA inference code [![FACPA inference code. Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1GM9N23eK5-HZc-TPz6Fyts5NhbAG1OoQ/view?usp=sharing)

FACPA training code [![FACPA training code. Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://drive.google.com/file/d/1gkOi7rT3RG4fE1YwRL0yYjj-azCFwY4k/view?usp=sharing)

[Download pre-trained models](https://drive.google.com/drive/folders/1ei3WdDpSEnLmwvEVmABpBSPXygzVxobu) for attacks on [PaQ-2-PiQ](https://github.com/baidut/paq2piq), [Linearity](https://github.com/lidq92/LinearityIQA), [VSFA](https://github.com/lidq92/VSFA), [MDTVSFA](https://github.com/lidq92/MDTVSFA), [KonCept512](https://github.com/ZhengyuZhao/koniq-PyTorch), [Nima](https://github.com/truskovskiyk/nima.pytorch/tree/v1), and [SPAQ](https://github.com/h4nwei/SPAQ) 



## Citation

If you use this code for your research, please cite our paper.

```
@inproceedings{DBLP:conf/iclr/ShumitskayaAV23,
  author       = {Ekaterina Shumitskaya and
                  Anastasia Antsiferova and
                  Dmitriy S. Vatolin},
  editor       = {Krystal Maughan and
                  Rosanne Liu and
                  Thomas F. Burns},
  title        = {Fast Adversarial CNN-based Perturbation Attack on No-Reference Image-
                  and Video-Quality Metrics},
  booktitle    = {The First Tiny Papers Track at {ICLR} 2023, Tiny Papers @ {ICLR} 2023,
                  Kigali, Rwanda, May 5, 2023},
  publisher    = {OpenReview.net},
  year         = {2023},
  url          = {https://openreview.net/pdf?id=xKf-LSD2-Jg},
  timestamp    = {Tue, 18 Jul 2023 16:40:49 +0200},
  biburl       = {https://dblp.org/rec/conf/iclr/ShumitskayaAV23.bib},
  bibsource    = {dblp computer science bibliography, https://dblp.org}
}
```
