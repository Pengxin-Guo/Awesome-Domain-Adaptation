# Awesome-Domain-Adaptation
Various Domain Adaptation Setting.

The first work to propose this setting.

## Unsupervised Domain Adaptation (UDA)

## Semi-Supervised Domain Adaptation (SSDA)

## Multi-Source Domain Adaptation (MSDA)

[**A-SVMs**] Yang, J., Yan, R., & Hauptmann, A. G. [Cross-domain video concept detection using adaptive svms](https://dl.acm.org/doi/abs/10.1145/1291233.1291276?casa_token=CRYiwLHWxVsAAAAA:CF81_j9sOX_mEGPCe9I-_DgD_Quqm4Iup2XCp_T2VBJL4XPZWDpgPsde4YW03Okkc6AN8cjmD8R6 "A-SVMs"). **MM**, 2007.

- **Motivation**: how to transform existing classifier(s) into an effective classifier for a new dataset that only has a limited number of labeled examples.
- **Method**: They propose Adaptive Support Vector Machines (**A-SVMs**) as a general method to adapt one or more existing classifiers of any type to the new dataset. It aims to learn the “delta function” between the original and adapted classifier using an objective function similar to SVMs.

[**DCTN**] Xu, R., Chen, Z., Zuo, W., Yan, J., & Lin, L. [Deep cocktail network: Multi-source unsupervised domain adaptation with category shift](https://openaccess.thecvf.com/content_cvpr_2018/html/Xu_Deep_Cocktail_Network_CVPR_2018_paper.html "DCTN"). **CVPR**, 2018.

- **Motivation**: Unsupervised domain adaptation (UDA) conventionally assumes labeled source samples coming from a single underlying source distribution. Whereas **in practical scenario, labeled data are typically collected from diverse sources**.
- **Method**: They propose a deep cocktail network (**DCTN**) to battle the domain and category shifts among multiple sources.
- **Dataset**: Office-31, ImageCLEF-DA, Digits-five.

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