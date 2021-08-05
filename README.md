### 👋 介绍

大家好, 我是 **Shao Eric**，本科就读于江南大学（211），物联网工程专业，保研江南大学控制科学与工程。

### 📫 联系方式

[知乎](https://www.zhihu.com/people/shaoeric) |  ✉️ [Email](mailto:shaoeric@foxmail.com) | 💬 [Issue](https://github.com/shaoeric/shaoeric/issues) 

### 💡 主要工作

- [**小样本目标检测框架**](https://github.com/shaoeric/modified_LSTD_pytorch): 该项目是我本科毕业设计课题，针对LSTD框架进行了复现和改进，复现和改进耗时二十天，项目个人独立完成，最终获得学校优秀毕业设计的**第一名**，该项目在申请专利中。
- [**GTZAN音乐风格分类**](https://github.com/shaoeric/musical_genres_classification): 该项目是我兴趣使然做的关于深度学习的第一个项目，主要使用的keras框架对GTZAN的10类风格共1000个样本执行分类处理，没有使用经典的模型做骨干网络，而是提取了两个人工特征后搭建了层数较少的网络。
- [**pynotice**](https://github.com/shaoeric/pynotice): 空闲时间写的一个模块，用来在程序运行结束或者报错的时候通过邮件等方式提醒用户的（数据处理和训练模型比较耗时，又不知道什么时候结束），已经上传到**pypi**可以在线安装了

### 📚 竞赛

- [**CCF BDCI 2019 工件质量预测冠军**](https://discussion.datafountain.cn/questions/2234/answers/23331)：在团队中主要负责特征工程与模型搭建的工作,在与团队交流的过程中学到了很多。还需要提升的技能主要是对于数据的分析能力。
- [**biendata 智源抗疫 - 药物研发小分子性质预测赛15th/624teams**](https://www.biendata.xyz/competition/molecule/final-leaderboard/): 个人独立参赛，主要是对一些异常值进行清洗、特征工程以及后处理方法矫正，在使用hyperparameter_hunter模块进行模型调参时，发现其不足，并提交了pull request。在学习冠军方案后,学会了如何使用神经网络来处理表格高维数据.
- [**2020中国高校计算机大赛·华为云大数据挑战赛19th/1491teams**](https://competition.huaweicloud.com/information/1000037843/bdc2020?track=107):赛题为运单ETA预测问题，难点在于如何对海量数据进行数据清洗，并合理分配样本标签。在团队中，主要是进行了数据分析，特征工程，比较幸运的是，最后得到了相关性0.86的强特。在对该赛题使用上一场比赛中学到的神经网络方案时，发现神经网络无法收敛的问题，而且构造的特征对结果提升十分不稳定，分析原因是各个运单样本存在大量的相同特征，神经网络对这类样本学习效果较差，最终放弃神经网络，改用树模型完成。
- [**Kaggle Google Smartphone Decimeter Challenge铜牌70th/822teams**](https://www.kaggle.com/c/google-smartphone-decimeter-challenge/overview): 学习code区和discussion区的开源方案，对每一个collection使用lgb对是否停车进行建模，将刚出发点与要停车点中间的行驶区域过滤出来，然后使用position shift对不同路段做预处理得到较好的baseline，使用snap2grid+kdtreee将sjc路段牵至最近的ground truth路网上，并通过限速的方法将匹配后出现的离群点置空，为了防止后续的平滑方法过度平滑，我们将连续为空的窗口扩展为更大的空窗口，使用线性插值填空。使用自适应高斯滤波和卡尔曼滤波、phone mean、position shift。此外，我们使用了迭代法将所有后处理再执行第二次，所有的参数通过optuna进行优化。由于选取了lb比较好的结果，导致pb严重shake。三个月的follow收获颇多。
