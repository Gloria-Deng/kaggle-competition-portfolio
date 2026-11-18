# 我的 Kaggle 项目

这里收录了我在 Kaggle 做过的数据分析、模型实验和公开方案复现。我把分析代码、笔记本和具体结果放在各项目页里。

## 推荐从这三个看起

- **NFL 球员追踪。** 我把体测中的折返轨迹和比赛里的 31,035 条接球路线对应起来，分析再加速和防守间距的关系。关联方向随路线类型而变，分开看比给出一个全局平均更有意义。[文章与分析代码](projects/nfl-route-analysis/)
- **大模型回答偏好。** 长对话只保留开头会切掉一部分回答。我改成同时保留开头和结尾，双模型方案的公开榜对数损失从 0.82756 降到 0.82728。[改动与公开笔记本](projects/llm-preference-prediction/)
- **零售销量预测。** 直接平均多个相似的公开预测，会让它们在组合里占比过高。我先按预测差异分组，再给各组分配权重。组合后的公开榜 RMSLE 为 0.37699。[预测组合](projects/retail-sales-forecasting/)

## 其他实验

| 方向 | 项目 |
| --- | --- |
| 几何与智能体 | [方中方装箱](projects/square-packing/) · [Gemma 软件开发智能体](projects/gemma-developer-agent/) |
| 文本分类 | [生成文本来源识别](projects/llm-authorship/) · [多语言自然语言推理](projects/multilingual-nli/) · [灾害推文识别](projects/disaster-tweet-classification/) |
| 表格数据 | [住宅价格回归](projects/house-prices/) · [房价预测组合](projects/home-data/) · [太空船乘客分类](projects/spaceship-passenger-classification/) · [乘客生存预测](projects/titanic-survival/) |
| 图像与质谱 | [手写数字识别](projects/handwritten-digit-recognition/) · [质谱候选结构排序](projects/mass-spectrometry-molecule-id/) |

项目页注明公开方案的来源。榜单名次保留记录时的日期和时间。量子线路的代码和计算笔记在 [Verifiable Quantum Circuits](https://github.com/Gloria-Deng/verifiable-quantum-circuits)。
