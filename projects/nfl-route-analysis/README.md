# NFL 体测与比赛表现分析

## 项目目标

利用 NFL Combine 球员追踪数据，研究折返后的再加速能力与常规赛接球路线中防守间距的关系。项目同时分析测量稳定性与跨赛季结果，输出可复核的研究报告和图表。

## 工作内容

1. 从 10 Hz 运动轨迹识别方向变化，提取转向角、减速与再加速等指标，并按球员、位置和赛季关联比赛数据。
2. 分路线类型建立回归分析，使用按球员聚类的标准误、重采样与置换方法评估结果；另按赛季留出数据检查方向是否保持。
3. 分别计算混合位置与位置内的测量一致性，发现混合位置会明显抬高该指标，因此以位置内结果解释球员指标。

## 结果

分析覆盖 **31,035 条外接手路线、83 名球员**。再加速指标与防守间距的标准化关联在 FLAT、CROSS、OUT 路线中分别为 **+0.0915、+0.0660、−0.0588**；结果应按路线类型理解。CROSS 和 OUT 在跨赛季检查中分别有 2/3、3/3 次保持相同方向。项目已发布研究文章，比赛采用报告评审。

## 使用

获取 [比赛数据](https://www.kaggle.com/competitions/nfl-big-data-bowl-2027/data) 后安装 `numpy`、`pandas`、`scipy` 和 `matplotlib`，将环境变量 `BDB27_DATA` 指向包含 `combine_tracking.csv`、`player_play.csv` 的目录，再运行：

```bash
python analysis/bdb27_r8_forward_validated.py
```

可用 `BDB27_OUT` 指定结果目录。代码默认执行完整分析，比赛数据由比赛页面提供。

## 相关链接

- [公开分析程序](https://www.kaggle.com/code/gloriachen0816/bdb27-r8-route-family-analysis)
- [公开研究文章](https://www.kaggle.com/code/gloriachen0816/bdb27-r8-route-family-writeup)
- [NFL Big Data Bowl 2027](https://www.kaggle.com/competitions/nfl-big-data-bowl-2027)
