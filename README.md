## DJI产品流行度分析

## 目标

编写一个爬虫，解析大疆社区中的作品展示，获得各产品流行度值，并通过图标直观给出各产品受欢迎程度

## 解决方案

1. 爬取[链接:https://bbs.dji.com/forum-60-1.html](https://bbs.dji.com/forum-60-1.html)，获取帖子链接列表和帖子对应发帖人所用设备（没有则为空），并统计DJI产品设备名。
2. 判断发帖人设备是否存在，如果存在，该设备流行度加一；如果不存在，保存该链接；
3. 爬去步骤二中的链接，检测整个页面是否出现步骤一中的设备名称，如果存在，该设备流行度加一，否则跳过该链接
4. 将步骤2/3中统计的流行度值归一化并制成图表，发到电子邮箱中;

## 分工

YANAN: 步骤2/4

FUAN：步骤3

YINBIAO：步骤1

