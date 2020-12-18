# VBF-qq2Hqq-uncertainties
[![DOI](https://zenodo.org/badge/187642785.svg)](https://zenodo.org/badge/latestdoi/187642785)


This is a simple tool to estimate VBF uncertainties in STXS stage 1.1 bins.
The details of the calculation can be found [here](https://indico.cern.ch/event/796065/contributions/3307675/attachments/1799797/2935242/VBF-STSX-HXSWG-WG1-FEB.pdf).

## How to run:
```bash
g++ -std=c++11 -o tool qq2Hqq_uncert_scheme.cpp
./tool
```

This should print the impact of VBF uncertainties in different STXS bins:

```
 ========================================================
 === relative uncertainties [%]
 BIN: Yield    | PTH200   | Mjj60    | Mjj120   | Mjj350   | Mjj700   | Mjj1000  | Mjj1500  | PTH25    | JET01    | TOT
 200:  0.37988 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |  0.37988
 201:  0.38007 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |  -1.0252 |   1.0934
 202:   0.3799 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |   -1.025 |   1.0931
 203:  0.37893 |        0 |  -17.771 |        0 |        0 |        0 |        0 |        0 |  -3.1532 |  0.89229 |   18.075
 204:  0.38116 |        0 |  0.49356 |  -7.2424 |        0 |        0 |        0 |        0 |  -3.1526 |  0.89211 |   7.9735
 205:  0.37966 |        0 |  0.49421 |  0.36041 |  -1.5481 |        0 |        0 |        0 |  -3.1534 |  0.89063 |   3.6949
 206:  0.37982 | 0.031298 |  0.49415 |  0.36071 |  0.51503 | -0.68464 |        0 |        0 |  -3.1535 |  0.89125 |    3.463
 207:  0.38051 | 0.031285 |  0.49368 |  0.36107 |  0.51491 |  0.43442 |  -1.0058 |        0 |  -3.1537 |  0.88993 |   3.5669
 208:  0.38001 | 0.031315 |  0.49358 |  0.36094 |   0.5145 |  0.43456 |  0.48332 | -0.42639 |  -3.1534 |  0.89123 |   3.4823
 209:   0.3792 | 0.031296 |  0.49323 |  0.36111 |  0.51432 |  0.43474 |  0.48317 |   0.3657 |  -3.1548 |  0.89224 |   3.4768
 210:  0.37972 |  -0.2573 |  0.49377 |  0.36034 |  0.51378 |  0.43445 |  0.48353 |   0.3659 |  -3.1565 |  0.88803 |   3.4866
 211:  0.38072 | -0.25729 |  0.49216 |  0.35852 |  0.51239 |  0.43462 |  0.48344 |  0.36594 |  -3.1485 |  0.89775 |   3.4813
 212:  0.37471 | -0.25731 |  0.49208 |   0.3623 |  0.51779 |  0.43502 |  0.48301 |  0.36579 |  -3.1545 |  0.88525 |   3.4841
 213:  0.37638 |  -0.2574 |  0.49428 |  0.36279 |  0.51679 |   0.4332 |  0.48233 |   0.3661 |  -3.1479 |   0.8907 |   3.4796
 214:   0.3788 |        0 |  -17.768 |        0 |        0 |        0 |        0 |        0 |   6.0414 |  0.89322 |   18.792
 215:  0.37998 |        0 |  0.49386 |  -7.2419 |        0 |        0 |        0 |        0 |   4.6332 |  0.89154 |   8.6658
 216:  0.38002 |        0 |  0.49404 | 0.036051 |   -1.548 |        0 |        0 |        0 |   1.9251 |  0.89092 |   2.6992
 217:  0.37981 |  0.03129 |  0.49397 |  0.36056 |  0.51518 | -0.68473 |        0 |        0 |   1.2005 |   0.8907 |   1.8676
 218:  0.37956 | 0.031294 |    0.494 |  0.36069 |  0.51525 |  0.43445 |  -1.0058 |        0 |   1.0361 |  0.89089 |   1.9627
 219:  0.37962 | 0.031285 |  0.49425 |  0.36045 |  0.51501 |  0.43454 |  0.48311 | -0.42638 |  0.92811 |  0.89125 |   1.7448
 220:  0.37994 | 0.031277 |  0.49376 |  0.36068 |  0.51522 |  0.43451 |  0.48315 |  0.36578 |  0.69146 |   0.8911 |   1.6164
 221:  0.38063 | -0.25741 |  0.49523 |  0.36045 |    0.514 |  0.43376 |  0.48277 |  0.36594 |   2.9883 |  0.89218 |   3.3364
 222:  0.38361 |  -0.2574 |  0.49306 |  0.36148 |  0.51529 |  0.43424 |  0.48372 |  0.36581 |   2.1599 |  0.89402 |   2.6218
 223:  0.37768 | -0.25738 |  0.49598 |  0.36028 |   0.5149 |  0.43487 |  0.48347 |  0.36564 |   1.9304 |  0.89469 |   2.4359
 224:  0.38151 | -0.25738 |  0.49483 |  0.36128 |  0.51403 |  0.43419 |  0.48306 |  0.36583 |   1.4181 |  0.88851 |   2.0512
 ========================================================
 ========================================================
 === absolute uncertainties [fb]
 BIN: Yield    | PTH200   | Mjj60    | Mjj120   | Mjj350   | Mjj700   | Mjj1000  | Mjj1500  | PTH25    | JET01    | TOT
 200:    1.041 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |    1.041
 201:    1.106 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |   -2.984 |    3.182
 202:    5.006 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |        0 |   -13.51 |     14.4
 203:   0.1368 |        0 |   -6.415 |        0 |        0 |        0 |        0 |        0 |   -1.138 |   0.3221 |    6.524
 204:   0.2126 |        0 |   0.2753 |    -4.04 |        0 |        0 |        0 |        0 |   -1.758 |   0.4976 |    4.447
 205:   0.6764 |        0 |   0.8805 |   0.6421 |   -2.758 |        0 |        0 |        0 |   -5.618 |    1.587 |    6.583
 206:   0.5575 |  0.04594 |   0.7253 |   0.5295 |    0.756 |   -1.005 |        0 |        0 |   -4.629 |    1.308 |    5.083
 207:   0.2468 |  0.02029 |   0.3202 |   0.2342 |    0.334 |   0.2818 |  -0.6524 |        0 |   -2.045 |   0.5772 |    2.313
 208:   0.2037 |  0.01678 |   0.2646 |   0.1935 |   0.2758 |   0.2329 |   0.2591 |  -0.2285 |    -1.69 |   0.4777 |    1.866
 209:   0.1561 |  0.01288 |    0.203 |   0.1487 |   0.2117 |    0.179 |   0.1989 |   0.1505 |   -1.299 |   0.3673 |    1.431
 210:  0.07582 | -0.05138 |   0.0986 |  0.07195 |   0.1026 |  0.08675 |  0.09655 |  0.07306 |  -0.6303 |   0.1773 |   0.6962
 211:  0.04757 | -0.03215 |   0.0615 |   0.0448 |  0.06403 |  0.05431 |  0.06041 |  0.04573 |  -0.3934 |   0.1122 |    0.435
 212:  0.05055 | -0.03471 |  0.06638 |  0.04887 |  0.06985 |  0.05868 |  0.06516 |  0.04935 |  -0.4255 |   0.1194 |     0.47
 213:  0.05352 |  -0.0366 |  0.07029 |  0.05159 |  0.07349 |   0.0616 |  0.06859 |  0.05206 |  -0.4476 |   0.1267 |   0.4948
 214:  0.07136 |        0 |   -3.347 |        0 |        0 |        0 |        0 |        0 |    1.138 |   0.1683 |     3.54
 215:   0.1442 |        0 |   0.1874 |   -2.748 |        0 |        0 |        0 |        0 |    1.758 |   0.3384 |    3.289
 216:    1.109 |        0 |    1.442 |   0.1052 |   -4.518 |        0 |        0 |        0 |    5.618 |      2.6 |    7.878
 217:    1.464 |   0.1206 |    1.905 |     1.39 |    1.986 |    -2.64 |        0 |        0 |    4.629 |    3.434 |    7.201
 218:   0.7493 |  0.06178 |   0.9752 |   0.7121 |    1.017 |   0.8577 |   -1.986 |        0 |    2.045 |    1.759 |    3.875
 219:   0.6913 |  0.05697 |   0.9001 |   0.6564 |   0.9379 |   0.7913 |   0.8798 |  -0.7765 |     1.69 |    1.623 |    3.177
 220:   0.7136 |  0.05875 |   0.9274 |   0.6774 |   0.9677 |   0.8161 |   0.9075 |    0.687 |    1.299 |    1.674 |    3.036
 221:  0.08028 | -0.05429 |   0.1045 |  0.07603 |   0.1084 |  0.09149 |   0.1018 |  0.07718 |   0.6303 |   0.1882 |   0.7037
 222:  0.06987 | -0.04689 |  0.08981 |  0.06584 |  0.09386 |   0.0791 |  0.08811 |  0.06663 |   0.3934 |   0.1628 |   0.4776
 223:  0.08326 | -0.05674 |   0.1093 |  0.07942 |   0.1135 |  0.09586 |   0.1066 |   0.0806 |   0.4255 |   0.1972 |    0.537
 224:   0.1204 | -0.08124 |   0.1562 |    0.114 |   0.1623 |   0.1371 |   0.1525 |   0.1155 |   0.4476 |   0.2805 |   0.6475
 ========================================================

```
