
# 常见的规划问题都有哪些
- LP：Linear Programming 线性规划 研究的是在线性约束条件下线性目标函数的极值问题
  ILP：Integer Linear Programming 整数线性规划问题，就是全部决策的变量都必须是整数
  MIP：Mixed Integer Programming 混合整数规划，混合整数规划是LP的一种，其中部分的决策变量是整数，不需要都是整数
  VRP：Vehicle Routing Problem 车辆路径问题

  以上的所有规划问题其实就是数学里面的optimization，最优化问题，也就是一般也称为凸优化，求解目标函数的极值解



# 常用的规划工具包都有哪些
- 1. Pulp 能够解决包括整数规划在内的绝大多数线性规划问题，并且能提供多种solver
  2. Ortools 支持线性规划、整数规划、可以方便的求解Routing、Bin packing、Network flows、Assignment、Scheduling等问题



# RFM模型的原理是怎样的
- RFM是由三个英文单词的首字母组成的，即Recency（最近一次消费时间间隔）、Frequency（一段时间内的消费频率）和Monetary（一段时间内的消费金额）（RFM分析模型介绍）
（1） 最近一次消费时间间隔（R），上一次消费离得越近，R值越小，用户价值越高。
（2） 消费频率（F），购买的频率越高，F值越大，用户价值越高
（3） 消费金额（M），消费金额越高，M值越大，用户价值越高。
 每一个指标都有高-低两个值，222之后，就得到八类用户：
 1. 重要价值用户
 2. 重要发展用户
 3. 重要保持用户
 4. 重要挽留用户
 5. 一般价值用户
 6. 一般发展用户
 7. 一般保持用户
 8. 一般挽留用户



