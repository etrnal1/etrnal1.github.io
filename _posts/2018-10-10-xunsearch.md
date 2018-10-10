

### Xunsearch 

全文检索 服务 开源

##### www.xunsearch.com 

完美的支持中文。中小型企业

#### xunsearch 文档

[chm版](https://pan.baidu.com/s/1OtRNPub1Iza_4a1DCkykAg)

[pdf版](https://pan.baidu.com/s/10O1bLDTgYi2Tt7QlguVzwg)

##### 安装xunsearch

   目前支持php 语言  做业务逻辑

```
wget http://www.xunsearch.com/download/xunsearch-full-latest.tar.bz2

sh  set.sh
```

第一次安装是特别的慢

  用 c 语言封装的接口，扩展来调用

#### xunsearch 的基本目录

![](https://ws1.sinaimg.cn/large/006tNbRwly1fw3izr8p2mj30jh08aq42.jpg)

  索引服务器端口

  搜索服务器端口

#### Xunsearch 的目录配文件

```
#项目
project.name = sample
#项目语言
    project.default_charset = GBK
    #索引服务器 端口号
    ;server.index = 8383
    #搜索服务器 端口号
    ;server.search = 8384

    [pid]
    type = id

    [subject]
    type = title

    [message]
    type = body

    [dateline]
    type = numeric

    [author]
    index = both

    [authorid]

    [tid]
    index = self
    tokenizer = full

    [fid]
    index = self
    tokenizer = full

    [flag]

```



###   字段

![](https://ws4.sinaimg.cn/large/006tNbRwly1fw3i1nwsf2j309c0dfdh7.jpg)



#### 中间件

操作服务器数据库的一个中间件

Mysql 中间件

阿里巴巴做了一个

  Cobar

https://github.com/alibaba/cobar

![](https://ws2.sinaimg.cn/large/006tNbRwly1fw3ixfzqlkj30k10diabh.jpg)



​    

