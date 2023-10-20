# [NeurIPS 2023] Bridging Semantic Gaps for Language Supervised Semantic Segmentation

This is the official repository of the following paper.
> **[Bridging Semantic Gaps for Language Supervised Semantic Segmentation](https://arxiv.org/abs/2309.13505)**<br>
> [Yun Xing](https://scholar.google.com/citations?user=uOAYTXoAAAAJ&hl=en&oi=ao), [Jian Kang](https://www.linkedin.com/in/alan-kang-6497b5239), [Aoran Xiao](https://scholar.google.com/citations?user=yGKsEpAAAAAJ&hl=en), [Jiahao Nie](https://niejiahao1998.github.io/), [Ling Shao](https://scholar.google.com/citations?user=z84rLjoAAAAJ&hl=zh-CN&oi=ao), [Shijian Lu](https://scholar.google.com/citations?user=uYmK-A0AAAAJ&hl=en&oi=ao)<br>

Code will be released soon. Please stay tuned.

## Updates

- [09/2023] arXiv available.
- [09/2023] accepted by [NeurIPS 2023](https://nips.cc/).

## Environmental Setup
```
conda create -n cocu python=3.7 -y
conda activate cocu

conda install pytorch==1.8.0 torchvision==0.9.0 cudatoolkit=11.1 -c pytorch -c conda-forge
pip install mmcv-full==1.3.14 -f https://download.openmmlab.com/mmcv/dist/cu111/torch1.8.0/index.html
pip install packaging mmsegmentation==0.18.0 webdataset==0.1.103 timm==0.4.12 opencv-python==4.4.0.46 termcolor==1.1.0 diffdist einops omegaconf nltk ftfy regex tqdm clip-retrieval

git clone https://github.com/NVIDIA/apex
cd apex
pip install -v --disable-pip-version-check --no-cache-dir --no-build-isolation --global-option="--cpp_ext" --global-option="--cuda_ext" ./
```
##### dependency
```

```

## Data Preparation

Please refer to [here](https://github.com/xing0047/CoCu/tree/main/data).

## Citation

Please consider citing our paper if you find our work useful for you.
```
@misc{xing2023bridging,
      title={Bridging Semantic Gaps for Language-Supervised Semantic Segmentation}, 
      author={Yun Xing and Jian Kang and Aoran Xiao and Jiahao Nie and Shao Ling and Shijian Lu},
      year={2023},
      eprint={2309.13505},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```

## Acknowledgement

The repo is built on [GroupViT](https://github.com/NVlabs/GroupViT) and [clip-retrieval](https://github.com/rom1504/clip-retrieval).
