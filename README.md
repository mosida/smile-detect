# smile-detect
> 基于 Android OpenCV 实现实时的简单人脸、笑脸识别 Demo APP

> 例子使用了 OpenCV 自带的训练级联分类器的文件，进行人脸检测，然后进行微笑检测。

演示效果
> 摄像头实时检测多张人脸并且识别是否微笑
<p align="center">
  <img src="https://github.com/mosida/smile-detect/blob/main/res/demo.jpg">
</p>

### 项目研究背景和历史实现原理
2011 年时期跟广州农商银行进行了项目合作，开发了一款笑脸识别 APP。
当时实现方案：
1. 基于 OpenCV 进行实现，先实现人脸检测方案，并且对图片进行裁切。
2. 收集大量人脸图片，人工对笑脸打分，这些作为训练集，使用这个训练集训练神经网络模型，让模型中的参数拟合训练集的输入输出。
3. 训练好的模型可以对其它不在训练集的人脸进行打分。

<p align="center">
  <img src="https://github.com/mosida/smile-detect/blob/main/res/app-1.jpg">
  <img src="https://github.com/mosida/smile-detect/blob/main/res/app-2.jpg">
  <img src="https://github.com/mosida/smile-detect/blob/main/res/app-3.jpg">
</p>

### 参考资料
- [神经网络入门](https://www.ruanyifeng.com/blog/2017/07/neural-network.html)
- [OpenCV中支持的人脸检测方法整理与汇总](https://cloud.tencent.com/developer/article/1690500)
