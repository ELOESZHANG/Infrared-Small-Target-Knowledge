#Source

https://github.com/YimianDai/open-atac

Task

General CNN Backbone (Activation Function)

Type

Code / Model / Plug-in Module

Paper

Attention as Activation

Why it is useful
提出 ATAC（Attentional Activation），首次将**激活函数（Activation）与注意力机制（Attention）**统一起来。
作者认为：
ReLU 本质上也是一种门控（Gate）。
Attention 也是一种门控。
因此可以直接用 Attention 替代传统激活函数。
提出 Local Channel Attention：
不采用 SE 那样的全局平均池化；
而是在局部通道之间建立关系，学习更加细粒度的特征表达。
ATAC 可以直接替换：
ReLU
LeakyReLU
PReLU
Swish
Mish
网络几乎无需修改，只需替换 Activation Layer 即可获得性能提升。
Notes

ICPR 2020

主要创新：

Attention as Activation
Local Channel Attention
Activation 与 Attention 的统一设计

对我的启发：

可以考虑将普通 ReLU/GELU 替换为 ATAC 思想设计的注意力激活模块。
在红外小目标检测中，可增强目标区域响应，同时抑制背景噪声。
在遥感语义分割中，可用于 Decoder、Mamba Block 或 FFN 中，提高特征表达能力，而无需增加复杂的注意力模块。
