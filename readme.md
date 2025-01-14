# 【sese-engine】新时代的搜索引擎！

大家平时都会用百度和谷歌来搜索资料吧。不过大家有没有怀疑过，也许它们不那么可信？

百度很坏，之前也有和竞价排名相关的丑闻。谷歌好一点，它说它不作恶，但我也不完全相信它，毕竟每个人的善恶观本身就不同。我想，它们或多或少都藏起了一些什么。

那怎么办呢？

我发明了强大并且安全的sese-engine。它是一个轻量级的搜索引擎，可以快速部署在个人电脑上。

sese-engine通过爬取互联网上的数据，在本地建立各个网页的索引。这样一来，你就有了自己的搜索引擎，可以在本地直接搜索互联网上的信息。你也可以修改你的爬取和搜索配置，让搜索的结果能满足个性化的需求。

数据即未来，我们的未来要掌握在自己手中。

<img align='right' src='https://upyun.yunyoujun.cn/images/sese-rimo-and-xiao-yun.png' width='320px'>


## 测试环境

一起来玩吧: https://sese.yyj.moe

对了，服务器是1年70元租的机器，配置很低。所以第一次查询可能会卡几秒，这是正常现象，大概率是服务进程被交换到硬盘里了。


## 部署

只需要1个Python3.8。数据库什么的都不用装，配环境很方便，好耶！

具体步骤是这些: 

1. 安装1个Python3.8

    Python版本太高的话，下一步会有依赖装不上。

2. 用pip安装依赖

    ```sh
    pip install -r requirements.txt
    ```

3. 运行 `启动.cmd` 或者 `启动.sh`

    你可能会很奇怪为什么之前没有`.sh`，这是因为我买的服务器是windows的。


这样你的搜索引擎服务应该就可以用了，你可以 `curl http://127.0.0.1:4950/search?q=test` 试一下。

然后前端的仓库在这里: [YunYouJun/sese-engine-ui](https://github.com/YunYouJun/sese-engine-ui)。前端怎么部署呢，去看看云游君怎么说吧。

如果你想用刀客部署的话，可以参照: [xiongnemo/sese-engine-docker](https://github.com/xiongnemo/sese-engine-docker)。

## 代价

sese-engine的消耗不大，一个便宜的服务器或者树莓派就够用了。

默认配置下，sese-engine的爬虫大约需要1\~2个CPU和1\~2G的内存，搜索服务几乎没有消耗。

此外，需要的硬盘空间会缓慢增长，尽管它会增长得越来越慢但并没有上界……所以最好给树莓派插一个移动硬盘。


## 赞助

如果你觉得sese-engine对你的工作或学习有帮助，欢迎来当我的女朋友。

要可爱的，最好是白发贫乳傲娇双马尾。
