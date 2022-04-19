## 核心思想
### 图像分类任务
- 不平衡(imbalanced)学习和标签的价值(value)
	- 标签监督(supervision)比无监督的效果要好
	- 极度(heavily)不平衡数据会引发分类器的**标签偏差(bias)**, 即决策边界会被多数(majority)类改变
	- 类不平衡(class-imbalanced)学习可受益于半监督学习和自监督方式
	- 专门技术: 数据重采样(re-sampling)方法和类平衡(class-balanced)损失, 在极度(extreme)类不平衡情况下性能仍会下降
- 半监督学习: 利用更多的未标记(unlabeled)数据(额外数据)
	- 利用伪标签(pseudo-labeling)策略
	- 理论证明中的最优贝叶斯分类器推导存疑
	- 从定理中可看出: 
		- 训练数据不平衡影响估计的精度: 越不平衡, p-q越大, 影响估计和要学习值之间的closeness
		- 未标记数据不平衡影响获得好估计的概率: 对于好的基分类器, 可大致将未标记数据集中估计的正负样本数看作是实际的正负样本数; 对于概率的第二项, 当且仅当正负样本数相等时(数据集平衡)取最大值; 对于第3,4项, 少数类对应的项会占统治地位; 当数据集平衡, 概率会更高, 但任何情况下, 更多未标记数据总是有用的
![semi_theorem_1](images/semi_theorem_1.jpg)
![semi_theorem_2](images/semi_theorem_2.jpg)
![semi_theorem_3](images/semi_theorem_3.jpg)
- 自监督学习: 预训练分类器
	- 在最初的时候抛弃标签
	- 定理一的证明中误差概率对应的事件是小于0(存疑), 以及推导公式第2-3行/3-4行的变换(存疑)
	- 自监督给出的更好的分类器的函数形式(存疑)
	- sub-exponential随机变量(存疑)
	- 定理二的证明中推导公式第3-4行的变换(存疑)
	- 各种形式的concentration不等式(存疑)
![self_theorem_1](images/self_theorem_1.jpg)
![self_theorem_2](images/self_theorem_2.jpg)
![self_theorem_3](images/self_theorem_3.jpg)
![self_theorem_4](images/self_theorem_4.jpg)
![self_theorem_5](images/self_theorem_5.jpg)


## 参考文献
- Rethinking the Value of Labels for Improving Class-Imbalanced Learning
- [concentration inequality](https://www.stat.berkeley.edu/~mjwain/stat210b/Chap2_TailBounds_Jan22_2015.pdf)