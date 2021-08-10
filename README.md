### 👋 介绍

大家好, 我是 **Shao Eric**。

本科：江南大学（211），物联网工程专业

研究生：江南大学，控制科学与控制工程（保研）

### 📫 联系方式

[知乎](https://www.zhihu.com/people/shaoeric) |  ✉️ [Email](mailto:shaoeric@foxmail.com) | 💬 [Issue](https://github.com/shaoeric/shaoeric/issues) 

### 💡 主要工作

- [**小样本目标检测框架**](https://github.com/shaoeric/modified_LSTD_pytorch): 该项目是我本科毕业设计课题，针对[LSTD](https://ojs.aaai.org/index.php/AAAI/article/view/11716)框架进行了复现和改进，复现和改进耗时二十天，项目个人独立完成，最终获得学校优秀毕业设计的**第一名**，该项目在申请专利中
  - 提出了使用统计特征方法改进背景抑制模块，减少了训练时的参数量和计算量
  - 提出了一种分类器热启动训练机制，加快分类器的训练收敛速度（trick）
- [**GTZAN音乐风格分类**](https://github.com/shaoeric/musical_genres_classification): 该项目是我兴趣使然做的关于深度学习的第一个项目，主要使用的keras框架对GTZAN的10类风格共1000个样本执行分类处理
  - 使用了改进预加权的MFCC特征以及logbank特征作为网络的两个输入
  - 使用了two-input网络提取特征，再concat后分类。 网络结构相对简单
- [**pynotice**](https://github.com/shaoeric/pynotice): 空闲时间写的一个模块，用来在程序运行结束或者报错的时候通过邮件等方式提醒用户的（数据处理和训练模型比较耗时，又不知道什么时候结束），已经上传到**pypi**可以在线安装了

### 📚 竞赛

- [**CCF BDCI 2019 工件质量预测冠军**](https://discussion.datafountain.cn/questions/2234/answers/23331)：西门子提供的赛题，目的是通过工业生产的一些参数，对零件的质量进行分类。在团队中主要负责特征工程与模型搭建的工作,在与团队交流的过程中学到了很多。还需要提升的技能主要是对于数据的分析能力。主要贡献：
  - 精度统一：将一些保留精度不同的数值类型特征统一精度，将其作为类别型特征处理。
  - 软测量方法：通过可视化方法发现A类特征相对于label有明显的分界，使用XGB模型对P类特征建模去预测A类特征，再使用A类特征对label进行建模。
- [**biendata 智源抗疫 - 药物研发小分子性质预测赛15th/624teams**](https://www.biendata.xyz/competition/molecule/final-leaderboard/): 智源提供的赛题，目的是通过大量的药物分子的特征预测五种化学性质。个人独立参赛。在学习冠军方案后,学会了如何使用神经网络来处理表格高维数据。
  - 分布调整：使用不同的变换函数对5个target的分布进行变换。
  - 二分类网络矫正：评价函数SMAPE在零附近的结果以及正负预测错误的结果损失更大，提出用二分类网络对target的正负号建模，对预测网络的结果进行矫正。
- [**2020中国高校计算机大赛·华为云大数据挑战赛19th/1491teams**](https://competition.huaweicloud.com/information/1000037843/bdc2020?track=107):赛题为运单ETA预测问题，难点在于如何对海量数据进行数据清洗，并合理分配样本标签。在团队中，主要是进行了数据分析，特征工程。
  - 特征工程：使用经纬度特征，构造出相关性0.86的强特。
  - 特征清洗：港口特征存在大量的相同港口但港口名不同的情况，使用geohash将港口名统一。
  - 路段匹配：通过航线的经纬度与港口的经纬度计算距离，限制其距离至一定阈值认为其经过了哪些港口，并设置起始港口。
- [**Kaggle Google Smartphone Decimeter Challenge铜牌60th/810teams**](https://www.kaggle.com/c/google-smartphone-decimeter-challenge/overview): 谷歌主办的手机室外定位赛，目的是提高智能手机的GNSS 定位精度。由于选取了lb比较好的结果，导致有些过拟合，pb shake。三个月的follow收获颇多。主要贡献：
  - 偏移纠正：基于已有定位结果，估算手机位置偏移程度，统一纠正。
  - 停车检测：采用规则和LGBM预测汽车出发和结束时停车时段，同时，规则捕捉行驶过程中停车时段，使用中位数替换停车窗口的定位点。
  - 路网匹配：将定位点匹配到地图路网上，匹配过程中，基于平移速度、最近邻候选点和与最近邻路网点的距离做异常值剔除。
  - 轨迹平滑：结合高斯滤波和卡尔曼滤波，平滑数据，同时对同一采集时段的轨迹，插值填空和平均轨迹。
  - 参数调优：针对不同类型的路段，采用optuna自动调参。 
