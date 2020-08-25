
# 当我们思考数据源的时候，都有哪些维度，如果你想要使用爬虫抓取数据，都有哪些工具
- 当进行数据分析建模的时候，往往会遇到Feature（特征）纬度不够的情况，这时候就会需要思考数据的补充，关于新增数据源，主要可以从4个纬度考虑：  
 1. 开放数据源 - 一些对外公开的数据库，例如imageNet，Netflix Prize DataSet，LETOR，MSLR，Yahoo Learning to Rank数据集等
 2. 爬虫抓取 - 这里主要分两种，一是使用市面上的一些爬虫工具：例如八爪鱼、火车头、后羿等，这类型具备可视化且易操作；再一个就是自己写爬虫代码，抓取特定的网站或者APP
 3. 传感器 - 比如无人驾驶的传感器数据，新零售的传感器数据，采集的是物理信息（图像、视频、或者某个物体的速度、热度、压强等）
 4. 4.日志采集 - 前端埋点：前端JS代码自动捕捉、后端脚本，例如Google analysis、神策(sensors data) 

# 企业的数据源来自多个维度，请思考什么是企业的数据中台，你是如何理解一方数据，二方数据，三方数据？
- 我理解的数据中台应该是介于前台和后台之间的，它能够弥补后台开发和前台应用的作用。数据中台就收到海量的数据（第一方数据、第二方数据、第三方数据），通过数据技术，对海量数据进行采集、计算、存储、加工，同时统一标准和口径，然后服务到客户层面的应用层。
	1. 第一方数据应该是指self，就是自己企业内部的数据
	2. 第二方数据应该是指合作方的数据，例如在天猫买东西，从天猫获取的数据就是二方数据
	3. 第三方数据是指公开数据，其他的渠道获取的数据，例如微博上面沉淀的数据