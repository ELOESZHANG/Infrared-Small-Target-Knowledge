# ATAC

## Source
https://github.com/YimianDai/open-atac

## Task
Infrared small target detection

## Type
Code / Model /Single

## Paper

Attention as Activation

## Why it is useful
提出 ATAC（Attentional Activation），首次将**激活函数（Activation）与注意力机制（Attention）**统一起来。
ReLU 本质上也是一种门控（Gate）,Attention 也是一种门控。可以直接用 Attention 替代传统激活函数。
提出 Local Channel Attention：不采用 SE 那样的全局平均池化；而是在局部通道之间建立关系，学习更加细粒度的特征表达。
网络几乎无需修改，只需替换 Activation Layer 即可获得性能提升。

## Notes
ICPR 2021

