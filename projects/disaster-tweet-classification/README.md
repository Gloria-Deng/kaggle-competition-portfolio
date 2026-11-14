# 灾害推文识别

## 项目目标

识别推文是否描述真实灾害，以 F1 分数评价分类结果。

## 工作内容

- 复现 BERTweet 和 DeBERTa 的公开方案，并训练、比较多模型组合。
- 使用交叉验证预测比较组合权重与分类阈值；对无法确认样本顺序一致的外部预测不纳入组合。

## 结果

公开榜最佳 **F1 0.84983**；2026 年 11 月 14 日 17:17（北京时间）位列 **26 / 563 队**。公开方案复现与调整后的组合都曾达到这一公开榜分数。

## 相关链接

- [公开方案复现](https://www.kaggle.com/code/gloriachen0816/fork-nlp-bertweet-deberta-0849)
- [三模型实验](https://www.kaggle.com/code/gloriachen0816/nlp-ens3-r6)
- [Natural Language Processing with Disaster Tweets](https://www.kaggle.com/competitions/nlp-getting-started)
