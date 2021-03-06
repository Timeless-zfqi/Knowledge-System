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

π΄π π‘π’π΅ --> Priority from highest to lowest

## TLS malware traffic detection

### __Related work__

_Overview_

```
π΄2021 ACM CS[J]. A Survey on Encrypted Network Traffic Analysis Applications, Techniques, and Countermeasures
π 2020 ISA[J]. Deep learning for cyber security intrusion detection: Approaches, datasets, and comparative study
π‘2021 AS[J]. A Survey on TLS-Encrypted Malware Network Traffic Analysis Applicable to Security Operations Centers
```

_Machine Learning_

```
π΄2017 CVHT[J]. Deciphering Malwareβs use of TLS (without Decryption) 
π΄2016 ACM[C]. Identifying Encrypted Malware Traffic with Contextual Flow Data
π΄2017 ACM SIGKDD[C]. Machine Learning for Encrypted Malware Traffic Classification: Accounting for Noisy Labels and Non-Stationarity
π΄2014 IEEE INFOCOM[C]. Markov Chain Fingerprinting to Classify Encrypted Traffic
π 2020 CCNS[C]. TLS Encrypted Application Classification Using Machine Learning with Flow Feature Engineering
π 2019 IEEE MILCOM[C]. Detection of Encrypted Malicious Network Traffic using Machine Learning
π‘2017 IEEE TIFS[J]. Classification of Encrypted Traffic With Second-Order Markov Chains and Application Attribute Bigrams
π‘2021 ASB[J]. Machine Learning-Based Malicious X.509 Certificates' Detection
π’2022 Electronics[J]. Encrypted Malicious Traffic Detection Based on Word2Vec
```

_Deep Learning_

```
π 2018 ACM WAIS[C]. Hunting Malicious TLS Certificates with Deep Neural Network
π 2018 IEEE ICHPCC[C]. TLS/SSL Encrypted Traffic Classification with Autoencoder and Convolutional Neural Network
π‘2021 SCN[J]. Malicious Encryption Traffic Detection Based on NLP
```

_Ensemble Learning_

```
π 2021 ICCS. MGEL: A Robust Malware Encrypted Traffic Detection Method Based onΒ Ensemble Learning with Multi-grained Features
π‘2021 IEEE TIFS MBTree: Detecting Encryption RATs Communication Using Malicious Behavior Tree
```

*Unbalanced data*

```
π΄2017 IEEE PRMRC[J]. Deep Learning for Malicious Flow Detection
```

*Lightweight*



### **Existing problems**

ιηε ε―ζζ―ηεΉΏζ³εΊη¨δ»₯εζ°εη½η»ζζ―ηδΈζ­ζ΄θΏ­οΌη½η»η»ζζ₯θΆε€ζοΌε ε―ζ΅ιεη°ηηΈεΌε’ιΏοΌε°€εΆιη**TLS1.3/DNSε ε―ε/QUIC**ε ε―εθ??ηζΌθΏεζ¨εΉΏοΌε¨ε ε―ζΆδ»£ζηΆζ₯δΈ΄γ

ε ε―ζ΅ιζ£ζ΅ηη η©ΆδΈη΄ζ―ε­¦ζ―ηεε·₯δΈηι½ιεΈΈε³ζ³¨ηζζ―ζΉεοΌεζηε―Ήθ±‘ε³θ―ε«θΏη¨δΈ­ηθΎε₯ε½’εΌοΌεζ¬ζ°ζ?**εηΊ§γζ°ζ?ζ΅ηΊ§γδΈ»ζΊηΊ§γη€ΎεΊηΊ§**η­οΌζ΅ιθ―ε«ηη?ζ δΉζ―ε€ζ ·ηοΌεζ¬**ε ε―δΈιε ε―ζ΅ιθ―ε«**γ**ε ε―εθ??θ―ε«**οΌε¦SSLγSSHγIPSecγQUICη­οΌγζε‘θ―ε«οΌε¦η½ι‘΅ζ΅θ§γζ΅εͺδ½γε³ζΆιδΏ‘γη½η»ε­ε¨η­οΌγ**ε ε―εΊη¨θ½―δ»Άθ―ε«**οΌε¦ζ·ε?γεΎ?δΏ‘γSkypeη­οΌθΏε―θΏδΈζ­₯**η²Ύη»εεη±»**εΊη¨ζε±η±»εοΌε¦Skypeε―δ»₯εδΈΊε³ζΆζΆζ―γθ―­ι³ιθ―γθ§ι’ιθ―γζδ»ΆδΌ θΎη­οΌοΌθΏζζ΄η»η²εΊ¦ηε ε―ζ΅ι**εε?Ήεζ°θ―ε«**οΌε¦εζζ¬γζ’ηΊ’εγθ§ι’ζΈζ°εΊ¦η­οΌγη½η«ζηΊΉθ―ε«οΌηΉε?ζζη½η«οΌγεΌεΈΈε ε―ζ΅ιθ―ε«οΌε¦ζΆζθ½―δ»ΆιδΏ‘ζ΅ιγι»ε?’ε·₯ε·δΊ§ηηζ΅ιη­οΌη­γ

