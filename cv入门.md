
计算机视觉（computer vision）的目的是让机器拥有视觉功能。人的视觉功能非常强大，比如判别一个物体“是什么”和“在哪里”，前者是目标检测与识别，用到机器学习的知识，后者是视觉测量和定位，涉及摄像机几何知识。

计算机视觉入门需要的基础知识包括：编程（C++和python）、数学（线性代数和概率论）、计算机视觉基础。

# 1. C++，python编程

## C++编程基础（必学）

了解：C++标准库 STL

会用：C++运算符重载、迭代器、智能指针

熟练使用：vector，引用&，类模版，函数模版，c++多线程编程

自己到图书馆找包含上述内容的教材，或者直接看 C++ Primer（中文版 第5版）

## python编程基础

可以边用边学，需要用到什么学什么。

如果想系统学习，廖雪峰的教程还不错  http://www.liaoxuefeng.com 

## 编程环境和开发工具

算法一般是平台无关，Windows和Linux环境二选一即可，但涉及到具体项目，两个平台都有可能涉及。

经常会用到开源项目，因此上github 和cmake的简单使用必不可少。

windows下git或github的用法见 https://github.com/micvlab/doc ，github使用说明.txt

Windows下建议采用win7/10 64位，visual studio是最好用的IDE，建议使用，vs2013、2015、2017均可。

Linux建议采用Ubuntu Desktop for developers 14或16，https://www.ubuntu.com/desktop/developers

可在windows下安装ubuntu虚拟机，vmware和virtualbox都很好用，后者免费，推荐。

Python开发环境搭建：

windows下建议安装anaconda，然后装pycharm，在pycharm下编程，详见https://github.com/micvlab/doc/tree/master/yangli/python-windows.md  

linux下python开发非常友好，先装anaconda或原版python，然后装pycharm。

如果没有明确要求，python2.7就够了，你也可以2.7和3.x版本都装，不同版本可以共存。

# 2. 数学基础

需要用到的数学基础如下，这也是人工智能领域入门最基本的数学知识。先不用专门去学。

## 线性代数、概率论

大一就学了，这应该不成问题。

## 最优化

最优化方法常用到，特别是梯度下降法和非线性最小二乘，只要会微积分求导就没问题。

# 3. 计算机视觉

## SLAM相关

《视觉SLAM十四讲》高博。这是一本新书，有电子版，有配套代码，强烈推荐，重点学1~9讲及附录，其中第4讲李群比较理论化，可以先不必深究。（必学）

建议调试和阅读 ORB_SLAM2这个开源项目代码，此算法效果好，适合入门。https://github.com/raulmur/ORB_SLAM2 
推荐它的一个国内详细注释的版本 https://git.oschina.net/paopaoslam/ORB-SLAM2  （必学）

slam中有一个基础性工作——摄像机标定，opencv的标定模型和程序用的比较多，《学习opencv》这本书里有讲，虽然这本书有点老，里面的代码是旧版本的接口，但第11章摄像机模型与标定值得看。opencv源码的sample目录下有calibration的例子。

Multiple View Geometry in Computer Vision 2ed - Hartley 这是经典之作，但暂不要求通读。

《计算机视觉中的数学方法》与上述英文书内容相似，可以参考，重点阅读摄像机几何、两视点几何这两章。（必学）

注：1）微信公众号，泡泡机器人，建议关注。2）资源列表 https://github.com/OpenSLAM/awesome-SLAM-list 

## opencv（必学）

从官网下载opencv最新版，要求windows和linux两个平台都会编译。

利用opencv实现至少10个小例子，每个例子实现一个小功能，至少应包括：图像缩放、边缘检测、人脸检测、目标跟踪、特征点匹配、摄像机标定。

windows平台的opencv的基本用法可参考“opencv入门教程.pdf”（于仕琪），用的是vs2010，但vs2013以上版本用法基本一样。

opencv有C和C++两套接口，前者是旧的接口，建议不要使用。如何分辨新旧接口？以小写cv开头的函数都是旧接口。

这里有我收集的一些小例子供参考 http://git.oschina.net/walkup/opencvexample

opencv官方源码的sample目录下有非常丰富的例子。

这几本书可以参考：OpenCV3编程入门_毛星云，Mastering OpenCV with Practical Computer Vision，OpenCV for Secret Agents

这些书上自带的例子也很不错。

# 4. 机器学习（以下内容3选1必学）

推荐的优秀教材和视频：

1. 统计学习方法，李航。这是一本机器学习的国内经典之作。

2. 机器学习，周志华。这是继统计学习方法之后的又一本经典之作。建议阅读1~10章。

3. Andrew NG机器学习课程。注意！是coursera上的machine learning课程，不是网易公开课的。 可在coursera上直接观看或下载学习，有中英文字幕。


# 5. 深度学习

参考 https://github.com/micvlab/doc/tree/master/practice  入门学习任务表
 

