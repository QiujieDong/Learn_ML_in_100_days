# Logistic Regression

逻辑回归被用来处理不同的分类问题，这里的目的是预测当前被观察的对象属于哪个组。它会给你提供一个离散的二进制输出结果。一个简单的例子就是判断一个人是否会在即将到来的选举中进行投票。

逻辑回归到底是什么，以及它背后的数学是什么。学习如何计算代价函数，以及如何使用梯度下降法来将代价函数降低到最小。

## How Does It Work?

逻辑回归通过逻辑函数确定特征与标签之间的关系，进而更深的预测问题。

## Making Predictions

问题应该被转换成二进制问题，以方便最终的预测。使用S函数作为逻辑回归函数，使值位于（0-1）之间。

## Logistic &  Linear

逻辑回归给出离散的输出结果，然而线性回归给出的是连续的输出结果。

## Sigmoid函数

Sigmoid函数是一个S形曲线，可以实现将任意真实值映射为值域范围为0-1的值。

<p align="center">
    <img src="https://github.com/QiujieDong/Learn_ML_in_100_days/blob/master/Info_graphs/Day%204.jpg">
</p>

## 数据集

<p align="center">
  <img src="https://github.com/QiujieDong/Learn_ML_in_100_days/blob/master/Other%20Docs/data.PNG">
</p> 

该数据集包含了社交网络中用户的信息。这些信息涉及用户ID,性别,年龄以及预估薪资。一家汽车公司刚刚推出了他们新型的豪华SUV，我们尝试预测哪些用户会购买这种全新SUV。并且在最后一列用来表示用户是否购买。我们将建立一种模型来预测用户是否购买这种SUV，该模型基于两个变量，分别是年龄和预计薪资。因此我们的特征矩阵将是这两列。我们尝试寻找用户年龄与预估薪资之间的某种相关性，以及他是否购买SUV的决定。

## 可视化的结果

<p align="center">
  <img src="https://github.com/QiujieDong/Learn_ML_in_100_days/blob/master/Other%20Docs/training.png">
</p> 
<p align="center">
  <img src="https://github.com/QiujieDong/Learn_ML_in_100_days/blob/master/Other%20Docs/testing.png">
</p> 