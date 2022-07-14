This is a summary system of scientific information.
# Knowledge System

Induction:  To be or not to be is a question.

Author: Faqi Zhao

# Catalog

* Encrypted Traffic Detection(#Encrypted-Traffic-Detection)
  * TLS malware traffic detection
    * Related work
    * Existing problems
    * Research ideas
  * Protocol classification
  * App classification

* Artificial Intelligence

  * Category

  * Data-certric AI
  * Materials

* Feature engineering

* Mathematics and Methodology

  * Mathematics
  * Methodology

* Software & Tools
  * Scientific
  * Tools
  * Github

* Writing
  * SCI
  * EI
  * Core
  * Readme

* Tips & Bug & Solution
  * Windows
  * Python
  * Zeek
  * Book & open source



# Encrypted Traffic Detection

This section focuses on the related work and problems associated with the study of encrypted traffic, including but not limited to TLS encrypted traffic measurement analysis. This section is continuously updated. ML-based NIDSs.

🔴🟠🟡🟢🔵 --> Priority from highest to lowest

## TLS malware traffic detection

### __Related work__

_Overview_

```
🔴2021 ACM CS[J]. A Survey on Encrypted Network Traffic Analysis Applications, Techniques, and Countermeasures
🟠2020 ISA[J]. Deep learning for cyber security intrusion detection: Approaches, datasets, and comparative study
🟡2021 AS[J]. A Survey on TLS-Encrypted Malware Network Traffic Analysis Applicable to Security Operations Centers
```

_Machine Learning_

```
🔴2017 CVHT[J]. Deciphering Malware’s use of TLS (without Decryption) 
🔴2016 ACM[C]. Identifying Encrypted Malware Traffic with Contextual Flow Data
🔴2017 ACM SIGKDD[C]. Machine Learning for Encrypted Malware Traffic Classification: Accounting for Noisy Labels and Non-Stationarity
🔴2014 IEEE INFOCOM[C]. Markov Chain Fingerprinting to Classify Encrypted Traffic
🟠2020 CCNS[C]. TLS Encrypted Application Classification Using Machine Learning with Flow Feature Engineering
🟠2019 IEEE MILCOM[C]. Detection of Encrypted Malicious Network Traffic using Machine Learning
🟡2017 IEEE TIFS[J]. Classification of Encrypted Traffic With Second-Order Markov Chains and Application Attribute Bigrams
🟡2021 ASB[J]. Machine Learning-Based Malicious X.509 Certificates' Detection
🟢2022 Electronics[J]. Encrypted Malicious Traffic Detection Based on Word2Vec
```

_Deep Learning_

```
🟠2018 ACM WAIS[C]. Hunting Malicious TLS Certificates with Deep Neural Network
🟠2018 IEEE ICHPCC[C]. TLS/SSL Encrypted Traffic Classification with Autoencoder and Convolutional Neural Network
🟡2021 SCN[J]. Malicious Encryption Traffic Detection Based on NLP
```

_Ensemble Learning_

```
🟠2021 ICCS. MGEL: A Robust Malware Encrypted Traffic Detection Method Based on Ensemble Learning with Multi-grained Features
🟡2021 IEEE TIFS MBTree: Detecting Encryption RATs Communication Using Malicious Behavior Tree
```

*Unbalanced data*

```
🔴2017 IEEE PRMRC[J]. Deep Learning for Malicious Flow Detection
```

*Lightweight*



### **Existing problems**

随着加密技术的广泛应用以及新型网络技术的不断更迭，网络结构日趋复杂，加密流量呈现爆炸式增长，尤其随着**TLS1.3/DNS加密化/QUIC**加密协议的演进和推广，全加密时代悄然来临。

加密流量检测的研究一直是学术界和工业界都非常关注的技术方向，分析的对象即识别过程中的输入形式，包括数据**包级、数据流级、主机级、社区级**等，流量识别的目标也是多样的，包括**加密与非加密流量识别**、**加密协议识别**（如SSL、SSH、IPSec、QUIC等）、服务识别（如网页浏览、流媒体、即时通信、网络存储等）、**加密应用软件识别**（如淘宝、微信、Skype等，还可进一步**精细化分类**应用所属类型，如Skype可以分为即时消息、语音通话、视频通话、文件传输等），还有更细粒度的加密流量**内容参数识别**（如发文本、抢红包、视频清晰度等）、网站指纹识别（特定敏感网站）、异常加密流量识别（如恶意软件通信流量、黑客工具产生的流量等）等。

1、特征信息不足

2、概念漂移问题

3、标注样本缺乏

4、开集识别问题

5、推理性能待提升

*Tips:*

[如何深入理解TLS协议? - 知乎](https://www.zhihu.com/question/399317260)

[一篇文章让你彻底弄懂SSL/TLS协议 - 知乎](https://zhuanlan.zhihu.com/p/133375078)

### **Research ideas**

**_Worked_**

```
多特征融合的煤矿网络加密恶意流量检测[J]. 工矿自动化
基于stacking和多特征融合的加密恶意流量检测研究[J]. 计算机工程
AS-DMF_A Lightweight Malware Encrypted Traffic Detection Method Based on Active Learning and Feature Reduction
```

*Github:* [AS-DMF framework](https://github.com/Timeless-zfqi/AS-DMF-framework)

**_To be solved_**

1. 构建真实网络环境下的数据集
2. 基于AI大数据统计规律
3. 与传统规则结合
4. 分层检测体系

### **Dataset**

1. [CTU-13](https://www.stratosphereips.org/datasets-ctu13)
2. [CIC-IDS2017](https://www.unb.ca/cic/datasets/ids-2017.html )
3. [ML-Based NIDS Datasets](https://staff.itee.uq.edu.au/marius/NIDS_datasets/)
3. [网络流量领域公开数据集](https://blog.csdn.net/jmh1996/article/details/90666499)

## Protocol classification



## App classification

***Machine Learning***

```
🔴FS-Net: A Flow Sequence Network For Encrypted Traffic Classification
```

# Artificial Intelligence

This section mainly records the algorithms of machine learning, deep learning, active learning, reinforcement learning and model interpretability and robustness issues in artificial intelligence.

## Category

### ***Machine Learning***

[机器学习专业名词中英文对照 ](https://cloud.tencent.com/developer/article/1443929)

[机器学习 | Coursera](https://www.coursera.org/learn/machine-learning?ranMID=40328&ranEAID=OyHlmBp2G0c&ranSiteID=OyHlmBp2G0c-PcI1nI4To7kp4foLjOi_3g&siteID=OyHlmBp2G0c-PcI1nI4To7kp4foLjOi_3g&utm_content=10&utm_medium=partners&utm_source=linkshare&utm_campaign=OyHlmBp2G0c#syllabus)

**_Algorithms_**

*KNN*

[KNN原理](https://www.cnblogs.com/pinard/p/6061661.html )

[基于scikit-learn包实现机器学习之KNN(K近邻)博客园](https://www.cnblogs.com/xiaotan-code/p/6680438.html)

*NB*

[朴素贝叶斯算法原理](https://www.cnblogs.com/zhoudayang/p/5058264.html)

**_Model interpretability_**

[机器学习模型可解释性进行到底1 - SHAP值理论](https://zhuanlan.zhihu.com/p/364919024)

[机器学习模型可解释性进行到底2 - 从SHAP值到预测概率](https://zhuanlan.zhihu.com/p/364920925) 

[机器学习模型可解释性进行到底3 - DP&amp;ICE图](https://zhuanlan.zhihu.com/p/364921771 ) 

[机器学习模型可解释性进行到底4 - 特征重要性](https://zhuanlan.zhihu.com/p/364922142 ) 

[机器学习模型可解释性❤](https://zhuanlan.zhihu.com/p/258988892 ) 



### ***Deep Learning***

**_Algorithms_**

*CNN*

* [CNN Explainer](https://poloclub.github.io/cnn-explainer/)



### ***Active learning***

_paper_

```
🔴2014 CSD[T]. Active Learning Literature Survey
🔴2022 ACM CS[J]. A Survey on Active Deep Learning: From Model-Driven to Data-Driven
🔴2021 IEEE TNNLS[J]. Fast and Effective Active Clustering Ensemble Based on Density Peak --(Q1)
🔴2017 EAS[J]. Active learning through density clustering
🟠2020 IEEE ICDM[C]. Meta-AAD: Active Anomaly Detection with Deep Reinforcement Learning
🟠2020 IEEE TVT[J]. Importance-Aware Data Selection and Resource Allocation in Federated Edge Learning System
🟠2014 Science[J]. Clustering by fast search and find of density peaks --(Q1)
🟡2018 ICML[J]. Not All Samples Are Created Equal: Deep Learning with Importance Sampling
```

_Tips_

* [主动学习(Active Learning)，看这一篇就够了](https://zhuanlan.zhihu.com/p/377045943)

* [不确定度采样（Uncertainty Sampling）](https://blog.csdn.net/qq_39856931/article/details/106433187)

* [什么是主动学习](https://www.zhihu.com/question/352299820 )

* [Multi-Criteria-based Active Learning](https://blog.csdn.net/weixin_30502157/article/details/99482577 )

_Tools & packet_

* https://github.com/modAL-python/modAL
* https://github.com/NUAA-AL/ALiPy
* https://github.com/google/active-learning
* https://github.com/baal-org/baal

* [Python 密度聚类](https://cloud.tencent.com/developer/article/1738535 )



### Ensemble Learning

* [Stacking方法详解 博客园](https://www.cnblogs.com/Christina-Notebook/p/10063146.html)

* [GBDT--原来是这么回事(附代码) 博客园](https://www.cnblogs.com/mantch/p/11160496.html)
* [终于有人说清楚了--XGBoost算法](https://www.cnblogs.com/mantch/p/11164221.html)
* [通俗易懂--模型集成(多模型)讲解(算法+案例)  博客园](https://www.cnblogs.com/mantch/p/10203143.html)
* [【模型融合】Bagging，Boosting，Stacking](https://blog.csdn.net/xiaohutong1991/article/details/107976781)
* [模型融合及python实现 - 知乎](https://zhuanlan.zhihu.com/p/61705517)
* [XGBClassifier的默认参数和调参总结 - 知乎](https://zhuanlan.zhihu.com/p/365030773)
* [1.11. 集成方法 - sklearn](https://www.scikitlearn.com.cn/0.21.3/12/#11121)
* [深入理解LightGBM - 知乎](https://zhuanlan.zhihu.com/p/99069186)
* [GitHub - kaz-Anova/StackNet: StackNet is a computational, scalable and analytical Meta modelling framework](https://github.com/kaz-Anova/StackNet)

### ***Reinforcement Learning***

* [一文看懂什么是强化学习？（基本概念+应用场景+主流算法）](https://easyai.tech/ai-definition/reinforcement-learning/)

### ***Semi-supervised Learning***



### ***Unsupervised Learning*** 



## Model credibility

* [模型知识抽取促进模型可信任](https://mp.weixin.qq.com/s?__biz=MzIyODYzNTU2OA==&amp;mid=2247489820&amp;idx=1&amp;sn=9d514bf3a20fba3440fed729942ae754&amp;scene=19#wechat_redirect )

* [模型度量 · Machine Learning](https://shunliz.gitbooks.io/machine-learning/content/ml/pythonml/ml-metrics.html)

## Data-certric AI

***Data lightweight***

*Based on active learning*

Move to *Artificial Intelligence - Category - Active learning*



***Data analysis***

_Tips_

* [Data-centric AI](https://zhuanlan.zhihu.com/p/438817550 )

* [数据分析：相关性分析](https://zhuanlan.zhihu.com/p/136771737 )

* [样本类别增加](https://mp.weixin.qq.com/s/DqoiHshO17_QSjw0utJofg )



# Feature engineering

_Tips_

* [深度了解特征工程](https://zhuanlan.zhihu.com/p/111296130)

* [自动化提取特征](https://mp.weixin.qq.com/s/CGS_nAnFAJYhcjmQr6nS3A)
* [你想知道的特征工程，机器学习优化方法](https://www.cnblogs.com/mantch/p/11254026.html)

## Feature Dimensionality Reduction

* [Python机器学习笔记：使用scikit-learn工具进行PCA降维](https://www.cnblogs.com/wj-1314/p/10144700.html)

# Mathematics and Methodology

## Mathematics

*MI & MIC*

* [MIC](https://blog.csdn.net/qq_27586341/article/details/90603140 )
* [MIC-1](https://www.deeplearn.me/1466.html )

* [Maximal Information Coefficient (MIC)最大互信息系数详解与实现](https://blog.csdn.net/FontThrone/article/details/85227239)



## Methodology





# Software and Tools

***Scientific***

`Wireshark`

 `Zeek`

 `Matlab`

`Python` : Pytorh/ Jupyter/ Pycharm

***Github***

* [Github使用技巧](https://zhuanlan.zhihu.com/p/150584178 )

`Zat `: 

* [from log to python](https://github.com/SuperCowPowers/zat "Zat")

`ALiPy` : 

* [Active learning packet](https://github.com/NUAA-AL/ALiPy  "ALiPy")

* [解析ALipy：主动学习的Python工具箱](https://blog.csdn.net/qq_36317312/article/details/117981682 )

`modAL` : 

* [Active learning packet](https://github.com/modAL-python/modAL )

`Zat`

* [ZAT-机器学习-威胁检测](https://www.freebuf.com/articles/es/245516.html)

***Tools***

| Tools  |    function    | source |
| :----: | :------------: | :----: |
| ediary |                |        |
| Typora | .md --> Readme |        |
| Xmind  |                |        |
| DeepL  |  translation   |        |

* [VMware Tools安装](https://blog.csdn.net/love20165104027/article/details/83377758)



# Writing

*Tips*

* [英文论文写作经验 - 知乎](https://zhuanlan.zhihu.com/p/158599066)

## **SCI**

* [Sci-Hub:](https://sci-hub.se/)

* [SCI写作高频词]( https://zhuanlan.zhihu.com/p/80384925 )
* [影响因子查询](http://www.letpub.com.cn/index.php?page=journalapp&amp;fieldtag=4&amp;firstletter= ) or Web of science --> Journal Citation Report

* [SCI期刊分区检索目录及影响因子查询系统-ShengSci](https://www.shengsci.com/sci/)

* [citexs-赛特新思生物医学科研助手](https://www.citexs.com/)

## EI



## Conference

* [CCF会议 - Conference Partner (会伴)](https://www.myhuiban.com/conferences/ccf)



## Patents

* [国家知识产权局](https://www.cnipa.gov.cn/)
* [专利缴费](https://zhuanlan.zhihu.com/p/115498826)

## Core

Submission comments refer to the "小木虫"

* [计算机核心期刊（北大核心）投稿意见](https://www.cnblogs.com/smuxiaolei/p/8081342.html)



## **Readme**

* [Readme的书写规范](https://blog.csdn.net/A33280000f/article/details/115836658 )

* [markdown-cheatsheet](https://github.com/tchapi/markdown-cheatsheet#heading-1 )
* [如何写一个优秀的Readme](https://blog.csdn.net/MOY37RQW1JarN33BgZk/article/details/84207318 )  or [Readme](https://zhuanlan.zhihu.com/p/29136209)
* [Readme好看指南](https://zhuanlan.zhihu.com/p/151291463 )

## Layout

*Tips:*

* [word两栏格式公式居中，编号右对齐](https://blog.csdn.net/weixin_44105113/article/details/118445043)

# Tips & Bug & Solution

## Windows



## linux

* [Linux命令](https://www.linuxcool.com/)



## python

***sklearn***

* [sklearn](https://scikit-learn.org/stable/index.html )
* [sklearn-中文社区](https://scikit-learn.org.cn/ )
* [sklearn-交叉验证](https://blog.csdn.net/rocling/article/details/93717335 )
* [CountVectorizer详解](https://blog.csdn.net/weixin_38278334/article/details/82320307 )



[使用sklearn进行集成学习——理论](https://www.cnblogs.com/jasonfreak/p/5657196.html)

[使用sklearn做单机特征工程](https://www.cnblogs.com/jasonfreak/p/5448385.html)

[使用sklearn优雅地进行数据挖掘 - 博客园](https://www.cnblogs.com/jasonfreak/p/5448462.html)



[机器学习stacking算法之我见 - 知乎](https://zhuanlan.zhihu.com/p/70757784)

***python***

* [Python中文教程](https://docs.python.org/zh-cn/3/)
* [python划分训练集、验证集和测试集](https://blog.csdn.net/haoji007/article/details/106165488)
* [修改jupyter notebook默认打开浏览器(Windows操作系统)](https://blog.csdn.net/tunerf/article/details/90767377)



## Zeek

* [Zeek documents](https://docs.zeek.org/en/current/quickstart.html#a-minimal-starting-configuration )

* [Zeek install](https://docs.zeek.org/en/master/get-started.html)

## Open source

***Class***

[2019年机器之心干货教程都在这里了](https://mp.weixin.qq.com/s?__biz=MzA3MzI4MjgzMw==&mid=2650779244&idx=1&sn=f961d29c4be9288ee31d573a25c0f93e&chksm=871a6a12b06de304d90bac98dc5e2e8d70b52bf43444cdcee5a1564c466816d526c58f287f0f&mpshare=1&scene=1&srcid=1023UT4OyAaWvqHDmpBYsvYG&sharer_sharetime=1603441563266&sharer_shareid=84d5fc173d51bf1365bb32f022e3807d&key=0ac52f944ed0d7b1bad9f9c791891ab85d0ff4222f705f34578e1fb440bcbe855abbe2f39516928b9d6327b850fc0d6fcea973424426b8eeb09e6cb93693478c0555daf8ef468a26683079c1d5324c515740f6f0bdc682b04872e9ebfaf94cea69d42404abb706dd5137df20965d7b77615bcab9fdec4a73d1400840a5ac08b5&ascene=1&uin=Mjc0MzE1MTI0NA%3D%3D&devicetype=Windows+10+x64&version=6300002f&lang=zh_CN&exportkey=Ab1ZC%2FSbM4E3ZzDLxnfXXfA%3D&pass_ticket=cN9rBpfgt8w6bvNaYcVsIzioqpyunTIjecZmRoUoPXQQLGDqacHzzZH1cqSIyKAc&wx_header=0)

[机器学习必学10大算法](https://mp.weixin.qq.com/s?__biz=MzA3MzI4MjgzMw==&mid=2650758853&idx=4&sn=fad1a71a12a0ec07b05bc255202ba5c3&chksm=871a9abbb06d13ad1683d02a3c29767b5ab0adbf8299b891f22bd5658df96996be4b00e29bb7&scene=21#wechat_redirect)



***Encrypted traffic detection***

《加密流量测量和分析》-- 程光

[一篇报告了解国内首个针对加密流量的检测引擎 - 安全牛](https://www.aqniu.com/tools-tech/45207.html)

[加密恶意流量优秀检测思路分享](https://cloud.tencent.com/developer/article/1792547)

[安全协议学习之TLS协议与HTTPS恶意流量分析](https://blog.csdn.net/qq_43968080/article/details/107086152)



***Computer/ software engineering***

[Software Engineering](chrome://bookmarks/?id=402)



***Cyber-security***

《网络安全中的数据挖掘技术》 -- 李涛

[HTTP,TCP/IP,DNS之间的关系及作用之见解 - 知乎](https://zhuanlan.zhihu.com/p/60721237)

[HTTP、TCP/IP、DNS之间的关系](https://blog.csdn.net/forevershow55/article/details/108756688 )





***Industry Reports***

[免费行业报告_免费研究报告-前沿报告库](https://wk.askci.com/)

[国家统计局](http://www.stats.gov.cn/)

[腾讯研究院](https://www.tisi.org/)



***TLS/SSL***

[Joy：一款用于捕获和分析网络内部流量数据的工具](https://www.freebuf.com/sectool/161431.html)

[传输层抓包分析-SSL/TLS](https://www.freebuf.com/articles/network/116497.html )

[DataCon2020 清华战队 TLS](https://datacon.qianxin.com/blog/archives/122 )

[DataCon2019 DNS恶意流量分析第一](https://zhuanlan.zhihu.com/p/68009679 )

[TLS加密流现状分析 -- Technology report](https://news.sophos.com/en-us/2021/04/21/nearly-half-of-malware-now-use-tls-to-conceal-communications/ )

[恶意软件加密流量的思考](https://mp.weixin.qq.com/s/hVq3eBMDsX6tj1PsoUpy8Q )

[研究：恶意软件在沙盒中应该执行多长时间？ - 安全内参 | 决策者的网络安全知识库](https://www.secrss.com/articles/30599)



***Some website***

[Hack Inn](https://www.hackinn.com/)

[攻防世界](https://adworld.xctf.org.cn/)

[2020年网络安全产业深度对话论坛 - Hack Inn](https://www.hackinn.com/index.php/archives/746/)











