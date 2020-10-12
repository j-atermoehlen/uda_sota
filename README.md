# Unsupervised Domain Adapation for Semantic Segmentation - SOTA
## Overview
:construction: **This table is still under construction. The checkmarks indicating the employed approaches style transfer (ST), adversarial adaptaion (AA) and self learning (SL) will be added in the near future. For now check the compiled PDF or the LaTeX source code.** :construction:
| Method       | Feature Extractor | ST  | AA  | SL | mIoU [%] | Code |
| ------------ | :---------------: | --- | --- | -- | -------: | :--: |
| FCN-ITW [[1]](https://arxiv.org/abs/1612.02649) | VGG-16            | :x: | ✔   | :x: | 27.1     | -    | 
| SIBAN [2]    | VGG-16            |  |  |  | 27.1     | -    | 
||||
DCAN [5]               | ResNet-101 | | | | 38.5 | [✔](http://zxwu.azurewebsites.net/dcan.zip)
DLOW [13]       | ResNet-101 |  | | | 42.3 | [✔](https://github.com/ETHRuiGong/DLOW)
AdaptSegNet [14] 	   | ResNet-101 |  | | | 42.4 | [✔](https://github.com/wasidennis/AdaptSegNet)	
SIBAN [2]			   | ResNet-101 |  | | | 42.6 | - 
CyCADA [3]  		   | ResNet-101 | | | |  42.7 | [✔](https://github.com/jhoffman/cycada_release)
CLAN		   | ResNet-101 | | | | 43.2 | -
SWD            | ResNet-101 | | | | 44.5 | [✔](https://github.com/apple/ml-cvpr2019-swd)
SSF-DAN		   | ResNet-101 | | | | 45.4 | -
ADVENT         | ResNet-101 | | | | 45.5 | [✔](https://github.com/valeoai/ADVENT)
IntraDA        | ResNet-101 | | | | 46.3 | [✔](https://github.com/feipan664/IntraDA)
MSL            | ResNet-101 | | | | 46.4 | [✔](https://github.com/ZJULearning/MaxSquareLoss)		
PANDA		   | ResNet-101 | | | | 46.5 | -
DPR			   | ResNet-101 | | | | 46.5 | -
SWLS		   | ResNet-101 | | | | 47.2 | -
PyCDA		   | ResNet-101 | | | | 47.4 | -
LSE+FL	       | ResNet-101 | | | | 47.5 | -
BDL            | ResNet-101 | | | | 48.5 | [✔](https://github.com/liyunsheng13/BDL)
CSCL           | ResNet-101 | | | | 48.6 | -
CrCDA          | ResNet-101 | | | | 48.6 | -
SISC-PWL	   | ResNet-101 | | | | 49.0 | -
SIM            | ResNet-101 | | | | 49.2 | [✔](https://github.com/SHI-Labs/Unsupervised-Domain-Adaptation-with-Differential-Treatment)
LDR            | ResNet-101 | | | | 49.5 | -
CCM            | ResNet-101 | | | | 49.9 | [✔](https://github.com/Solacex/CCM)
CAG-UDA        | ResNet-101 | | | | 50.2 | [✔](https://github.com/luanyunteng/pytorch-be-your-own-teacher)
LTIR           | ResNet-101 | | | | 50.2 | [✔](https://github.com/MyeongJin-Kim/Learning-Texture-Invariant-Representation)
FDA-MBT        | ResNet-101 | | | | 50.5 | [✔](https://github.com/YanchaoYang/FDA)
CRST(MRKLD) + TPLD | ResNet-101 | | | | 51.2 | -
IAST         | ResNet-101 | | | | 51.5 | [✔](https://github.com/Raykoooo/IAST)
IAST-MST          | ResNet-101 | | | | 52.2 | [✔](https://github.com/Raykoooo/IAST)

## References
<sub>[[1]  J. Hoffman, D. Wang, F. Yu, and T. Darrell, **“FCNs in the Wild: Pixel-Level Adversarial and ConstraintBased Adaptation,”** arXiv, Dec. 2016.](https://arxiv.org/abs/1612.02649)  
[2] Y. Luo, P. Liu, T. Guan, J. Yu, and Y. Yang, **“Significance-Aware Information Bottleneck for Domain Adaptive Semantic Segmentation,”** in Proc. of ICCV, (Seoul, Korea), pp. 6778–6787, Oct. 2019.  
[3] J. Hoffman, E. Tzeng, T. Park, J.-Y. Zhu, P. Isola, K. Saenko, A. A. Efros, and T. Darrell, **“CyCADA: Cycle-Consistent Adversarial Domain Adaptation,”** in Proc. of ICML, (Stockholm, Sweden), pp. 1989– 1998, July 2018.
</sub>
