# Q1: 什么是监督学习，无监督学习，半监督学习?

## A1:

1. 监督学习（Supervised learning）
   有标签的机器学习过程。标签就是告诉模型在什么样的数据特征下输出什么样的结果。又分为分类和回归。
2. 无监督学习（Unsupervised Learning）
   无标签的机器学习，将数据自身的特征在不同的模型中进行不同的表现。
3. 半监督学习（Semi-Supervised learning）
   部分有标签，部分无标签。有标签的数据作用于无标签的数据，也可以作用于有标签的数据，规范与引导聚类或者关联的方向，同时无标签的数据，也可以作用于有标签的数据，时刻获得模型对于数据整体情况的影响和反馈。

它们的主要区分点在于是否所有数据都有标签。

# Q2: K-means中的k值如何选取?

## A2:

手肘法(elbow method)，找到聚类的数量K与各个点到cluster中心的距离的平方的和所构成的函数的极值点，这个极值点所对应的K值被认为是合适的K值。

# Q3: 随机森林采用了bagging集成学习，bagging指的是什么？

## A3:
bagging首先随机有放回地抽取训练集，训练多个弱分类器。然后通过取平均，或者投票(voting)的方式决定最终的分类结果。

bagging思想，将若干个弱分类器的分类结果进行投票选择，从而组成一个强分类器
bagging。
它不用单棵决策树来做预测，增加了预测准确率，即：不容易过拟合，减少了预测方差。

# Q4: 主动学习和半监督学习的区别是什么?(课上已将表征学习更改为主动学习)
##  A4:
1. 对于主动学习：
是给人一部分数据，让人做出标注，然后将标注结果放入训练集中训练模型，使得模型可以以此主动标注好模型。它可以使用较少的样本达到较好的分类结果。主动学习中有人的参与。

2. 对于半监督学习：
指在有标签的训练数据十分稀少的情况下，利用没有标签的数据，提高模型效果的方法。半监督学习没有人的参与。

