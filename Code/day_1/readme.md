# Day1：Data Preprocessing（数据预处理）

## step1:  导入包

对于数据处理与数据分析来说，pandas与numpy包是两个必须的包。

numpy包是python的一个数值计算扩展，其对于存储和处理大型矩阵非常高效方便。

pandas包是基于numpy的一个数据分析工具。

## step2: 导入数据集

目前各大比赛以及各种开放数据集均使用CSV格式的，CSV格式文件以纯文本的形式，文件的每一行为一条数据记录，每一列为特征记录，我们使用pandas中的read_csv方法读取CSV文件中的内容，读取的内容为DataFrame格式。

## step3: 处理缺失数据

在处理数据过程中，我们经常会遇到数据缺失问题，我们使用的最简单的处理方法是按均值和中位数对NaN数据进行替换，使用sklearn.preprocessing

## step4: 编码分类数据

分类数据通常包含的标签值的变量而不是数值型，例如“Yes”与“No”，所以我们需要将其转换为数值形式，使用sklearn.preprocessing的LabelEncoder。或者使用pandas中的map方法。

## step5: 数据集划分为训练集与测试集

将数据按8:2或分为训练集与测试集，使用sklearn.crossvalidation中的train_test_split()方法

## step6: 特征缩放

大多数机器学习算法使用的欧几里得算法计算两个数据点之间的距离，特征缩放一是提高梯度下降发求解最优解的速度，二是有可能提高精度，更利于模型的训练，但是对于决策树模型等分类方法更注重的是数值之间的分布情况，因此不需要特征归一化

<p align="center">
    <img src="https://github.com/QiujieDong/Learn_ML_in_100_days/blob/master/Info_graphs/Day%201.jpg">
</p>
