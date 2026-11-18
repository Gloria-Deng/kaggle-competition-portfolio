# 大模型回答偏好预测

我从 snaykey 的 Gemma-2 和 Llama-3 双模型方案出发，改了长对话截断。原做法只留开头，长输入容易丢掉末尾的回答。我让两个模型同时看到开头和结尾，在 Kaggle 的双 T4 环境中重跑，公开榜对数损失由 **0.82756 降到 0.82728**。

我还复现了 andyuuzou 的另一套公开方案，得分 **0.82685**。这份提交在 2026 年 11 月 14 日 17:17（北京时间）排 **9 / 322**，两份笔记本分别对应下面的两个链接。

- [本人的截断调整版本](https://www.kaggle.com/code/gloriachen0816/llmclf-headtail-r6)
- [本人的公开方案复现](https://www.kaggle.com/code/gloriachen0816/llmclf-ander-r7)
- [snaykey 原始双模型方案](https://www.kaggle.com/code/snaykey/gemma-2-llama-3-preference-ensemble-on-2xt4)
- [比赛页面](https://www.kaggle.com/competitions/llm-classification-finetuning)
