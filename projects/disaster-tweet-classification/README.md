# 灾害推文识别

一句话是在报道灾害，还是把「灾难」当成比喻？我复现了 BERTweet 和 DeBERTa 的公开做法，也用交叉验证预测比较组合权重和分类阈值。外部预测需要先确认与原样本逐行对应。

公开方案复现和调整后的组合都达到过 **F1 0.84983**。2026 年 11 月 14 日 17:17（北京时间）的记录为 **26 / 563**。

- [公开方案复现](https://www.kaggle.com/code/gloriachen0816/fork-nlp-bertweet-deberta-0849)
- [三模型实验](https://www.kaggle.com/code/gloriachen0816/nlp-ens3-r6)
- [Natural Language Processing with Disaster Tweets](https://www.kaggle.com/competitions/nlp-getting-started)
