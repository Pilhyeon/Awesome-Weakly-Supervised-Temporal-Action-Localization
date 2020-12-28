# weakly-superivsed-temporal-action-localization
A paper list on weakly-supervised temporal action localization. This repository is made to facilitate navigating the mainstream on weakly-supervised temporal action localization.

*Last updated: 2020/12/28*

## Performance table

### THUMOS'14

| Year | Venue | Model<br/>(or Authors) | mAP@0.1 | mAP@0.2 | mAP@0.3 | mAP@0.4 | mAP@0.5 | mAP@0.6 | mAP@0.7 | AVG|
|:----:|:-----:|:----------------------:|:-------:|:-------:|:-------:|:-------:|:-------:|:-------:|:-------:|:------------:|
| 2017 | CVPR  | UntrimmedNets          |  44.4   |  37.7   |  28.2   |  21.1   |  13.7   |    -    |    -    |      -       |
| 2017 | ICCV  | Hide-and-seek          |  36.4   |  27.8   |  19.5   |  12.7   |   6.8   |    -    |    -    |      -       |
| 2018 | CVPR  | STPN                   |  52.0   |  44.7   |  35.5   |  25.8   |  16.9   |   9.9   |   4.3   |    27.0      |
| 2018 | ECCV  | AutoLoc                |    -    |    -    |  35.8   |  29.0   |  21.2   |  13.4   |   5.8   |      -       |
| 2018 | ECCV  | W-TALC                 |  55.2   |  49.6   |  40.1   |  31.1   |  22.8   |    -    |   7.6   |      -       |
| 2019 | AAAI  | TSRNet                 |  55.90  |  46.90  |  38.30  |  28.10  |  18.60  |  11.00  |   5.59  |    29.2      |
| 2019 | AAAI  | STAR&dagger;           |**68.8** |  60.0   |  48.7   |  34.7   |  23.0   |    -    |    -    |      -       |
| 2019 | ICLR  | MAAN                   |  59.8   |  50.8   |  41.1   |  30.6   |  20.3   |  12.0   |   6.9   |    31.6      |
| 2019 | CVPR  | Liu et al.             |  57.4   |  50.8   |  41.2   |  32.1   |  23.1   |  15.0   |   7.0   |    32.4      |
| 2019 | ICIP  | Park et al.            |    -    |    -    |  40.2   |  32.2   |  21.7   |    -    |   9.2   |      -       |
| 2019 | ICIP  | ACN                    |    -    |    -    |  35.9   |  30.7   |  24.2   |  15.7   |   7.4   |      -       |
| 2019 | MM    | ASSG                   |  65.6   |  59.4   |  50.4   |  38.7   |  25.4   |  15.0   |   6.6   |    37.3      |
| 2019 | ICCV  | CleanNet               |    -    |    -    |  37.0   |  30.9   |  23.9   |  13.9   |   7.1   |      -       |
| 2019 | ICCV  | TSM	                  |    -    |    -    |  39.5   |    -    |  24.5   |    -    |   7.1   |      -       |
| 2019 | ICCV  | 3C-Net&dagger;         |  59.1   |  53.5   |  44.2   |  34.1   |  26.6   |    -    |   8.1   |      -       |
| 2019 | ICCV  | Nguyen et al.          |  60.4   |  56.0   |  46.6   |  37.5   |  26.8   |  17.6   |   9.0   |    36.3      |
| 2020 | AAAI  | PreTrimNet&Dagger;     |  57.5   |  50.7   |  41.4   |  32.1   |  23.1   |  14.2   |   7.7   |    32.4      |
| 2020 | AAAI  | BaS-Net                |  58.2   |  52.3   |  44.6   |  36.0   |  27.0   |  18.6   |  10.4   |    35.3      |
| 2020 | AAAI  | RPN                    |  62.3   |  57.0   |  48.2   |  37.2   |  27.9   |  16.7   |   8.1   |    36.8      |
| 2020 | WACV  | WSGN                   |  57.9   |  51.2   |  42.0   |  33.1   |  25.1   |  16.7   |   8.9   |    33.6      |
| 2020 | WACV  | Islam and Radke        |  62.3   |    -    |  46.8   |    -    |  29.6   |    -    |   9.7   |      -       |
| 2020 | WACV  | Action Graphs          |  63.7   |  56.9   |  47.3   |  36.4   |  26.1   |    -    |    -    |      -       |
| 2020 | CVPR  | ActionBytes            |    -    |    -    |  43.0   |  35.8   |  29.0   |    -    |   9.5   |      -       |
| 2020 | CVPR  | DGAM	                  |  60.0   |  54.2   |  46.8   |  38.2   |  28.8   |  19.8   |  11.4   |    37.0      |
| 2020 | CVPR  | Gong et al.            |    -    |    -    |  46.9   |  38.9   |  30.1   |  19.8   |  10.4   |      -       |
| 2020 | ECCV  | EM-MIL                 |  59.1   |  52.7   |  45.5   |  36.8   |  30.5   |  22.7   |**16.4** |    37.7      |
| 2020 | ECCV  | A2CL-PT                |  61.2   |  56.1   |  48.1   |  39.0   |  30.1   |  19.2   |  10.6   |    37.8      |
| 2020 | ECCV  | TSCN                   |  63.4   |  57.6   |  47.8   |  37.7   |  28.7   |  19.4   |  10.2   |    37.8      |
| 2020 | MM    | ACM-BANet              |  64.6   |  57.7   |  48.9   |  40.9   |  32.3   |  21.9   |  13.5   |    40.0      |
| 2021 | AAAI  | Lee et al.             |  67.5   |**61.2** |**52.3** |**43.4** |**33.7** |**22.9** |  12.1   |    41.9      |

## Contact & Feedback

If you have any suggestions for this repository, please feel free to contact me.

- [e-mail](mailto:lph1114@yonsei.ac.kr)
- [pull request](https://github.com/Pilhyeon/weakly-supervised-temporal-action-localization/pulls)
