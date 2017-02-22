# 房屋信息爬虫
基于Scrapy-Redis框架的分布式爬虫
## 信息来源
[中房网](http://www.fangchan.com/)<br>
[房天下](http://wuhan.fang.com/)<br>
[安居客](http://wuhan.anjuke.com)<br>
## 数据格式
`经纬度`、`小区名`、`小区位置`、`房屋面积`、`朝向`、`装修程度`、`楼层`、<br>
`户型`、`单价`、`首付`、`住宅类型`、`总价`、`标题`、`房屋描述`、`月供`。<br>

## 项目基本说明
* 这是学校的一个小项目
* 去重采用Bloomfilter算法
* 防Ban，采用更换User-agent和禁cookies
* 此次演示只是在单机上面执行，分布式请自己部署


## 主要运行环境
* Windows7及以上
* Python27
* Scrapy1.2以上
* Scrapy-Redis相关模块
* bs4
* mongodb
* redis 

## 运行准备
* 启动Mongodb服务
* 启动Redis服务
* 启动lpush.py
* 启动crawlall.py

## 注意
    **lpush.py是压入初始URL到Redis数据库中，不要重复执行。**
    
## 运行结果截图
