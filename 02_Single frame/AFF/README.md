AFF
Source

https://github.com/YimianDai/open-aff

Task

General Feature Fusion (Classification / Detection / Segmentation)

Type

Code / Model / Plug-in Module

Paper

Attentional Feature Fusion

Why it is useful
提出 AFF（Attentional Feature Fusion），一种通用的特征融合模块，可直接替代网络中的 Addition 或 Concatenation。
认为不同层、不同尺度的特征直接相加会产生语义不一致（Semantic Inconsistency），导致融合效果受限，因此引入注意力机制进行自适应融合。
提出 MS-CAM（Multi-Scale Channel Attention Module），同时利用局部信息和全局上下文计算融合权重，而不是仅依赖全局平均池化（SE模块）。
提出 iAFF（Iterative Attentional Feature Fusion），通过两阶段注意力融合缓解第一次融合带来的信息损失，使融合更加充分。
可直接应用于：
ResNet Shortcut
FPN
U-Net Skip Connection
Inception
Encoder-Decoder
即插即用，几乎不改变原始网络结构，广泛应用于分类、检测、分割和遥感等任务。
Notes

WACV 2021

主要创新：

AFF（Attentional Feature Fusion）
MS-CAM（Multi-Scale Channel Attention）
iAFF（Iterative Attentional Feature Fusion）

对我的启发：

SegMAN Decoder 的多尺度融合可以直接借鉴 AFF。
频域特征（High Frequency）与空间特征（Spatial Feature）融合时，也可以采用 AFF，而不是直接 concat 或 add。
在遥感语义分割中，AFF 特别适合融合浅层边界信息与深层语义信息。
