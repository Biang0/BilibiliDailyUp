## 哔哩哔哩升级脚本-青龙/云函数

## 前言

>于2023/2/24 重写了代码,开放了源代码，有能力得可以自己添加功能，因为不常使用，可能不会再维护了

## 功能

### 已实现功能

![](https://img.ifool.me/i/2022/08/15/vqq5q6.webp)

> 其他功能如漫画签到,直播输赢压硬币等以后随缘添加,因为本来就是自己用的，很多功能自己也用不着

## 配置

> 配置文件是`config/config.py`文件
![](https://img.ifool.me/i/2022/08/15/vrehpf.webp)


## 本地运行

- 安装依赖`pip3 install -r requirements.txt`
- `python3 main.py`

## 云端部署

> 阿里云函数我自己不用,理论上来说和腾讯云函数类似

### 腾讯云函数☁️
> 云函数的入口函数代码在example文件夹中
- 1.新建python3.6空白函数

- 2.在高级配置-环境配置中把初始化时间和执行超时时间改成最大![](https://img.ifool.me/i/2022/08/15/fq93if.webp)

- 3.在创建好的云函数中对着脚本里的文件新建文件复制黏贴代码![](https://img.ifool.me/i/2022/08/15/fs5ua7.webp)

- 4.修改配置文件`config.py`
- 5.部署运行测试
- 6.添加每日定时运行规则

### 青龙面板🐉

> 演示机器腾讯云上海4h3g ubuntu22.04

- 1.打开青龙面板
- 2.拉取代码
- 3.填写config/config.py的配置文件
- 4.设置运行规则，运行测试
- 运行测试![](https://img.ifool.me/i/2022/08/15/qo0ptr.webp)

## COOKIE抓取

- 打开哔哩哔哩网页端登录好
- 新建一个浏览器页面,打开开发者模式,复制链接`http://account.bilibili.com/site/getCoin`黏贴打开
- 复制`cookie`黏贴到脚本即可![](https://img.ifool.me/i/2022/08/15/h9n8b4.webp)

## up主UID获取

如下图问号前面的一串数字就是UID

![](https://img.ifool.me/i/2022/08/15/hhnbpl.webp)

## 运行截图

![](https://img.ifool.me/i/2022/08/15/hb1oly.webp)

