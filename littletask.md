# 一、视觉几何和图像相关

## task 1 标定你自己的相机
任务描述：用你的手机，摄像模式，对着标定板拍摄，要求从不同角度去拍摄完整的标定板。或者拿你的usb摄像头或笔记本自带摄像头，写一个opencv程序采集一组图像。然后用标定程序标定摄像头参数。

素材：在opencv的目录下搜索pattern，搜索到一副黑白棋盘格图像，名字大概是pattern.png，图像分辨率非常大，把它在显示器上打开，用摄像头对着它拍摄。这幅棋盘格的规格是9x6，指的是它的内角点个数，水平9个，垂直6个。如果拍摄的是视频，你需要把视频里的图像截取出来，10张左右就ok。

标定代码参考opencv samples目录下的calibration.cpp，程序需要输入标定板图像列表，以及标定板的规格9x6.

## task 2 图像旋转
任务描述：写一个小程序，功能是输入一张图像，把它旋转任意指定的角度，输出。

## task 3 场景识别
任务描述：实现《视觉SLAM十四讲》中讲到的DBOW3 的例子，并在实际场景中展示效果。要求掌握算法原理。

## task 4 orbslam 真实场景演示
实现此任务，你需要先标定你自己的相机，把标定结果填到yaml文件里，https://git.oschina.net/paopaoslam/ORB-SLAM2 里面有yaml文件的例子。

你还需要一个字典文件，在 https://github.com/raulmur/ORB_SLAM2  的 Vocabulary目录下。

然后你就可以在手机上运行orbslam的app看到效果了，apk文件在这里 https://github.com/FangGet/ORB_SLAM2_Android

## task 5 orbslam 调试和源码阅读
todo

## task 6 编译opencv及opencv_contrib
任务描述：在windows或linux下编译opencv及opencv_contrib

素材：到opencv官网下载最新版 opencv.org ， opencv_contrib 到这里下载： https://github.com/opencv/opencv_contrib
opencv_contrib 是最新的尚未加入正式版的算法。

编译需要用到cmake。网上有不少参考文章。

# 二、机器学习相关

## task 1 背景建模
任务描述：输入一段监控视频（即摄像机固定不动），将背景和前景分割开来。跑通程序功能，评估各种算法效果和性能，并搞懂算法原理。

素材：https://git.oschina.net/walkup/opencvexample 我整理的这个opencv例子下面，motion 是一个前景分割的例子，包含两种算法，均来自opencv的官方例子。可以直接跑。

另外Opencv_contrib 里有个模块，bgsegm: Background segmentation algorithm combining statistical background image estimation and per-pixel Bayesian segmentation. 其中也包含背景建模的很多种新方法的实现。

## task 2 目标检测

实现一个目标检测的例子，用来在视频中检测某一特定目标，例如人脸、行人、车辆等。具体实现方式及参考资源询问老师。

## task 3 手写字符识别
todo
