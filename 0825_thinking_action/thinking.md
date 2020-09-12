
# 关联规则中的支持度、置信度和提升度代表的什么，如何计算
- 1. 支持度它是一个百分比值，它代表某个商品组合同时出现的概率，使用该商品组合出现的次数刍议总次数来计算。
  2. 置信度是个条件概率，代表当买了商品A，再购买商品B的概率，使用同事购买A、B的总数除以购买商品A的数量。
  3. 提升度代表商品A的出现，对商品B的出现概率提升的程度，计算公式：置信度(A -> B) / 支持度(B) ；提升度大于1，表示有提升、提升度等于1，表示没有提升也没有下降、提升度小于1，代表有下降


# 关联规则与协同过滤的区别
- 关联规则是整体的，从大量数据中整体去挖掘出有价值的数据项之间的关系，主要面向的是transaction。
  协同过滤是基于个体的个性化推荐，主要面向的是用户偏好（评分），具体实现是先协同，找到相似的人或物，再过滤，是用户注重个性化的场景，如音乐电影之类的。


# 为什么我们需要多种推荐算法
- 因为每种推荐算法使用的规则以及适用的场景不一样，为了适应不同的场景和需求，我们需要不一样的推荐算法。比如基于用户的协同过滤适用于物品数量大于用户数量，如新闻、博客等信息类推荐系统；基于物品的协同过滤适用于用户数量远大于物品数量，且物品数量相对稳定不会频繁更新，如电子商务等在线网站。


# 关联规则中的最小支持度、最小置信度该如何确定
- 这两个值可以理解为超参数，是没有一个固定值的，要根据训练数据和场景的接受程度来给定。这两个阈值给的越大，得到的有相关性的item就越好，但item的数量也越少。也就是说，数量多，但相关性会差。所以主要根据需要给出的推荐item的数量及item间的相关性来决定这两个参数的值。


# 都有哪些常见的回归分析方法，评价指标是什么
- 常见的回归分析有：线性回归(Linear Regression)、多项式回归(Polinomial Regression)、岭回归(Ridge Regression)、套索回归(Lasso Regression)、ElasticNet回归、自回归(Auto Regression)等。
  评价指标可以评价回归模型的性能好坏，常见的有：
	1. 平均绝对误差（Mean Absolute Error，MAE）
	2. 均方误差（Mean Squared Error，MSE）
	3. 平均绝对百分误差（Mean Absolute Percentage Error，MAPE）
	4. 均方根误差（Root Mean Squared Error）
	5. R2（R-Square）
  