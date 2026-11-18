# 折返后的再加速和接球空间

外接手在体测中折返后的再加速能力，和比赛中甩开防守人的距离有关吗？我从 10 Hz 的 NFL Combine 轨迹里找出转向点，再把转向角、减速和再加速连到同一球员的比赛路线。

我分析了 **83 名球员的 31,035 条路线**。FLAT 和 CROSS 的标准化关联为正（+0.0915、+0.0660），OUT 为负（−0.0588）。按赛季留出复查时，CROSS 有 2/3 次保持原来的方向，OUT 有 3/3 次。把不同位置混在一起会抬高体测指标的一致性，我因此用同位置的结果来解释这些差异。

路线分析按球员处理重复观测，并用重采样和置换检查结果。这项工作写成了公开研究文章。

## 运行分析

获取 [比赛数据](https://www.kaggle.com/competitions/nfl-big-data-bowl-2027/data) 后安装 `numpy`、`pandas`、`scipy` 和 `matplotlib`。将 `BDB27_DATA` 指向包含 `combine_tracking.csv`、`player_play.csv`、`players.csv` 和 `games.csv` 的目录，从本项目页所在目录运行：

```bash
python analysis/bdb27_r8_forward_validated.py
```

可用 `BDB27_OUT` 指定结果目录。代码默认执行完整分析，比赛数据由比赛页面提供。

- [公开分析程序](https://www.kaggle.com/code/gloriachen0816/bdb27-r8-route-family-analysis)
- [公开研究文章](https://www.kaggle.com/code/gloriachen0816/bdb27-r8-route-family-writeup)
- [NFL Big Data Bowl 2027](https://www.kaggle.com/competitions/nfl-big-data-bowl-2027)
