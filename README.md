# Virus-Detection
DC/数字城市大赛/网络安全病毒检测/top1
## 

### 1.运行说明
环境：  
Linux  Python2  Xgboost  Scikit-learn

运行：  
a. 将文件”/home/data/all_data_1019.csv”放入”./data/”  
b. 直接运行” ./src/main.py”。

### 2.算法说明

传统步骤：  
a. 数据导入  
b. 特征提取  
c. 算法模型  
d. 输出结果  

### 3.个人心得

a. 数据量  
本次赛题数据量相对较小，个人第一想法就是先不考虑神经网络算法。

b. 标签  
通过数据的标签，可以看出这个是个十分不平横的分类问题。考虑是否要对数据进行重采样（多）或者降采样（少）。

c. 竞赛圈  
竞赛圈有很多很优秀的开源分享.前期的对数据的导入和处理，与简单算法实现都有很大帮助。

d. trick  
训练词表时,一定要将所有train、test 一起训练。  
模型除了线性分类器,一定要对于提取的文本tf，tfidf特征进行降维，维度一般不要超过200，否则速度慢,收益少。  
分布不平衡时,可以考虑自定义目标函数.二分类不一定非要以预测概率1/2为分类界限。  

e. 不足  
单模型.未模型集成bagging、stacking...或nn...等,主要原因单模型太高,大家得分都超过,内心基本放弃,不想花太多时间。  

### 4.总结
运气高于一切。
