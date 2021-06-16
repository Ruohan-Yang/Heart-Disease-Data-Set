# Heart-Disease-Data-Set
processed.cleveland.csv是从UCI Heart Disease Data Set 官网下载的数据集  
heart-disease.txt是UCI Heart Disease Data Set 官网对数据集的描述解释  

数据属性说明：  
1）age-年龄  
2）sex-性别 （1 =男性； 0 =女性）  
3）cp-胸痛类型（4个值，值1：典型的心绞痛，值2：非典型心绞痛，值3：非心绞痛，值4：无症状）  
4）trestbps-患者入院时的静息血压（单位：mm Hg）  
5）chol-血清胆固醇水平（单位：mg / dl）  
6）fbs-空腹血糖（> 120 mg / dl ，1=真；0=假）  
7）restecg-静息心电图结果（值0：正常，值1：有ST-T波异常（T波倒置和/或ST升高或降低> 0.05 mV），值2：根据Estes的标准显示可能或确定的左心室肥大）  
8）thalach-达到的最大心率  
9）exang-运动引起的心绞痛（1 =是； 0 =否）  
10 ）oldpeak-运动相对于休息引起的ST压低  
11）slope-最高运动ST段的斜率，（值1：上坡，值2：平坦，值3 ：下坡）  
12）ca-萤光显色的主要血管数目（0-3）  
13）thal-一种称为地中海贫血的血液疾病（3=正常；6=固定缺陷；7=可逆缺陷）  
14）target- 患者是否患有心脏病。它是从0（不存在）到4的整数值。 Cleveland 数据库的实验集中在试图区分存在（值1、2、3、4）和不存在（值0）。
  
  
UCI Heart Disease Dataset.csv是对官网数据集稍做处理后的数据集  
1-12相同  
13）thal-一种称为地中海贫血的血液疾病（0 =正常；1 =固定缺陷；2 =可逆缺陷）  
14）target- 患者是否患有心脏病。存在（值1）和不存在（值0）。  

处理内容：  
官网原始数据集一共有303行, 14列，行索引从0-302  
其中ca列有4个缺失值，行索引分别为166，192，287，302  
其中thal列有2个缺失值，行索引分别为87，266  
去除缺失值后，UCI Heart Disease Dataset数据集[297 rows x 14 columns]  
thal指标用0，1，2进行替换  
target指标换为存在（值1）和不存在（值0），方便做二分类。  
