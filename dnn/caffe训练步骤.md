以下是用caffe做图像分类训练的步骤，
典型的问题是，根据输入图像，将图像分为N类（例如N个目标人，或N种物体）

杨力 2016.1.7

## 1. 准备图像
典型的情况是，图像根目录下有N个子目录，每个子目录下为某一类别的很多幅图像。

## 2. 生成图像列表txt文件
图像列表文件格式为：每行一个图像文件名，空格，类别ID
应准备两个列表，train.txt和val.txt，分别为训练集和验证集。
注：图像文件名采用相对路径，即相对于图像根目录的路径。
可以自己用c++/python/matlab写一个生成列表的脚本，
listfile目录下提供了一个脚本，具体用法见注释。


## 3. 转换图像 
可以直接用列表文件训练，但最好先转换。
转换脚本为：examples/imagenet/create_imagenet.sh
linux下可直接用，windows下可稍加修改为.bat文件。
注：此处应指明图像根目录的绝对路径。

## 4. 计算图像均值
此步骤可选，理论上可提高训练准确率。
脚本为 ./examples/imagenet/make_imagenet_mean.sh

## 5. 开始训练
linux下脚本为./build/tools/caffe train --solver=models/bvlc_reference_caffenet/solver.prototxt
一般应分为两个阶段，用不同的learning rate进行训练。
solver.prototxt中应指定具体的网络结构的另一个 prototxt文件。

## 6. 训练结束
如何判断训练结束？一般training loss 不再下降，test accuracy 不再升高，即可结束，或进入更小learning rate的新一轮训练。
如果training loss比 test loss小很多，说明已经overfit。

以上步骤，可进一步参考：
http://caffe.berkeleyvision.org/gathered/examples/imagenet.html



