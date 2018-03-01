# PredictWonderfulTV

twtech-Paddle-综艺节目精彩片段预测

## 大赛数据说明

百度提供了1470个来自爱奇艺的电视综艺视频的数据，总共约1200个小时。

视频每秒都抽取了一帧图像提取图片特征，因此视频已都被转换为了视频帧的图片特征序列，但也都提供了观看链接。

其中每个视频都被仔细地标注了“精彩片段”的时间戳，单位为秒，总共标记出了18000段、约750小时的“精彩片段”。

BROAD数据集的格式为pkl\(pickle\), 读取的方式总结如下：

```
数据集的路径请移步参赛指南中查看。
# 方法一：传统Python方法
import cPickle
with open(BROAD_filepath/xxxx.pkl,'rb') as f:
tmp1 = cPickle.load(f)
print tmp1

# 方法二：利用Pandas读取
import pandas as pd
tmp2 = pd.read_pickle(BROAD_filepath/xxxx.pkl)
tmp2

# 方法三：利用Numpy读取
import numpy as np
tmp3 = np.load(BROAD_filepath/xxxx.pkl)
tmp3
```

## 使用Paddle


## 使用Tensorflow

