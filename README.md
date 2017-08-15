# 一些有趣的项目
收集的一些有趣的项目

概述
---
项目名称: FlappyBird（深度强化学习 DQN ）

项目地址: https://github.com/yenchenlin/DeepLearningFlappyBird

项目依赖: Python、TensorFlow、PyGame、OpenCV2

屏幕截图: 

![image](images/FlappyBird.gif)


项目名称: MarI/O（神经网络+遗传算法 NEATEvolve ）

源码地址: http://pastebin.com/ZZmSNaHX

项目依赖: [BizHawk模拟器] https://github.com/TASVideos/BizHawk
          [Lua API] http://tasvideos.org/Bizhawk/LuaFunctions.html
屏幕截图: 

![image](images/Mario.gif)


项目名称: FaceRank（卷积神经网络 CNN ）

项目地址: https://github.com/fendouai/FaceRank

项目依赖: Python、TensorFlow、OpenCV2

屏幕截图:

![image](images/FaceRank.png)


项目名称: 图片生成（深度感知生成对抗网络 DCGAN ）

项目地址: 

项目依赖: 

屏幕截图: 

![image](images/FaceRank.png)

项目实现: 

1. 数据采集     http://konachan.net/

2. 头像截取     https://github.com/nagadomi/lbpcascade_animeface

3. 模型训练     https://github.com/carpedm20/DCGAN-tensorflow

`
if config.dataset == 'mnist':
            data_X, data_y = self.load_mnist()
        else:
            data = glob(os.path.join("./data", config.dataset, "*.jpg"))
`

在data文件夹中再新建一个anime文件夹，把图片直接放到这个文件夹里，运行时指定--dataset anime

//python main.py --image_size 96 --output_size 48 --dataset anime --is_crop True --is_train True --epoch 300 --input_fname_pattern "*.jpg"

python main.py --input_height 96 --input_width 96 --output_height 48 --output_width 48 --dataset anime --crop --train --epoch 300 --input_fname_pattern "*.jpg"

参考:

https://zhuanlan.zhihu.com/p/24767059?utm_source=weibo&utm_medium=social

https://zhuanlan.zhihu.com/p/25542274

keras-rl

http://www.cs.cmu.edu/~tom7/mario/
suckerpinch
youtu.be/xOCurBYI_gY


FlappyBird安装方法:
---

1. 安装 Python 2.7.X 或 3.5.x [Python官网](https://www.python.org/download/releases/)

2. 安装 PyGame 1.9.X [PyGame官网](http://www.pygame.org/download.shtml)

3. 获取代码: `git clone https://github.com/sourabhv/FlappyBirdClone.git`

4. 使用命令: `python flappy.py` 运行脚本

5. 按 <kbd>&uarr;</kbd> 键或 <kbd>Space</kbd> 键开始,按 <kbd>Esc</kbd> 键结束。

Ubuntu安装OpenCV2
---
1. 获取代码: 

`wget https://github.com/opencv/opencv/archive/2.4.13.3.zip`

2. 解压: 

`unzip 2.4.13.3.zip`

3. 安装环境:

`sudo apt-get install build-essential`

`sudo apt-get install cmake git libgtk2.0-dev pkg-config libavcodec-dev libavformat-dev libswscale-dev`

`sudo apt-get install python-dev python-numpy`

`sudo apt-get install libtbb2 libtbb-dev libjpeg-dev libpng-dev libtiff-dev libjasper-dev libdc1394-22-dev`

`cd ~/opencv-2.4.13.3`

`mkdir release`

`cd release`

4. 编译安装:

`cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local ..`

`sudo make`

`sudo make install`