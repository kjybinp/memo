# Residual Attention Network for Image Classification
- Link: <https://arxiv.org/abs/1704.06904>
- 「Attention-based Multi-Context Guiding for Few-Shot Semantic Segmentation」で引用されていたので読んでいる。
- 日本語解説(<https://www.slideshare.net/DeepLearningJP2016/dl-residual-attention-network-for-image-classification>)
- Attentionはsequece dataの視点変化に使われてきたが、feed forwardの画像分類にも使える。
- Residual Attention Blockでは、Feature_inputからAttentionと次のFeature_truckを作り、Feature_input=(1+Feature_truck)*Attentionなので、Attentionは必ずしも対象物ではなく、無視してほしいものに注意を向けていることもある。