1γηΉεΎδΏ‘ζ―δΈθΆ³

2γζ¦εΏ΅ζΌη§»ι?ι’

3γζ ζ³¨ζ ·ζ¬ηΌΊδΉ

4γεΌιθ―ε«ι?ι’

5γζ¨ηζ§θ½εΎζε

*Tips:*

[ε¦δ½ζ·±ε₯ηθ§£TLSεθ??? - η₯δΉ](https://www.zhihu.com/question/399317260)

[δΈη―ζη« θ?©δ½ ε½»εΊεΌζSSL/TLSεθ?? - η₯δΉ](https://zhuanlan.zhihu.com/p/133375078)

### **Research ideas**

**_Worked_**

```
ε€ηΉεΎθεηη€ηΏη½η»ε ε―ζΆζζ΅ιζ£ζ΅[J]. ε·₯ηΏθͺε¨ε
εΊδΊstackingεε€ηΉεΎθεηε ε―ζΆζζ΅ιζ£ζ΅η η©Ά[J]. θ?‘η?ζΊε·₯η¨
AS-DMF_A Lightweight Malware Encrypted Traffic Detection Method Based on Active Learning and Feature Reduction
```

*Github:* [AS-DMF framework](https://github.com/Timeless-zfqi/AS-DMF-framework)

**_To be solved_**

1. ζε»Ίηε?η½η»η―ε’δΈηζ°ζ?ι
2. εΊδΊAIε€§ζ°ζ?η»θ?‘θ§εΎ
3. δΈδΌ η»θ§εη»ε
4. εε±ζ£ζ΅δ½η³»

### **Dataset**

1. [CTU-13](https://www.stratosphereips.org/datasets-ctu13)
2. [CIC-IDS2017](https://www.unb.ca/cic/datasets/ids-2017.html )
3. [ML-Based NIDS Datasets](https://staff.itee.uq.edu.au/marius/NIDS_datasets/)
3. [η½η»ζ΅ιι’εε¬εΌζ°ζ?ι](https://blog.csdn.net/jmh1996/article/details/90666499)

## Protocol classification



## App classification

***Machine Learning***

```
π΄FS-Net: A Flow Sequence Network For Encrypted Traffic Classification
```

# Artificial Intelligence

This section mainly records the algorithms of machine learning, deep learning, active learning, reinforcement learning and model interpretability and robustness issues in artificial intelligence.

## Category

### ***Machine Learning***

[ζΊε¨ε­¦δΉ δΈδΈεθ―δΈ­θ±ζε―Ήη§ ](https://cloud.tencent.com/developer/article/1443929)

[ζΊε¨ε­¦δΉ  | Coursera](https://www.coursera.org/learn/machine-learning?ranMID=40328&ranEAID=OyHlmBp2G0c&ranSiteID=OyHlmBp2G0c-PcI1nI4To7kp4foLjOi_3g&siteID=OyHlmBp2G0c-PcI1nI4To7kp4foLjOi_3g&utm_content=10&utm_medium=partners&utm_source=linkshare&utm_campaign=OyHlmBp2G0c#syllabus)

**_Algorithms_**

*KNN*

[KNNεη](https://www.cnblogs.com/pinard/p/6061661.html )

[εΊδΊscikit-learnεε?η°ζΊε¨ε­¦δΉ δΉKNN(KθΏι»)εε?’ε­](https://www.cnblogs.com/xiaotan-code/p/6680438.html)

*NB*

[ζ΄η΄ θ΄εΆζ―η?ζ³εη](https://www.cnblogs.com/zhoudayang/p/5058264.html)

**_Model interpretability_**

[ζΊε¨ε­¦δΉ ζ¨‘εε―θ§£ιζ§θΏθ‘ε°εΊ1 - SHAPεΌηθ?Ί](https://zhuanlan.zhihu.com/p/364919024)

[ζΊε¨ε­¦δΉ ζ¨‘εε―θ§£ιζ§θΏθ‘ε°εΊ2 - δ»SHAPεΌε°ι’ζ΅ζ¦η](https://zhuanlan.zhihu.com/p/364920925) 

[ζΊε¨ε­¦δΉ ζ¨‘εε―θ§£ιζ§θΏθ‘ε°εΊ3 - DP&amp;ICEεΎ](https://zhuanlan.zhihu.com/p/364921771 ) 

[ζΊε¨ε­¦δΉ ζ¨‘εε―θ§£ιζ§θΏθ‘ε°εΊ4 - ηΉεΎιθ¦ζ§](https://zhuanlan.zhihu.com/p/364922142 ) 

[ζΊε¨ε­¦δΉ ζ¨‘εε―θ§£ιζ§β€](https://zhuanlan.zhihu.com/p/258988892 ) 



### ***Deep Learning***

**_Algorithms_**

*CNN*

* [CNN Explainer](https://poloclub.github.io/cnn-explainer/)



### ***Active learning***

_paper_

```
π΄2014 CSD[T]. Active Learning Literature Survey
π΄2022 ACM CS[J]. A Survey on Active Deep Learning: From Model-Driven to Data-Driven
π΄2021 IEEE TNNLS[J]. Fast and Effective Active Clustering Ensemble Based on Density Peak --(Q1)
π΄2017 EAS[J]. Active learning through density clustering
π 2020 IEEE ICDM[C]. Meta-AAD: Active Anomaly Detection with Deep Reinforcement Learning
π 2020 IEEE TVT[J]. Importance-Aware Data Selection and Resource Allocation in Federated Edge Learning System
π 2014 Science[J]. Clustering by fast search and find of density peaks --(Q1)
π‘2018 ICML[J]. Not All Samples Are Created Equal: Deep Learning with Importance Sampling
```

_Tips_

* [δΈ»ε¨ε­¦δΉ (Active Learning)οΌηθΏδΈη―ε°±ε€δΊ](https://zhuanlan.zhihu.com/p/377045943)

* [δΈη‘?ε?εΊ¦ιζ ·οΌUncertainty SamplingοΌ](https://blog.csdn.net/qq_39856931/article/details/106433187)

* [δ»δΉζ―δΈ»ε¨ε­¦δΉ ](https://www.zhihu.com/question/352299820 )

* [Multi-Criteria-based Active Learning](https://blog.csdn.net/weixin_30502157/article/details/99482577 )

_Tools & packet_

* https://github.com/modAL-python/modAL
* https://github.com/NUAA-AL/ALiPy
* https://github.com/google/active-learning
* https://github.com/baal-org/baal

* [Python ε―εΊ¦θη±»](https://cloud.tencent.com/developer/article/1738535 )



### Ensemble Learning

* [StackingζΉζ³θ―¦θ§£ εε?’ε­](https://www.cnblogs.com/Christina-Notebook/p/10063146.html)

* [GBDT--εζ₯ζ―θΏδΉεδΊ(ιδ»£η ) εε?’ε­](https://www.cnblogs.com/mantch/p/11160496.html)
* [η»δΊζδΊΊθ―΄ζΈζ₯δΊ--XGBoostη?ζ³](https://www.cnblogs.com/mantch/p/11164221.html)
* [ιδΏζζ--ζ¨‘ειζ(ε€ζ¨‘ε)θ?²θ§£(η?ζ³+ζ‘δΎ)  εε?’ε­](https://www.cnblogs.com/mantch/p/10203143.html)
* [γζ¨‘εθεγBaggingοΌBoostingοΌStacking](https://blog.csdn.net/xiaohutong1991/article/details/107976781)
* [ζ¨‘εθεεpythonε?η° - η₯δΉ](https://zhuanlan.zhihu.com/p/61705517)
* [XGBClassifierηι»θ?€εζ°εθ°εζ»η» - η₯δΉ](https://zhuanlan.zhihu.com/p/365030773)
* [1.11. ιζζΉζ³ - sklearn](https://www.scikitlearn.com.cn/0.21.3/12/#11121)
* [ζ·±ε₯ηθ§£LightGBM - η₯δΉ](https://zhuanlan.zhihu.com/p/99069186)
* [GitHub - kaz-Anova/StackNet: StackNet is a computational, scalable and analytical Meta modelling framework](https://github.com/kaz-Anova/StackNet)

### ***Reinforcement Learning***

* [δΈζηζδ»δΉζ―εΌΊεε­¦δΉ οΌοΌεΊζ¬ζ¦εΏ΅+εΊη¨εΊζ―+δΈ»ζ΅η?ζ³οΌ](https://easyai.tech/ai-definition/reinforcement-learning/)

### ***Semi-supervised Learning***



### ***Unsupervised Learning*** 



## Model credibility

* [ζ¨‘εη₯θ―ζ½εδΏθΏζ¨‘εε―δΏ‘δ»»](https://mp.weixin.qq.com/s?__biz=MzIyODYzNTU2OA==&amp;mid=2247489820&amp;idx=1&amp;sn=9d514bf3a20fba3440fed729942ae754&amp;scene=19#wechat_redirect )

* [ζ¨‘εεΊ¦ι Β· Machine Learning](https://shunliz.gitbooks.io/machine-learning/content/ml/pythonml/ml-metrics.html)

## Data-certric AI

***Data lightweight***

*Based on active learning*

Move to *Artificial Intelligence - Category - Active learning*



***Data analysis***

_Tips_

* [Data-centric AI](https://zhuanlan.zhihu.com/p/438817550 )

* [ζ°ζ?εζοΌηΈε³ζ§εζ](https://zhuanlan.zhihu.com/p/136771737 )

* [ζ ·ζ¬η±»ε«ε’ε ](https://mp.weixin.qq.com/s/DqoiHshO17_QSjw0utJofg )



# Feature engineering

_Tips_

* [ζ·±εΊ¦δΊθ§£ηΉεΎε·₯η¨](https://zhuanlan.zhihu.com/p/111296130)

* [θͺε¨εζεηΉεΎ](https://mp.weixin.qq.com/s/CGS_nAnFAJYhcjmQr6nS3A)
* [δ½ ζ³η₯ιηηΉεΎε·₯η¨οΌζΊε¨ε­¦δΉ δΌεζΉζ³](https://www.cnblogs.com/mantch/p/11254026.html)

## Feature Dimensionality Reduction

* [PythonζΊε¨ε­¦δΉ η¬θ?°οΌδ½Ώη¨scikit-learnε·₯ε·θΏθ‘PCAιη»΄](https://www.cnblogs.com/wj-1314/p/10144700.html)

# Mathematics and Methodology

## Mathematics

*MI & MIC*

* [MIC](https://blog.csdn.net/qq_27586341/article/details/90603140 )
* [MIC-1](https://www.deeplearn.me/1466.html )

* [Maximal Information Coefficient (MIC)ζε€§δΊδΏ‘ζ―η³»ζ°θ―¦θ§£δΈε?η°](https://blog.csdn.net/FontThrone/article/details/85227239)



## Methodology





# Software and Tools

***Scientific***

`Wireshark`

 `Zeek`

 `Matlab`

`Python` : Pytorh/ Jupyter/ Pycharm

***Github***

* [Githubδ½Ώη¨ζε·§](https://zhuanlan.zhihu.com/p/150584178 )

`Zat `: 

* [from log to python](https://github.com/SuperCowPowers/zat "Zat")

`ALiPy` : 

* [Active learning packet](https://github.com/NUAA-AL/ALiPy  "ALiPy")

* [θ§£ζALipyοΌδΈ»ε¨ε­¦δΉ ηPythonε·₯ε·η?±](https://blog.csdn.net/qq_36317312/article/details/117981682 )

`modAL` : 

* [Active learning packet](https://github.com/modAL-python/modAL )

`Zat`

* [ZAT-ζΊε¨ε­¦δΉ -ε¨θζ£ζ΅](https://www.freebuf.com/articles/es/245516.html)

***Tools***

| Tools  |    function    | source |
| :----: | :------------: | :----: |
| ediary |                |        |
| Typora | .md --> Readme |        |
| Xmind  |                |        |
| DeepL  |  translation   |        |

* [VMware Toolsε?θ£](https://blog.csdn.net/love20165104027/article/details/83377758)



# Writing

*Tips*

* [θ±ζθ?Ίζεδ½η»ιͺ - η₯δΉ](https://zhuanlan.zhihu.com/p/158599066)

## **SCI**

* [Sci-Hub:](https://sci-hub.se/)

* [SCIεδ½ι«ι’θ―]( https://zhuanlan.zhihu.com/p/80384925 )
* [ε½±εε ε­ζ₯θ―’](http://www.letpub.com.cn/index.php?page=journalapp&amp;fieldtag=4&amp;firstletter= ) or Web of science --> Journal Citation Report

* [SCIζεεεΊζ£η΄’η?ε½εε½±εε ε­ζ₯θ―’η³»η»-ShengSci](https://www.shengsci.com/sci/)

* [citexs-θ΅ηΉζ°ζηη©ε»ε­¦η§η ε©ζ](https://www.citexs.com/)

## EI



## Conference

* [CCFδΌθ?? - Conference Partner (δΌδΌ΄)](https://www.myhuiban.com/conferences/ccf)



## Patents

* [ε½ε?Άη₯θ―δΊ§ζε±](https://www.cnipa.gov.cn/)
* [δΈε©ηΌ΄θ΄Ή](https://zhuanlan.zhihu.com/p/115498826)

## Core

Submission comments refer to the "ε°ζ¨θ«"

* [θ?‘η?ζΊζ ΈεΏζεοΌεε€§ζ ΈεΏοΌζη¨Ώζθ§](https://www.cnblogs.com/smuxiaolei/p/8081342.html)



## **Readme**

* [ReadmeηδΉ¦εθ§θ](https://blog.csdn.net/A33280000f/article/details/115836658 )

* [markdown-cheatsheet](https://github.com/tchapi/markdown-cheatsheet#heading-1 )
* [ε¦δ½εδΈδΈͺδΌη§ηReadme](https://blog.csdn.net/MOY37RQW1JarN33BgZk/article/details/84207318 )  or [Readme](https://zhuanlan.zhihu.com/p/29136209)
* [Readmeε₯½ηζε](https://zhuanlan.zhihu.com/p/151291463 )

## Layout

*Tips:*

* [wordδΈ€ζ ζ ΌεΌε¬εΌε±δΈ­οΌηΌε·ε³ε―Ήι½](https://blog.csdn.net/weixin_44105113/article/details/118445043)

# Tips & Bug & Solution

## Windows



## linux

* [Linuxε½δ»€](https://www.linuxcool.com/)



## python

***sklearn***

* [sklearn](https://scikit-learn.org/stable/index.html )
* [sklearn-δΈ­ζη€ΎεΊ](https://scikit-learn.org.cn/ )
* [sklearn-δΊ€ειͺθ―](https://blog.csdn.net/rocling/article/details/93717335 )
* [CountVectorizerθ―¦θ§£](https://blog.csdn.net/weixin_38278334/article/details/82320307 )



[δ½Ώη¨sklearnθΏθ‘ιζε­¦δΉ ββηθ?Ί](https://www.cnblogs.com/jasonfreak/p/5657196.html)

[δ½Ώη¨sklearnεεζΊηΉεΎε·₯η¨](https://www.cnblogs.com/jasonfreak/p/5448385.html)

[δ½Ώη¨sklearnδΌιε°θΏθ‘ζ°ζ?ζζ - εε?’ε­](https://www.cnblogs.com/jasonfreak/p/5448462.html)



[ζΊε¨ε­¦δΉ stackingη?ζ³δΉζθ§ - η₯δΉ](https://zhuanlan.zhihu.com/p/70757784)

***python***

* [PythonδΈ­ζζη¨](https://docs.python.org/zh-cn/3/)
* [pythonεεθ?­η»ιγιͺθ―ιεζ΅θ―ι](https://blog.csdn.net/haoji007/article/details/106165488)
* [δΏ?ζΉjupyter notebookι»θ?€ζεΌζ΅θ§ε¨(Windowsζδ½η³»η»)](https://blog.csdn.net/tunerf/article/details/90767377)



## Zeek

* [Zeek documents](https://docs.zeek.org/en/current/quickstart.html#a-minimal-starting-configuration )

* [Zeek install](https://docs.zeek.org/en/master/get-started.html)

## Open source

***Class***

[2019εΉ΄ζΊε¨δΉεΏεΉ²θ΄§ζη¨ι½ε¨θΏιδΊ](https://mp.weixin.qq.com/s?__biz=MzA3MzI4MjgzMw==&mid=2650779244&idx=1&sn=f961d29c4be9288ee31d573a25c0f93e&chksm=871a6a12b06de304d90bac98dc5e2e8d70b52bf43444cdcee5a1564c466816d526c58f287f0f&mpshare=1&scene=1&srcid=1023UT4OyAaWvqHDmpBYsvYG&sharer_sharetime=1603441563266&sharer_shareid=84d5fc173d51bf1365bb32f022e3807d&key=0ac52f944ed0d7b1bad9f9c791891ab85d0ff4222f705f34578e1fb440bcbe855abbe2f39516928b9d6327b850fc0d6fcea973424426b8eeb09e6cb93693478c0555daf8ef468a26683079c1d5324c515740f6f0bdc682b04872e9ebfaf94cea69d42404abb706dd5137df20965d7b77615bcab9fdec4a73d1400840a5ac08b5&ascene=1&uin=Mjc0MzE1MTI0NA%3D%3D&devicetype=Windows+10+x64&version=6300002f&lang=zh_CN&exportkey=Ab1ZC%2FSbM4E3ZzDLxnfXXfA%3D&pass_ticket=cN9rBpfgt8w6bvNaYcVsIzioqpyunTIjecZmRoUoPXQQLGDqacHzzZH1cqSIyKAc&wx_header=0)

[ζΊε¨ε­¦δΉ εΏε­¦10ε€§η?ζ³](https://mp.weixin.qq.com/s?__biz=MzA3MzI4MjgzMw==&mid=2650758853&idx=4&sn=fad1a71a12a0ec07b05bc255202ba5c3&chksm=871a9abbb06d13ad1683d02a3c29767b5ab0adbf8299b891f22bd5658df96996be4b00e29bb7&scene=21#wechat_redirect)



***Encrypted traffic detection***

γε ε―ζ΅ιζ΅ιεεζγ-- η¨ε

[δΈη―ζ₯εδΊθ§£ε½ει¦δΈͺιε―Ήε ε―ζ΅ιηζ£ζ΅εΌζ - ε?ε¨η](https://www.aqniu.com/tools-tech/45207.html)

[ε ε―ζΆζζ΅ιδΌη§ζ£ζ΅ζθ·―εδΊ«](https://cloud.tencent.com/developer/article/1792547)

[ε?ε¨εθ??ε­¦δΉ δΉTLSεθ??δΈHTTPSζΆζζ΅ιεζ](https://blog.csdn.net/qq_43968080/article/details/107086152)



***Computer/ software engineering***

[Software Engineering](chrome://bookmarks/?id=402)



***Cyber-security***

γη½η»ε?ε¨δΈ­ηζ°ζ?ζζζζ―γ -- ζζΆ

[HTTP,TCP/IP,DNSδΉι΄ηε³η³»εδ½η¨δΉθ§θ§£ - η₯δΉ](https://zhuanlan.zhihu.com/p/60721237)

[HTTPγTCP/IPγDNSδΉι΄ηε³η³»](https://blog.csdn.net/forevershow55/article/details/108756688 )





***Industry Reports***

[εθ΄Ήθ‘δΈζ₯ε_εθ΄Ήη η©Άζ₯ε-εζ²Ώζ₯εεΊ](https://wk.askci.com/)

[ε½ε?Άη»θ?‘ε±](http://www.stats.gov.cn/)

[θΎθ?―η η©Άι’](https://www.tisi.org/)



***TLS/SSL***

[JoyοΌδΈζ¬Ύη¨δΊζθ·εεζη½η»ει¨ζ΅ιζ°ζ?ηε·₯ε·](https://www.freebuf.com/sectool/161431.html)

[δΌ θΎε±ζεεζ-SSL/TLS](https://www.freebuf.com/articles/network/116497.html )

[DataCon2020 ζΈεζι TLS](https://datacon.qianxin.com/blog/archives/122 )

[DataCon2019 DNSζΆζζ΅ιεζη¬¬δΈ](https://zhuanlan.zhihu.com/p/68009679 )

[TLSε ε―ζ΅η°ηΆεζ -- Technology report](https://news.sophos.com/en-us/2021/04/21/nearly-half-of-malware-now-use-tls-to-conceal-communications/ )

[ζΆζθ½―δ»Άε ε―ζ΅ιηζθ](https://mp.weixin.qq.com/s/hVq3eBMDsX6tj1PsoUpy8Q )

[η η©ΆοΌζΆζθ½―δ»Άε¨ζ²ηδΈ­εΊθ―₯ζ§θ‘ε€ιΏζΆι΄οΌ - ε?ε¨εε | ε³η­θηη½η»ε?ε¨η₯θ―εΊ](https://www.secrss.com/articles/30599)



***Some website***

[Hack Inn](https://www.hackinn.com/)

[ζ»ι²δΈη](https://adworld.xctf.org.cn/)

[2020εΉ΄η½η»ε?ε¨δΊ§δΈζ·±εΊ¦ε―Ήθ―θ?Ίε - Hack Inn](https://www.hackinn.com/index.php/archives/746/)











