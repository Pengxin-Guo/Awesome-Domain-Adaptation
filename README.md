# Awesome-Domain-Adaptation
Various Domain Adaptation Setting.

The first work to propose this setting.

## Unsupervised Domain Adaptation (UDA)

## Semi-Supervised Domain Adaptation (SSDA)

## Multi-Source DA (MSDA)

## Multi-Target DA (MTDA)

## Domain Generalization (DG)

[**DICA**] Muandet, K., Balduzzi, D., & Schölkopf, B. [Domain generalization via invariant feature representation](https://proceedings.mlr.press/v28/muandet13.html "DICA"). **ICML**, 2013.

## Blending-Target Domain Adaptation (BTDA)

## Open Compound Domain Adaptation (OCDA)

## Partial Domain Adaptation (PDA)

[**PADA**] Cao, Z., Ma, L., Long, M., & Wang, J. [Partial adversarial domain adaptation](https://openaccess.thecvf.com/content_ECCV_2018/html/Zhangjie_Cao_Partial_Adversarial_Domain_ECCV_2018_paper.html "PADA"). **ECCV**, 2018.

- **Motivation**: Existing domain adaptation methods generally assume that the source and the target domains share identical label space but follow different distributions. However, in real applications, it is usually not easy to find a source domain with identical label space as the target domain of interest. Towards the aforementioned ambition, they introduce a novel **partial domain adaptation** problem, which assumes that **the target label space is a subspace of the source label space**.
- **Method**: They present Partial Adversarial Domain Adaptation (**PADA**), which simultaneously **aligns the feature distributions of the source and target data in the shared label space** and more importantly, **identifies the irrelevant source data belonging to the outlier source classes and down-weighs their importance** automatically. 
- **Dataset**: Office-31, Office-Home, ImageNet-Caltech, VisDA2017.
- **Code**: [https://github.com/thuml/PADA](https://github.com/thuml/PADA).

## Open Set Domain Adaptation (OSDA)

## Universal Domain Adaptation (UDA)

## Self-Supervised Domain Adaptation (SSDA)

## Distant Domain Adaptation

## Source-Free Domain Adaptation

## Federated Domain Adaptation

## Noisy Universal Domain Adaptation

------

Please create an issue if you find we missed any setting.