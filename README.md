Fast Adversarial CNN-based Perturbation Attack on No-Reference Image- and Video-Quality Metrics (ICLR Tiny Papers 2023)
==============

[[OpenReview.net](https://openreview.net/forum?id=xKf-LSD2-Jg)] [[ArXiv](https://arxiv.org/abs/2305.15544)] [[DBLP](https://dblp.org/rec/conf/iclr/ShumitskayaAV23.html4)]

Updates:
* Attacked FullHD dataset [added](https://github.com/katiashh/FACPA?tab=readme-ov-file#results-on-fullhd-videos)
* Paper related to the topic published [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S107731422300293X?via%3Dihub)

Modern neural-network-based no-reference image- and video-quality metrics exhibit performance as high as full-reference metrics. These metrics are widely
used to improve visual quality in computer vision methods and compare video processing methods. However, these metrics are not stable to traditional adversarial attacks, which can cause incorrect results. Our goal is to investigate the boundaries of no-reference metrics applicability, and in this paper, we propose a
fast adversarial perturbation attack on no-reference quality metrics. The proposed attack (FACPA) can be exploited as a preprocessing step in real-time video processing and compression algorithms. This research can yield insights to further
aid in designing of stable neural-network-based no-reference quality metrics.

![image](https://drive.google.com/uc?export=view&id=1ym97ObrVcL-Ak9NdpE5OCNXJK7of6Y3o)

## Results on FullHD videos
Results of FACPA attack on 10 FullHD videos and 3 attacked video-quality metrics. Metric scores were calculated on compressed videos (x264 codec, preset Medium, crf 16). Clear and attacked videos available [here](https://drive.google.com/drive/folders/1eHUJ-kPCIWQIjieLsAAx0rsLQsmlELrB?usp=drive_link). 

| Video | [Linearity](https://github.com/lidq92/LinearityIQA) clear | [Linearity](https://github.com/lidq92/LinearityIQA) attacked | [VSFA](https://github.com/lidq92/VSFA) clear | [VSFA](https://github.com/lidq92/VSFA) attacked | [MDTVSFA](https://github.com/lidq92/MDTVSFA) clear | [MDTVSFA](https://github.com/lidq92/MDTVSFA) attacked |
| - | - | - | - | - | - | - |
| Rush Hour | -67.4 | 201.7 | 0.48 | 1.72 | 0.41 | 0.79 |
| Blue Sky | -22.0 | 177.3 | 0.58 | 1.43 | 0.53 | 0.78 |
| Crowd Run | 53.8 | 135.2 | 0.79 |	1.42 | 0.66 | 0.78 |
| Old Town Cross | 8.9 | 148.9 | 0.72 |	1.37 | 0.58 | 0.79 |
| Tractor | -14.2 |	145.7 | 0.72 | 1.32 | 0.58 | 0.78 |
| Pedestrian Area | -40.0 | 192.3 |	0.65 | 1.60	| 0.58 | 0.79 |
| Controlled Burn | 5.9 | 173.5 | 0.71 | 1.57 | 0.57 | 0.79 |
| Red Kayak | 16.6 | 162.8 | 0.67 | 1.45 | 0.63 | 0.79 |
| Ducks | 52.0 | 100.6 | 0.68 | 0.85 | 0.54 | 0.68 |
| Park | 38.9 | 162.3 |	0.66 | 1.39 | 0.56 | 0.78 |

![image](https://drive.google.com/file/d/1KnmBmlVq7Q-c0dyepxMCCDAmFruNJmac)

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
