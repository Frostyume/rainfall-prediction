### Kaggle机器学习|降雨概率预测 Binary Prediction with a Rainfall Dataset
#### 问题描述
该项目的重点是开发一个基于气象数据预测降雨的机器学习模型。该模型旨在准确预测某一天是否会下雨，这代表了一个二元分类问题，其中目标变量“降雨量”被编码为1（雨）或0（无雨），最后提交的是具体降雨概率。
#### 数据总览
数据集包含每日气象观测指标，具体字段如下：

| 变量名称          | 描述                                      |
|--------------------|-------------------------------------------|
| Day               | 观测日顺序标识符                          |
| Pressure          | 大气压力测量值（单位：hPa）               |
| Maxtemp           | 当日最高温度（单位：°C）                  |
| Temperature       | 当日平均温度（单位：°C）                  |
| Mintemp           | 当日最低温度（单位：°C）                  |
| Dewpoint          | 露点温度（单位：°C）                      |
| Humidity          | 相对湿度百分比          |
| Cloud             | 云覆盖率                                  |
| Sunshine          | 日照时间（单位：小时）                    |
| Winddirection     | 风向（单位：度）                          |
| Windspeed         | 风速（单位：km/h）                        |
| Rainfall          | 目标变量（1=降雨，0=无雨）               |

#### 评价指标
使用ROC-AUC评估模型的性能。这种评估方法特别适用于二元分类问题，并对模型在各种概率阈值下区分雨天和非雨天的能力进行了全面评估，ROC-AUC度量在处理天气预报场景中潜在的不平衡类分布时尤其有价值
