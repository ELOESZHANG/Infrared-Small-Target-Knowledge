# ALCNet

## Source
https://github.com/YimianDai/open-alcnet

## Task
Infrared small target detection

## Type
Code / Model /Single

## Paper
Attentional Local Contrast Networks for Infrared Small Target Detection

## Why it is useful
-不是在原图计算特征值的差值，而是计算特征图的差值，cnn可以学习哪些亮点是目标，哪些亮点是干扰，并把空洞值从单个变成多个
-使用平移相减而不是卷积的方法来提升flops
-直接拼接而不是平均，得到最好的局部对比响应
-BLAM（低层指导高层）

## Notes
2021 TGRS
