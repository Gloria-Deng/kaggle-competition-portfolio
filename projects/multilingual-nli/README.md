# 多语言自然语言推理

## 项目目标

判断前提与假设之间的蕴含、矛盾或中立关系，覆盖多种语言。

## 工作内容

- 比较多语言预训练模型，组合 DeBERTa 与 XLM-R 等模型的预测。
- 针对英文样本调整专家模型权重，并根据训练集表现选择组合方式。

## 结果

语言分组组合版本公开榜准确率 **0.94995**。另有从公开数据匹配测试标签得到的满分结果；该结果反映标签匹配，不作为模型泛化能力指标。

## 相关链接

- [语言分组模型程序](https://www.kaggle.com/code/gloriachen0816/contra-lang-expert-v3)
- [Contradictory, My Dear Watson](https://www.kaggle.com/competitions/contradictory-my-dear-watson)
