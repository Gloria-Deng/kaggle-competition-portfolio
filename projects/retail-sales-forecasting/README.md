# 零售门店销量预测

把几份 Favorita 销量预测按门店和商品对齐后，我发现有些方案给出的结果很接近。直接给每份预测相同的权重，会让相似的方案合起来占得太多。我试了按差异分组，再比较组内平均、中位数和权重组合。

最终采用公开预测的分组组合，公开榜 RMSLE 从 **0.41288 降到 0.37699**，在 2026 年 11 月 14 日 17:17（北京时间）排 **20 / 635**。我做的是预测的对齐、组合和比较，单份预测来自其原作者。

- [Store Sales – Time Series Forecasting](https://www.kaggle.com/competitions/store-sales-time-series-forecasting)
