# STAT1013-final-projet
---
jupyter:
  kernelspec:
    display_name: Python (Pyodide)
    language: python
    name: python
  language_info:
  nbformat: 4
  nbformat_minor: 4
---

<div class="cell markdown">

background：目前经济发展迅速，许多地区的环境污染也随之愈来愈严重。借此，我想将中国南北方两个代表城市（北京、香港）的污染指标做对比，分析两个地区的污染情况的差异。
这两个数据集分别包含北京和香港2017-2020年初每日的6种主要污染物指标，共采集上千份数据。我们从两个数据表中可以发现pm2.5为主要污染成分因此我将分析两组数据的pm2.5的平均值，由此来推出究竟哪个城市的污染更严重。

1.  Which city has a much high pm2.5 index
2.  （1）Beijing pm2.5 index and HK pm2.5 index （2）pm2.5 index
    （3）It's quatitative
3.  I suppose that Beijing might have a higher average index of pm2.5
    than HongKong, it may because that a higher humidity would be found
    in HK rather than Beijing.
4.  I will collect data sets from github
5.  It would be a much pursuative, precise and believable if we collect
    them through interview or survey from thousands of people.

</div>

<div class="cell code" trusted="true">

``` python
import pandas as pd
df = pd.read_csv('https://raw.githubusercontent.com/prasertcbs/basic-dataset/master/air_quality_index/hong-kong-air-quality.csv')
```

</div>

<div class="cell code" trusted="true">

``` python
df['pm25']
```

</div>

<div class="cell code" trusted="true">

``` python
df.head(5)
```

</div>

<div class="cell code" trusted="true">

``` python
df.describe()
```

</div>

<div class="cell code" trusted="true">

``` python
df.shape()
```

</div>

<div class="cell code" trusted="true">

``` python
df.info()
```

</div>
