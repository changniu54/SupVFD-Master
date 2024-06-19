# Superclass-Aware Visual Feature Disentangling for Generalized Zero-Shot Learning



The code repository for "Superclass-Aware Visual Feature Disentangling for Generalized Zero-Shot Learning"



## SupVFD: Superclass-Aware Visual Feature Disentangling 

Zero-shot learning (ZSL) aims to learn a model trained on seen samples with the ability to recognize samples from unseen classes, while generalized ZSL (GZSL) takes a step closer to realistic scenarios by recognizing both of seen and unseen samples. The existing methods rely on the semantic descriptions as the side-information and conduct explicitly alignment between the visual and semantic space. However, the tight modality alignment may result in incomplete representations, leading to the loss of originally detailed and discriminative information. In this paper, we propose a simple yet effective superclass-aware visual feature disentangling method termed as SupVFD for GZSL.  We use the neighbor relations of the semantic descriptions to define superclass and with the guide of superclass, our method disentangles visual features into discriminative and transferable factors. To this end, the semantic descriptions are used as implicit supervision, which preserves the valuable detailed and discriminative information in the visual features. Further, we introduce transferability theory for analytically evaluating the transfer performance by regarding ZSL as an extreme case of transfer learning. The extensive experiments in both ZSL and GZSL settings prove our method outperforms the state-of-the-art methods for image object classification as well as video action recognition.




<div align="center">
  <img src="resources/framework.jpg" width="90%">



## Prerequisites

- [torch](https://github.com/pytorch/pytorch)
- [torchvision](https://github.com/pytorch/vision)
- [numpy](https://github.com/numpy/numpy)


## Training scripts on image datasets

- Train AWA1

  ```
  ./image-scripts/run_awa1.py
  ```
- Train AWA2

  ```
  ./image-scripts/run_awa2.py
  ```
- Train CUB

  ```
  ./image-scripts/run_cub.py
  ```

- Train FLO

  ```
  ./image-scripts/run_flo.py
  ```

- Train SUN

  ```
  ./image-scripts/run_sun.py
  ```

## Training scripts on action datasets

- Train HMDB51

  ```
  ./action-scripts/run_hmdb51.py
  ```
- Train UCF101

  ```
  ./action-scripts/run_ucf101.py
  ```

## Contact

If there are any questions, please feel free to contact with the author: Chang Niu (eeniu@mail.scut.edu.cn) or (niuchang54@163.com)