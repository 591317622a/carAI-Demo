# carAI-Demo# carAI-Demo
此项目运行需要额外安装numpy和pygame库
此项目使用pygame搭建了一个简单的赛道，使用一些正方形作为赛车，同时对每个赛车生成一个神经网络来控制它的方向和速度；使用遗传算法来挑选表现好的神经网络。经过多次迭代后，可以训练出驾驶小车成功到达终点的神经网络。

做这个demo的原因戳这里:
https://zhuanlan.zhihu.com/p/56319305
###1.文件说明
#####mainGame.py
程序的入口，其中GameStart()使用遗传算法来训练神经网络
testAI()可以单独观察训练好的神经网络效果
#####myItem.py
赛车类car:
其中包含赛车当前的位置，角度，速度，以及距离赛道边缘的长度等赛车的属性
circle类:
主要用于生成赛道
#####myCarAI.py
CarAI类:接收赛车的角度、速度以及距离赛道边缘长度作为输入；输出两个值控制赛车的角度和速度
gene_algo类:使用遗传算法生成新的网络。不过这里我只是简单的进行了权值扰动生成新的网络。
#####para_data文件夹
存放了一个训练好的神经网络

##视频连接戳这里:
