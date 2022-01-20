# DORO: Distributional and Outlier Robust Optimization
**Runtian Zhai\*, Chen Dan\*, J. Zico Kolter, Pradeep Ravikumar**  
In ICML 2021  
Paper: [Link](http://proceedings.mlr.press/v139/zhai21a/zhai21a.pdf)


## Quick Start
To install the required packages, use
```shell
pip install -r requirements.txt
```


## Introduction
While DRO has been proved to be effective against subpopulation shift, its performance is significantly downgraded by the outliers existing in the dataset. DORO enhances the outlier-robustness of DRO by filtering out a small fraction of instances with high training loss that are potentially outliers. First we show that DRO is sensitive to outliers with some intriguing experimental results on COMPAS. Then we conduct large-scale experiments on COMPAS, CelebA and CivilComments-Wilds. Our strong theoretical and empirical results demonstrate the effectiveness of DORO.

### Run on CelebA
CelebA official website: http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html

We run the experiments on one NVIDIA GTX 1080ti. To reproduce the results in the paper, please use the following command with the hyperparameters listed in Appendix B.3 of our paper:
```shell
python celeba.py --data_root [ROOT] --alg [ALG] --alpha [ALPHA] --eps [EPSILON] --seed [SEED]
```
Please use `--download` to download the dataset if you are running for the first time.


