# GitHub 2019 数据年报

## 简介

在开源日益重要的今天，我们需要一份建立在全域大数据基础上的相对完整、可以反复进行推演的数据报告（报告、数据、算法均需开源）。本项目为X-lab 开放实验室团队发起，旨在通过分析Github全网的开发者行为日志，通过数据的视角，来观察全球范围内的开源现状、进展趋势、演化特征、以及未来挑战等问题，除了展现目前开源世界全貌之外，我们特别关注中国的开发者和企业组织在整个开源产业中的表现。本报告中使用 2019 年全年 GitHub 日志进行统计，总日志条数约 5.46 亿条。

**关键词**：开源、行为数据、开发者行为、Github、数字报告

## 数据年脑

关于数据年报，请点击[原文](./REPORT.md)。

本报告使用 2019 年全年 GitHub 日志进行统计，总日志条数约 5.46 亿条，相较 2018 年的 4.21 亿条增长约 29.7%。在上述开发者活跃度与项目活跃度的定义下，统计得到 2019 年总活跃项目数量约 512W 个，相较 2018 年的约 313W 增长约 63.6%，2019 年总活跃开发者数量约 360W，相较 2018 年的约 303W 增长约 18.8%。

**世界 Top 10 开发者账号**

![global_top_10_dev_act](file:///Users/tianyi/github/github-analysis-report-2019/static/global_top_10_dev_act.png?lastModify=1580617710)

**世界 Top 10 项目**

![global_top_10_dev_act](/Users/tianyi/github/github-analysis-report-2019/static/global_top_10_repo_act.png)

**中国 Top 20 项目分析**

![chinese_top_20_act](file:///Users/tianyi/github/github-analysis-report-2019/static/chinese_top_20_act.png?lastModify=1580617776)

## 原始数据

关于数据，请访问[CDN](http://cdn.opensource-service.cn/github-analysis-report-2019/data.json.gz)

由于原始的日志文本数据数据量较大（约 1.45TB），故随本文开放的数据为统计处理并压缩后的数据文件，总大小约为 225MB，解压后文件内容为文本内容，总大小约 1.3GB，总行数约 2169 万行。每行为一个记录项，由 Json格式编码，该文件不再区分具体日期，直接给出每个账号在每个项目中的2019全年的操作次数，以方便处理。内容说明如下：

| 字段 | 类型   | 说明     |
| ---- | ------ | -------- |
| r    | string | 项目名称 |
| u    | string | 账号名称 |
| t    | number | 操作类型 |
| c    | number | 操作次数 |



## 分析程序

分析程序使用命令：

```shell
$npm i
$npm start -- --help
$npm start
```

