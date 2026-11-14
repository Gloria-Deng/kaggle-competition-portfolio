# 大模型回答偏好预测

## 项目目标

根据同一提示下两段模型回答，预测用户更偏好的回答或平局，评价指标为对数损失，越低越好。

## 工作内容

- 复用 snaykey 的 Gemma-2 与 Llama-3 双模型方案，在长对话处理上改为同时保留开头和结尾，减少截断末尾回答的问题。
- 比较不同公开方案及推理配置，并在 Kaggle 的双 T4 环境中完成提交。
- 分开记录自行调整版本与直接复用其他作者版本的成绩。

## 结果

调整截断方式后，对数损失从 **0.82756 降至 0.82728**。之后复用 andyuuzou 的公开方案得到 **0.82685**；2026 年 11 月 14 日 17:17（北京时间）位列 **9 / 322 队**。两个成绩对应不同方案。

## 相关链接

- [本人的截断调整版本](https://www.kaggle.com/code/gloriachen0816/llmclf-headtail-r6)
- [本人的公开方案复现](https://www.kaggle.com/code/gloriachen0816/llmclf-ander-r7)
- [snaykey 原始双模型方案](https://www.kaggle.com/code/snaykey/gemma-2-llama-3-preference-ensemble-on-2xt4)
- [比赛页面](https://www.kaggle.com/competitions/llm-classification-finetuning)
