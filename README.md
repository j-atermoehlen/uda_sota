# Unsupervised Domain Adaptation for Semantic Segmentation - SOTA
## Overview
:construction: **This table is still under construction. The checkmarks indicating the employed approaches style transfer (ST), adversarial adaptation (AA) and self learning (SL) will be added in the near future. For now check the compiled PDF or the LaTeX source code.** :construction:
| Method       | Feature Extractor | ST  | AA  | SL | mIoU [%] | Code |
| ------------ | :---------------: | --- | --- | -- | -------: | :--: |
| FCN-ITW [[1]](https://arxiv.org/abs/1612.02649) | VGG-16            | :x: | ✔   | :x: | 27.1     | -    | 
| SIBAN [2]    | VGG-16            |  |  |  | 27.1     | -    | 
||||
DCAN [5]               | ResNet-101 |  ✔  | :o: | :x: | 38.5 | [✔](http://zxwu.azurewebsites.net/dcan.zip)
DLOW [13]              | ResNet-101 |  ✔  |  ✔  | :x: | 42.3 | [✔](https://github.com/ETHRuiGong/DLOW)
AdaptSegNet [14] 	     | ResNet-101 | :x: |  ✔  | :x: | 42.4 | [✔](https://github.com/wasidennis/AdaptSegNet)	
SIBAN [2]			         | ResNet-101 |  | | |  42.6 | - 
CyCADA [3]  		       | ResNet-101 | ✔ | ✔ | :x: |  42.7 | [✔](https://github.com/jhoffman/cycada_release)
CLAN [6]		           | ResNet-101 | | | | 43.2 | -
SWD [15]            | ResNet-101 | | | | 44.5 | [✔](https://github.com/apple/ml-cvpr2019-swd)
SSF-DAN [16]		   | ResNet-101 | | | | 45.4 | -
ADVENT [17]         | ResNet-101 | :x: | ✔ | :x: | 45.5 | [✔](https://github.com/valeoai/ADVENT)
IntraDA [18]        | ResNet-101 | | | | 46.3 | [✔](https://github.com/feipan664/IntraDA)
MSL [19]            | ResNet-101 | | | | 46.4 | [✔](https://github.com/ZJULearning/MaxSquareLoss)		
PANDA [20]		   | ResNet-101 | | | | 46.5 | -
DPR [7]			   | ResNet-101 | | | | 46.5 | -
SWLS [21]		   | ResNet-101 | | | | 47.2 | -
PyCDA [22]		   | ResNet-101 | | | | 47.4 | -
LSE+FL [23]	       | ResNet-101 | | | | 47.5 | -
BDL [24]           | ResNet-101 | ✔ | ✔ | ✔ | 48.5 | [✔](https://github.com/liyunsheng13/BDL)
CSCL [25]           | ResNet-101 | | | | 48.6 | -
CrCDA [26]          | ResNet-101 | | | | 48.6 | -
SISC-PWL [27]	   | ResNet-101 | | | | 49.0 | -
SIM [9]            | ResNet-101 | ✔ | ✔ | ✔ | 49.2 | [✔](https://github.com/SHI-Labs/Unsupervised-Domain-Adaptation-with-Differential-Treatment)
LDR [28]            | ResNet-101 | | | | 49.5 | -
CCM [29]            | ResNet-101 | :x: | :x: | ✔ | 49.9 | [✔](https://github.com/Solacex/CCM)
CAG-UDA [30]       | ResNet-101 | :x: | :x: | ✔ | 50.2 | [✔](https://github.com/RogerZhangzz/CAG_UDA)
LTIR [11]           | ResNet-101 | ✔ | ✔ | ✔ | 50.2 | [✔](https://github.com/MyeongJin-Kim/Learning-Texture-Invariant-Representation)
FDA-MBT [10]       | ResNet-101 | ✔ | :x: | ✔ | 50.5 | [✔](https://github.com/YanchaoYang/FDA)
CRST(MRKLD) + TPLD [31] | ResNet-101 | :x: | ✔ | ✔ | 51.2 | -
IAST [32]         | ResNet-101 | :x: | ✔ | ✔ | 51.5 | [✔](https://github.com/Raykoooo/IAST)
IAST-MST [32]          | ResNet-101 | :x: | ✔ | ✔ | 52.2 | [✔](https://github.com/Raykoooo/IAST)

## References
<sub> [[1]  J. Hoffman, D. Wang, F. Yu, and T. Darrell, **“FCNs in the Wild: Pixel-Level Adversarial and ConstraintBased Adaptation,”** arXiv, Dec. 2016.](https://arxiv.org/abs/1612.02649)  
[[2] Y. Luo, P. Liu, T. Guan, J. Yu, and Y. Yang, **“Significance-Aware Information Bottleneck for Domain Adaptive Semantic Segmentation,”** in Proc. of ICCV, (Seoul, Korea), pp. 6778–6787, Oct. 2019.](https://openaccess.thecvf.com/content_ICCV_2019/papers/Luo_Significance-Aware_Information_Bottleneck_for_Domain_Adaptive_Semantic_Segmentation_ICCV_2019_paper.pdf)  
[[3] J. Hoffman, E. Tzeng, T. Park, J.-Y. Zhu, P. Isola, K. Saenko, A. A. Efros, and T. Darrell, **“CyCADA: Cycle-Consistent Adversarial Domain Adaptation,”** in Proc. of ICML, (Stockholm, Sweden), pp. 1989– 1998, July 2018.](http://proceedings.mlr.press/v80/hoffman18a.html)  
[[4] Y. Zou, Z. Yu, B. V. K. Vijaya Kumar, and J. Wang, **“Unsupervised Domain Adaptation for Semantic Segmentation via Class-Balanced Self-Training,”** in Proc. of ECCV, (Munich, Germany), pp. 289–305, Sept. 2018.](http://www.ecva.net/papers/eccv_2018/papers_ECCV/html/Yang_Zou_Unsupervised_Domain_Adaptation_ECCV_2018_paper.php)    
[[5] Z. Wu, X. Han, Y.-L. Lin, M. G. Uzunbas, T. Goldstein, S. N. Lim, and L. S. Davis, **“DCAN: Dual Channel-Wise Alignment Networks for Unsupervised Scene Adaptation,”** in Proc. of ECCV, (Munich, Germany), pp. 535–552, Sept. 2018.](https://www.ecva.net/papers/eccv_2018/papers_ECCV/papers/Zuxuan_Wu_DCAN_Dual_Channel-wise_ECCV_2018_paper.pdf)    
[[6] Y. Luo, L. Zheng, T. Guan, J. Yu, and Y. Yang, **“Taking a Closer Look at Domain Shift: CategoryLevel Adversaries for Semantics Consistent Domain Adaptation,”** in Proc. of CVPR, (Long Beach, CA, USA), pp. 2507–2516, June 2019.](https://openaccess.thecvf.com/content_CVPR_2019/papers/Luo_Taking_a_Closer_Look_at_Domain_Shift_Category-Level_Adversaries_for_CVPR_2019_paper.pdf)  
[[7] Y.-H. Tsai, K. Sohn, S. Schulter, and M. Chandraker, **“Domain Adaptation for Structured Output via Discriminative Patch Representations,”** in Proc. of ICCV, (Seoul, Korea), pp. 1456–1465, Oct. 2019.](https://openaccess.thecvf.com/content_ICCV_2019/html/Tsai_Domain_Adaptation_for_Structured_Output_via_Discriminative_Patch_Representations_ICCV_2019_paper.html)    
[[8] S. Zhao, B. Li, X. Yue, Y. Gu, P. Xu, R. Hu, H. Chai, and K. Keutzer, **“Multi-Source Domain Adaptation for Semantic Segmentation,”** in Proc. of NeurIPS, (Vancouver, Canada), pp. 7285–7298, Dec. 2019.](https://papers.nips.cc/paper/8949-multi-source-domain-adaptation-for-semantic-segmentation)    
[[9] Z. Wang, M. Yu, Y. Wei, R. Feris, J. Xiong, W. mei Hwu, T. S. Huang, and H. Shi, **“Differential Treatment for Stuff and Things: A Simple Unsupervised Domain Adaptation Method for Semantic Segmentation,”** in Proc. of CVPR, (Seattle, WA, USA), pp. 12635–12644, June 2020.](https://openaccess.thecvf.com/content_CVPR_2020/html/Wang_Differential_Treatment_for_Stuff_and_Things_A_Simple_Unsupervised_Domain_CVPR_2020_paper.html)    
[[10] Y. Yang and S. Soatto, **“FDA: Fourier Domain Adaptation for Semantic Segmentation,”** in Proc. of CVPR, (Seattle, WA, USA), pp. 4085–4095, June 2020.](https://openaccess.thecvf.com/content_CVPR_2020/html/Yang_FDA_Fourier_Domain_Adaptation_for_Semantic_Segmentation_CVPR_2020_paper.html)    
[[11] M. Kim and H. Byun, **“Learning Texture Invariant Representationfor Domain Adaptation of Semantic Segmentation,”** in Proc. of CVPR, (Seattle, WA, USA), pp. 12975–12984, June 2020.](https://openaccess.thecvf.com/content_CVPR_2020/html/Kim_Learning_Texture_Invariant_Representation_for_Domain_Adaptation_of_Semantic_Segmentation_CVPR_2020_paper.html)  
[[12] J. Choi, T. Kim, and C. Kim, **“Self-Ensembling With GAN-based Data Augmentation for Domain Adaptation in Semantic Segmentation,”** in Proc. of ICCV, (Seoul, Korea), pp. 6830–6840, Oct. 2019.](https://openaccess.thecvf.com/content_ICCV_2019/html/Choi_Self-Ensembling_With_GAN-Based_Data_Augmentation_for_Domain_Adaptation_in_Semantic_ICCV_2019_paper.html)  
[[13] R. Gong, W. Li, Y. Chen, and L. V. Gool, **“DLOW: Domain Flow for Adaptation and Generalization,”** in Proc. of CVPR, (Long Beach, CA, USA), June 2019.](https://openaccess.thecvf.com/content_CVPR_2019/html/Gong_DLOW_Domain_Flow_for_Adaptation_and_Generalization_CVPR_2019_paper.html)  
[[14] Y.-H. Tsai, W.-C. Hung, S. Schulter, K. Sohn, M.- H. Yang, and M. Chandraker, **“Learning to Adapt Structured Output Space for Semantic Segmentation,”** in Proc. of CVPR, (Salt Lake City, UT, USA), pp. 7472–7481, June 2018.](https://openaccess.thecvf.com/content_cvpr_2018/html/Tsai_Learning_to_Adapt_CVPR_2018_paper.html)
[[15] C.-Y. Lee, T. Batra, M. H. Baig, and D. Ulbricht, **“Sliced Wasserstein Discrepancy for Unsupervised Domain Adaptation,”** in Proc. of CVPR, (Long Beach, CA, USA), June 2019.](https://openaccess.thecvf.com/content_CVPR_2019/html/Lee_Sliced_Wasserstein_Discrepancy_for_Unsupervised_Domain_Adaptation_CVPR_2019_paper.html)  
[[16] L. Du, J. Tan, H. Yang, J. Feng, X. Xue, Q. Zheng, X. Ye, and X. Zhang, **“SSF-DAN: Separated Semantic Feature Based Domain Adaptation Network for Semantic Segmentation,”** in Proc. of ICCV, (Seoul, Korea), pp. 982–991, Oct. 2019.](https://openaccess.thecvf.com/content_ICCV_2019/html/Du_SSF-DAN_Separated_Semantic_Feature_Based_Domain_Adaptation_Network_for_Semantic_ICCV_2019_paper.html)  
[[17] T.-H. Vu, H. Jain, M. Bucher, M. Cord, and P. Perez, **“ADVENT: Adversarial Entropy Minimization for Domain Adaptation in Semantic Segmentation,”** in Proc. of CVPR, (Long Beach, CA, USA), June 2019.](https://openaccess.thecvf.com/content_CVPR_2019/html/Vu_ADVENT_Adversarial_Entropy_Minimization_for_Domain_Adaptation_in_Semantic_Segmentation_CVPR_2019_paper.html)  
[[18] F. Pan, I. Shin, F. Rameau, S. Lee, and I. S. Kweon, **“Unsupervised Intra-Domain Adaptation for Semantic Segmentation Through Self-Supervision,”** in Proc. of CVPR, (Seattle, WA, USA), pp. 3764–3773, June 2020.](https://openaccess.thecvf.com/content_CVPR_2020/html/Pan_Unsupervised_Intra-Domain_Adaptation_for_Semantic_Segmentation_Through_Self-Supervision_CVPR_2020_paper.html)  
[[19] M. Chen, H. Xue, and D. Cai, **“Domain Adaptation for Semantic Segmentation With Maximum Squares Loss,”** in Proc. of ICCV, (Seoul, Korea), pp. 2090– 2099, Oct. 2019.](https://openaccess.thecvf.com/content_ICCV_2019/html/Chen_Domain_Adaptation_for_Semantic_Segmentation_With_Maximum_Squares_Loss_ICCV_2019_paper.html)  
[[20] D. Hu, J. Liang, Q. Hou, H. Yan, Y. Chen, S. Yan, and J. Feng, **“PANDA: Prototypical Unsupervised Domain Adaptation,”** arXiv, Mar. 2020.](https://arxiv.org/abs/2003.13274)  
[[21] J. Dong, Y. Cong, G. Sun, and D. Hou, **“Semantic Transferable Weakly-Supervised Endoscopic Lesions Segmentation,”** in Proc. of ICCV, (Seoul, Korea), pp. 10712–10721, Oct. 2019.](https://openaccess.thecvf.com/content_ICCV_2019/html/Dong_Semantic-Transferable_Weakly-Supervised_Endoscopic_Lesions_Segmentation_ICCV_2019_paper.html)  
[[22] Q. Lian, F. Lv, L. Duan, and B. Gong, **“Constructing Self-Motivated Pyramid Curriculums for Cross-Domain Semantic Segmentation: A Non-Adversarial Approach,”** in Proc. of ICCV, (Seoul, Korea), pp. 6758–6767, Oct. 2019.](https://openaccess.thecvf.com/content_ICCV_2019/html/Lian_Constructing_Self-Motivated_Pyramid_Curriculums_for_Cross-Domain_Semantic_Segmentation_A_Non-Adversarial_ICCV_2019_paper.html)  
[[23] M. N. Subhani and M. Ali, **“Learning from Scale Invariant Examples for Domain Adaptation in Semantic Segmentation,”** in Proc. of ECCV, (Glasgow, UK), pp. 1–17, Aug. 2020.](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/4042_ECCV_2020_paper.php)  
[[24] Y. Li, L. Yuan, and N. Vasconcelos, **“Bidirectional Learning for Domain Adaptation of Semantic Segmentation,”** in Proc. of CVPR, (Long Beach, CA, USA), pp. 6936–6945, June 2019.](https://openaccess.thecvf.com/content_CVPR_2019/html/Li_Bidirectional_Learning_for_Domain_Adaptation_of_Semantic_Segmentation_CVPR_2019_paper.html)  
[[25] J. Dong, Y. Cong, G. Sun, Y. Liu, and X. Xu, **“CSCL: Critical Semantic-Consistent Learning for Unsupervised Domain Adaptation,”** in Proc. of ECCV, (Glasgow, UK), pp. 1–17, Aug. 2020.](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/696_ECCV_2020_paper.php)  
[[26] J. Huang, S. Lu, D. Guan, and X. Zhang, **“Contextual-Relation Consistent Domain Adaptation for Semantic Segmentation,”** in Proc of ECCV, (Glasow, UK), pp. 1–18, Aug. 2020.](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/2442_ECCV_2020_paper.php)  
[[27] J. Iqbal and M. Ali, **“MLSL: Multi-Level SelfSupervised Learning for Domain Adaptation with Spatially Independent and Semantically Consistent Labeling,”** in Proc. of WACV, (Aspen, CO, USA), pp. 1864–1873, Mar. 2020.](https://arxiv.org/abs/1909.13776)  
[[28] J. Yang, W. An, S. Wang, X. Zhu, C. Yan, and J. Huang, **“Label-Driven Reconstruction for Domain Adaptation in Semantic Segmentation,”** in Proc. of ECCV, (Glasgow, UK), pp. 1–18, Aug. 2020.](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/5818_ECCV_2020_paper.php)  
[[29] G. Li, G. Kang, W. Liu, Y. Wei, and Y. Yang, **“Content-Consistent Matching for Domain Adaptive Semantic Segmentation,”** in Proc. of ECCV, (Glasgow, UK), pp. 1–18, Aug. 2020.](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/2178_ECCV_2020_paper.php)  
[[30] Q. Zhang, J. Zhang, W. Liu, and D. Tao, **“Category Anchor-Guided Unsupervised Domain Adaptation for Semantic Segmentation,”** in Proc. of NeurIPS, (Vancouver, Canada), pp. 433–443, Dec. 2019.](https://papers.nips.cc/paper/8335-category-anchor-guided-unsupervised-domain-adaptation-for-semantic-segmentation)  
[[31] I. Shin, S. Woo, F. Pan, and I. s. Kweon, **“Two-phase Pseudo Label Densification for Self-training based Domain Adaptation,”** in Proc. of ECCV, (Glasgow, UK), pp. 1–17, Aug. 2020.](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/1960_ECCV_2020_paper.php)  
[[32] K. Mei, C. Zhu, J. Zou, and S. Zhang, **“Instance Adaptive Self-Training for Unsupervised Domain Adaptation,”** in Proc. of ECCV, (Glasgow, UK), pp. 1–16, Aug. 2020.](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/5406_ECCV_2020_paper.php)  
[[33] P.-Y. Chen, A. H. Liu, Y.-C. Liu, and Y.-C. F. Wang, **“Towards Scene Understanding: Unsupervised Monocular Depth Estimation With SemanticAware Representation,”** in Proc. of CVPR, (Long Beach, CA, USA), pp. 2624–2632, June 2019.](https://openaccess.thecvf.com/content_CVPR_2019/html/Chen_Towards_Scene_Understanding_Unsupervised_Monocular_Depth_Estimation_With_Semantic-Aware_Representation_CVPR_2019_paper.html) 
</sub>
