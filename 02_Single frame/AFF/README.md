# AFF

## Source
https://github.com/YimianDai/open-aff

## Task
Infrared small target detection

## Type
Code / Model /Single

## Paper

Attentional Feature Fusion

## Why it is useful
提出 AFF（Attentional Feature Fusion），一种通用的特征融合模块，可直接替代网络中的 Addition 或 Concatenation。
认为不同层、不同尺度的特征直接相加会产生语义不一致（Semantic Inconsistency），导致融合效果受限，因此引入注意力机制进行自适应融合。
提出 MS-CAM（Multi-Scale Channel Attention Module），同时利用局部信息和全局上下文计算融合权重，而不是仅依赖全局平均池化（SE模块）。
提出 iAFF（Iterative Attentional Feature Fusion），通过两阶段注意力融合缓解第一次融合带来的信息损失，使融合更加充分。

## Notes
WACV 2021
