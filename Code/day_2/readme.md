# Day2 Simple Linear Regression

## step1: Data preprocess 

使用Day1中的数据预处理方法完成此次数据的处理

- 导入数据库
- 导入数据集
- 检查数据缺失
- 划分数据集:在最新版本的sklearn中train_test_split()函数在sklearn.model_selection下
- 特征缩放(直接使用线性回归模型中的来实现)

## step2：训练线性回归模型

使用sklearn.linear_model库中的LinearRegression类，使用其fit()方法完成训练

## step3: 预测

使用生成的模型对测试集进行预测

## step4:可视化

使用matplotlib.pyplot对结果进行可视化，同时将训练集和测试集做成散点图，观看预测效果