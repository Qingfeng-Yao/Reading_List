## 核心思想
### 密度估计任务
- Flow++: (1)通过变分推断进行去量化(dequantization); (2)改善耦合层
	- (存疑)理解退化结果(连续模型应用于离散数据上)产生的具体原因, 均匀去量化则不会退化
	- (存疑)均匀去量化的缺点, 将均匀密度赋予单位超体, 不自然
	- (存疑)仿射耦合层定义中的行列式计算公式
	- (存疑)K个logistics的混合的累积(cumulative)分布函数(CDF)形式推导
	- (存疑)逻辑混合的CDF的范围及其逆的值域
	- (存疑)CDF本身可通过平分(bisection)进行有效逆，因为它是单调递增函数
	- (存疑)逻辑混合CDF耦合变换的雅可比行列式涉及计算逻辑混合的概率密度函数
	- (存疑)条件的表达能力: 每个block结构
![flow++_1](images/flow%2B%2B_1.jpg)
![flow++_2](images/flow%2B%2B_2.jpg)
![flow++_3](images/flow%2B%2B_3.jpg)
![flow++_4](images/flow%2B%2B_4.jpg)
![flow++_5](images/flow%2B%2B_5.jpg)

### 语言建模任务
- Categorical Normalizing Flows: 重点是隐含空间的学习
	- 解码器: 条件独立; 确定的
	- 编码器: 被优化以提供类变量的合适的表示给流，同时在隐含空间中分开不同的类
	- 编码器和解码器共享参数
	- (存疑)真实后验和近似后验之间的关系


## 参考文献
- Flow++: Improving Flow-Based Generative Models with Variational Dequantization and Architecture Design
- Categorical Normalizing Flows via Continuous Transformations