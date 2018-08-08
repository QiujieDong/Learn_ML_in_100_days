# Multiple Linear Regression

多元线性回归尝试通过一个线性方程来适配观测数据，这个线性方程最少有两个及以上特征和标签数据之间构建一个关系。多元线性回归方程实现与简单线性回归很相似，只是在评估方面不同。可以用其分析出特征重要度以及不同变量之间的相互关联。

## Assumptions(假设)

要完成线性回归分析，须确定下列假设是否成立：

- 线性：特征变量与标签值变量之间的关系是线性的。
- 保持误差项的方差齐性(常数方差)：误差项的分散(方差)必须等同
- 多元正态分布：多元回归假定残差符合正态分布
- 缺少多重共线性：假定数据有极少甚至没有多重共线性。即数据是保持相互独立的，不然会造成过拟合。

## Dummy Variables(虚拟变量)

在多元回归模型中，当数据集存在非数值型数据时，使用分类数据。比如，按性别将男、女用数值1、0替代，更深入一点使用one-hot编码。

## Dummy Variable Trap(虚拟变量陷阱)

若存在两个特征不是相互独立，那么在进行线性回归时，容易造成过拟合。

## Note(注意事项)

- 向前选择法
- 向后选择法（向后剔除法/向后消元法）
- 向前向后法：即结合了上面说的向前向后法，先用向前法筛选一遍，再用向后法筛选一遍，直到最后无论怎么筛选模型变量都不在发生变化，结束 。

## step1: Data Preprocessing

- 导入库
- 导入数据集
- 检查数据缺失
- 数据分割
- 编辑虚拟变量
- 特征缩放

## step2：Training Model

使用sklearn.linear_model库的LinearRegression类，训练模型。

## step3: Predict

用predict进行预测


<p align="center">
    <img src="https://github.com/QiujieDong/Learn_ML_in_100_days/blob/master/Info_graphs/Day%203.jpg">
</p>