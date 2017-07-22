# 1 C++，python编程

## 1.1 编程基础

了解：C++标准库 STL

会用：C++运算符重载、迭代器、智能指针

熟练使用：vector，引用&，类模版，函数模版，c++多线程编程

自己到图书馆找包含上述内容的教材，或者直接看 C++ Primer（中文版 第5版）

python编程：根据项目需要，现学现用，廖雪峰的教程还不错  http://www.liaoxuefeng.com 

附编程环境和开发工具：

做深度学习，你需要有一台配置较好的电脑：台式机i5（笔记本最好i7）处理器，NVidia独立显卡2G以上显存。

Windows下建议采用win7/10 64位，visual studio 2013及以上版本，2015、2017均可

Linux建议采用Ubuntu Desktop for developers 14或16，https://www.ubuntu.com/desktop/developers

可在windows下安装ubuntu虚拟机，vmware和virtualbox都很好用，后者免费，推荐。但注意虚拟机是跑不了GPU的。

Python开发环境搭建：windows下建议安装anaconda，然后装pycharm，在pycharm下编程，详见python-windows.md；

linux下python开发非常友好，先装anaconda或原版python，然后也可以用pycharm。


## 1.2 caffe的安装（难度低）
要求完成caffe的安装，Windows或linux平台二选一，两个平台都会用则更好。

如果有nvidia独立显卡，可以尝试GPU版本，如果没有，则编译CPU版本。

参考caffe官网 http://caffe.berkeleyvision.org/

caffe中文 http://caffecn.cn/  其中有个caffe官方教程中译本

参考文章有很多，例如 http://blog.csdn.net/ubunfans/article/details/47724341

Caffe windows版本  https://github.com/BVLC/caffe/tree/windows

参考 windows下编译调试caffe.md

## 1.3 caffe训练和预测实例（难度低）
要求完成caffe的训练实例。用我们自己转换后的手写字符数据集一部分进行训练，剩余进行测试。

建议采用cpu版本的caffe即可。

完成：生成图像列表、转换为lmdb、训练、绘制loss和accuracy曲线、网络结构可视化、编写测试程序。其中编写测试程序要求python和C++两个版本。

参考 caffe训练步骤.md

## 1.4 caffe官方实例代码理解和运行（难度中）
caffe官网 http://caffe.berkeleyvision.org/

Examples 部分有以下例子：

ImageNet tutorial 要求看懂 

LeNet MNIST Tutorial 要求看懂并运行结果正确

CIFAR-10 tutorial 要求看懂

Fine-tuning for style recognition 要求看懂

Fine-tune the ImageNet-trained CaffeNet on the "Flickr Style" dataset. 要求看懂

Feature extraction with Caffe C++ code.  要求看懂代码extract_features.cpp，运行结果正确，代码添加详细注释

CaffeNet C++ Classification example 要求看懂代码classification.cpp并运行结果正确，代码添加详细注释

以上涉及c++源码，都要求会单步调试。
以上Windows或linux平台，至少完成一个

## 1.5 caffe python实例代码理解和运行（难度低）

找两个python调用caffe的实例，调试成功并运行结果正确，要求会单步调试python代码

以上Windows或linux平台，至少完成一个

## 1.6 caffe代码理解（难度中）
找不少于2000行尽可能连贯的caffe内核代码，添加详细注释。

# 2 机器学习

## 2.1 周志华《机器学习》1~10章（难度低）

## 2.2 Andrew NG机器学习课程（难度低）

注意是coursera上的machine learning课程，不是网易公开课的。

可在coursera上直接观看或下载学习，有中英文字幕。也有下载好的视频。

## 2.3 深度学习 [deep learning] Ian Goodfellow， Yoshua Bengio等著

有免费英文版和中文版翻译，国内有出版，初学者无人指导可能有一定难度。

## 2.4 斯坦福CS231n—深度学习与计算机视觉
适合入门：
https://cs231n.github.io/

http://study.163.com/course/introduction/1003223001.htm

# 3 计算机视觉
## 3.1 opencv的编译（难度低）
从官网下载opencv最新版，要求完成windows和linux两个平台都会编译。

## 3.2 opencv使用（难度低）
利用opencv实现10个小例子，每个例子实现一个小功能，

至少应包括：图像缩放、边缘检测、人脸检测、行人检测、目标跟踪、特征点匹配。

windows或linux两个平台都必须掌握。

windows平台的opencv的基本用法可参考“opencv入门教程”（于仕琪），用的是vs2010，但vs2013以上版本用法基本一样。

opencv有C和C++两套接口，前者是旧的接口，建议不要使用。如何分辨新旧接口？以小写cv开头的函数都是旧接口。

这几本书可以参考：OpenCV3编程入门_毛星云，Mastering OpenCV with Practical Computer Vision，OpenCV for Secret Agents

电子版我已上传到qq群，这些书上自带的例子也很不错。





