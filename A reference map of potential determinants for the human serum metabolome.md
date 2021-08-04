# A reference map of potential determinants for the human serum metabolome  
人血清代谢组潜在决定因素的参考图 

----

### Something we should know firstly

* serum metabolome 血清代谢组

  **血清代谢组**的主要研究对象是血清所含有的各种**生物标志物**。血清代谢组中含有很多的生物标志物，其中一些是内源性产生的，有些是从环境中吸收，有些是病原体产生的。

* Anthropometric Measurements 人体测量

  人体测量是评估和概念化人体脂肪总量的一种方法。测量通常是一系列的，通常包括体重和身高、皮肤皱褶密度和在某些精确点进行的测量，尤其是臀部和手腕。那些将数字制成表格的人，通常是医生、护士或健身专家，利用这些结果来评估一个人的整体健康状况。如常见的**BMI**

* feature attribution analysis

  特征归因分析，

### WHY this study?



对于血液中的代谢物的研究有助于了解多种疾病，但是对于血液中的代谢物来讲，大多数代谢物的决定因素我们仍然知之甚少。





方法学：

491个健康人，共1251个样本，使用机器学习算法(4)

基于宿主遗传学，肠道微生物，临床指标，饮食，生活习惯，人体测量应用机器学习算法预测个体代谢物水平。（结果很nice超76%准确率？？）

使用

结果：

饮食和微生物组在预测中贡献度最高（有多高呢？甚至在某些代谢物上贡献率超50%）；使用的验证集：cohort7,8两种在地理上独立的数据，结果是展现出了高度一致性，证明了模型准确性。

使用特征归因分析揭示了特定饮食和细菌间的相互作用。



这些饮食和细菌间的一些相互作用可能是因果的，因为在？？面包干预的随机临床试验？？后，发现预测的一些代谢物与面包呈正相关。



发现超过800种代谢物的潜在决定性因素。

意义：

在不同情况下代谢物转移，并且对于设计操纵循环代谢物水平的干预手段提供了思路。







**如何解释机器学习模型**

 Consistent individualized feature attribution for tree ensembles.  为了解释集成树模型问题。

**Tree SHAP：**  （Shapley Additive explanation）即 shapley加法解释，基于博弈论和局部解释的统一思想，通过树集成和加法方法激活shap值用于特征归因。Scott M. Lundberg等人在NeurIPS 2017上提出了一个框架，该框架统一了包括LIME在内的各种附加特征归因方法。在该论文中+

，SHAP（代表SHapley Additive exPlanation）值被用作特征重要性的统一度量