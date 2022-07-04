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
- **Datasets**: Office-31, ImageCLEF-DA, Digits-five.

## Multi-Target Domain Adaptation (MTDA)

## Domain Generalization (DG)

[**DICA**] Muandet, K., Balduzzi, D., & Schölkopf, B. [Domain generalization via invariant feature representation](https://proceedings.mlr.press/v28/muandet13.html "DICA"). **ICML**, 2013.

- **Motivation**: This paper investigates domain generalization: **How to take knowledge acquired from an arbitrary number of related domains and apply it to previously unseen domains?**
- **Method**:  They propose Domain-Invariant Component Analysis (**DICA**), a kernel-based optimization algorithm that learns an invariant transformation by minimizing the dissimilarity across domains, whilst preserving the functional relationship between input and output variables.

[**CCSA**] Motiian, S., Piccirilli, M., Adjeroh, D. A., & Doretto, G. [Unified deep supervised domain adaptation and generalization](https://openaccess.thecvf.com/content_iccv_2017/html/Motiian_Unified_Deep_Supervised_ICCV_2017_paper.html "CCSA"). **ICCV**, 2017.

- **Method**: The main idea is to exploit the Siamese architecture to learn an embedding subspace that is discriminative, and where mapped visual domains are semantically aligned and yet maximally separated.
- **Datasets**: VLCS, MNIST.

## Open Set Domain Adaptation (OSDA)

[**ATI**] Panareda Busto, P., & Gall, J. [Open set domain adaptation](https://openaccess.thecvf.com/content_iccv_2017/html/Busto_Open_Set_Domain_ICCV_2017_paper.html "ATI"). **ICCV**, 2017.

- **Motivation**: They propose open set domain adaptation (**OSDA**). In this setting, **both source and target domain contain images that do not belong to the classes of interest**. Furthermore, **the target domain contains images that are not related to any image in the source domain and vice versa**.
- **Method**: They map the feature space of the source domain to the target domain. The mapping is estimated by assigning images in the target domain to some categories of the source domain. The assignment problem is defined by a binary linear program that also includes an implicit outlier handling, which discards images that are not related to any image in the source domain.
- **Datasets**: Office-31, Cross-Dataset Analysis.

Saito, K., Yamamoto, S., Ushiku, Y., & Harada, T. [Open set domain adaptation by backpropagation](https://openaccess.thecvf.com/content_ECCV_2018/html/Kuniaki_Saito_Adversarial_Open_Set_ECCV_2018_paper.html). **ECCV**, 2018.

- **Motivation**: They present a more challenging open set domain adaptation (**OSDA**) that **does not provide any unknown source samples**, and they propose a method for it. That is, they propose a method where they have **access to only known source samples and unlabeled target samples** for open set domain adaptation.
- **Method**: They propose a new approach of adversarial learning that enables generator to **separate target samples into known and unknown classes**.
- **Datasets**: Office-31, VisDA2017.

## Partial Domain Adaptation (PDA)

[**PADA**] Cao, Z., Ma, L., Long, M., & Wang, J. [Partial adversarial domain adaptation](https://openaccess.thecvf.com/content_ECCV_2018/html/Zhangjie_Cao_Partial_Adversarial_Domain_ECCV_2018_paper.html "PADA"). **ECCV**, 2018.

- **Motivation**: Existing domain adaptation methods generally assume that the source and the target domains share identical label space but follow different distributions. However, in real applications, it is usually not easy to find a source domain with identical label space as the target domain of interest. Towards the aforementioned ambition, they introduce a novel **partial domain adaptation** problem, which assumes that **the target label space is a subspace of the source label space**.
- **Method**: They present Partial Adversarial Domain Adaptation (**PADA**), which simultaneously **aligns the feature distributions of the source and target data in the shared label space** and more importantly, **identifies the irrelevant source data belonging to the outlier source classes and down-weighs their importance** automatically. 
- **Datasets**: Office-31, Office-Home, ImageNet-Caltech, VisDA2017.
- **Code**: [https://github.com/thuml/PADA](https://github.com/thuml/PADA).

## Universal Domain Adaptation (UDA)

[**UAN**] You, K., Long, M., Cao, Z., Wang, J., & Jordan, M. I. [Universal domain adaptation](https://openaccess.thecvf.com/content_CVPR_2019/html/You_Universal_Domain_Adaptation_CVPR_2019_paper.html "UAN"). **CVPR**, 2019.

- **Motivation**: They introduce Universal Domain Adaptation (**UDA**) that requires **no prior knowledge on the label sets**. For a given source label set and a target label set, they may contain a common label set and hold a private label set respectively, bringing up an additional category gap. UDA requires a model to either (1) classify the target sample correctly if it is associated with a label in the common label set, or (2) mark it as “unknown” otherwise. 
- **Method**: They propose Universal Adaptation Network (**UAN**). It quantifies sample-level transferability to discover the common label set and the label sets private to each domain, thereby **promoting the adaptation in the automatically discovered common label set** and **recognizing the “unknown” samples** successfully.
- **Datasets**: Office-31, Office-Home, VisDA2017, ImageNet-Caltech.
- **Code**: [https://github.com/thuml/Universal-Domain-Adaptation](https://github.com/thuml/Universal-Domain-Adaptation).

## Blending-Target Domain Adaptation (BTDA)

[**AMEAN**] Chen, Z., Zhuang, J., Liang, X., & Lin, L. [Blending-target domain adaptation by adversarial meta-adaptation networks](https://openaccess.thecvf.com/content_CVPR_2019/html/Chen_Blending-Target_Domain_Adaptation_by_Adversarial_Meta-Adaptation_Networks_CVPR_2019_paper.html "AMEAN"). **CVPR**, 2019.

- **Motivation**: In this paper, they consider a more realistic transfer scenario: **our target domain is comprised of multiple sub-targets implicitly blended with each other**, so that learners could not identify which sub-target each unlabeled sample belongs to.
- **Method**: They propose Adversarial Meta-Adaptation Network (**AMEAN**), a adversarial transfer framework incorporating meta-learner dynamically inducing meta-sub-targets to auto-design adversarial adaptation losses, which effectively achieve transfers in BTDA.
- **Datasets**: MNIST, MNIST-M, SVHN, USPS, Synthetic Digits, Office-31, Office-Home.

## Open Compound Domain Adaptation (OCDA)

Liu, Z., Miao, Z., Pan, X., Zhan, X., Lin, D., Yu, S. X., & Gong, B. [Open compound domain adaptation](https://openaccess.thecvf.com/content_CVPR_2020/html/Liu_Open_Compound_Domain_Adaptation_CVPR_2020_paper.html). **CVPR**, 2020.

- **Motivation**: They study an open compound domain adaptation (**OCDA**) problem, in which **the target is a compound of multiple homogeneous domains without domain labels**, reflecting realistic data collection from mixed and novel situations.
- **Method**: They propose a new approach based on two technical insights into OCDA: 1) a curriculum domain adaptation strategy to bootstrap generalization across domains in a datadriven self-organizing fashion and 2) a memory module to increase the model’s agility towards novel domains.
- **Datasets**: C-Digits, C-Faces, C-Driving, C-Mazes (designed by themselves).
- **Code**: [https://github.com/zhmiao/OpenCompoundDomainAdaptation-OCDA](https://github.com/zhmiao/OpenCompoundDomainAdaptation-OCDA).

## Self-Supervised Domain Adaptation (SSDA)

## Distant Domain Adaptation

## Source-Free Domain Adaptation

## Unsupervised Federated Domain Adaptation (UFDA)

[**FADA**] Peng, X., Huang, Z., Zhu, Y., & Saenko, K. [Federated Adversarial Domain Adaptation](https://openreview.net/forum?id=HJezF3VYPB "FADA"). **ICLR**, 2020.

- **Motivation**:  They address the problem of **transferring knowledge from the decentralized nodes to a new node with a different data domain**, without requiring any additional supervision from the user. They define this novel problem Unsupervised Federated Domain Adaptation (**UFDA**).
- **Method**: They propose Federated Adversarial Domain Adaptation (**FADA**) which aims to tackle domain shift in a federated learning system through adversarial techniques.
- **Datasets**: Digit-Five, Office-Caltech10, DomainNet, Amazon Review.

## Noisy Universal Domain Adaptation (Noisy UniDA)

Yu, Q., Hashimoto, A., & Ushiku, Y. [Divergence optimization for noisy universal domain adaptation](https://openaccess.thecvf.com/content/CVPR2021/html/Yu_Divergence_Optimization_for_Noisy_Universal_Domain_Adaptation_CVPR_2021_paper.html ""). **CVPR**, 2021.

- **Motivation**: They consider a new realistic setting called Noisy UniDA, in which **classifiers are trained with noisy labeled data from the source domain** and unlabeled data with an unknown class distribution from the target domain.
- **Method**: They introduce a two-head convolutional neural network framework to solve all problems simultaneously. Their network consists of one common feature generator and two classifiers with different decision boundaries. By optimizing the divergence between the two classifiers’ outputs, they can **detect noisy source samples**, **find “unknown” classes in the target domain**, and **align the distribution of the source and target domains**.
- **Datasets**: Office-31, Office-Home, VisDA2017.

------

Please create an issue if you find we missed any setting.