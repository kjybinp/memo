# Attention-based Multi-Context Guiding for Few-Shot Semantic Segmentation(AAAI2019)
Link:<http://taohu.me/note/few-shot-seg.pdf>
## Abstract
- anotation dataが少ない場合でも、うまくSematntic Segmentationしたい。
- Attention- based Multi-Context Guiding (A-MCG) networkを提案。
- support, quecy, and feature fusionの３つのbranchで構成されている（branch?/）。
- ポイントは、support and query branchからのマルチスケールのcontext feature..?であり、
これがsupport set(参考にする画像？)によるガイドを効率的にしている。
- several scaleのattentionがone shotに効果的？
- 精度はあがった？

## Introduction
- few-shot learningは、image classficationでは活発だけど、semantic segmentationでは、まだ少ない。
- 従来法ってのは、図１上で示されるような、query branchとsupport branchで構成されたもの。
- support branchは、discriminative support feature、query branchは、feature extractorらしい。
- p1最後にはなにやら課題が書いているが、正直従来法がよくわからないので、よくわらない...

## Our Method
### Probrem Formulation
- PASCALのクラスごとにtrain,testに分類。test時にはtrainにないクラスの領域が登場する。
### Atention Mechanism Review
- Residual Attention Moduleとは？（[Residual Attention Network for Image Classification(Wang 2017)](https://arxiv.org/abs/1704.06904)）→(1+Attention)*Featureってな感じで、強調する場所を考える機構がある。
### Attention-based MCG
- Fig2の"+"の部分がよくわからない。ネットワーク芸なので、結果をみて考える。
### Convolutional LSTM for k-shot learning
- k-shot learningに拡張しようとした時に、従来法(OSLSM)では、Logical OR operationでいけていないと作者は思っている。
- LSTMの隠れ層に知見を貯めこんでいくイメージ？
## Experimental Result
### Traing detail
### Dataset and Metric
- DatasetはPASCAL、クラスを４つに分けて、３つで訓練、残りで検証（つまり、４回）。
- metricはmIOU。
### Ablation Study
