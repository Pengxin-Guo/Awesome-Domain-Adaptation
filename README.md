# Awesome-Domain-Adaptation
Various Domain Adaptation Setting.

The first work to propose this setting.

## Unsupervised Domain Adaptation (UDA)

## Semi-Supervised Domain Adaptation (SSDA)

## Multi-Source Domain Adaptation (MSDA)

## Multi-Target Domain Adaptation (MTDA)

## Domain Generalization (DG)

[**DICA**] Muandet, K., Balduzzi, D., & Schölkopf, B. [Domain generalization via invariant feature representation](https://proceedings.mlr.press/v28/muandet13.html "DICA"). **ICML**, 2013.

- **Motivation**: This paper investigates domain generalization: **How to take knowledge acquired from an arbitrary number of related domains and apply it to previously unseen domains?**
- **Method**:  They propose Domain-Invariant Component Analysis (**DICA**), a kernel-based optimization algorithm that learns an invariant transformation by minimizing the dissimilarity across domains, whilst preserving the functional relationship between input and output variables.

## Partial Domain Adaptation (PDA)

[**PADA**] Cao, Z., Ma, L., Long, M., & Wang, J. [Partial adversarial domain adaptation](https://openaccess.thecvf.com/content_ECCV_2018/html/Zhangjie_Cao_Partial_Adversarial_Domain_ECCV_2018_paper.html "PADA"). **ECCV**, 2018.

- **Motivation**: Existing domain adaptation methods generally assume that the source and the target domains share identical label space but follow different distributions. However, in real applications, it is usually not easy to find a source domain with identical label space as the target domain of interest. Towards the aforementioned ambition, they introduce a novel **partial domain adaptation** problem, which assumes that **the target label space is a subspace of the source label space**.
- **Method**: They present Partial Adversarial Domain Adaptation (**PADA**), which simultaneously **aligns the feature distributions of the source and target data in the shared label space** and more importantly, **identifies the irrelevant source data belonging to the outlier source classes and down-weighs their importance** automatically. 
- **Dataset**: Office-31, Office-Home, ImageNet-Caltech, VisDA2017.
- **Code**: [https://github.com/thuml/PADA](https://github.com/thuml/PADA).

## Blending-Target Domain Adaptation (BTDA)

[**AMEAN**] Chen, Z., Zhuang, J., Liang, X., & Lin, L. [Blending-target domain adaptation by adversarial meta-adaptation networks](https://openaccess.thecvf.com/content_CVPR_2019/html/Chen_Blending-Target_Domain_Adaptation_by_Adversarial_Meta-Adaptation_Networks_CVPR_2019_paper.html "AMEAN"). **CVPR**, 2019.

- **Motivation**: In this paper, they consider a more realistic transfer scenario: **our target domain is comprised of multiple sub-targets implicitly blended with each other**, so that learners could not identify which sub-target each unlabeled sample belongs to.
- **Method**: They propose Adversarial Meta-Adaptation Network (**AMEAN**), a adversarial transfer framework incorporating meta-learner dynamically inducing meta-sub-targets to auto-design adversarial adaptation losses, which effectively achieve transfers in BTDA.
- **Dataset**: MNIST, MNIST-M, SVHN, USPS, Synthetic Digits, Office-31, Office-Home.

## Open Compound Domain Adaptation (OCDA)

## Open Set Domain Adaptation (OSDA)

## Universal Domain Adaptation (UDA)

## Self-Supervised Domain Adaptation (SSDA)

## Distant Domain Adaptation

## Source-Free Domain Adaptation

## Federated Domain Adaptation

## Noisy Universal Domain Adaptation

------

Please create an issue if you find we missed any setting.