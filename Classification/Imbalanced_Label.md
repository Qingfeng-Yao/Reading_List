## 核心思想
### 图像分类任务
- 不平衡(imbalanced)学习和标签的价值(value)
	- 标签监督(supervision)比无监督的效果要好
	- 极度(heavily)不平衡数据会引发分类器的**标签偏差(bias)**, 即决策边界会被多数(majority)类改变
	- 类不平衡(class-imbalanced)学习可受益于半监督学习和自监督方式
	- 专门技术: 数据重采样(re-sampling)方法和类平衡(class-balanced)损失, 在极度(extreme)类不平衡情况下性能仍会下降
- 半监督学习: 利用更多的未标记(unlabeled)数据
- 自监督学习: 预训练分类器


## 参考文献
- Rethinking the Value of Labels for Improving Class-Imbalanced Learning