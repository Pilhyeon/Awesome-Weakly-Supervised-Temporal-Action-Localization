# weakly-superivsed temporal action localization
A curated publication list on weakly-supervised temporal action localization.

This repository was built to facilitate navigating the mainstream on weakly-supervised temporal action localization.
Please note that only **accepted** papers (for reliability) by **conferences** (for brevity) are contained here.

*Last updated: 2020/12/28*

##

## Table of Contents
- [Performance Tables](#performance-tables)
  - [THUMOS14](#thumos14)
  - [ActivityNet1.2](#activitynet12)
  - [ActivityNet1.3](#activitynet13)
- [Paper List](#paper-list)
- [Feedback](#feedback)

##

## Performance Tables
The mean average precisions (mAPs) under the standard intersection over union (IoU) thresholds are reported.
For example, '@0.5' indicates the mAP score at the IoU threshold of 0.5.  
The AVG denotes the average mAP under the IoU thresholds from 0.1 to 0.7 (for THUMOS14) or from 0.5 to 0.95 with a step size of 0.05 (for ActivityNet both versions).

In addition, links to the implementations are attached with their framework specification if available. 'o-' and 'u-' indicate the official and the unofficial implementations, respectively.

(*: additional use of trimmed videos, &dagger;: additional use of action count information, &Dagger;: additional use of pose information)

##

### THUMOS14

| ID | Year | Venue | Model<br/>(or Authors) |  @0.1   |  @0.2   |  @0.3   |  @0.4   |  @0.5   |  @0.6   |  @0.7   |   AVG   |  code  |
|:--:|:----:|:-----:|:----------------------:|:-------:|:-------:|:-------:|:-------:|:-------:|:-------:|:-------:|:-------:|:------:|
| 1  | 2017 | CVPR  | UntrimmedNets          |  44.4   |  37.7   |  28.2   |  21.1   |  13.7   |    -    |    -    |    -    |[`[o-matlab]`](https://github.com/wanglimin/UntrimmedNet)|
| 2  | 2017 | ICCV  | Hide-and-seek          |  36.4   |  27.8   |  19.5   |  12.7   |   6.8   |    -    |    -    |    -    |[`[o-torch]`](https://github.com/kkanshul/Hide-and-Seek)|
| 3  | 2018 | CVPR  | STPN                   |  52.0   |  44.7   |  35.5   |  25.8   |  16.9   |   9.9   |   4.3   |  27.0   |[`[u-tensorflow]`](https://github.com/bellos1203/STPN)|
| 4  | 2018 | ECCV  | AutoLoc                |    -    |    -    |  35.8   |  29.0   |  21.2   |  13.4   |   5.8   |    -    |[`[o-caffe]`](https://github.com/zhengshou/AutoLoc)|
| 5  | 2018 | ECCV  | W-TALC                 |  55.2   |  49.6   |  40.1   |  31.1   |  22.8   |    -    |   7.6   |    -    |[`[o-pytorch]`](https://github.com/sujoyp/wtalc-pytorch)<br/>[`[o-tensorflow]`](https://github.com/sujoyp/wtalc-tensorflow)|
| 6  | 2018 | MM    | Zhong et al.           |  45.8   |  39.0   |  31.1   |  22.5   |  15.9   |    -    |    -    |    -    |        |
| 7  | 2019 | AAAI  | TSRNet*                |  55.9   |  46.9   |  38.3   |  28.1   |  18.6   |  11.0   |   5.6   |  29.2   |        |
| 8  | 2019 | AAAI  | STAR&dagger;           |**68.8** |  60.0   |  48.7   |  34.7   |  23.0   |    -    |    -    |    -    |        |
| 9  | 2019 | ICLR  | MAAN                   |  59.8   |  50.8   |  41.1   |  30.6   |  20.3   |  12.0   |   6.9   |  31.6   |[`[o-pytorch]`](https://github.com/yyuanad/MAAN)|
| 10 | 2019 | CVPR  | Liu et al.             |  57.4   |  50.8   |  41.2   |  32.1   |  23.1   |  15.0   |   7.0   |  32.4   |[`[o-pytorch]`](https://github.com/Finspire13/CMCS-Temporal-Action-Localization)|
| 11 | 2019 | ICIP  | Park et al.            |    -    |    -    |  40.2   |  32.2   |  21.7   |    -    |   9.2   |    -    |        |
| 12 | 2019 | ICIP  | ACN                    |    -    |    -    |  35.9   |  30.7   |  24.2   |  15.7   |   7.4   |    -    |        |
| 13 | 2019 | MM    | ASSG                   |  65.6   |  59.4   |  50.4   |  38.7   |  25.4   |  15.0   |   6.6   |  37.3   |        |
| 14 | 2019 | ICCV  | CleanNet               |    -    |    -    |  37.0   |  30.9   |  23.9   |  13.9   |   7.1   |    -    |        |
| 15 | 2019 | ICCV  | TSM	                   |    -    |    -    |  39.5   |    -    |  24.5   |    -    |   7.1   |    -    |        |
| 16 | 2019 | ICCV  | 3C-Net&dagger;         |  59.1   |  53.5   |  44.2   |  34.1   |  26.6   |    -    |   8.1   |    -    |[`[o-pytorch]`](https://github.com/naraysa/3c-net)|
| 17 | 2019 | ICCV  | Nguyen et al.          |  60.4   |  56.0   |  46.6   |  37.5   |  26.8   |  17.6   |   9.0   |  36.3   |        |
| 18 | 2020 | AAAI  | PreTrimNet&Dagger;     |  57.5   |  50.7   |  41.4   |  32.1   |  23.1   |  14.2   |   7.7   |  32.4   |        |
| 19 | 2020 | AAAI  | BaS-Net                |  58.2   |  52.3   |  44.6   |  36.0   |  27.0   |  18.6   |  10.4   |  35.3   |[`[o-pytorch]`](https://github.com/Pilhyeon/BaSNet-pytorch)|
| 20 | 2020 | AAAI  | RPN                    |  62.3   |  57.0   |  48.2   |  37.2   |  27.9   |  16.7   |   8.1   |  36.8   |        |
| 21 | 2020 | WACV  | WSGN                   |  57.9   |  51.2   |  42.0   |  33.1   |  25.1   |  16.7   |   8.9   |  33.6   |        |
| 22 | 2020 | WACV  | Islam and Radke        |  62.3   |    -    |  46.8   |    -    |  29.6   |    -    |   9.7   |    -    |[`[o-pytorch]`](https://github.com/asrafulashiq/wsad)|
| 23 | 2020 | WACV  | Rashid et al.          |  63.7   |  56.9   |  47.3   |  36.4   |  26.1   |    -    |    -    |    -    |[`[o-pytorch]`](https://github.com/menorashid/action_graphs)|
| 24 | 2020 | CVPR  | ActionBytes            |    -    |    -    |  43.0   |  35.8   |  29.0   |    -    |   9.5   |    -    |        |
| 25 | 2020 | CVPR  | DGAM	                 |  60.0   |  54.2   |  46.8   |  38.2   |  28.8   |  19.8   |  11.4   |  37.0   |[`[o-pytorch]`](https://github.com/bfshi/DGAM-Weakly-Supervised-Action-Localization)|
| 26 | 2020 | CVPR  | Gong et al.            |    -    |    -    |  46.9   |  38.9   |  30.1   |  19.8   |  10.4   |    -    |[`[o-pytorch]`](https://github.com/GGQ1996/action_co_localization/tree/master/ACL_Anet_release)|
| 27 | 2020 | ECCV  | EM-MIL                 |  59.1   |  52.7   |  45.5   |  36.8   |  30.5   |  22.7   |**16.4** |  37.7   |        |
| 28 | 2020 | ECCV  | A2CL-PT                |  61.2   |  56.1   |  48.1   |  39.0   |  30.1   |  19.2   |  10.6   |  37.8   |[`[o-pytorch]`](https://github.com/MichiganCOG/A2CL-PT)|
| 29 | 2020 | ECCV  | TSCN                   |  63.4   |  57.6   |  47.8   |  37.7   |  28.7   |  19.4   |  10.2   |  37.8   |        |
| 30 | 2020 | MM    | ACM-BANet              |  64.6   |  57.7   |  48.9   |  40.9   |  32.3   |  21.9   |  13.5   |  40.0   |        |
| 31 | 2021 | AAAI  | Lee et al.             |  67.5   |**61.2** |**52.3** |**43.4** |**33.7** |**22.9** |  12.1   |**41.9** |[`[o-pytorch]`](https://github.com/Pilhyeon/WTAL-Uncertainty-Modeling)|

##

### ActivityNet1.2

| ID | Year | Venue | Model<br/>(or Authors) |  @0.5   |  @0.75  |  @0.95  |   AVG   |  code  |
|:--:|:----:|:-----:|:----------------------:|:-------:|:-------:|:-------:|:-------:|:------:|
| 4  | 2018 | ECCV  | AutoLoc                |  27.3   |  15.1   |   3.3   |  16.0   |[`[o-caffe]`](https://github.com/zhengshou/AutoLoc)|
| 5  | 2018 | ECCV  | W-TALC                 |  37.0   |    -    |    -    |  18.0   |[`[o-pytorch]`](https://github.com/sujoyp/wtalc-pytorch)<br/>[`[o-tensorflow]`](https://github.com/sujoyp/wtalc-tensorflow)|
| 6  | 2018 | MM    | Zhong et al.           |  27.3   |  14.7   |   2.9   |  15.6   |        |
| 10 | 2019 | CVPR  | Liu et al.             |  36.8   |  22.0   |   5.6   |  22.4   |[`[o-pytorch]`](https://github.com/Finspire13/CMCS-Temporal-Action-Localization)|
| 11 | 2019 | ICIP  | Park et al.            |  33.7   |    -    |    -    |    -    |        |
| 12 | 2019 | ICIP  | ACN                    |  30.4   |  15.4   |   3.7   |  17.0   |        |
| 14 | 2019 | ICCV  | CleanNet               |  37.1   |  20.3   |   5.0   |  21.6   |        |
| 15 | 2019 | ICCV  | TSM	                   |  28.3   |  17.0   |   3.5   |  17.1   |        |
| 16 | 2019 | ICCV  | 3C-Net&dagger;         |  37.2   |    -    |    -    |  21.7   |[`[o-pytorch]`](https://github.com/naraysa/3c-net)|
| 19 | 2020 | AAAI  | BaS-Net                |  38.5   |  24.2   |   5.6   |  24.3   |[`[o-pytorch]`](https://github.com/Pilhyeon/BaSNet-pytorch)|
| 20 | 2020 | AAAI  | RPN                    |  37.6   |  23.9   |   5.4   |  23.3   |        |
| 22 | 2020 | WACV  | Islam and Radke        |  35.2   |    -    |    -    |    -    |[`[o-pytorch]`](https://github.com/asrafulashiq/wsad)|
| 23 | 2020 | WACV  | Rashid et al.          |  29.4   |    -    |    -    |    -    |[`[o-pytorch]`](https://github.com/menorashid/action_graphs)|
| 24 | 2020 | CVPR  | ActionBytes            |  39.4   |    -    |    -    |    -    |        |
| 25 | 2020 | CVPR  | DGAM	                 |  41.0   |  23.5   |   5.3   |  24.4   |[`[o-pytorch]`](https://github.com/bfshi/DGAM-Weakly-Supervised-Action-Localization)|
| 26 | 2020 | CVPR  | Gong et al.            |  40.0   |  25.0   |   4.6   |  24.6   |[`[o-pytorch]`](https://github.com/GGQ1996/action_co_localization/tree/master/ACL_Anet_release)|
| 27 | 2020 | ECCV  | EM-MIL                 |  37.4   |    -    |    -    |  20.3   |        |
| 29 | 2020 | ECCV  | TSCN                   |  37.6   |  23.7   |   5.7   |  23.6   |        |
| 31 | 2021 | AAAI  | Lee et al.             |**41.2** |**25.6** | **6.0** |**25.9** |[`[o-pytorch]`](https://github.com/Pilhyeon/WTAL-Uncertainty-Modeling)|

##

### ActivityNet1.3

| ID | Year | Venue | Model<br/>(or Authors) |  @0.5   |  @0.75  |  @0.95  |   AVG   |  code  |
|:--:|:----:|:-----:|:----------------------:|:-------:|:-------:|:-------:|:-------:|:------:|
| 3  | 2018 | CVPR  | STPN                   |  29.3   |  16.9   |   2.6   |    -    |[`[u-tensorflow]`](https://github.com/bellos1203/STPN)|
| 7  | 2019 | AAAI  | TSRNet*                |  33.1   |  18.7   |   3.3   |  21.8   |        |
| 8  | 2019 | AAAI  | STAR&dagger;           |  31.1   |  18.8   |   4.7   |    -    |        |
| 9  | 2019 | ICLR  | MAAN                   |  33.7   |  21.9   |   5.5   |    -    |[`[o-pytorch]`](https://github.com/yyuanad/MAAN)|
| 10 | 2019 | CVPR  | Liu et al.             |  34.0   |  20.9   |   5.7   |  21.2   |[`[o-pytorch]`](https://github.com/Finspire13/CMCS-Temporal-Action-Localization)|
| 13 | 2019 | MM    | ASSG                   |  32.3   |  20.1   |   4.0   |    -    |        |
| 15 | 2019 | ICCV  | TSM	                   |  30.3   |  19.0   |   4.5   |    -    |        |
| 17 | 2019 | ICCV  | Nguyen et al.          |  36.4   |  19.2   |   2.9   |    -    |        |
| 18 | 2020 | AAAI  | PreTrimNet&Dagger;     |  34.8   |  20.9   |   5.3   |  22.5   |        |
| 19 | 2020 | AAAI  | BaS-Net                |  34.5   |  22.5   |   4.9   |  22.2   |[`[o-pytorch]`](https://github.com/Pilhyeon/BaSNet-pytorch)|
| 28 | 2020 | ECCV  | A2CL-PT                |  36.8   |  22.0   |   5.2   |  22.5   |[`[o-pytorch]`](https://github.com/MichiganCOG/A2CL-PT)|
| 29 | 2020 | ECCV  | TSCN                   |  35.3   |  21.4   |   5.3   |  21.7   |        |
| 30 | 2020 | MM    | ACM-BANet              |**37.6** |**24.7** | **6.5** |**24.4** |        |
| 31 | 2021 | AAAI  | Lee et al.             |  37.0   |  23.9   |   5.7   |  23.7   |[`[o-pytorch]`](https://github.com/Pilhyeon/WTAL-Uncertainty-Modeling)|

##

## Paper List

1. **[UntrimmedNets]** | **CVPR'17** | UntrimmedNets for Weakly Supervised Action Recognition and Detection | [`[pdf]`](https://arxiv.org/pdf/1703.03329.pdf) | [`[o-matlab]`](https://github.com/wanglimin/UntrimmedNet)
2. **[Hide-and-seek]** | **ICCV'17** | Hide-and-Seek: Forcing a Network to be Meticulous for Weakly-supervised Object and Action Localization | [`[pdf]`](https://arxiv.org/pdf/1704.04232.pdf) | [`[o-torch]`](https://github.com/kkanshul/Hide-and-Seek)
3. **[STPN]** | **CVPR'18** | Weakly Supervised Action Localization by Sparse Temporal Pooling Network | [`[pdf]`](https://arxiv.org/pdf/1712.05080.pdf) | [`[u-tensorflow]`](https://github.com/bellos1203/STPN)
4. **[AutoLoc]** | **ECCV'18** | AutoLoc: Weakly-supervised Temporal Action Localization in Untrimmed Videos | [`[pdf]`](https://arxiv.org/pdf/1807.08333.pdf) | [`[o-caffe]`](https://github.com/zhengshou/AutoLoc)
5. **[W-TALC]** | **ECCV'18** | W-TALC: Weakly-supervised Temporal Activity Localization and Classification | [`[pdf]`](https://arxiv.org/pdf/1807.10418.pdf) | [`[o-pytorch]`](https://github.com/sujoyp/wtalc-pytorch) | [`[o-tensorflow]`](https://github.com/sujoyp/wtalc-tensorflow)
6. **[Zhong et al.]** | **MM'18** | Step-by-step Erasion, One-by-one Collection: A Weakly Supervised Temporal Action Detector | [`[pdf]`](https://arxiv.org/pdf/1807.02929.pdf)
7. **[TSR-Net]** | **AAAI'19** | Learning Transferable Self-attentive Representations for Action Recognition in Untrimmed Videos with Weak Supervision | [`[pdf]`](https://arxiv.org/pdf/1902.07370.pdf)
8. **[STAR]** | **AAAI'19** | Learning Transferable Self-attentive Representations for Action Recognition in Untrimmed Videos with Weak Supervision | [`[pdf]`](https://arxiv.org/pdf/1811.07460.pdf)
9. **[MAAN]** | **ICLR'19** | Marginalized Average Attentional Network for Weakly-Supervised Learning | [`[pdf]`](https://arxiv.org/pdf/1905.08586.pdf)
10. **[Liu et al.]** | **CVPR'19** | Completeness Modeling and Context Separation for Weakly Supervised
Temporal Action Localization | [`[pdf]`](https://openaccess.thecvf.com/content_CVPR_2019/papers/Liu_Completeness_Modeling_and_Context_Separation_for_Weakly_Supervised_Temporal_Action_CVPR_2019_paper.pdf) | [`[o-pytorch]`](https://github.com/Finspire13/CMCS-Temporal-Action-Localization)
11. **[Park et al.]** | **ICIP'19** | Graph Regularization Network with Semantic Affinity for Weakly-Supervised Temporal Action Localization | [`[pdf]`](https://easy00.github.io/assets/publication/icip19_Jungin_Park.pdf)
12. **[ACN]** | **ICIP'19** | Action Coherence Network for Weakly Supervised Temporal Action Localization | [`[pdf]`](https://www.yhzhai.com/publications/Action-Coherence-Network-for-Weakly-Supervised-Temporal-Action-Localization.pdf)
13. **[ASSG]** | **MM'19** | Adversarial Seeded Sequence Growing for Weakly-Supervised Temporal Action Localization | [`[pdf]`](https://arxiv.org/pdf/1908.02422.pdf)
14. **[CleanNet]** | **ICCV'19** | Weakly Supervised Temporal Action Localization through Contrast based Evaluation Networks | [`[pdf]`](https://openaccess.thecvf.com/content_ICCV_2019/papers/Liu_Weakly_Supervised_Temporal_Action_Localization_Through_Contrast_Based_Evaluation_Networks_ICCV_2019_paper.pdf)
15. **[TSM]** | **ICCV'19** | Temporal Structure Mining for Weakly Supervised Action Detection | [`[pdf]`](https://openaccess.thecvf.com/content_ICCV_2019/papers/Yu_Temporal_Structure_Mining_for_Weakly_Supervised_Action_Detection_ICCV_2019_paper.pdf)
16. **[3C-Net]** | **ICCV'19** | 3C-Net: Category Count and Center Loss for Weakly-Supervised Action Localization | [`[pdf]`](https://arxiv.org/pdf/1908.08216.pdf) | [`[o-pytorch]`](https://github.com/naraysa/3c-net)
17. **[Nguyen et al.]** | **ICCV'19** | Weakly-supervised Action Localization with Background Modeling | [`[pdf]`](https://arxiv.org/pdf/1908.06552.pdf)
18. **[PreTrimNet]** | **AAAI'20** | Multi-Instance Multi-Label Action Recognition and Localization Based on Spatio-Temporal Pre-Trimming for Untrimmed Videos | [`[pdf]`](https://ojs.aaai.org/index.php/AAAI/article/download/6986/6840)
19. **[BaS-Net]** | **AAAI'20** | Background Suppression Network for Weakly-supervised Temporal Action Localization | [`[pdf]`](https://arxiv.org/pdf/1911.09963.pdf) | [`[o-pytorch]`](https://github.com/Pilhyeon/BaSNet-pytorch)
20. **[RPN]** | **AAAI'20** | Relational Prototypical Network for Weakly Supervised Temporal Action Localization | [`[pdf]`](http://ir.ia.ac.cn/bitstream/173211/39128/1/AAAI-HuangL.1235.pdf)
21. **[WSGN]** | **WACV'20** | Weakly Supervised Gaussian Networks for Action Detection | [`[pdf]`](https://arxiv.org/pdf/1904.07774.pdf)
22. **[Islam and Radke]** | **WACV'20** | Weakly Supervised Temporal Action Localization Using Deep Metric Learning | [`[pdf]`](https://arxiv.org/pdf/2001.07793.pdf) | [`[o-pytorch]`](https://github.com/asrafulashiq/wsad)
23. **[Rashid et al.]** | **WACV'20** | Action Graphs: Weakly-supervised Action Localization with Graph Convolution Networks | [`[pdf]`](https://arxiv.org/pdf/2002.01449.pdf) | [`[o-pytorch]`](https://github.com/menorashid/action_graphs)
24. **[ActionBytes]** | **CVPR'20** | ActionBytes: Learning from Trimmed Videos to Localize Actions | [`[pdf]`](https://openaccess.thecvf.com/content_CVPR_2020/papers/Jain_ActionBytes_Learning_From_Trimmed_Videos_to_Localize_Actions_CVPR_2020_paper.pdf)
25. **[DGAM]** | **CVPR'20** | Weakly-Supervised Action Localization by Generative Attention Modeling | [`[pdf]`](https://arxiv.org/pdf/2003.12424.pdf) | [`[o-pytorch]`](https://github.com/bfshi/DGAM-Weakly-Supervised-Action-Localization)
26. **[Gong et al.]** | **CVPR'20** | Learning Temporal Co-Attention Models for Unsupervised Video Action Localization | [`[pdf]`](https://openaccess.thecvf.com/content_CVPR_2020/papers/Gong_Learning_Temporal_Co-Attention_Models_for_Unsupervised_Video_Action_Localization_CVPR_2020_paper.pdf) | [`[o-pytorch]`](https://github.com/GGQ1996/action_co_localization/tree/master/ACL_Anet_release)
27. **[EM-MIL]** | **ECCV'20** | Weakly-Supervised Action Localization with Expectation-Maximization Multi-Instance Learning | [`[pdf]`](https://arxiv.org/pdf/2004.00163.pdf)
28. **[A2CL-PT]** | **ECCV'20** | Adversarial Background-Aware Loss for Weakly-supervised Temporal Activity Localization | [`[pdf]`](https://arxiv.org/pdf/2007.06643.pdf) | [`[o-pytorch]`](https://github.com/MichiganCOG/A2CL-PT)
29. **[TSCN]** | **ECCV'20** | Two-Stream Consensus Network for Weakly-Supervised Temporal Action Localization | [`[pdf]`](https://arxiv.org/pdf/2010.11594.pdf)
30. **[ACM-BANet]** | **MM'20** | Action Completeness Modeling with Background Aware Networks for Weakly-Supervised Temporal Action Localization | [`[pdf]`](https://dl.acm.org/doi/pdf/10.1145/3394171.3413687)
31. **[Lee et al.]** | **AAAI'21** | Weakly-supervised Temporal Action Localization by Uncertainty Modeling | [`[pdf]`](https://arxiv.org/pdf/2006.07006.pdf) | [`[o-pytorch]`](https://github.com/Pilhyeon/WTAL-Uncertainty-Modeling)

##

## Feedback

If you have any suggestions or find missing papers, please feel free to contact me.

- [e-mail](mailto:lph1114@yonsei.ac.kr)
- [pull request](https://github.com/Pilhyeon/weakly-supervised-temporal-action-localization/pulls)

