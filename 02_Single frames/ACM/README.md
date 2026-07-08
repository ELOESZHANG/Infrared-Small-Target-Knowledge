# ACM

## Source
https://github.com/YimianDai/open-acm


## Type
Code / Model /Single  

## Paper
Asymmetric Contextual Modulation for Infrared Small Target Detection

## Why it is useful
- 一个像素级通道注意力调制
- 建立了一个数据集

## Notes
1.小目标的定义：在一张256*256的图像中小于80个像素的目标
2.小目标的核心难题：分辨率和语义之间的矛盾：既需要对整个红外图像具有高层次的语义理解，又需要一张高分辨率的预测图。既要全局又要局部
  神经网络通过逐步减小特征尺寸来学习语义表示，减小到一定程度小目标就没了。
3.针对上述问题需要重新调整网络:调整下采样方案，调整注意力模块，调整融合方法
