# 用kdevelop 编译调试caffe
杨力 2017.2.22

## 1）安装
sudo apt install build-essential cmake 

sudo apt install kdevelop

## 2）安装
按照caffe官网说明 http://caffe.berkeleyvision.org/install_apt.html

sudo apt-get install libprotobuf-dev libleveldb-dev libsnappy-dev libopencv-dev libhdf5-serial-dev protobuf-compiler

sudo apt-get install --no-install-recommends libboost-all-dev

sudo apt install liblmdb-dev

## 3）建立工程

打开 kdevelop ，菜单， open import project，选中caffe根目录下的cmakelists.txt，旋转按提示操作，建立工程

## 4）点击按钮build，开始编译

有可能碰到错误: autoreconf: not found

因为没有安装automake 工具，sudo apt-get install autoconf automake libtool 即可，再点build

## 5）运行

编译成功后，菜单run，configure launches, 选择project target, 选一个可执行工程，选择executable，选一个可执行文件。

还可以填入arguments，work directory

## 6）调试

点击Execute 或debug，开始执行或调试。代码可以设置断点。

## 7）如何改变caffe编译选项

在工程名上右键，open configuration，选cmake，可以看到很多选项，特别提醒，CMAKE_BUILD_TYPE用来选择Release或Debug。

## 8）如何新建自己的可执行程序

在tools目录下新建自己的cpp源文件，代码都写在单个源文件里，cmake会自动为这个cpp文件生成可执行文件。

这是因为tools有个cmakelists.txt，里面自动为每一个cpp生成可执行文件。
